# Comparing `tmp/ts_task_script_utils-1.7.0.tar.gz` & `tmp/ts_task_script_utils-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ts_task_script_utils-1.7.0.tar", max compression
+gzip compressed data, was "ts_task_script_utils-1.8.0.tar", max compression
```

## Comparing `ts_task_script_utils-1.7.0.tar` & `ts_task_script_utils-1.8.0.tar`

### file list

```diff
@@ -1,29 +1,30 @@
--rw-r--r--   0        0        0    11357 2023-05-22 17:11:52.874755 ts_task_script_utils-1.7.0/LICENSE
--rw-r--r--   0        0        0     6752 2023-05-22 17:11:52.874755 ts_task_script_utils-1.7.0/README.md
--rw-r--r--   0        0        0     1238 2023-05-22 17:11:52.878755 ts_task_script_utils-1.7.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-22 17:11:52.878755 ts_task_script_utils-1.7.0/task_script_utils/__init__.py
--rw-r--r--   0        0        0     1123 2023-05-22 17:11:52.878755 ts_task_script_utils-1.7.0/task_script_utils/check_file_type.py
--rw-r--r--   0        0        0     2454 2023-05-22 17:11:52.878755 ts_task_script_utils-1.7.0/task_script_utils/convert_datetime_to_ts_format.py
--rw-r--r--   0        0        0     3596 2023-05-22 17:11:52.878755 ts_task_script_utils-1.7.0/task_script_utils/datacubes/README.md
--rw-r--r--   0        0        0     5309 2023-05-22 17:11:52.878755 ts_task_script_utils-1.7.0/task_script_utils/datacubes/parquet.py
--rw-r--r--   0        0        0    24970 2023-05-22 17:11:52.878755 ts_task_script_utils-1.7.0/task_script_utils/datetime_parser/README.md
--rw-r--r--   0        0        0       96 2023-05-22 17:11:52.878755 ts_task_script_utils-1.7.0/task_script_utils/datetime_parser/__init__.py
--rw-r--r--   0        0        0     2680 2023-05-22 17:11:52.878755 ts_task_script_utils-1.7.0/task_script_utils/datetime_parser/datetime_config.py
--rw-r--r--   0        0        0    30200 2023-05-22 17:11:52.878755 ts_task_script_utils-1.7.0/task_script_utils/datetime_parser/datetime_info.py
--rw-r--r--   0        0        0    88298 2023-05-22 17:11:52.878755 ts_task_script_utils-1.7.0/task_script_utils/datetime_parser/flowcharts/parse.png
--rw-r--r--   0        0        0    70421 2023-05-22 17:11:52.878755 ts_task_script_utils-1.7.0/task_script_utils/datetime_parser/flowcharts/short-date-format-resolution.png
--rw-r--r--   0        0        0     1827 2023-05-22 17:11:52.878755 ts_task_script_utils-1.7.0/task_script_utils/datetime_parser/fractional_seconds_formatter.py
--rw-r--r--   0        0        0   104888 2023-05-22 17:11:52.878755 ts_task_script_utils-1.7.0/task_script_utils/datetime_parser/parse-white.png
--rw-r--r--   0        0        0     2248 2023-05-22 17:11:52.878755 ts_task_script_utils-1.7.0/task_script_utils/datetime_parser/parser.py
--rw-r--r--   0        0        0      841 2023-05-22 17:11:52.878755 ts_task_script_utils-1.7.0/task_script_utils/datetime_parser/parser_exceptions.py
--rw-r--r--   0        0        0     3999 2023-05-22 17:11:52.878755 ts_task_script_utils-1.7.0/task_script_utils/datetime_parser/ts_datetime.py
--rw-r--r--   0        0        0      178 2023-05-22 17:11:52.878755 ts_task_script_utils-1.7.0/task_script_utils/datetime_parser/tz_dicts.py
--rw-r--r--   0        0        0     2357 2023-05-22 17:11:52.878755 ts_task_script_utils-1.7.0/task_script_utils/datetime_parser/tz_list.py
--rw-r--r--   0        0        0     3710 2023-05-22 17:11:52.878755 ts_task_script_utils-1.7.0/task_script_utils/datetime_parser/utils/manipulation.py
--rw-r--r--   0        0        0     4558 2023-05-22 17:11:52.878755 ts_task_script_utils-1.7.0/task_script_utils/datetime_parser/utils/parsing.py
--rw-r--r--   0        0        0     7486 2023-05-22 17:11:52.878755 ts_task_script_utils-1.7.0/task_script_utils/extract_to_decorate.py
--rw-r--r--   0        0        0      424 2023-05-22 17:11:52.878755 ts_task_script_utils-1.7.0/task_script_utils/is_number.py
--rw-r--r--   0        0        0     4227 2023-05-22 17:11:52.878755 ts_task_script_utils-1.7.0/task_script_utils/parse.py
--rw-r--r--   0        0        0     2795 2023-05-22 17:11:52.878755 ts_task_script_utils-1.7.0/task_script_utils/random.py
--rw-r--r--   0        0        0     3153 2023-05-22 17:11:52.882755 ts_task_script_utils-1.7.0/task_script_utils/workflow_logging.py
--rw-r--r--   0        0        0     7680 1970-01-01 00:00:00.000000 ts_task_script_utils-1.7.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-20 15:48:19.225946 ts_task_script_utils-1.8.0/LICENSE
+-rw-r--r--   0        0        0     9323 2023-06-20 15:48:19.225946 ts_task_script_utils-1.8.0/README.md
+-rw-r--r--   0        0        0     1238 2023-06-20 15:48:19.229946 ts_task_script_utils-1.8.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-20 15:48:19.229946 ts_task_script_utils-1.8.0/task_script_utils/__init__.py
+-rw-r--r--   0        0        0     1139 2023-06-20 15:48:19.229946 ts_task_script_utils-1.8.0/task_script_utils/check_file_type.py
+-rw-r--r--   0        0        0     2471 2023-06-20 15:48:19.229946 ts_task_script_utils-1.8.0/task_script_utils/convert_datetime_to_ts_format.py
+-rw-r--r--   0        0        0     3596 2023-06-20 15:48:19.229946 ts_task_script_utils-1.8.0/task_script_utils/datacubes/README.md
+-rw-r--r--   0        0        0     5339 2023-06-20 15:48:19.229946 ts_task_script_utils-1.8.0/task_script_utils/datacubes/parquet.py
+-rw-r--r--   0        0        0    24970 2023-06-20 15:48:19.229946 ts_task_script_utils-1.8.0/task_script_utils/datetime_parser/README.md
+-rw-r--r--   0        0        0       96 2023-06-20 15:48:19.229946 ts_task_script_utils-1.8.0/task_script_utils/datetime_parser/__init__.py
+-rw-r--r--   0        0        0     2691 2023-06-20 15:48:19.229946 ts_task_script_utils-1.8.0/task_script_utils/datetime_parser/datetime_config.py
+-rw-r--r--   0        0        0    30167 2023-06-20 15:48:19.229946 ts_task_script_utils-1.8.0/task_script_utils/datetime_parser/datetime_info.py
+-rw-r--r--   0        0        0    88298 2023-06-20 15:48:19.233946 ts_task_script_utils-1.8.0/task_script_utils/datetime_parser/flowcharts/parse.png
+-rw-r--r--   0        0        0    70421 2023-06-20 15:48:19.233946 ts_task_script_utils-1.8.0/task_script_utils/datetime_parser/flowcharts/short-date-format-resolution.png
+-rw-r--r--   0        0        0     1827 2023-06-20 15:48:19.233946 ts_task_script_utils-1.8.0/task_script_utils/datetime_parser/fractional_seconds_formatter.py
+-rw-r--r--   0        0        0   104888 2023-06-20 15:48:19.233946 ts_task_script_utils-1.8.0/task_script_utils/datetime_parser/parse-white.png
+-rw-r--r--   0        0        0     2240 2023-06-20 15:48:19.233946 ts_task_script_utils-1.8.0/task_script_utils/datetime_parser/parser.py
+-rw-r--r--   0        0        0      841 2023-06-20 15:48:19.233946 ts_task_script_utils-1.8.0/task_script_utils/datetime_parser/parser_exceptions.py
+-rw-r--r--   0        0        0     4407 2023-06-20 15:48:19.233946 ts_task_script_utils-1.8.0/task_script_utils/datetime_parser/ts_datetime.py
+-rw-r--r--   0        0        0      178 2023-06-20 15:48:19.233946 ts_task_script_utils-1.8.0/task_script_utils/datetime_parser/tz_dicts.py
+-rw-r--r--   0        0        0     2357 2023-06-20 15:48:19.233946 ts_task_script_utils-1.8.0/task_script_utils/datetime_parser/tz_list.py
+-rw-r--r--   0        0        0     3897 2023-06-20 15:48:19.233946 ts_task_script_utils-1.8.0/task_script_utils/datetime_parser/utils/manipulation.py
+-rw-r--r--   0        0        0     4560 2023-06-20 15:48:19.233946 ts_task_script_utils-1.8.0/task_script_utils/datetime_parser/utils/parsing.py
+-rw-r--r--   0        0        0     7524 2023-06-20 15:48:19.233946 ts_task_script_utils-1.8.0/task_script_utils/extract_to_decorate.py
+-rw-r--r--   0        0        0      424 2023-06-20 15:48:19.233946 ts_task_script_utils-1.8.0/task_script_utils/is_number.py
+-rw-r--r--   0        0        0     4218 2023-06-20 15:48:19.233946 ts_task_script_utils-1.8.0/task_script_utils/parse.py
+-rw-r--r--   0        0        0     3023 2023-06-20 15:48:19.233946 ts_task_script_utils-1.8.0/task_script_utils/plate_reader.py
+-rw-r--r--   0        0        0     3282 2023-06-20 15:48:19.233946 ts_task_script_utils-1.8.0/task_script_utils/random.py
+-rw-r--r--   0        0        0     3153 2023-06-20 15:48:19.233946 ts_task_script_utils-1.8.0/task_script_utils/workflow_logging.py
+-rw-r--r--   0        0        0    10251 1970-01-01 00:00:00.000000 ts_task_script_utils-1.8.0/PKG-INFO
```

### Comparing `ts_task_script_utils-1.7.0/LICENSE` & `ts_task_script_utils-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ts_task_script_utils-1.7.0/pyproject.toml` & `ts_task_script_utils-1.8.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 line-length = 88
 target-version = ['py37', 'py38', 'py39']
 include = '\.pyi?$'
 extend-exclude = 'snapshots'
 
 [tool.poetry]
 name = "ts-task-script-utils"
-version = "1.7.0"
+version = "1.8.0"
 description = "Python utility for Tetra Task Scripts"
 authors = ["Tetrascience <developers@tetrascience.com>"]
 license = "Apache License 2.0"
 readme = "README.md"
 include = ["LICENSE"]
 classifiers =[
   "Programming Language :: Python :: 3",
```

### Comparing `ts_task_script_utils-1.7.0/task_script_utils/check_file_type.py` & `ts_task_script_utils-1.8.0/task_script_utils/check_file_type.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,19 +10,19 @@
         expected_type (t.Union[str, list]): either a string with the expected
         filetype or a list of strings with expected file types
     """
     # get the extension from filename
 
     extension = filename.rstrip().split(".")[-1].lower()
     try:
-        if type(expected_type) == str:
+        if isinstance(expected_type, str):
             # lower case both the extension and expected_type, do a string match
             assert extension == expected_type.lower()
-        elif type(expected_type) == list:
+        elif isinstance(expected_type, list):
             assert extension in [file_type.lower() for file_type in expected_type]
         else:
             raise ValueError(f"expected string or list but received {expected_type}")
     except AssertionError:
         sys.exit(
-            # pylint: disable=C0301
+            # pylint: disable=line-too-long
             f"The pipeline is expecting the file type to be {expected_type}, but the provided file has a file type of {extension}."  # noqa E501
         )
```

### Comparing `ts_task_script_utils-1.7.0/task_script_utils/convert_datetime_to_ts_format.py` & `ts_task_script_utils-1.8.0/task_script_utils/convert_datetime_to_ts_format.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-from typing import Union
 import warnings
-import dateparser
+from typing import Union
+
 import arrow
+import dateparser
 from dateutil import tz
 
 
 def convert_datetime_to_ts_format(
     datetime, datetime_format: str = "", timezone: Union[tz.tzoffset, str] = ""
 ):
     """
@@ -39,26 +40,26 @@
         parser_name = "arrow"
     else:
         parsed_time = dateparser.parse(datetime)
         parser_name = "dateparser"
 
     if parsed_time is None:
         raise ValueError(
-            # pylint: disable=C0301
+            # pylint: disable=line-too-long
             f"Could not parse input datetime string {datetime} using {parser_name} and the following input formats: {datetime_format}"  # noqa: E501
         )
 
     timezone_to_use = parsed_time.tzinfo
 
     if timezone:
         try:
             timezone_to_use = tz.gettz(timezone)
         except TypeError:
             warnings.warn(
-                # pylint: disable=C0301
+                # pylint: disable=line-too-long
                 "The provided timezone can't be parsed by dateutil tz, going to use the plain value"  # noqa: E501
             )
             timezone_to_use = timezone
 
     datetime_iso_local = ""
     utc_indicator = ""
```

### Comparing `ts_task_script_utils-1.7.0/task_script_utils/datacubes/README.md` & `ts_task_script_utils-1.8.0/task_script_utils/datacubes/README.md`

 * *Files identical despite different names*

### Comparing `ts_task_script_utils-1.7.0/task_script_utils/datacubes/parquet.py` & `ts_task_script_utils-1.8.0/task_script_utils/datacubes/parquet.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,18 +43,18 @@
         measure_arrays = np.array(measures, dtype=np.float_)
     except ValueError as exception:
         raise ValueError(
             "Measure data can only contain null or numeric values when converting to Parquet."
         ) from exception
 
     # Check measures and dimensions have compatible shapes
-    for i, measure_array in enumerate(measure_arrays):
+    for idx, measure_array in enumerate(measure_arrays):
         if measure_array.shape != dimension_shape:
             raise ValueError(
-                f"Measure {i} has a shape of {measure_array.shape} which is "
+                f"Measure {idx} has a shape of {measure_array.shape} which is "
                 f"incompatible with the dimension shape of {dimension_shape}."
             )
 
     # Reshape all measures from N-dimensional arrays of shape (a, b, c, ...) into a
     # table with shape (a*b*c*..., M) for M measures
     flat_measures = np.stack([measure.flatten() for measure in measure_arrays]).T
 
@@ -67,24 +67,24 @@
 
 
 def dataframe_to_parquet(df: pd.DataFrame) -> bytes:
     """Create a parquet file as bytes from a Pandas DataFrame"""
     # `fastparquet` needs to write to a file-like object and doesn't accept BytesIO.
     # An in-memory file system using `fsspec` is recommended here:
     # https://github.com/dask/fastparquet/issues/586#issuecomment-861647325
-    fs = fsspec.filesystem("memory")
+    file_sys = fsspec.filesystem("memory")
     temp_parquet_path = "memory://temp.parquet"
 
     # Pandas can write DataFrames to parquet with the engines `fastparquet` or `pyarrow`
     # which must be installed separately. `fastparquet` is used because it is a smaller
     # dependency.
     df.to_parquet(temp_parquet_path, engine="fastparquet")
-    parquet_bytes = fs.cat(temp_parquet_path)
+    parquet_bytes = file_sys.cat(temp_parquet_path)
 
-    fs.delete(temp_parquet_path)
+    file_sys.delete(temp_parquet_path)
 
     return parquet_bytes
 
 
 # Overload type hints for 1D, 2D, 3D and 4D datacubes (assuming 5D and above are rare)
 # This annotates that N `dimensions` correspond to N levels of nesting in `measures`,
 # so that type checkers can raise errors for this kind of incompatibility
@@ -134,9 +134,9 @@
         [[1, 2, 3]],
         [[4, 5, 6]]
     )
 
     datacube_parquet = datacube_to_parquet(dimensions, measures)
     ```
     """
-    df = datacube_to_dataframe(dimensions, measures)
-    return dataframe_to_parquet(df)
+    dframe = datacube_to_dataframe(dimensions, measures)
+    return dataframe_to_parquet(dframe)
```

### Comparing `ts_task_script_utils-1.7.0/task_script_utils/datetime_parser/README.md` & `ts_task_script_utils-1.8.0/task_script_utils/datetime_parser/README.md`

 * *Files identical despite different names*

### Comparing `ts_task_script_utils-1.7.0/task_script_utils/datetime_parser/datetime_config.py` & `ts_task_script_utils-1.8.0/task_script_utils/datetime_parser/datetime_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from typing import Optional
+
 from .utils.manipulation import map_offset_to_seconds
 
 
-# pylint: disable=R0903
 class DatetimeConfig:
     """DatetimeConfig provides complementary information on how to mark
     parsed digits as day, month or year.
     It also provides an option to handle abbreviated time zones and
     fold for parsing ambiguous timestamps during daylight saving transitions.
     Ideally, DatetimeConfig should be constructed from pipeline configuration
     passed to task scripts.
     """
 
+    # pylint: disable=W0102,R0913
     def __init__(
         self,
         day_first: Optional[bool] = None,
         year_first: Optional[bool] = None,
         tz_dict: dict = {},
         fold: Optional[int] = None,
         require_unambiguous_formats: bool = False,
```

### Comparing `ts_task_script_utils-1.7.0/task_script_utils/datetime_parser/datetime_info.py` & `ts_task_script_utils-1.8.0/task_script_utils/datetime_parser/datetime_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-import re
 import json
+import re
 from datetime import datetime as dt
 from itertools import product
 from typing import Optional, Tuple
 
 import pendulum
 from pendulum.locales.en import locale
 
 # pylint: disable=C0401
 from pydash.arrays import flatten
 
 from .datetime_config import DatetimeConfig
-from .tz_list import _all_abbreviated_tz_list
-from .ts_datetime import TSDatetime
-from .utils.parsing import _parse_with_formats
 from .parser_exceptions import (
+    AmbiguousDateError,
     DatetimeParserError,
-    InvalidOffsetError,
-    OffsetNotKnownError,
     InvalidDateError,
+    InvalidOffsetError,
     InvalidTimeError,
+    InvalidYearError,
     MultipleOffsetsError,
-    AmbiguousDateError,
     MultipleTimesFoundError,
-    InvalidYearError,
+    OffsetNotKnownError,
 )
+from .ts_datetime import TSDatetime
+from .tz_list import _all_abbreviated_tz_list
+from .utils.parsing import _parse_with_formats
 
 
 # pylint: disable=R0902
 class DateTimeInfo:
     """DatetimeInfo acts as base class for ShortDatetimeInfo and
     LongDatetimeInfo. This class definer the parsing logic. _parse
     takes a list of matcher functions. Child class should define
@@ -125,21 +125,16 @@
 
         Returns:
             str/None: A datetime string
         """
         if self.parsed_datetime:
             return self.parsed_datetime.isoformat()
 
-        if (
-            self.day
-            and self.month
-            and self.year
-            and self.hour
-            and self.minutes
-            and self.seconds
+        if all(
+            [self.day, self.month, self.year, self.hour, self.minutes, self.seconds]
         ):
             dt_str = f"{self.year}-{self.month}-{self.day}"
             dt_str += f" {self.hour}:{self.minutes}:{self.seconds}"
             if self.fractional_seconds:
                 # This property along with dt_format is used to create
                 # a datetime object. Since python datetime support 6 digits for
                 # microseconds, therefore truncating fraction seconds to
@@ -229,15 +224,15 @@
 
         offset = datetime_.strftime("%z")
         if offset:
             sign = offset[0]
             val = offset[1:]
             self.offset_ = f"{sign}{val[:2]}:{val[2:]}"
 
-        self.fractional_seconds = ts_datetime._subseconds
+        self.fractional_seconds = ts_datetime.subseconds
         self.parsed_datetime = ts_datetime
 
 
 class LongDateTimeInfo(DateTimeInfo):
     """LongDatetimeInfo defines matchers:
     - `_match_day_of_week_token`
     - `_match_month_token`
@@ -470,15 +465,15 @@
             - InvalidTimeError: When time like string is parsed, but the
             numeric value of hrs, minutes and seconds are out of bound.
 
         Returns:
             bool: Returns True if time is parsed successfully, else
             return False
         """
-        # pylint: disable=C0301
+        # pylint: disable=line-too-long
         hh_mm_ss_pattern = r"\d{1,2}:\d{1,2}:\d{1,2}\.\d+|^\d{1,2}:\d{1,2}:\d{1,2}$|^\d{1,2}:\d{1,2}:\d{1,2}[+-]"  # noqa E501
         hh_mm_pattern = r"^(?![+-])\d{1,2}:\d{1,2}$|^(?![+-])\d{1,2}:\d{1,2}[+-]{1,1}"
 
         matches = re.findall(hh_mm_ss_pattern, token)
         if not matches:
             matches = re.findall(hh_mm_pattern, token)
             if not matches:
@@ -691,15 +686,15 @@
                 day, month = self._disambiguate_day_and_month(*others)
 
         # Validate day, year, month
         try:
             dt(day=int(day), month=int(month), year=int(year))
         except ValueError as val_error:
             msg = f"{str(val_error)}, date={date_parts}, config={self.config}"
-            raise InvalidDateError(msg)
+            raise InvalidDateError(msg) from val_error
 
         day = f"{int(day):02d}"
         month = f"{int(month):02d}"
 
         return day, month, year
 
     # pylint: disable=R0912
@@ -755,15 +750,15 @@
         month = f"{int(month):02d}"
 
         # Validate day, year, month
         try:
             dt(day=int(day), month=int(month), year=int(year))
         except ValueError as val_error:
             msg = f"{str(val_error)}, date={'-'.join(date_parts)}, {self.config}"
-            raise InvalidDateError(msg)
+            raise InvalidDateError(msg) from val_error
 
         return day, month, year
 
     @staticmethod
     def _disambiguate_day_and_month(first_token: str, second_token: str) -> tuple:
         """Takes two tokens as input and tries to
         decide which token is day and which is month.
```

### Comparing `ts_task_script_utils-1.7.0/task_script_utils/datetime_parser/flowcharts/parse.png` & `ts_task_script_utils-1.8.0/task_script_utils/datetime_parser/flowcharts/parse.png`

 * *Files identical despite different names*

### Comparing `ts_task_script_utils-1.7.0/task_script_utils/datetime_parser/flowcharts/short-date-format-resolution.png` & `ts_task_script_utils-1.8.0/task_script_utils/datetime_parser/flowcharts/short-date-format-resolution.png`

 * *Files identical despite different names*

### Comparing `ts_task_script_utils-1.7.0/task_script_utils/datetime_parser/fractional_seconds_formatter.py` & `ts_task_script_utils-1.8.0/task_script_utils/datetime_parser/fractional_seconds_formatter.py`

 * *Files identical despite different names*

### Comparing `ts_task_script_utils-1.7.0/task_script_utils/datetime_parser/parse-white.png` & `ts_task_script_utils-1.8.0/task_script_utils/datetime_parser/parse-white.png`

 * *Files identical despite different names*

### Comparing `ts_task_script_utils-1.7.0/task_script_utils/datetime_parser/parser.py` & `ts_task_script_utils-1.8.0/task_script_utils/datetime_parser/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from typing import Sequence
 
 import pendulum
-from task_script_utils.datetime_parser.parser_exceptions import (
-    DatetimeParserError,
-)
+
+from task_script_utils.datetime_parser.parser_exceptions import DatetimeParserError
 from task_script_utils.datetime_parser.ts_datetime import TSDatetime
 
 from .datetime_config import DEFAULT_DATETIME_CONFIG, DatetimeConfig
-from .datetime_info import ShortDateTimeInfo, LongDateTimeInfo
-from .utils.parsing import _parse_with_formats
+from .datetime_info import LongDateTimeInfo, ShortDateTimeInfo
 from .utils.manipulation import replace_z_with_offset
+from .utils.parsing import _parse_with_formats
 
 
 def parse(
     datetime_raw_str: str,
     formats: Sequence[str] = (),
     config: DatetimeConfig = DEFAULT_DATETIME_CONFIG,
 ) -> TSDatetime:
```

### Comparing `ts_task_script_utils-1.7.0/task_script_utils/datetime_parser/parser_exceptions.py` & `ts_task_script_utils-1.8.0/task_script_utils/datetime_parser/parser_exceptions.py`

 * *Files identical despite different names*

### Comparing `ts_task_script_utils-1.7.0/task_script_utils/datetime_parser/ts_datetime.py` & `ts_task_script_utils-1.8.0/task_script_utils/datetime_parser/ts_datetime.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,14 +17,25 @@
         if not isinstance(datetime_, datetime):
             raise TypeError("datetime_ must be a datetime object")
 
         self._datetime: datetime = datetime_
         self._subseconds: Optional[str] = subseconds
 
     @property
+    def subseconds(self) -> Optional[str]:
+        """
+        Subseconds represent fractional part of seconds value that was parsed from
+        raw datetime as string.
+        eg: In `05-26-1991 12:12:23.000000023`, `000000023` as string would represent
+        subseconds.
+        Subseconds is None when it is not present in raw datetime string
+        """
+        return self._subseconds
+
+    @property
     def tzinfo(self) -> datetime.tzinfo:
         """Returns tzinfo for the stored datetime object"""
         return self._datetime.tzinfo
 
     @property
     def datetime(self) -> datetime:
         """Return a new `datetime` object after replacing `microseconds`
```

### Comparing `ts_task_script_utils-1.7.0/task_script_utils/datetime_parser/tz_list.py` & `ts_task_script_utils-1.8.0/task_script_utils/datetime_parser/tz_list.py`

 * *Files identical despite different names*

### Comparing `ts_task_script_utils-1.7.0/task_script_utils/datetime_parser/utils/manipulation.py` & `ts_task_script_utils-1.8.0/task_script_utils/datetime_parser/utils/manipulation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import datetime as dt
 import re
 from itertools import product
 from typing import Mapping, Optional, Sequence, Tuple
 
+from pendulum import datetime as pendulum_datetime
 from pendulum import now
 from pendulum.tz import timezone as pendulum_timezone
-from pendulum import datetime as pendulum_datetime
 from pydash.arrays import flatten
+
 from task_script_utils.datetime_parser.fractional_seconds_formatter import (
     FractionalSecondsFormatter,
 )
 from task_script_utils.datetime_parser.ts_datetime import TSDatetime
 
 _formatter = FractionalSecondsFormatter()
 
@@ -30,24 +31,26 @@
     return {
         tz.upper(): convert_offset_to_seconds(utc_offset)
         for tz, utc_offset in tz_dict.items()
     }
 
 
 def get_time_formats_for_long_date(fractional_seconds: Optional[str]) -> Tuple:
+    """Generate time parts(tokens) for long datetime formats"""
+
     def map_am_pm(time_format):
         return time_format if time_format.startswith("H") else time_format + " A"
 
     time_formats = [":".join(tokens) for tokens in product(*TIME_PARTS)]
     if fractional_seconds:
         token = "SSSSSS"
         time_formats = map(lambda x: [x, f"{x}.{token}"], time_formats)
 
     time_formats = flatten(time_formats)
-    time_formats = map(lambda x: map_am_pm(x), time_formats)
+    time_formats = [map_am_pm(format) for format in time_formats]
     time_formats = map(
         lambda x: [x, x + " Z", x + " z", x + " ZZ", x + " Z z", x + " ZZ z"],
         time_formats,
     )
     time_formats = flatten(time_formats)
     return tuple(time_formats)
 
@@ -74,14 +77,17 @@
     """
     for tz_name in tz_dict:
         if tz_name in datetime_str:
             return datetime_str.replace(tz_name, tz_dict[tz_name])
     return datetime_str
 
 
+# pylint: disable=invalid-name
+# `Z` is token to specify timezone. Function name, in this case,
+# conveys the logic
 def replace_zz_with_Z(formats: Sequence[str] = ()):
     """
     eg. `DD-MM-YYYY hh:m:ss zz` -> `DD-MM-YYYY hh:m:ss Z`
     """
     result_formats = list(formats)
     for idx, format_ in enumerate(result_formats):
         if "zz" in format_:
```

### Comparing `ts_task_script_utils-1.7.0/task_script_utils/datetime_parser/utils/parsing.py` & `ts_task_script_utils-1.8.0/task_script_utils/datetime_parser/utils/parsing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 from collections import Counter
 from copy import copy
 from re import error as re_error
 from typing import Optional, Sequence, Tuple
+
 import pendulum
-from task_script_utils.datetime_parser.ts_datetime import TSDatetime
-from task_script_utils.datetime_parser.utils.manipulation import (
-    replace_z_with_offset,
-    replace_abbreviated_tz_with_utc_offset,
-    replace_zz_with_Z,
-    from_pendulum_format,
+
+from task_script_utils.datetime_parser.datetime_config import (
+    DEFAULT_DATETIME_CONFIG,
+    DatetimeConfig,
 )
 from task_script_utils.datetime_parser.parser_exceptions import (
-    DatetimeParserError,
     AmbiguousDatetimeFormatsError,
+    DatetimeParserError,
 )
-from task_script_utils.datetime_parser.datetime_config import (
-    DEFAULT_DATETIME_CONFIG,
-    DatetimeConfig,
+from task_script_utils.datetime_parser.ts_datetime import TSDatetime
+from task_script_utils.datetime_parser.utils.manipulation import (
+    from_pendulum_format,
+    replace_abbreviated_tz_with_utc_offset,
+    replace_z_with_offset,
+    replace_zz_with_Z,
 )
 
 
 def parse_with_formats(
     datetime_raw_str: str,
     formats: Sequence[str] = (),
     config: DatetimeConfig = DEFAULT_DATETIME_CONFIG,
```

### Comparing `ts_task_script_utils-1.7.0/task_script_utils/extract_to_decorate.py` & `ts_task_script_utils-1.8.0/task_script_utils/extract_to_decorate.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """
 Derived from extract-to-decorate function from ts-task-script-file-util
 """
 
 from __future__ import annotations
-from typing import Callable, Dict, List
 
 import re
+from typing import Callable, Dict, List
+
 import pydash
 
 
 def process_metadata(function: Callable, metadata: Dict[str, any]) -> Dict[str, any]:
     """
     Applies a function to all values in a metadata object.
     :param function: a function that can be applied to a string
@@ -65,17 +66,17 @@
 
 def sanitize_output(text: str) -> str:
     """
     Removes characters that will cause pipeline errors if in metadata.
     Currently, the Regex for metadata values is ^[0-9a-zA-Z-_+.,/ ]+$
     Replaces with whitespace, then reduces multiple adjoining whitespace to single
     """
-    ILLEGAL_CHAR_REGEX = re.compile(r"[^0-9a-zA-Z-_+.,/ ]")
+    illegal_char_regex = re.compile(r"[^0-9a-zA-Z-_+.,/ ]")
 
-    replaced_text = ILLEGAL_CHAR_REGEX.sub(" ", text)
+    replaced_text = illegal_char_regex.sub(" ", text)
 
     # Remove multiple adjoining spaces
     # (e.g. "A & B" becomes "A B" instead of "A   B")
     return " ".join([t for t in replaced_text.split(" ") if t != ""])
 
 
 def do_mapping_extraction(
@@ -161,14 +162,15 @@
     return (
         metadata,
         pydash.uniq(tags),
         pydash.uniq_by(labels, lambda l: f"{l['name']}@{l['value']}"),
     )
 
 
+# pylint: disable=too-many-arguments
 def extract_to_decorate(
     mappings: List[Dict[str, any]],
     source_value: str,
     re_flags=0,
     sanitize=False,
     title_case=False,
     logger: Callable = print,
```

### Comparing `ts_task_script_utils-1.7.0/task_script_utils/parse.py` & `ts_task_script_utils-1.8.0/task_script_utils/parse.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 """A collection of useful functions to parse raw values into a more useable form."""
-import math
 from collections import defaultdict
-
 from decimal import Decimal, InvalidOperation
 from typing import DefaultDict, Optional, Set
 
 
 def to_int(value: str) -> Optional[int]:
     """
     Converts given value to its equivalent integer.
@@ -106,19 +104,19 @@
     for original_value in false_set:
         lowercase_value = to_lowercase(original_value)
         false_set_compare[lowercase_value].add(lowercase_value)
 
     true_and_false_intersection = set(true_set_compare) & set(false_set_compare)
     if true_and_false_intersection:
         true_intersection: Set[str] = set()
-        for value in true_and_false_intersection:
-            true_intersection.update(true_set_compare[value])
+        for value_ in true_and_false_intersection:
+            true_intersection.update(true_set_compare[value_])
         false_intersection: Set[str] = set()
-        for value in true_and_false_intersection:
-            false_intersection.update(false_set_compare[value])
+        for value_ in true_and_false_intersection:
+            false_intersection.update(false_set_compare[value_])
 
         raise ValueError(
             f"'true_set' and 'false_set' have values in common. "
             f"true_set: ({', '.join(true_intersection)}). "
             f"false_set: ({', '.join(false_intersection)})."
         )
```

### Comparing `ts_task_script_utils-1.7.0/task_script_utils/random.py` & `ts_task_script_utils-1.8.0/task_script_utils/random.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,46 @@
 """Utility to generate a random UUID"""
 import random as _py_random
 import uuid as _uuid
 from hashlib import sha512
-from typing import Hashable
+from typing import Any, Dict, Hashable, Type, TypeVar
 
 
-class NoPreviouslyCreatedSingletonError(Exception):
-    pass
+class NoPreviouslyCreatedInstanceError(Exception):
+    """No previously created instance error"""
 
 
-class Singleton(type):
-    _instances = {}
-    _last_created_instance = None
+T = TypeVar("T")
+
+
+class CacheLast(type):
+    """Metaclass that caches the last created instance"""
+
+    # _last_created_instance is a heterogeneous collection of type dict[Type[T], T] for
+    # the different T's that use this metaclass
+    _last_created_instance: Dict[Any, Any] = {}
 
     def __call__(cls, *args, **kwargs):
-        key = (cls, args)
-        if key not in cls._instances:
-            cls._instances[key] = super(Singleton, cls).__call__(*args, **kwargs)
-        cls._last_created_instance = cls._instances[key]
-        return cls._instances[key]
-
-    def get_last_created(cls):
-        if cls._last_created_instance is None:
-            raise NoPreviouslyCreatedSingletonError()
-        return cls._last_created_instance
+        # Create an instance
+        instance = super(CacheLast, cls).__call__(*args, **kwargs)
+
+        # Cache the instance
+        CacheLast._last_created_instance[cls] = instance
+
+        return instance
+
+    def get_last_created(cls: Type[T]) -> T:
+        """Get the last created instance"""
+        if cls not in CacheLast._last_created_instance:
+            raise NoPreviouslyCreatedInstanceError()
+
+        # Promise to the type system that we are fetching a T (which we are)
+        instance: T = CacheLast._last_created_instance[cls]
+
+        return instance
 
 
 class TSRandom:
     """
     Generate random values that are not available from Python 3.7's random module.
     """
 
@@ -58,33 +71,35 @@
 
         for part in content:
             hash_.update(part)
         rng_seed = hash_.digest()
         self._random.seed(rng_seed)
         self._is_seeded = True
 
-    def randbytes(self, n: int) -> bytes:
+    def randbytes(self, n_bytes: int) -> bytes:
         """Generate n random bytes."""
         if hasattr(self._random, "randbytes"):
-            return self._random.randbytes(n)
+            return self._random.randbytes(n_bytes)
 
         # Adapted from the Python 3.9+ random.randbytes method.
-        return self._random.getrandbits(n * 8).to_bytes(n, "little")
+        return self._random.getrandbits(n_bytes * 8).to_bytes(n_bytes, "little")
 
     def uuid(self) -> _uuid.UUID:
         """Create a pseudo random UUID"""
         return _uuid.UUID(bytes=self.randbytes(16))
 
 
-class TaskScriptUUIDGenerator(TSRandom, metaclass=Singleton):
+class TaskScriptUUIDGenerator(TSRandom, metaclass=CacheLast):
+    """UUID generator for use in Task Scripts"""
+
     def __init__(self, task_script_identifier: str, file_identifier: Hashable):
         super().__init__(task_script_identifier, file_identifier)
 
     @classmethod
     def from_task_script_identifier_parts(
-        cls, namespace: str, slug: str, version: str, file_identifier: Hashable
-    ) -> "TaskScriptUUIDGenerator":
+        cls: Type[T], namespace: str, slug: str, version: str, file_identifier: Hashable
+    ) -> T:
         """
         A convenience method that takes the parts of a task script identifier (namespace, slug, and version) and an
         identifier for the file (e.g. file location, file contents), then returns an instance of the generator class.
         """
         return cls(f"{namespace}/{slug}:{version}", file_identifier)
```

### Comparing `ts_task_script_utils-1.7.0/task_script_utils/workflow_logging.py` & `ts_task_script_utils-1.8.0/task_script_utils/workflow_logging.py`

 * *Files identical despite different names*

### Comparing `ts_task_script_utils-1.7.0/PKG-INFO` & `ts_task_script_utils-1.8.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ts-task-script-utils
-Version: 1.7.0
+Version: 1.8.0
 Summary: Python utility for Tetra Task Scripts
 License: Apache-2.0
 Author: Tetrascience
 Author-email: developers@tetrascience.com
 Requires-Python: >=3.7.2,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -21,32 +21,32 @@
 Requires-Dist: pendulum (>=2.1.2,<3.0.0)
 Requires-Dist: pydash (>=5.1.0,<6.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Description-Content-Type: text/markdown
 
 # ts-task-script-utils <!-- omit in toc -->
 
-[![Build Status](https://travis-ci.com/tetrascience/ts-task-script-utils.svg?branch=master)](https://travis-ci.com/tetrascience/ts-task-script-utils)
-
 ## Version <!-- omit in toc -->
 
-v1.7.0
+v1.8.0
 
 ## Table of Contents <!-- omit in toc -->
 
 - [Summary](#summary)
 - [Installation](#installation)
 - [Usage](#usage)
   - [Parsing Numbers](#parsing-numbers)
   - [Parsing Datetimes](#parsing-datetimes)
     - [`parse` Usage](#parse-usage)
   - [Generating Random UUIDs for Task Scripts](#generating-random-uuids-for-task-scripts)
   - [Creating datacube Parquet files](#creating-datacube-parquet-files)
-  - [Logging warning messages in Task Scripts](#logging-warning-messages-in-task-scripts)
+  - [Using Python's `logging` module in Task Scripts](#using-pythons-logging-module-in-task-scripts)
+  - [WellPosition](#wellposition)
 - [Changelog](#changelog)
+  - [v1.8.0](#v180)
   - [v1.7.0](#v170)
   - [v1.6.0](#v160)
   - [v1.5.0](#v150)
   - [v1.4.0](#v140)
   - [v1.3.1](#v131)
   - [v1.3.0](#v130)
   - [v1.2.0](#v120)
@@ -179,15 +179,15 @@
 This utility is a wrapper for the `context` logger which allows Task Scripts to use Python's `logging` module for creating TDP workflow logs, instead of directly using the `context` logger object. This means the `context` logger object doesn't need to be passed around to each function which needs to do logging, and Task Script code can benefit from other features of the Python `logging` module such as [integration with `pytest`](https://docs.pytest.org/en/7.1.x/how-to/logging.html).
 
 To log warning messages on the platform from a task script do the following:
 
 - Setup the log handler in `main.py`:
 
 ```python
-from task_script_utils.logging import (
+from task_script_utils.workflow_logging import (
     setup_ts_log_handler,
 )
 ```
 
 - Then within the function called by the protocol:
 
 ```python
@@ -203,19 +203,73 @@
 
 - Log a warning message with:
 
 ```python
 logger.warning("This is a warning message")
 ```
 
+### WellPosition
+
+For plate readers, you can parse the well label using `task_script_utils.plate_reader.WellPosition`.
+
+`WellPosition` encapsulates row and column indexes for a well on a plate.
+
+You can use `WellPosition.from_well_label` to parse the `well_label: str` and get the `WellPosition` object.
+
+For example:
+
+```python
+from plate_reader import WellPosition
+WellPosition.from_well_label("P45") # returns WellPosition(row=16, column=45)
+```
+
+A `well_label` must satisfy following conditions:
+
+  1. It must start with a letter
+  2. It can contain at max two letters
+      - When it contains two letters, they must both be uppercase
+  3. Letter(s) must be followed by at least one and at max two digits
+
+If the label cannot be parsed, `InvalidWellLabelError` is raised.
+
+eg, `A45, a45, A01, A1, z1, z01, AC23` are valid well labels
+
+Following are the example of invalid well labels:
+
+- `A245`: `well_label` with more than 2 digits is not supported
+- `A` or `a` or `aa`: `well_label`  doesn't contain any digit. Hence it is not supported.
+- `aB02, Ab02, ab02`: Both letters must be uppercase.
+
+Parsing for `well_label` containing a single letter is case sensitive ie. well labels A02 and a02 represent different wells on the plate
+
+Parsing for `well_label` containing two letters is limited to uppercase only ie. AB01 is supported but ab01, Ab01 and aB01 are not supported
+
+The following are the only supported sequence of rows for a plate:
+
+  1. A -> Z and then a -> z
+  2. A -> Z and then AA -> AZ
+
+For `well_label` with single letter, even though well labels starting with `w`, `x`, `y`, and `z` are supported by the parser, in real life this is not possible as the largest plate contains `3456 wells` which is `48x72`, so the last well label is going to be `v72`.
+
+Similarly, for `well_label` with two letters, in real life the largest possible `well_label` would be `AV72` for a plate with 3456 wells. However, `well_label` beyond `AV72` are also supported by parser.
+
 ## Changelog
 
+### v1.8.0
+
+- Add `task_script_utils.plate_reader.WellPosition` for parsing well labels
+- Update `task_script_utils.random.Singleton` used by `TaskScriptUUIDGenerator` and rename to `task_script_utils.random.CacheLast`
+  - `CacheLast` no longer provides singleton behavior, but it still provides the method `get_last_created`
+  - Instantiating `TaskScriptUUIDGenerator` always seeds the random generator. A second instance will repeat the same sequence of UUIDs as the first instance (if instantiated with the same arguments).
+  - Rename `NoPreviouslyCreatedSingletonError` to `NoPreviouslyCreatedInstanceError`
+  - Add type information to `get_last_created`
+
 ### v1.7.0
 
-- Add `task_script_utils.logging` for logging warning messages in task scripts
+- Add `task_script_utils.workflow_logging` for logging warning messages in task scripts
 
 ### v1.6.0
 
 - Add `task_script_utils.datacubes.parquet` for creating Parquet file representations of datacubes
 
 ### v1.5.0
```

