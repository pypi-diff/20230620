# Comparing `tmp/pymavlog-0.3.1.tar.gz` & `tmp/pymavlog-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymavlog-0.3.1.tar", max compression
+gzip compressed data, was "pymavlog-0.4.0.tar", max compression
```

## Comparing `pymavlog-0.3.1.tar` & `pymavlog-0.4.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1073 2023-06-13 07:27:16.807077 pymavlog-0.3.1/LICENSE
--rw-r--r--   0        0        0     1993 2023-06-13 07:27:16.807077 pymavlog-0.3.1/README.md
--rw-r--r--   0        0        0      196 2023-06-13 07:27:16.807077 pymavlog-0.3.1/pymavlog/__init__.py
--rw-r--r--   0        0        0     9086 2023-06-13 07:27:16.807077 pymavlog-0.3.1/pymavlog/core.py
--rw-r--r--   0        0        0      137 2023-06-13 07:27:16.807077 pymavlog-0.3.1/pymavlog/errors.py
--rw-r--r--   0        0        0      121 2023-06-13 07:27:16.807077 pymavlog-0.3.1/pymavlog/helpers.py
--rw-r--r--   0        0        0     1072 2023-06-13 07:27:26.143138 pymavlog-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     3110 1970-01-01 00:00:00.000000 pymavlog-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-06-20 09:40:10.444885 pymavlog-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1993 2023-06-20 09:40:10.444885 pymavlog-0.4.0/README.md
+-rw-r--r--   0        0        0      196 2023-06-20 09:40:10.444885 pymavlog-0.4.0/pymavlog/__init__.py
+-rw-r--r--   0        0        0    10619 2023-06-20 09:40:10.444885 pymavlog-0.4.0/pymavlog/core.py
+-rw-r--r--   0        0        0      137 2023-06-20 09:40:10.444885 pymavlog-0.4.0/pymavlog/errors.py
+-rw-r--r--   0        0        0      121 2023-06-20 09:40:10.444885 pymavlog-0.4.0/pymavlog/helpers.py
+-rw-r--r--   0        0        0     1072 2023-06-20 09:40:21.152981 pymavlog-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3110 1970-01-01 00:00:00.000000 pymavlog-0.4.0/PKG-INFO
```

### Comparing `pymavlog-0.3.1/LICENSE` & `pymavlog-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymavlog-0.3.1/README.md` & `pymavlog-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `pymavlog-0.3.1/pymavlog/core.py` & `pymavlog-0.4.0/pymavlog/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,14 +31,15 @@
         self,
         name: str,
         columns: t.List[str],
         types: t.List[type],
         column_alias: t.Dict[str, str] = {},
         msg_id: int = 1,
         convert_to_datetime: bool = False,
+        max_rate_hz: int = None,
     ) -> None:
         self.name = name
         self.id = msg_id
         self._to_datetime = convert_to_datetime
         self._column_alias = column_alias
 
         if len(columns) != len(types):
@@ -50,59 +51,99 @@
         else:
             self._types = [float]
 
         self._columns.extend(columns)
         self._types.extend(types)
         self._fields: t.Dict[str, t.List[t.Union[datetime, int, float]]] = {}
 
-        self.__set_series()
+        self._set_series()
 
-    def __set_series(self):
+        self._skip_messages = False
+
+        if max_rate_hz is not None:
+            self._skip_messages = True
+            if type(max_rate_hz) in [float, int] and max_rate_hz > 0:
+                self._max_rate_hz = max_rate_hz
+            else:
+                raise ValueError(f"invalid rate, should be higher than 0, {max_rate_hz}")
+            self._last_message_rate_t = {}
+
+    def _reduce_msg_rate(self, m: MAVLink_message) -> bool:
+        """
+        Function to skip messages based on the max rate (Hz)
+        """
+
+        mtype = m.get_type()
+
+        if mtype in ["PARM", "MSG", "FMT", "FMTU", "MULT", "MODE", "EVT"]:
+            return False
+
+        t = getattr(m, "_timestamp", None)
+
+        if t is None:
+            return False
+
+        if mtype not in self._last_message_rate_t:
+            self._last_message_rate_t[mtype] = t
+
+        dt = t - self._last_message_rate_t[mtype]
+
+        if dt <= 0 or dt >= 1.0 / self._max_rate_hz:
+            self._last_message_rate_t[mtype] = t
+            return False
+
+        return True
+
+    def _set_series(self):
         for c in self._columns:
             self._fields[self._column_alias.get(c, c)] = []
 
     @property
     def columns(self) -> t.List[str]:
         return self._columns
 
     @classmethod
     def from_df_format(
         cls,
         fmt: DFFormat,
         column_alias: t.Dict[str, str] = {},
         msg_id: int = 1,
         convert_to_datetime: bool = False,
+        max_rate_hz: int = None,
     ):
         return cls(
             name=fmt.name,
             columns=fmt.columns,
             types=fmt.msg_types,
             column_alias=column_alias,
             msg_id=msg_id,
             convert_to_datetime=convert_to_datetime,
+            max_rate_hz=max_rate_hz,
         )
 
     @classmethod
     def from_message(
         cls,
         msg: MAVLink_message,
         column_alias: t.Dict[str, str] = {},
         msg_id: int = 1,
         convert_to_datetime: bool = False,
+        max_rate_hz: int = None,
     ):
         msg_types = list(map(lambda x: cls.MSG_TYPES[x], msg.fieldtypes))
         columns = msg.get_fieldnames()
         name = msg.msgname
         return cls(
             name=name,
             columns=columns,
             types=msg_types,
             column_alias=column_alias,
             msg_id=msg_id,
             convert_to_datetime=convert_to_datetime,
+            max_rate_hz=max_rate_hz,
         )
 
     @property
     def fields(self) -> t.Dict[str, np.ndarray]:
         """
         The timeseries fields as a numpy array
         """
@@ -124,14 +165,17 @@
     def append_message(self, message: DFMessage) -> None:
         msg_dict = message.to_dict()
         msg_type = msg_dict["mavpackettype"]
 
         if msg_type != self.name:
             raise ValueError(f"Invalid message type, got {msg_type}, expected {self.name}")
 
+        if self._skip_messages and self._reduce_msg_rate(message):
+            return None
+
         timestamp = getattr(message, "_timestamp", None)
 
         msg_dict.pop("mavpackettype")
 
         if timestamp:
             if self._to_datetime:
                 self._fields["timestamp"].append(datetime.fromtimestamp(timestamp))
@@ -149,24 +193,26 @@
     def __init__(
         self,
         filepath: str,
         messages_to_ignore: t.List[str] = ["FMT", "FMTU"],
         types: t.List[str] = None,
         to_datetime: bool = False,
         map_columns: t.Dict[str, str] = {},
+        max_rate_hz: float = None,
     ):
         self._messages_ignore = messages_to_ignore
         self._mlog: mavutil.mavserial = mavutil.mavlink_connection(filepath)
 
         self._parsed_data: t.Dict[str, MavLinkMessageSeries] = {}
         self._msg_count = 0
         self._to_datetime = to_datetime
         self._map_columns = map_columns
         self._start_timestamp = None
         self._end_timestamp = None
+        self._max_rate_hz = max_rate_hz
 
     def __getitem__(self, item: str) -> MavLinkMessageSeries:
         return self._parsed_data[item]
 
     @property
     def parsed_data(self) -> t.Dict[str, MavLinkMessageSeries]:
         return self._parsed_data
@@ -245,37 +291,39 @@
     def __init__(
         self,
         filepath: str,
         messages_to_ignore: t.List[str] = ["FMT", "FMTU"],
         types: t.List[str] = None,
         to_datetime: bool = False,
         map_columns: t.Dict[str, str] = {},
+        max_rate_hz: float = None,
     ):
         super().__init__(
             filepath=filepath,
             messages_to_ignore=messages_to_ignore,
             types=types,
             to_datetime=to_datetime,
             map_columns=map_columns,
+            max_rate_hz=max_rate_hz,
         )
 
-        self.__set_parsed_data(types)
+        self._set_parsed_data(types)
 
-    def __set_parsed_data(self, types: t.List[str]):
+    def _set_parsed_data(self, types: t.List[str]):
         self._types = []
         for name, msg_id in self._mlog.name_to_id.items():
             fmt = self._mlog.formats[msg_id]
             msg_not_in_types = (types is not None) and (name not in types)
             ignore_type = (name in self._messages_ignore) or msg_not_in_types
             if ignore_type:
                 continue
 
             self._types.append(fmt.name)
             self._parsed_data[name] = MavLinkMessageSeries.from_df_format(
-                fmt, self._map_columns, msg_id, self._to_datetime
+                fmt, self._map_columns, msg_id, self._to_datetime, self._max_rate_hz
             )
         if not self._types:
             raise EmptyLogError("The log contains no message types")
 
 
 class MavTLog(MavLogBase):
     """
@@ -285,14 +333,15 @@
     def __init__(
         self,
         filepath: str,
         messages_to_ignore: t.List[str] = ["HEARTBEAT", "MAV"],
         types: t.List[str] = None,
         to_datetime: bool = False,
         map_columns: t.Dict[str, str] = {},
+        max_rate_hz: float = None,
     ):
         super().__init__(
             filepath=filepath,
             messages_to_ignore=messages_to_ignore,
             types=types,
             to_datetime=to_datetime,
             map_columns=map_columns,
@@ -307,11 +356,11 @@
             msg_not_in_types = (types is not None) and (name not in types)
             ignore_type = (name in self._messages_ignore) or msg_not_in_types
             if ignore_type:
                 continue
 
             self._types.append(name)
             self._parsed_data[name] = MavLinkMessageSeries.from_message(
-                msg, self._map_columns, msg_id, self._to_datetime
+                msg, self._map_columns, msg_id, self._to_datetime, self._max_rate_hz
             )
         if not self._types:
             raise EmptyLogError("The log contains no message types")
```

### Comparing `pymavlog-0.3.1/pyproject.toml` & `pymavlog-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pymavlog"
-version = "0.3.1"
+version = "0.4.0"
 description = "A lightweight python library to parse MavLink log files"
 readme = "README.md"
 license = "MIT"
 authors = [
     "Ricardo Martinez <rik@rmargar.net>"
 ]
 classifiers = [
```

### Comparing `pymavlog-0.3.1/PKG-INFO` & `pymavlog-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymavlog
-Version: 0.3.1
+Version: 0.4.0
 Summary: A lightweight python library to parse MavLink log files
 Home-page: https://github.com/rmargar/pymavlog
 License: MIT
 Author: Ricardo Martinez
 Author-email: rik@rmargar.net
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 1 - Planning
```

