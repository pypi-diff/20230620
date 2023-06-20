# Comparing `tmp/arcam-fmj-1.3.0.tar.gz` & `tmp/arcam-fmj-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arcam-fmj-1.3.0.tar", last modified: Wed Apr 19 19:00:15 2023, max compression
+gzip compressed data, was "arcam-fmj-1.4.0.tar", last modified: Tue Jun 20 08:53:29 2023, max compression
```

## Comparing `arcam-fmj-1.3.0.tar` & `arcam-fmj-1.4.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:00:15.739321 arcam-fmj-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-19 19:00:05.000000 arcam-fmj-1.3.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-04-19 19:00:15.739321 arcam-fmj-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-04-19 19:00:05.000000 arcam-fmj-1.3.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-19 19:00:15.739321 arcam-fmj-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-04-19 19:00:05.000000 arcam-fmj-1.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:00:15.739321 arcam-fmj-1.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:00:15.739321 arcam-fmj-1.3.0/src/arcam/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:00:15.739321 arcam-fmj-1.3.0/src/arcam/fmj/
--rw-r--r--   0 runner    (1001) docker     (123)    35847 2023-04-19 19:00:05.000000 arcam-fmj-1.3.0/src/arcam/fmj/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6872 2023-04-19 19:00:05.000000 arcam-fmj-1.3.0/src/arcam/fmj/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-04-19 19:00:05.000000 arcam-fmj-1.3.0/src/arcam/fmj/console.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 19:00:05.000000 arcam-fmj-1.3.0/src/arcam/fmj/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-04-19 19:00:05.000000 arcam-fmj-1.3.0/src/arcam/fmj/server.py
--rw-r--r--   0 runner    (1001) docker     (123)    15088 2023-04-19 19:00:05.000000 arcam-fmj-1.3.0/src/arcam/fmj/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-04-19 19:00:05.000000 arcam-fmj-1.3.0/src/arcam/fmj/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:00:15.739321 arcam-fmj-1.3.0/src/arcam_fmj.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-04-19 19:00:15.000000 arcam-fmj-1.3.0/src/arcam_fmj.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-19 19:00:15.000000 arcam-fmj-1.3.0/src/arcam_fmj.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 19:00:15.000000 arcam-fmj-1.3.0/src/arcam_fmj.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-19 19:00:15.000000 arcam-fmj-1.3.0/src/arcam_fmj.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-19 19:00:15.000000 arcam-fmj-1.3.0/src/arcam_fmj.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-19 19:00:15.000000 arcam-fmj-1.3.0/src/arcam_fmj.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:53:29.078013 arcam-fmj-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-20 08:53:15.000000 arcam-fmj-1.4.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-20 08:53:29.078013 arcam-fmj-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-06-20 08:53:15.000000 arcam-fmj-1.4.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-20 08:53:29.078013 arcam-fmj-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-06-20 08:53:15.000000 arcam-fmj-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:53:29.078013 arcam-fmj-1.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:53:29.078013 arcam-fmj-1.4.0/src/arcam/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:53:29.078013 arcam-fmj-1.4.0/src/arcam/fmj/
+-rw-r--r--   0 runner    (1001) docker     (123)    37106 2023-06-20 08:53:15.000000 arcam-fmj-1.4.0/src/arcam/fmj/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6872 2023-06-20 08:53:15.000000 arcam-fmj-1.4.0/src/arcam/fmj/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10056 2023-06-20 08:53:15.000000 arcam-fmj-1.4.0/src/arcam/fmj/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 08:53:15.000000 arcam-fmj-1.4.0/src/arcam/fmj/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-06-20 08:53:15.000000 arcam-fmj-1.4.0/src/arcam/fmj/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15606 2023-06-20 08:53:15.000000 arcam-fmj-1.4.0/src/arcam/fmj/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-06-20 08:53:15.000000 arcam-fmj-1.4.0/src/arcam/fmj/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:53:29.078013 arcam-fmj-1.4.0/src/arcam_fmj.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-20 08:53:29.000000 arcam-fmj-1.4.0/src/arcam_fmj.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-20 08:53:29.000000 arcam-fmj-1.4.0/src/arcam_fmj.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 08:53:29.000000 arcam-fmj-1.4.0/src/arcam_fmj.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-20 08:53:29.000000 arcam-fmj-1.4.0/src/arcam_fmj.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-20 08:53:29.000000 arcam-fmj-1.4.0/src/arcam_fmj.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-20 08:53:29.000000 arcam-fmj-1.4.0/src/arcam_fmj.egg-info/top_level.txt
```

### Comparing `arcam-fmj-1.3.0/LICENSE.txt` & `arcam-fmj-1.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `arcam-fmj-1.3.0/PKG-INFO` & `arcam-fmj-1.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arcam-fmj
-Version: 1.3.0
+Version: 1.4.0
 Summary: A python library for speaking to Arcam receivers
 Home-page: https://github.com/elupus/arcam_fmj
 Author: Joakim Plate
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
@@ -14,17 +14,16 @@
 Description-Content-Type: text/x-rst
 Provides-Extra: tests
 License-File: LICENSE.txt
 
 ********************************
 Arcam IP Control
 ********************************
-This module support controlling an arcam fmj received over it's network.
-It's built mainly for use with home-assistant project, but should work
-for other projects as well.
+This module supports controlling an Arcam FMJ receiver (as well as JBL and AudioControl processors) over the network.
+It's built mainly for use with the Home Assistant project, but should work for other projects as well.
 
 Status
 ______
 .. image:: https://github.com/elupus/arcam_fmj/actions/workflows/python-package.yml/badge.svg
     :target: https://github.com/elupus/arcam_fmj/actions
 
 Module
```

### Comparing `arcam-fmj-1.3.0/README.rst` & `arcam-fmj-1.4.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 ********************************
 Arcam IP Control
 ********************************
-This module support controlling an arcam fmj received over it's network.
-It's built mainly for use with home-assistant project, but should work
-for other projects as well.
+This module supports controlling an Arcam FMJ receiver (as well as JBL and AudioControl processors) over the network.
+It's built mainly for use with the Home Assistant project, but should work for other projects as well.
 
 Status
 ______
 .. image:: https://github.com/elupus/arcam_fmj/actions/workflows/python-package.yml/badge.svg
     :target: https://github.com/elupus/arcam_fmj/actions
 
 Module
```

### Comparing `arcam-fmj-1.3.0/setup.py` & `arcam-fmj-1.4.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, "README.rst"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="arcam-fmj",
-    version="1.3.0",
+    version="1.4.0",
     description="A python library for speaking to Arcam receivers",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     license="MIT",
     packages=["arcam.fmj"],
     package_dir={"": "src"},
     package_data = {
```

### Comparing `arcam-fmj-1.3.0/src/arcam/fmj/__init__.py` & `arcam-fmj-1.4.0/src/arcam/fmj/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,21 +79,25 @@
     def __init__(self, zn=None, cc=None, data=None):
         super().__init__(ac=AnswerCodes.INVALID_DATA_LENGTH,
                          zn=zn, cc=cc, data=data)
 
 class InvalidPacket(ArcamException):
     pass
 
+class NullPacket(ArcamException):
+    pass
+
 APIVERSION_450_SERIES = {"AVR380", "AVR450", "AVR750"}
 APIVERSION_860_SERIES = {"AV860", "AVR850", "AVR550", "AVR390", "SR250"}
 APIVERSION_SA_SERIES = {"SA10", "SA20", "SA30"}
 APIVERSION_HDA_SERIES = {"AVR5", "AVR10", "AVR20", "AVR30", "AV40", "AVR11", "AVR21", "ARV31", "AV41", "SDP-55", "SDP-58"}
 APIVERSION_HDA_PREMIUM_SERIES = {"AVR10", "AVR20", "AVR30", "AV40", "AVR11", "AVR21", "ARV31", "AV41", "SDP-55", "SDP-58"}
 APIVERSION_HDA_MULTI_ZONE_SERIES = {"AVR20", "AVR30", "AV40", "AVR21", "ARV31", "AV41", "SDP-55", "SDP-58"}
 APIVERSION_PA_SERIES = {"PA720", "PA240", "PA410"}
+APIVERSION_ST_SERIES = {"ST60"}
 
 APIVERSION_DAB_SERIES = {"AVR450", "AVR750"}
 APIVERSION_DAB_SERIES.update("AV860", "AVR850", "AVR550", "AVR390")
 APIVERSION_DAB_SERIES.update(APIVERSION_HDA_SERIES)
 
 APIVERSION_ZONE2_SERIES = set()
 APIVERSION_ZONE2_SERIES.update(APIVERSION_450_SERIES)
@@ -134,14 +138,15 @@
 
 class ApiModel(enum.Enum):
     API450_SERIES = 1
     API860_SERIES = 2
     APISA_SERIES = 3
     APIHDA_SERIES = 4
     APIPA_SERIES = 5
+    APIST_SERIES = 6
 
 _T = TypeVar("_T", bound="IntOrTypeEnum")
 class IntOrTypeEnum(enum.IntEnum):
     version: Optional[Set[str]]
 
     @classmethod
     def _missing_(cls, value):
@@ -321,14 +326,19 @@
     USB = enum.auto()
     STB = enum.auto()
     GAME = enum.auto()
     PHONO = enum.auto()
     ARC_ERC = enum.auto()
     UHD = enum.auto()
     BT = enum.auto()
+    DIG1 = enum.auto()
+    DIG2 = enum.auto()
+    DIG3 = enum.auto()
+    DIG4 = enum.auto()
+    NET_USB = enum.auto()
 
     @classmethod
     def from_bytes(cls, data: bytes, model: ApiModel, zn: int) -> 'SourceCodes':
         try:
             table = SOURCE_CODES[(model, zn)]
         except KeyError:
             raise ValueError("Unknown source map for model {} and zone {}".format(model, zn))
@@ -396,20 +406,27 @@
     AURO_MATIC_3D = 0x0F, APIVERSION_AURO_SERIES
     AURO_2D = 0x10, APIVERSION_AURO_SERIES
 
 
 POWER_WRITE_SUPPORTED = {
     ApiModel.APISA_SERIES,
     ApiModel.APIPA_SERIES,
+    ApiModel.APIST_SERIES,
 }
+
 MUTE_WRITE_SUPPORTED = POWER_WRITE_SUPPORTED
+
 SOURCE_WRITE_SUPPORTED = {
     ApiModel.APISA_SERIES,
 }
 
+VOLUME_STEP_SUPPORTED = {
+    ApiModel.APIST_SERIES,
+}
+
 DEFAULT_SOURCE_MAPPING = {
     SourceCodes.FOLLOW_ZONE_1: bytes([0x00]),
     SourceCodes.CD: bytes([0x01]),
     SourceCodes.BD: bytes([0x02]),
     SourceCodes.AV: bytes([0x03]),
     SourceCodes.SAT: bytes([0x04]),
     SourceCodes.PVR: bytes([0x05]),
@@ -456,23 +473,32 @@
     SourceCodes.SAT: bytes([0x08]),
     SourceCodes.GAME: bytes([0x09]),
     SourceCodes.NET: bytes([0x0B]),
     SourceCodes.USB: bytes([0x0B]),
     SourceCodes.ARC_ERC: bytes([0x0D]),
 }
 
+ST_SOURCE_MAPPING = {
+    SourceCodes.DIG1: bytes([0x01]),
+    SourceCodes.DIG2: bytes([0x02]),
+    SourceCodes.DIG3: bytes([0x03]),
+    SourceCodes.DIG4: bytes([0x04]),
+    SourceCodes.NET_USB: bytes([0x05]),
+}
+
 SOURCE_CODES = {
     (ApiModel.API450_SERIES, 1): DEFAULT_SOURCE_MAPPING,
     (ApiModel.API450_SERIES, 2): DEFAULT_SOURCE_MAPPING,
     (ApiModel.API860_SERIES, 1): DEFAULT_SOURCE_MAPPING,
     (ApiModel.API860_SERIES, 2): DEFAULT_SOURCE_MAPPING,
     (ApiModel.APIHDA_SERIES, 1): HDA_SOURCE_MAPPING,
     (ApiModel.APIHDA_SERIES, 2): HDA_SOURCE_MAPPING,
     (ApiModel.APISA_SERIES, 1): SA_SOURCE_MAPPING,
     (ApiModel.APISA_SERIES, 2): SA_SOURCE_MAPPING,
+    (ApiModel.APIST_SERIES, 1): ST_SOURCE_MAPPING,
 }
 
 RC5CODE_DECODE_MODE_MCH: Dict[Tuple[ApiModel, int], Dict[DecodeModeMCH, bytes]] = {
     (ApiModel.API450_SERIES, 1): {
         DecodeModeMCH.STEREO_DOWNMIX: bytes([16, 107]),
         DecodeModeMCH.MULTI_CHANNEL: bytes([16, 106]),
         DecodeModeMCH.DOLBY_D_EX_OR_DTS_ES: bytes([16, 118]),
@@ -548,14 +574,16 @@
         DecodeMode2CH.AURO_2D: bytes([16, 104]),
     },
     (ApiModel.APIHDA_SERIES, 2): {},
     (ApiModel.APISA_SERIES, 1): {},
     (ApiModel.APISA_SERIES, 2): {},
     (ApiModel.APIPA_SERIES, 1): {},
     (ApiModel.APIPA_SERIES, 2): {},
+    (ApiModel.APIST_SERIES, 1): {},
+    (ApiModel.APIST_SERIES, 2): {},
 }
 
 RC5CODE_SOURCE: Dict[Tuple[ApiModel, int], Dict[SourceCodes, bytes]] = {
     (ApiModel.API450_SERIES, 1): {
         SourceCodes.STB: bytes([16, 1]),
         SourceCodes.AV: bytes([16, 2]),
         SourceCodes.DAB: bytes([16, 72]),
@@ -674,14 +702,23 @@
         SourceCodes.AUX: bytes([16, 99]),
         SourceCodes.STB: bytes([16, 100]),
         SourceCodes.NET: bytes([16, 92]),
         SourceCodes.USB: bytes([16, 93]),
         SourceCodes.GAME: bytes([16, 97]),
         SourceCodes.ARC_ERC: bytes([16, 125])
     },
+    (ApiModel.APIST_SERIES, 1): {
+        SourceCodes.DIG1: bytes([21, 94]),
+        SourceCodes.DIG2: bytes([21, 98]),
+        SourceCodes.DIG3: bytes([21, 27]),
+        SourceCodes.DIG4: bytes([21, 97]),
+        SourceCodes.USB: bytes([21, 93]),
+        SourceCodes.NET: bytes([21, 92])
+    },
+    (ApiModel.APIST_SERIES, 2): {},
     (ApiModel.APIPA_SERIES, 1): {},
     (ApiModel.APIPA_SERIES, 2): {},
 }
 
 RC5CODE_POWER = {
     (ApiModel.API450_SERIES, 1): {
         True: bytes([16, 123]),
@@ -780,14 +817,18 @@
     (ApiModel.APISA_SERIES, 1): {
         True: bytes([16, 16]),
         False: bytes([16, 17]),
     },
     (ApiModel.APISA_SERIES, 2): {
         True: bytes([16, 16]),
         False: bytes([16, 17]),
+    },
+    (ApiModel.APIST_SERIES, 1): {
+        True: bytes([21, 86]),
+        False: bytes([21, 85]),
     }
 }
 
 class IncomingAudioFormat(IntOrTypeEnum):
     PCM = 0x00
     ANALOGUE_DIRECT = 0x01
     DOLBY_DIGITAL = 0x02
@@ -999,14 +1040,16 @@
         elif start == b"A":
             header = await reader.read(2)
             if header != b"MX":
                 raise InvalidPacket("Unexpected AMX header")
 
             data = await reader.readuntil(PROTOCOL_ETR)
             packet =  bytes([*start, *header, *data])
+        elif start == b"\x00":
+            raise NullPacket()
         else:
             raise InvalidPacket("unexpected str byte {!r}".format(start))
 
         return packet
 
     except TimeoutError as exception:
         raise ConnectionFailed() from exception
@@ -1032,14 +1075,17 @@
 async def read_response(reader: asyncio.StreamReader) -> Optional[Union[ResponsePacket, AmxDuetResponse]]:
     while True:
         try:
             data = await _read_response(reader)
         except InvalidPacket as e:
             _LOGGER.warning(str(e))
             continue
+        except NullPacket:
+            _LOGGER.debug("Ignoring 0x00 start byte sent from some devices")
+            continue
         return data
 
 
 async def _read_command(reader: asyncio.StreamReader) -> Optional[Union[CommandPacket, AmxDuetRequest]]:
     data = await _read_delimited(reader, 3)
     if not data:
         return None
```

### Comparing `arcam-fmj-1.3.0/src/arcam/fmj/client.py` & `arcam-fmj-1.4.0/src/arcam/fmj/client.py`

 * *Files identical despite different names*

### Comparing `arcam-fmj-1.3.0/src/arcam/fmj/console.py` & `arcam-fmj-1.4.0/src/arcam/fmj/console.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,14 +28,16 @@
 parser_state = subparsers.add_parser('state')
 parser_state.add_argument('--host', required=True)
 parser_state.add_argument('--port', default=50000)
 parser_state.add_argument('--zone', default=1, type=int)
 parser_state.add_argument('--volume', type=int)
 parser_state.add_argument('--source', type=auto_source)
 parser_state.add_argument('--monitor', action='store_true')
+parser_state.add_argument('--power-on', action=argparse.BooleanOptionalAction)
+parser_state.add_argument('--power-off', action=argparse.BooleanOptionalAction)
 
 parser_client = subparsers.add_parser('client')
 parser_client.add_argument('--host', required=True)
 parser_client.add_argument('--port', default=50000)
 parser_client.add_argument('--zone', default=1, type=int)
 parser_client.add_argument('--command', type=auto_int)
 parser_client.add_argument('--data', nargs='+', default=[0xF0], type=auto_int)
@@ -59,14 +61,20 @@
         await state.update()
 
         if args.volume is not None:
             await state.set_volume(args.volume)
 
         if args.source is not None:
             await state.set_source(args.source)
+        
+        if args.power_on is not None:
+            await state.set_power(True)
+
+        if args.power_off is not None:
+            await state.set_power(False)
 
         if args.monitor:
             async with state:
                 prev = repr(state)
                 while client.connected:
                     curr = repr(state)
                     if prev != curr:
```

### Comparing `arcam-fmj-1.3.0/src/arcam/fmj/server.py` & `arcam-fmj-1.4.0/src/arcam/fmj/server.py`

 * *Files identical despite different names*

### Comparing `arcam-fmj-1.3.0/src/arcam/fmj/state.py` & `arcam-fmj-1.4.0/src/arcam/fmj/state.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 from . import (
     APIVERSION_450_SERIES,
     APIVERSION_860_SERIES,
     APIVERSION_HDA_SERIES,
     APIVERSION_SA_SERIES,
     APIVERSION_PA_SERIES,
+    APIVERSION_ST_SERIES,
     AmxDuetRequest,
     AmxDuetResponse,
     AnswerCodes,
     ApiModel,
     CommandCodes,
     CommandInvalidAtThisTime,
     CommandNotRecognised,
@@ -25,14 +26,15 @@
     PresetDetail,
     ResponseException,
     ResponsePacket,
     SourceCodes,
     POWER_WRITE_SUPPORTED,
     MUTE_WRITE_SUPPORTED,
     SOURCE_WRITE_SUPPORTED,
+    VOLUME_STEP_SUPPORTED,
     RC5CODE_SOURCE,
     RC5CODE_POWER,
     RC5CODE_MUTE,
     RC5CODE_VOLUME,
     RC5CODE_DECODE_MODE_2CH,
     RC5CODE_DECODE_MODE_MCH,
 )
@@ -281,24 +283,28 @@
         return int.from_bytes(value, 'big')
 
     async def set_volume(self, volume: int) -> None:
         await self._client.request(
             self._zn, CommandCodes.VOLUME, bytes([volume]))
 
     async def inc_volume(self) -> None:
-        command = self.get_rc5code(RC5CODE_VOLUME, True)
-
-        await self._client.request(
-            self._zn, CommandCodes.SIMULATE_RC5_IR_COMMAND, command)
+        if self._api_model in VOLUME_STEP_SUPPORTED:
+            await self._client.request(self._zn, CommandCodes.VOLUME, bytes([0xF1]))
+        else:
+            command = self.get_rc5code(RC5CODE_VOLUME, True)
+            await self._client.request(
+                self._zn, CommandCodes.SIMULATE_RC5_IR_COMMAND, command)
 
     async def dec_volume(self) -> None:
-        command = self.get_rc5code(RC5CODE_VOLUME, False)
-
-        await self._client.request(
-            self._zn, CommandCodes.SIMULATE_RC5_IR_COMMAND, command)
+        if self._api_model in VOLUME_STEP_SUPPORTED:
+            await self._client.request(self._zn, CommandCodes.VOLUME, bytes([0xF2]))
+        else:
+            command = self.get_rc5code(RC5CODE_VOLUME, False)
+            await self._client.request(
+                self._zn, CommandCodes.SIMULATE_RC5_IR_COMMAND, command)
 
     def get_dab_station(self) -> Optional[str]:
         value = self._state.get(CommandCodes.DAB_STATION)
         if value is None:
             return None
         return value.decode('utf8').rstrip()
 
@@ -375,14 +381,17 @@
                     self._api_model = ApiModel.APIHDA_SERIES
 
                 if data.device_model in APIVERSION_SA_SERIES:
                     self._api_model = ApiModel.APISA_SERIES
 
                 if data.device_model in APIVERSION_PA_SERIES:
                     self._api_model = ApiModel.APIPA_SERIES
+                
+                if data.device_model in APIVERSION_ST_SERIES:
+                    self._api_model = ApiModel.APIST_SERIES
 
             except ResponseException as e:
                 _LOGGER.debug("Response error skipping %s", e.ac)
             except NotConnectedException as e:
                 _LOGGER.debug("Not connected skipping amx")
             except asyncio.TimeoutError:
                 _LOGGER.error("Timeout requesting amx")
```

### Comparing `arcam-fmj-1.3.0/src/arcam/fmj/utils.py` & `arcam-fmj-1.4.0/src/arcam/fmj/utils.py`

 * *Files identical despite different names*

### Comparing `arcam-fmj-1.3.0/src/arcam_fmj.egg-info/PKG-INFO` & `arcam-fmj-1.4.0/src/arcam_fmj.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arcam-fmj
-Version: 1.3.0
+Version: 1.4.0
 Summary: A python library for speaking to Arcam receivers
 Home-page: https://github.com/elupus/arcam_fmj
 Author: Joakim Plate
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
@@ -14,17 +14,16 @@
 Description-Content-Type: text/x-rst
 Provides-Extra: tests
 License-File: LICENSE.txt
 
 ********************************
 Arcam IP Control
 ********************************
-This module support controlling an arcam fmj received over it's network.
-It's built mainly for use with home-assistant project, but should work
-for other projects as well.
+This module supports controlling an Arcam FMJ receiver (as well as JBL and AudioControl processors) over the network.
+It's built mainly for use with the Home Assistant project, but should work for other projects as well.
 
 Status
 ______
 .. image:: https://github.com/elupus/arcam_fmj/actions/workflows/python-package.yml/badge.svg
     :target: https://github.com/elupus/arcam_fmj/actions
 
 Module
```

