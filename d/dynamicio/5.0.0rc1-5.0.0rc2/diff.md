# Comparing `tmp/dynamicio-5.0.0rc1.tar.gz` & `tmp/dynamicio-5.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynamicio-5.0.0rc1.tar", last modified: Thu May 11 14:07:00 2023, max compression
+gzip compressed data, was "dynamicio-5.0.0rc2.tar", last modified: Thu May 11 16:17:35 2023, max compression
```

## Comparing `dynamicio-5.0.0rc1.tar` & `dynamicio-5.0.0rc2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-11 14:07:00.480336 dynamicio-5.0.0rc1/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    35149 2023-05-11 14:06:49.000000 dynamicio-5.0.0rc1/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)    39883 2023-05-11 14:07:00.480336 dynamicio-5.0.0rc1/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)    39394 2023-05-11 14:06:49.000000 dynamicio-5.0.0rc1/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-11 14:07:00.476336 dynamicio-5.0.0rc1/dynamicio/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       78 2023-05-11 14:06:49.000000 dynamicio-5.0.0rc1/dynamicio/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3151 2023-05-11 14:06:49.000000 dynamicio-5.0.0rc1/dynamicio/inject.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-11 14:07:00.480336 dynamicio-5.0.0rc1/dynamicio/io/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      331 2023-05-11 14:06:49.000000 dynamicio-5.0.0rc1/dynamicio/io/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-11 14:07:00.480336 dynamicio-5.0.0rc1/dynamicio/io/file/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      273 2023-05-11 14:06:49.000000 dynamicio-5.0.0rc1/dynamicio/io/file/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1650 2023-05-11 14:06:49.000000 dynamicio-5.0.0rc1/dynamicio/io/file/csv.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1915 2023-05-11 14:06:49.000000 dynamicio-5.0.0rc1/dynamicio/io/file/hdf.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1648 2023-05-11 14:06:49.000000 dynamicio-5.0.0rc1/dynamicio/io/file/json.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1733 2023-05-11 14:06:49.000000 dynamicio-5.0.0rc1/dynamicio/io/file/parquet.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3745 2023-05-11 14:06:49.000000 dynamicio-5.0.0rc1/dynamicio/io/kafka.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2305 2023-05-11 14:06:49.000000 dynamicio-5.0.0rc1/dynamicio/io/keyed.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7553 2023-05-11 14:06:49.000000 dynamicio-5.0.0rc1/dynamicio/io/postgres.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-11 14:07:00.480336 dynamicio-5.0.0rc1/dynamicio/io/s3/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      278 2023-05-11 14:06:49.000000 dynamicio-5.0.0rc1/dynamicio/io/s3/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2322 2023-05-11 14:06:49.000000 dynamicio-5.0.0rc1/dynamicio/io/s3/contexts.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2363 2023-05-11 14:06:49.000000 dynamicio-5.0.0rc1/dynamicio/io/s3/csv.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5203 2023-05-11 14:06:49.000000 dynamicio-5.0.0rc1/dynamicio/io/s3/hdf.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2362 2023-05-11 14:06:49.000000 dynamicio-5.0.0rc1/dynamicio/io/s3/json.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2417 2023-05-11 14:06:49.000000 dynamicio-5.0.0rc1/dynamicio/io/s3/parquet.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      522 2023-05-11 14:06:49.000000 dynamicio-5.0.0rc1/dynamicio/utils.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       76 2023-05-11 14:06:49.000000 dynamicio-5.0.0rc1/dynamicio/validators.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-11 14:07:00.476336 dynamicio-5.0.0rc1/dynamicio.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    39883 2023-05-11 14:07:00.000000 dynamicio-5.0.0rc1/dynamicio.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1007 2023-05-11 14:07:00.000000 dynamicio-5.0.0rc1/dynamicio.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-05-11 14:07:00.000000 dynamicio-5.0.0rc1/dynamicio.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       48 2023-05-11 14:07:00.000000 dynamicio-5.0.0rc1/dynamicio.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      309 2023-05-11 14:07:00.000000 dynamicio-5.0.0rc1/dynamicio.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       16 2023-05-11 14:07:00.000000 dynamicio-5.0.0rc1/dynamicio.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      705 2023-05-11 14:06:49.000000 dynamicio-5.0.0rc1/pyproject.toml
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-05-11 14:07:00.480336 dynamicio-5.0.0rc1/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1888 2023-05-11 14:06:49.000000 dynamicio-5.0.0rc1/setup.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-11 14:07:00.480336 dynamicio-5.0.0rc1/tests/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-05-11 14:06:49.000000 dynamicio-5.0.0rc1/tests/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      525 2023-05-11 14:06:49.000000 dynamicio-5.0.0rc1/tests/conftest.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      125 2023-05-11 14:06:49.000000 dynamicio-5.0.0rc1/tests/constants.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-11 14:07:00.480336 dynamicio-5.0.0rc1/tests/s3/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-05-11 14:06:49.000000 dynamicio-5.0.0rc1/tests/s3/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      762 2023-05-11 14:06:49.000000 dynamicio-5.0.0rc1/tests/s3/conftest.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3141 2023-05-11 14:06:49.000000 dynamicio-5.0.0rc1/tests/s3/test_hdf.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2939 2023-05-11 14:06:49.000000 dynamicio-5.0.0rc1/tests/s3/test_s3_implementations.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1810 2023-05-11 14:06:49.000000 dynamicio-5.0.0rc1/tests/test_file_implementations.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2315 2023-05-11 14:06:49.000000 dynamicio-5.0.0rc1/tests/test_inject.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1052 2023-05-11 14:06:49.000000 dynamicio-5.0.0rc1/tests/test_kafka.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3329 2023-05-11 14:06:49.000000 dynamicio-5.0.0rc1/tests/test_keyed.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7516 2023-05-11 14:06:49.000000 dynamicio-5.0.0rc1/tests/test_postgres.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2222 2023-05-11 14:06:49.000000 dynamicio-5.0.0rc1/tests/test_validations.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-11 16:17:35.051582 dynamicio-5.0.0rc2/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    35149 2023-05-11 16:17:23.000000 dynamicio-5.0.0rc2/LICENSE
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    39883 2023-05-11 16:17:35.051582 dynamicio-5.0.0rc2/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    39394 2023-05-11 16:17:23.000000 dynamicio-5.0.0rc2/README.md
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-11 16:17:35.047582 dynamicio-5.0.0rc2/dynamicio/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       78 2023-05-11 16:17:23.000000 dynamicio-5.0.0rc2/dynamicio/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3151 2023-05-11 16:17:23.000000 dynamicio-5.0.0rc2/dynamicio/inject.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-11 16:17:35.047582 dynamicio-5.0.0rc2/dynamicio/io/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      289 2023-05-11 16:17:23.000000 dynamicio-5.0.0rc2/dynamicio/io/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-11 16:17:35.047582 dynamicio-5.0.0rc2/dynamicio/io/file/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      224 2023-05-11 16:17:23.000000 dynamicio-5.0.0rc2/dynamicio/io/file/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1407 2023-05-11 16:17:23.000000 dynamicio-5.0.0rc2/dynamicio/io/file/csv.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1665 2023-05-11 16:17:23.000000 dynamicio-5.0.0rc2/dynamicio/io/file/hdf.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1401 2023-05-11 16:17:23.000000 dynamicio-5.0.0rc2/dynamicio/io/file/json.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1441 2023-05-11 16:17:23.000000 dynamicio-5.0.0rc2/dynamicio/io/file/parquet.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3476 2023-05-11 16:17:23.000000 dynamicio-5.0.0rc2/dynamicio/io/kafka.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1959 2023-05-11 16:17:23.000000 dynamicio-5.0.0rc2/dynamicio/io/keyed.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7242 2023-05-11 16:17:23.000000 dynamicio-5.0.0rc2/dynamicio/io/postgres.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-11 16:17:35.051582 dynamicio-5.0.0rc2/dynamicio/io/s3/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      221 2023-05-11 16:17:23.000000 dynamicio-5.0.0rc2/dynamicio/io/s3/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2322 2023-05-11 16:17:23.000000 dynamicio-5.0.0rc2/dynamicio/io/s3/contexts.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2065 2023-05-11 16:17:23.000000 dynamicio-5.0.0rc2/dynamicio/io/s3/csv.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4881 2023-05-11 16:17:23.000000 dynamicio-5.0.0rc2/dynamicio/io/s3/hdf.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2062 2023-05-11 16:17:23.000000 dynamicio-5.0.0rc2/dynamicio/io/s3/json.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2108 2023-05-11 16:17:23.000000 dynamicio-5.0.0rc2/dynamicio/io/s3/parquet.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      522 2023-05-11 16:17:23.000000 dynamicio-5.0.0rc2/dynamicio/utils.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       76 2023-05-11 16:17:23.000000 dynamicio-5.0.0rc2/dynamicio/validators.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-11 16:17:35.047582 dynamicio-5.0.0rc2/dynamicio.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    39883 2023-05-11 16:17:35.000000 dynamicio-5.0.0rc2/dynamicio.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1007 2023-05-11 16:17:35.000000 dynamicio-5.0.0rc2/dynamicio.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-05-11 16:17:35.000000 dynamicio-5.0.0rc2/dynamicio.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       48 2023-05-11 16:17:35.000000 dynamicio-5.0.0rc2/dynamicio.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      309 2023-05-11 16:17:35.000000 dynamicio-5.0.0rc2/dynamicio.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       16 2023-05-11 16:17:35.000000 dynamicio-5.0.0rc2/dynamicio.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      705 2023-05-11 16:17:23.000000 dynamicio-5.0.0rc2/pyproject.toml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-05-11 16:17:35.051582 dynamicio-5.0.0rc2/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1888 2023-05-11 16:17:23.000000 dynamicio-5.0.0rc2/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-11 16:17:35.051582 dynamicio-5.0.0rc2/tests/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-05-11 16:17:23.000000 dynamicio-5.0.0rc2/tests/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      525 2023-05-11 16:17:23.000000 dynamicio-5.0.0rc2/tests/conftest.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      125 2023-05-11 16:17:23.000000 dynamicio-5.0.0rc2/tests/constants.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-11 16:17:35.051582 dynamicio-5.0.0rc2/tests/s3/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-05-11 16:17:23.000000 dynamicio-5.0.0rc2/tests/s3/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      762 2023-05-11 16:17:23.000000 dynamicio-5.0.0rc2/tests/s3/conftest.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3063 2023-05-11 16:17:23.000000 dynamicio-5.0.0rc2/tests/s3/test_hdf.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2693 2023-05-11 16:17:23.000000 dynamicio-5.0.0rc2/tests/s3/test_s3_implementations.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1444 2023-05-11 16:17:23.000000 dynamicio-5.0.0rc2/tests/test_file_implementations.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2315 2023-05-11 16:17:23.000000 dynamicio-5.0.0rc2/tests/test_inject.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1006 2023-05-11 16:17:23.000000 dynamicio-5.0.0rc2/tests/test_kafka.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1747 2023-05-11 16:17:23.000000 dynamicio-5.0.0rc2/tests/test_keyed.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7329 2023-05-11 16:17:23.000000 dynamicio-5.0.0rc2/tests/test_postgres.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2103 2023-05-11 16:17:23.000000 dynamicio-5.0.0rc2/tests/test_validations.py
```

### Comparing `dynamicio-5.0.0rc1/LICENSE` & `dynamicio-5.0.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `dynamicio-5.0.0rc1/PKG-INFO` & `dynamicio-5.0.0rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamicio
-Version: 5.0.0rc1
+Version: 5.0.0rc2
 Summary: Panda's wrapper for IO operations
 Author: Christos Hadjinikolis, Radu Ghitescu
 Author-email: christos.hadjinikolis@gmail.com, radu.ghitescu@gmail.com
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `dynamicio-5.0.0rc1/README.md` & `dynamicio-5.0.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `dynamicio-5.0.0rc1/dynamicio/inject.py` & `dynamicio-5.0.0rc2/dynamicio/inject.py`

 * *Files identical despite different names*

### Comparing `dynamicio-5.0.0rc1/dynamicio/io/file/csv.py` & `dynamicio-5.0.0rc2/dynamicio/io/file/csv.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,55 +1,46 @@
 # pylint: disable=protected-access
 """Csv config and resource."""
 from __future__ import annotations
 
 from copy import deepcopy
 from pathlib import Path
-from typing import Any, Dict, Type
+from typing import Any, Dict, Optional, Type
 
 import pandas as pd
 from pandera import SchemaModel
 from pydantic import BaseModel  # type: ignore
 
 from dynamicio.inject import check_injections, inject
 
 
-class CsvConfig(BaseModel):
-    """CSV Config."""
+class CsvResource(BaseModel):
+    """CSV Resource."""
 
     path: Path
     read_kwargs: Dict[str, Any] = {}
     write_kwargs: Dict[str, Any] = {"index": False}
+    pa_schema: Optional[Type[SchemaModel]] = None
 
-    def inject(self, **kwargs) -> "CsvConfig":
+    def inject(self, **kwargs) -> "CsvResource":
         """Inject variables into path. Immutable."""
         clone = deepcopy(self)
         clone.path = inject(clone.path, **kwargs)
         return clone
 
     def check_injections(self) -> None:
         """Check that all injections have been completed."""
         check_injections(self.path)
 
-
-class CsvResource:
-    """CSV Resource."""
-
-    def __init__(self, config: CsvConfig, pa_schema: Type[SchemaModel] | None = None):
-        """Initialize the CSV Resource."""
-        config.check_injections()
-        self.config = config
-        self.pa_schema = pa_schema
-
     def read(self) -> pd.DataFrame:
         """Read the CSV file."""
-        df = pd.read_csv(self.config.path, **self.config.read_kwargs)
+        df = pd.read_csv(self.path, **self.read_kwargs)
         if schema := self.pa_schema:
             df = schema.validate(df)
         return df
 
     def write(self, df: pd.DataFrame) -> None:
         """Write the CSV file."""
         if schema := self.pa_schema:
             df = schema.validate(df)  # type: ignore
-        self.config.path.parent.mkdir(parents=True, exist_ok=True)
-        df.to_csv(self.config.path, **self.config.write_kwargs)
+        self.path.parent.mkdir(parents=True, exist_ok=True)
+        df.to_csv(self.path, **self.write_kwargs)
```

### Comparing `dynamicio-5.0.0rc1/dynamicio/io/file/hdf.py` & `dynamicio-5.0.0rc2/dynamicio/io/s3/json.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,63 +1,65 @@
 # pylint: disable=protected-access
-"""Hdf config and resource."""
+"""Json Resource and resource."""
 from __future__ import annotations
 
 from copy import deepcopy
 from pathlib import Path
-from threading import Lock
-from typing import Any, Dict, Type
+from typing import Any, Dict, Optional, Type
 
+import boto3  # type: ignore
 import pandas as pd
 from pandera import SchemaModel
-from pydantic import BaseModel, Field
+from pydantic import BaseModel  # type: ignore
 
-from dynamicio import utils
 from dynamicio.inject import check_injections, inject
+from dynamicio.io.s3.contexts import s3_named_file_reader
 
-hdf_lock = Lock()
 
+class S3JsonResource(BaseModel):
+    """JSON Resource."""
 
-class HdfConfig(BaseModel):
-    """HDF Config."""
-
+    bucket: str
     path: Path
-    pickle_protocol: int = Field(4, ge=0, le=5)  # Default covers python 3.4+
+    force_read_to_memory: bool = False
     read_kwargs: Dict[str, Any] = {}
     write_kwargs: Dict[str, Any] = {}
+    pa_schema: Optional[Type[SchemaModel]] = None
 
-    def inject(self, **kwargs) -> "HdfConfig":
+    def inject(self, **kwargs) -> "S3JsonResource":
         """Inject variables into path. Immutable."""
         clone = deepcopy(self)
+        clone.bucket = inject(clone.bucket, **kwargs)
         clone.path = inject(clone.path, **kwargs)
         return clone
 
     def check_injections(self) -> None:
         """Check that all injections have been completed."""
+        check_injections(self.bucket)
         check_injections(self.path)
 
+    @property
+    def full_path(self) -> str:
+        """Full path to the resource, including the bucket name."""
+        return f"s3://{self.bucket}/{self.path}"
 
-class HdfResource:
-    """HDF Resource."""
+    def read(self) -> pd.DataFrame:
+        """Read JSON from S3."""
+        df = None
 
-    def __init__(self, config: HdfConfig, pa_schema: Type[SchemaModel] | None = None):
-        """Initialize the HDF Resource."""
-        config.check_injections()
-        self.config = config
-        self.pa_schema = pa_schema
+        if self.force_read_to_memory:
+            df = pd.read_json(self.full_path, **self.read_kwargs)  # type: ignore
+
+        if df is None:
+            with s3_named_file_reader(boto3.client("s3"), s3_bucket=self.bucket, s3_key=str(self.path)) as target_file:
+                df = pd.read_json(target_file.name, **self.read_kwargs)  # type: ignore
 
-    def read(self) -> pd.DataFrame:
-        """Read the HDF file."""
-        with hdf_lock:
-            df = pd.read_hdf(self.config.path, **self.config.read_kwargs)
         if schema := self.pa_schema:
             df = schema.validate(df)
+
         return df
 
     def write(self, df: pd.DataFrame) -> None:
-        """Write the HDF file."""
+        """Write JSON to S3."""
         if schema := self.pa_schema:
             df = schema.validate(df)  # type: ignore
-        self.config.path.parent.mkdir(parents=True, exist_ok=True)
-
-        with utils.pickle_protocol(protocol=self.config.pickle_protocol), hdf_lock:
-            df.to_hdf(self.config.path, key="df", mode="w", **self.config.write_kwargs)
+        df.to_json(self.full_path, **self.write_kwargs)
```

### Comparing `dynamicio-5.0.0rc1/dynamicio/io/file/json.py` & `dynamicio-5.0.0rc2/dynamicio/io/file/json.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,55 +1,46 @@
 # pylint: disable=protected-access
 """Json config and resource."""
 from __future__ import annotations
 
 from copy import deepcopy
 from pathlib import Path
-from typing import Any, Dict, Type
+from typing import Any, Dict, Optional, Type
 
 import pandas as pd
 from pandera import SchemaModel
 from pydantic import BaseModel  # type: ignore
 
 from dynamicio.inject import check_injections, inject
 
 
-class JsonConfig(BaseModel):
-    """JSON Config."""
+class JsonResource(BaseModel):
+    """JSON Resource."""
 
     path: Path
     read_kwargs: Dict[str, Any] = {}
     write_kwargs: Dict[str, Any] = {}
+    pa_schema: Optional[Type[SchemaModel]] = None
 
-    def inject(self, **kwargs) -> "JsonConfig":
+    def inject(self, **kwargs) -> "JsonResource":
         """Inject variables into path. Immutable."""
         clone = deepcopy(self)
         clone.path = inject(clone.path, **kwargs)
         return clone
 
     def check_injections(self) -> None:
         """Check that all injections have been completed."""
         check_injections(self.path)
 
-
-class JsonResource:
-    """JSON Resource."""
-
-    def __init__(self, config: JsonConfig, pa_schema: Type[SchemaModel] | None = None):
-        """Initialize the JSON Resource."""
-        config.check_injections()
-        self.config = config
-        self.pa_schema = pa_schema
-
     def read(self) -> pd.DataFrame:
         """Read the JSON file."""
-        df = pd.read_json(self.config.path, **self.config.read_kwargs)
+        df = pd.read_json(self.path, **self.read_kwargs)
         if schema := self.pa_schema:
             df = schema.validate(df)
         return df
 
     def write(self, df: pd.DataFrame) -> None:
         """Write the JSON file."""
         if schema := self.pa_schema:
             df = schema.validate(df)  # type: ignore
-        self.config.path.parent.mkdir(parents=True, exist_ok=True)
-        df.to_json(self.config.path, **self.config.write_kwargs)
+        self.path.parent.mkdir(parents=True, exist_ok=True)
+        df.to_json(self.path, **self.write_kwargs)
```

### Comparing `dynamicio-5.0.0rc1/dynamicio/io/file/parquet.py` & `dynamicio-5.0.0rc2/dynamicio/io/file/parquet.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,57 +1,46 @@
 # pylint: disable=protected-access
 """Parquet config and resource."""
 from __future__ import annotations
 
 from copy import deepcopy
 from pathlib import Path
-from typing import Any, Dict, Type
+from typing import Any, Dict, Optional, Type
 
 import pandas as pd
 from pandera import SchemaModel
 from pydantic import BaseModel  # type: ignore
 
 from dynamicio.inject import check_injections, inject
 
 
-class ParquetConfig(BaseModel):
-    """PARQUET Config."""
+class ParquetResource(BaseModel):
+    """PARQUET Resource."""
 
     path: Path
     read_kwargs: Dict[str, Any] = {}
     write_kwargs: Dict[str, Any] = {}
+    pa_schema: Optional[Type[SchemaModel]] = None
 
-    def inject(self, **kwargs) -> "ParquetConfig":
+    def inject(self, **kwargs) -> "ParquetResource":
         """Inject variables into path. Immutable."""
         clone = deepcopy(self)
         clone.path = inject(clone.path, **kwargs)
         return clone
 
     def check_injections(self) -> None:
         """Check that all injections have been completed."""
         check_injections(self.path)
 
-
-class ParquetResource:
-    """PARQUET Resource."""
-
-    config_type = ParquetConfig
-
-    def __init__(self, config: ParquetConfig, pa_schema: Type[SchemaModel] | None = None):
-        """Initialize the PARQUET Resource."""
-        config.check_injections()
-        self.config = config
-        self.pa_schema = pa_schema
-
     def read(self) -> pd.DataFrame:
         """Read the PARQUET file."""
-        df = pd.read_parquet(self.config.path, **self.config.read_kwargs)
+        df = pd.read_parquet(self.path, **self.read_kwargs)
         if schema := self.pa_schema:
             df = schema.validate(df)  # type: ignore
         return df
 
     def write(self, df: pd.DataFrame) -> None:
         """Write the PARQUET file."""
         if schema := self.pa_schema:
             df = schema.validate(df)  # type: ignore
-        self.config.path.parent.mkdir(parents=True, exist_ok=True)
-        df.to_parquet(self.config.path, **self.config.write_kwargs)
+        self.path.parent.mkdir(parents=True, exist_ok=True)
+        df.to_parquet(self.path, **self.write_kwargs)
```

### Comparing `dynamicio-5.0.0rc1/dynamicio/io/kafka.py` & `dynamicio-5.0.0rc2/dynamicio/io/kafka.py`

 * *Files 15% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 
     GZIP = "gzip"
     SNAPPY = "snappy"
     LZ4 = "lz4"
     ZSTD = "zstd"
 
 
-class KafkaConfig(BaseModel):
-    """Kafka Resource class.
+class KafkaResource(BaseModel):
+    """Kafka Resource.
 
     This class is used to write to Kafka topics. Reading is not yet supported.
     Only requires a `topic` and `server` to be initialized.
     """
 
     topic: str
     server: str
@@ -42,16 +42,17 @@
     document_transformer: Callable[[Mapping[Any, Any]], Mapping[Any, Any]] = lambda value: value
     # TODO: Give descriptions to all these callables that describe what they're being called with
 
     kafka_producer: Optional[KafkaProducer] = None
 
     compression_type: CompressionType = "snappy"  # type: ignore
     producer_kwargs: Dict[str, Any] = {}
+    pa_schema: Optional[Type[SchemaModel]] = None
 
-    def inject(self, **kwargs) -> "KafkaConfig":
+    def inject(self, **kwargs) -> "KafkaResource":
         """Inject variables into topic and server. Immutable."""
         clone = deepcopy(self)
         clone.topic = inject(clone.topic, **kwargs)
         clone.server = inject(clone.server, **kwargs)
         return clone
 
     def check_injections(self) -> None:
@@ -73,37 +74,27 @@
 
     class Config:
         """Pydantic Config class."""
 
         arbitrary_types_allowed = True
         validate_assignment = True
 
-
-class KafkaResource:
-    """Kafka Resource."""
-
-    def __init__(self, config: KafkaConfig, pa_schema: Type[SchemaModel] | None = None):
-        """Initialize the Kafka Resource."""
-        config.check_injections()
-        self.config = config
-        self.pa_schema = pa_schema
-
     def write(self, df: pd.DataFrame) -> None:
         """Handles Write operations for Kafka."""
-        kafka_producer = self.config.get_kafka_producer()
+        kafka_producer = self.get_kafka_producer()
 
-        logger.info(f"Sending {len(df)} messages to Kafka topic:{self.config.topic}")
+        logger.info(f"Sending {len(df)} messages to Kafka topic:{self.topic}")
 
         messages = df.reset_index(drop=True).to_dict("records")
 
         for idx, message in zip(df.index.values, messages):
             kafka_producer.send(
-                self.config.topic,
-                key=self.config.key_generator(idx, message),
-                value=self.config.document_transformer(message),
+                self.topic,
+                key=self.key_generator(idx, message),
+                value=self.document_transformer(message),
             )  # type: ignore
 
         kafka_producer.flush()  # type: ignore
 
     def read(self) -> pd.DataFrame:
         """Not yet implemented."""
         raise NotImplementedError("No kafka reader implemented")
```

### Comparing `dynamicio-5.0.0rc1/dynamicio/io/keyed.py` & `dynamicio-5.0.0rc2/dynamicio/io/keyed.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,70 +1,60 @@
 # pylint: disable=W0707
 """KeyedResource class for reading and writing to different resources based on a key."""
 from __future__ import annotations
 
 from copy import deepcopy
-from typing import Protocol, Tuple, Type
+from typing import Protocol, Type
 
 import pandas as pd
 from pandera import SchemaModel
 
 
-class IOConfig(Protocol):
-    """IOConfig Protocol."""
+class IOResource(Protocol):
+    """IOResource Protocol."""
 
-    def inject(self, **kwargs) -> "IOConfig":
+    def inject(self, **kwargs) -> "IOResource":
         """Inject variables. Immutable."""
         return deepcopy(self)
 
     def check_injections(self) -> None:
         """Check that all injections have been completed. Raise InjectionError if not."""
 
-
-class IOResource(Protocol):
-    """IOResource Protocol."""
-
-    def __init__(self, config: IOConfig, pa_schema: Type[SchemaModel] | None = None):
-        """Initialize the IO Resource."""
-
     def read(self) -> pd.DataFrame:
         """Read."""
 
     def write(self, df: pd.DataFrame) -> None:
         """Write."""
 
 
-BuildConfig = Tuple[Type[IOResource], IOConfig]
-
-
 class KeyedResource:
     """KeyedResource class for reading and writing based on a key and given configs and io."""
 
     def __init__(
         self,
-        keyed_build_configs: dict[str, BuildConfig],
+        keyed_resources: dict[str, IOResource],
         pa_schema: Type[SchemaModel] | None = None,
         default_key: str | None = None,
     ):
         """Initialize the KeyedResource."""
-        if len(keyed_build_configs) == 0:
-            raise ValueError("KeyedResource must have at least one build_config.")
-        self.keyed_build_configs = keyed_build_configs
+        if len(keyed_resources) == 0:
+            raise ValueError("KeyedResource must have at least one resource.")
+        self.keyed_build_configs = keyed_resources
         self.pa_schema = pa_schema
-        self.key = default_key or list(keyed_build_configs.keys())[0]
+        self.key = default_key or list(keyed_resources.keys())[0]
 
     def inject(self, **kwargs) -> "KeyedResource":
         """Inject variables into all configs. Immutable."""
         new = deepcopy(self)
-        for key, (resource, config) in new.keyed_build_configs.items():
-            new.keyed_build_configs[key] = (resource, config.inject(**kwargs))
+        for key, resource in new.keyed_build_configs.items():
+            new.keyed_build_configs[key] = resource.inject(**kwargs)
         return new
 
     def read(self) -> pd.DataFrame:
         """Read from the active key resource."""
-        resource, config = self.keyed_build_configs[self.key]
-        return resource(config, self.pa_schema).read()
+        resource = self.keyed_build_configs[self.key]
+        return resource.read()
 
     def write(self, df: pd.DataFrame) -> None:
         """Write to the active key resource."""
-        resource, config = self.keyed_build_configs[self.key]
-        return resource(config, self.pa_schema).write(df)
+        resource = self.keyed_build_configs[self.key]
+        return resource.write(df)
```

### Comparing `dynamicio-5.0.0rc1/dynamicio/io/postgres.py` & `dynamicio-5.0.0rc2/dynamicio/io/postgres.py`

 * *Files 9% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         session.close()  # pylint: disable=no-member
 
 
 class ConfigurationError(Exception):
     """Raised when configuration is wrong."""
 
 
-class PostgresConfig(BaseModel):
+class PostgresResource(BaseModel):
     """Postgres Resource class.
 
     This resource handles reading and writing to postgres databases. If a pa_schema has been given, it will
     construct a sql query that only fetches the columns specified in the schema, this pushes down
     the filtering to the database, prevents us from unnecessarily loading data.
 
     Warning: Special case, where even if you explicitly don't validate, but give a pa_schema with strict="filter",
@@ -66,27 +66,28 @@
     db_schema: str = "public"
     table_name: Optional[str] = Field(None, description="SQL table name. Needs to be given if no sql_query is given")
     sql_query: Optional[str] = Field(
         None, description="SQL query. Will fetch schema defined columns if this is not given."
     )
     truncate_and_append: bool = False
     kwargs: Dict[str, Any] = {}
+    pa_schema: Optional[Type[SchemaModel]] = None
 
     @property
     def connection_string(self) -> str:
         """Build connection string out of components."""
         password = f":{self.db_password}" if self.db_password else ""
         return f"postgresql://{self.db_user}{password}@{self.db_host}:{self.db_port}/{self.db_name}"
 
     @property
     def final_table_name(self) -> str:
         """Return schema and table name in a format of schema.table_name."""
         return f"{self.db_schema}.{self.table_name}"
 
-    def inject(self, **kwargs) -> "PostgresConfig":
+    def inject(self, **kwargs) -> "PostgresResource":
         """Inject variables into stuff. Not in place."""
         clone = deepcopy(self)
         clone.db_user = inject(clone.db_user, **kwargs)
         clone.db_password = inject(clone.db_password, **kwargs)
         clone.db_host = inject(clone.db_host, **kwargs)
         clone.db_name = inject(clone.db_name, **kwargs)
         clone.table_name = inject(clone.table_name, **kwargs)
@@ -100,63 +101,57 @@
         check_injections(self.db_password)
         check_injections(self.db_host)
         check_injections(self.db_name)
         check_injections(self.table_name)
         check_injections(self.sql_query)
         check_injections(self.db_schema)
 
-
-class PostgresResource:
-    """Postgres Resource."""
-
-    def __init__(self, config: PostgresConfig, pa_schema: Type[SchemaModel] | None = None):
-        """Initialize the Postgres Resource."""
-        config.check_injections()
-        self.config = config
-        self.pa_schema = pa_schema
-
-    def read(self):
+    def read(self) -> pd.DataFrame:
         """Handles Read operations for Postgres."""
-        if not bool(self.config.sql_query) ^ bool(self.config.table_name):  # Xor
+        if not bool(self.sql_query) ^ bool(self.table_name):  # Xor
             raise ConfigurationError("PostgresResource must define EITHER sql_query OR table_name.")
 
-        if self.pa_schema is not None and (not self.config.sql_query and self.pa_schema.Config.strict):
+        if self.pa_schema is not None and (not self.sql_query and self.pa_schema.Config.strict):
             # filtering can now be done at sql level
             columns: List[str] = list(self.pa_schema.to_schema().columns.keys())  # type: ignore
             columns_str = ", ".join(columns)
-            sql_query = f"SELECT {columns_str} FROM {self.config.final_table_name}"
-        elif self.config.sql_query is None:
-            sql_query = f"SELECT * FROM {self.config.final_table_name}"
+            sql_query = f"SELECT {columns_str} FROM {self.final_table_name}"
+        elif self.sql_query is None:
+            sql_query = f"SELECT * FROM {self.final_table_name}"
         else:
-            sql_query = self.config.sql_query
+            sql_query = self.sql_query
+
+        logger.info(f"Downloading table: {self.final_table_name} from: {self.db_host}:{self.db_name}")
+        with session_scope(self.connection_string) as session:
+            df = pd.read_sql(sql=sql_query, con=session.get_bind(), **self.kwargs)
 
-        logger.info(
-            f"Downloading table: {self.config.final_table_name} from: {self.config.db_host}:{self.config.db_name}"
-        )
-        with session_scope(self.config.connection_string) as session:
-            return pd.read_sql(sql=sql_query, con=session.get_bind(), **self.config.kwargs)
+        if self.pa_schema is not None:
+            df = self.pa_schema.validate(df)
+
+        return df
 
         # TODO: sqlalchemy 2.0 breaks here
         #       session.get_bind() is probably the culprit
         # TODO: Check if type coercion is needed here
         #       For example objects -> String(64)s
         #       For example date goes to Date and datetime64[ns] -> DateTime
 
     def write(self, df: pd.DataFrame):
         """Handles Write operations for Postgres."""
-        if not self.config.table_name:
+        if not self.table_name:
             raise ConfigurationError("PostgresResource must specify table_name for writing.")
 
-        with session_scope(self.config.connection_string) as session:
+        if schema := self.pa_schema:
+            df = schema.validate(df)  # type: ignore
+
+        with session_scope(self.connection_string) as session:
             session: SqlAlchemySession  # type: ignore # this is done for IDE purposes
-            if self.config.truncate_and_append:
-                logger.info(
-                    f"Writing to table (csv-hack): {self.config.final_table_name} from: {self.config.db_host}:{self.config.db_name}"
-                )
-                session.execute(f"TRUNCATE TABLE {self.config.final_table_name};")
+            if self.truncate_and_append:
+                logger.info(f"Writing to table (csv-hack): {self.final_table_name} from: {self.db_host}:{self.db_name}")
+                session.execute(f"TRUNCATE TABLE {self.final_table_name};")
 
                 # Speed hack: dump file as csv, use Postgres' CSV import function.
                 # https://stackoverflow.com/questions/2987433/how-to-import-csv-file-data-into-a-postgresql-table
                 with tempfile.NamedTemporaryFile(mode="r+") as temp_file:
                     df.to_csv(
                         temp_file,
                         index=False,
@@ -166,20 +161,18 @@
                         escapechar="\\",
                         quoting=csv.QUOTE_NONE,
                     )
                     temp_file.flush()
                     temp_file.seek(0)
 
                     cur = session.connection().connection.cursor()
-                    cur.execute(f"SET search_path TO {self.config.db_schema};")
-                    cur.copy_from(temp_file, self.config.table_name, columns=df.columns, null="")
+                    cur.execute(f"SET search_path TO {self.db_schema};")
+                    cur.copy_from(temp_file, self.table_name, columns=df.columns, null="")
             else:
-                logger.info(
-                    f"Writing to table: {self.config.final_table_name} from: {self.config.db_host}:{self.config.db_name}"
-                )
+                logger.info(f"Writing to table: {self.final_table_name} from: {self.db_host}:{self.db_name}")
                 df.to_sql(
-                    name=self.config.table_name,
+                    name=self.table_name,
                     con=session.get_bind(),
                     if_exists="replace",
                     index=False,
-                    schema=self.config.db_schema,
+                    schema=self.db_schema,
                 )
```

### Comparing `dynamicio-5.0.0rc1/dynamicio/io/s3/contexts.py` & `dynamicio-5.0.0rc2/dynamicio/io/s3/contexts.py`

 * *Files identical despite different names*

### Comparing `dynamicio-5.0.0rc1/dynamicio/io/s3/csv.py` & `dynamicio-5.0.0rc2/dynamicio/io/s3/csv.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 # pylint: disable=protected-access
 """Csv config and resource."""
 from __future__ import annotations
 
 from copy import deepcopy
 from pathlib import Path
-from typing import Any, Dict, Type
+from typing import Any, Dict, Optional, Type
 
 import boto3  # type: ignore
 import pandas as pd
 from pandera import SchemaModel
 from pydantic import BaseModel  # type: ignore
 
 from dynamicio.inject import check_injections, inject
 from dynamicio.io.s3.contexts import s3_named_file_reader
 
 
-class S3CsvConfig(BaseModel):
-    """CSV Config."""
+class S3CsvResource(BaseModel):
+    """CSV Resource."""
 
     bucket: str
     path: Path
     force_read_to_memory: bool = False
     read_kwargs: Dict[str, Any] = {}
     write_kwargs: Dict[str, Any] = {"index": False}
+    pa_schema: Optional[Type[SchemaModel]] = None
 
-    def inject(self, **kwargs) -> "S3CsvConfig":
+    def inject(self, **kwargs) -> "S3CsvResource":
         """Inject variables into path. Immutable."""
         clone = deepcopy(self)
         clone.bucket = inject(clone.bucket, **kwargs)
         clone.path = inject(clone.path, **kwargs)
         return clone
 
     def check_injections(self) -> None:
@@ -37,40 +38,28 @@
         check_injections(self.path)
 
     @property
     def full_path(self) -> str:
         """Full path to the resource, including the bucket name."""
         return f"s3://{self.bucket}/{self.path}"
 
-
-class S3CsvResource:
-    """CSV Resource."""
-
-    def __init__(self, config: S3CsvConfig, pa_schema: Type[SchemaModel] | None = None):
-        """Initialize the CSV Resource."""
-        config.check_injections()
-        self.config = config
-        self.pa_schema = pa_schema
-
     def read(self) -> pd.DataFrame:
         """Read CSV from S3."""
         df = None
 
-        if self.config.force_read_to_memory:
-            df = pd.read_csv(self.config.full_path, **self.config.read_kwargs)  # type: ignore
+        if self.force_read_to_memory:
+            df = pd.read_csv(self.full_path, **self.read_kwargs)  # type: ignore
 
         if df is None:
-            with s3_named_file_reader(
-                boto3.client("s3"), s3_bucket=self.config.bucket, s3_key=str(self.config.path)
-            ) as target_file:
-                df = pd.read_csv(target_file.name, **self.config.read_kwargs)  # type: ignore
+            with s3_named_file_reader(boto3.client("s3"), s3_bucket=self.bucket, s3_key=str(self.path)) as target_file:
+                df = pd.read_csv(target_file.name, **self.read_kwargs)  # type: ignore
 
         if schema := self.pa_schema:
             df = schema.validate(df)
 
         return df
 
     def write(self, df: pd.DataFrame) -> None:
         """Write CSV to S3."""
         if schema := self.pa_schema:
             df = schema.validate(df)  # type: ignore
-        df.to_csv(self.config.full_path, **self.config.write_kwargs)
+        df.to_csv(self.full_path, **self.write_kwargs)
```

### Comparing `dynamicio-5.0.0rc1/dynamicio/io/s3/hdf.py` & `dynamicio-5.0.0rc2/dynamicio/io/s3/hdf.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,25 +19,26 @@
 from dynamicio import utils
 from dynamicio.inject import check_injections, inject
 from dynamicio.io.s3.contexts import s3_named_file_reader, s3_reader, s3_writer
 
 hdf_lock = Lock()
 
 
-class S3HdfConfig(BaseModel):
-    """HDF Config."""
+class S3HdfResource(BaseModel):
+    """HDF Resource."""
 
     bucket: str
     path: Path
     pickle_protocol: int = Field(4, ge=0, le=5)  # Default covers python 3.4+
     force_read_to_memory: bool = False
     read_kwargs: Dict[str, Any] = {}
     write_kwargs: Dict[str, Any] = {}
+    pa_schema: Optional[Type[SchemaModel]] = None
 
-    def inject(self, **kwargs) -> "S3HdfConfig":
+    def inject(self, **kwargs) -> "S3HdfResource":
         """Inject variables into path. Immutable."""
         clone = deepcopy(self)
         clone.bucket = inject(clone.bucket, **kwargs)
         clone.path = inject(clone.path, **kwargs)
         return clone
 
     def check_injections(self) -> None:
@@ -46,51 +47,39 @@
         check_injections(self.path)
 
     @property
     def full_path(self) -> str:
         """Full path to the resource, including the bucket name."""
         return f"s3://{self.bucket}/{self.path}"
 
-
-class S3HdfResource:
-    """HDF Resource."""
-
-    def __init__(self, config: S3HdfConfig, pa_schema: Type[SchemaModel] | None = None):
-        """Initialize the HDF Resource."""
-        config.check_injections()
-        self.config = config
-        self.pa_schema = pa_schema
-
     def read(self) -> pd.DataFrame:
         """Read HDF from S3."""
         df = None
-        if self.config.force_read_to_memory:
-            with s3_reader(boto3.client("s3"), s3_bucket=self.config.bucket, s3_key=str(self.config.path)) as fobj:  # type: ignore
+        if self.force_read_to_memory:
+            with s3_reader(boto3.client("s3"), s3_bucket=self.bucket, s3_key=str(self.path)) as fobj:  # type: ignore
                 df = HdfIO().load(fobj)
         if df is None:
-            with s3_named_file_reader(
-                boto3.client("s3"), s3_bucket=self.config.bucket, s3_key=str(self.config.path)
-            ) as target_file:
+            with s3_named_file_reader(boto3.client("s3"), s3_bucket=self.bucket, s3_key=str(self.path)) as target_file:
                 with hdf_lock:
-                    df = pd.read_hdf(target_file.name, **self.config.read_kwargs)  # type: ignore
+                    df = pd.read_hdf(target_file.name, **self.read_kwargs)  # type: ignore
 
         if schema := self.pa_schema:
             df = schema.validate(df)  # type: ignore
 
         return df
 
     def write(self, df: pd.DataFrame) -> None:
         """Write HDF to s3."""
         if schema := self.pa_schema:
             df = schema.validate(df)  # type: ignore
 
-        with s3_writer(
-            boto3.client("s3"), s3_bucket=self.config.bucket, s3_key=str(self.config.path)
-        ) as fobj, utils.pickle_protocol(protocol=self.config.pickle_protocol):
-            HdfIO().save(df, fobj, **self.config.write_kwargs)
+        with s3_writer(boto3.client("s3"), s3_bucket=self.bucket, s3_key=str(self.path)) as fobj, utils.pickle_protocol(
+            protocol=self.pickle_protocol
+        ):
+            HdfIO().save(df, fobj, **self.write_kwargs)
 
 
 class InMemStore(pd.io.pytables.HDFStore):
     """A subclass of pandas HDFStore that does not manage the pytables File object."""
 
     _in_mem_table = None
```

### Comparing `dynamicio-5.0.0rc1/dynamicio/io/s3/json.py` & `dynamicio-5.0.0rc2/dynamicio/io/s3/parquet.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 # pylint: disable=protected-access
-"""Json config and resource."""
+"""Parquet Resource and resource."""
 from __future__ import annotations
 
 from copy import deepcopy
 from pathlib import Path
-from typing import Any, Dict, Type
+from typing import Any, Dict, Optional, Type
 
 import boto3  # type: ignore
 import pandas as pd
 from pandera import SchemaModel
 from pydantic import BaseModel  # type: ignore
 
 from dynamicio.inject import check_injections, inject
 from dynamicio.io.s3.contexts import s3_named_file_reader
 
 
-class S3JsonConfig(BaseModel):
-    """JSON Config."""
+class S3ParquetResource(BaseModel):
+    """S3 PARQUET Resource."""
 
     bucket: str
     path: Path
     force_read_to_memory: bool = False
     read_kwargs: Dict[str, Any] = {}
     write_kwargs: Dict[str, Any] = {}
+    pa_schema: Optional[Type[SchemaModel]] = None
 
-    def inject(self, **kwargs) -> "S3JsonConfig":
+    def inject(self, **kwargs) -> "S3ParquetResource":
         """Inject variables into path. Immutable."""
         clone = deepcopy(self)
         clone.bucket = inject(clone.bucket, **kwargs)
         clone.path = inject(clone.path, **kwargs)
         return clone
 
     def check_injections(self) -> None:
@@ -37,40 +38,28 @@
         check_injections(self.path)
 
     @property
     def full_path(self) -> str:
         """Full path to the resource, including the bucket name."""
         return f"s3://{self.bucket}/{self.path}"
 
-
-class S3JsonResource:
-    """JSON Resource."""
-
-    def __init__(self, config: S3JsonConfig, pa_schema: Type[SchemaModel] | None = None):
-        """Initialize the JSON Resource."""
-        config.check_injections()
-        self.config = config
-        self.pa_schema = pa_schema
-
     def read(self) -> pd.DataFrame:
-        """Read JSON from S3."""
+        """Read PARQUET from S3."""
         df = None
 
-        if self.config.force_read_to_memory:
-            df = pd.read_json(self.config.full_path, **self.config.read_kwargs)  # type: ignore
+        if self.force_read_to_memory:
+            df = pd.read_parquet(self.full_path, **self.read_kwargs)  # type: ignore
 
         if df is None:
-            with s3_named_file_reader(
-                boto3.client("s3"), s3_bucket=self.config.bucket, s3_key=str(self.config.path)
-            ) as target_file:
-                df = pd.read_json(target_file.name, **self.config.read_kwargs)  # type: ignore
+            with s3_named_file_reader(boto3.client("s3"), s3_bucket=self.bucket, s3_key=str(self.path)) as target_file:
+                df = pd.read_parquet(target_file.name, **self.read_kwargs)  # type: ignore
 
         if schema := self.pa_schema:
-            df = schema.validate(df)
+            df = schema.validate(df)  # type: ignore
 
         return df
 
     def write(self, df: pd.DataFrame) -> None:
-        """Write JSON to S3."""
+        """Write PARQUET to S3."""
         if schema := self.pa_schema:
             df = schema.validate(df)  # type: ignore
-        df.to_json(self.config.full_path, **self.config.write_kwargs)
+        df.to_parquet(self.full_path, **self.write_kwargs)
```

### Comparing `dynamicio-5.0.0rc1/dynamicio/utils.py` & `dynamicio-5.0.0rc2/dynamicio/utils.py`

 * *Files identical despite different names*

### Comparing `dynamicio-5.0.0rc1/dynamicio.egg-info/PKG-INFO` & `dynamicio-5.0.0rc2/dynamicio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamicio
-Version: 5.0.0rc1
+Version: 5.0.0rc2
 Summary: Panda's wrapper for IO operations
 Author: Christos Hadjinikolis, Radu Ghitescu
 Author-email: christos.hadjinikolis@gmail.com, radu.ghitescu@gmail.com
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `dynamicio-5.0.0rc1/dynamicio.egg-info/SOURCES.txt` & `dynamicio-5.0.0rc2/dynamicio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dynamicio-5.0.0rc1/pyproject.toml` & `dynamicio-5.0.0rc2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dynamicio-5.0.0rc1/setup.py` & `dynamicio-5.0.0rc2/setup.py`

 * *Files identical despite different names*

### Comparing `dynamicio-5.0.0rc1/tests/conftest.py` & `dynamicio-5.0.0rc2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dynamicio-5.0.0rc1/tests/s3/conftest.py` & `dynamicio-5.0.0rc2/tests/s3/conftest.py`

 * *Files identical despite different names*

### Comparing `dynamicio-5.0.0rc1/tests/s3/test_hdf.py` & `dynamicio-5.0.0rc2/tests/s3/test_hdf.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from pathlib import Path
 from typing import IO, Generator
 from unittest.mock import Mock, patch
 
 import pandas as pd
 import pytest
 
-from dynamicio import S3HdfConfig, S3HdfResource
+from dynamicio import S3HdfResource
 from tests import constants
 from tests.resources.schemas import SampleSchema
 
 sample_path = constants.TEST_RESOURCES / "data/input/hdf_sample.h5"
 
 
 @pytest.fixture
@@ -55,59 +55,56 @@
     with patch("dynamicio.io.s3.hdf.s3_writer", new=plain_s3_writer) as target:
         yield target
 
 
 @pytest.fixture()
 def hdf_s3_resource() -> S3HdfResource:
     return S3HdfResource(
-        S3HdfConfig(
-            bucket="my_bucket",
-            path="some/path.hdf",
-        )
+        bucket="my_bucket",
+        path="some/path.hdf",
     )
 
 
 @pytest.fixture()
-def hdf_s3_config() -> S3HdfResource:
-    return S3HdfConfig(
-        bucket="my_bucket",
-        path="some/path.hdf",
-    )
+def hdf_s3_config() -> dict:
+    return {
+        "bucket": "my_bucket",
+        "path": "some/path.hdf",
+    }
 
 
 @pytest.fixture()
 def hdf_df(hdf_s3_resource) -> pd.DataFrame:
     return pd.read_hdf(sample_path)
 
 
 def test__resource_read(s3_stubber, hdf_s3_resource, hdf_df, mock_s3_named_file_reader):
     df = hdf_s3_resource.read()
     pd.testing.assert_frame_equal(df, hdf_df)
 
 
 def test__resource_read_with_schema(s3_stubber, hdf_s3_config, hdf_df, mock_s3_named_file_reader):
-    df = S3HdfResource(hdf_s3_config, SampleSchema).read()
+    df = S3HdfResource(**hdf_s3_config, pa_schema=SampleSchema).read()
     pd.testing.assert_frame_equal(df, hdf_df)
 
 
 def test__resource_read_no_disk_space(s3_stubber, hdf_s3_config, hdf_df, mock_s3_reader):
-    hdf_s3_config.force_read_to_memory = True
-    df = S3HdfResource(hdf_s3_config).read()
+    hdf_s3_config["force_read_to_memory"] = True
+    df = S3HdfResource(**hdf_s3_config).read()
     pd.testing.assert_frame_equal(df, hdf_df)
 
 
-class MockS3HdfConfig(S3HdfConfig):
+class MockS3HdfResource(S3HdfResource):
     @property
     def _full_path(self) -> Path:
         return self.path
 
 
 def test__resource_write(s3_stubber, hdf_df, mock_s3_writer, tmp_path):
     tmp_location = tmp_path / "sample_file.hdf"
-    config = MockS3HdfConfig(
+    resource = MockS3HdfResource(
         bucket="my_bucket",
         path=tmp_location,
     )
-    resource = S3HdfResource(config)
     resource.write(hdf_df)
     df = pd.read_hdf(tmp_location)
     pd.testing.assert_frame_equal(df, hdf_df)
```

### Comparing `dynamicio-5.0.0rc1/tests/s3/test_s3_implementations.py` & `dynamicio-5.0.0rc2/tests/s3/test_s3_implementations.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,97 +2,91 @@
 from pathlib import Path
 from typing import Generator
 from unittest.mock import Mock, patch
 
 import pandas as pd
 import pytest
 
-from dynamicio import S3CsvConfig, S3CsvResource, S3JsonConfig, S3JsonResource, S3ParquetConfig, S3ParquetResource
+from dynamicio import S3CsvResource, S3JsonResource, S3ParquetResource
 from tests import constants
 from tests.resources.schemas import SampleSchema
 
 input_path = constants.TEST_RESOURCES / "data/input"
 s3_bucket = "my_bucket"
 
 
 @pytest.fixture(
     params=[
-        (S3CsvConfig, "csv_sample.csv", pd.read_csv, S3CsvResource, "csv"),
-        (S3ParquetConfig, "parquet_sample.parquet", pd.read_parquet, S3ParquetResource, "parquet"),
-        (S3JsonConfig, "json_sample.json", pd.read_json, S3JsonResource, "json"),
+        ("csv_sample.csv", pd.read_csv, S3CsvResource, "csv"),
+        ("parquet_sample.parquet", pd.read_parquet, S3ParquetResource, "parquet"),
+        ("json_sample.json", pd.read_json, S3JsonResource, "json"),
     ],
     ids=lambda v: v[1],
 )
 def config_file_function(request):
     return request.param
 
 
 @pytest.fixture
 def mock_reader(config_file_function):
-    return Mock(return_value=type("FileObj", (object,), {"name": input_path / config_file_function[1]})())
+    return Mock(return_value=type("FileObj", (object,), {"name": input_path / config_file_function[0]})())
 
 
 @pytest.fixture
 def s3_named_file_reader(mock_reader, config_file_function):
     @contextmanager
     def plain_s3_reader(s3_client, s3_bucket: str, s3_key: str) -> Generator:
         yield mock_reader(s3_client, s3_bucket, s3_key)
 
-    module = config_file_function[4]
+    module = config_file_function[3]
 
     with patch(f"dynamicio.io.s3.{module}.s3_named_file_reader", new=plain_s3_reader) as target:
         yield target
 
 
 # --- Tests ---
 
 
 def test_s3_config_read(s3_stubber, s3_named_file_reader, config_file_function):
-    config_class, file_name, read_func, resource_class, _ = config_file_function
+    file_name, read_func, resource_class, _ = config_file_function
     resource = resource_class(
-        config_class(
-            bucket=s3_bucket,
-            path=f"some/{file_name}",
-        )
+        bucket=s3_bucket,
+        path=f"some/{file_name}",
     )
     expected_df = read_func(input_path / file_name)
     df = resource.read()
     pd.testing.assert_frame_equal(df, expected_df)
 
 
 def test_s3_config_read_with_schema(s3_stubber, s3_named_file_reader, config_file_function):
-    config_class, file_name, read_func, resource_class, _ = config_file_function
-    config = config_class(
-        bucket=s3_bucket,
-        path=f"some/{file_name}",
-    )
+    file_name, read_func, resource_class, _ = config_file_function
 
     expected_df = read_func(input_path / file_name)
 
-    df = resource_class(config, SampleSchema).read()
+    df = resource_class(bucket=s3_bucket, path=f"some/{file_name}", pa_schema=SampleSchema).read()
 
     pd.testing.assert_frame_equal(df, expected_df)
 
 
 def test_s3_config_write(s3_stubber, s3_named_file_reader, tmpdir, config_file_function):
-    config_class, file_name, read_func, resource_class, _ = config_file_function
+    file_name, read_func, resource_class, _ = config_file_function
 
-    class MockConfig(config_class):
-        @property
-        def full_path(self) -> Path:
-            return self.path
+    def mock_full_path(self) -> Path:
+        return self.path
 
-    config = MockConfig(
-        bucket=s3_bucket,
-        path=f"some/{file_name}",
-        allow_no_schema=True,
-    )
+    resource_class.full_path = property(mock_full_path)
 
     expected_df = read_func(input_path / file_name)
 
     target_location = tmpdir / "sample"
-    config.path = target_location
 
-    resource = resource_class(config)
+    resource = resource_class(
+        bucket=s3_bucket,
+        path=f"some/{file_name}",
+        allow_no_schema=True,
+    )
+    resource.path = target_location
+
     resource.write(expected_df)
     df = resource.read()
+
     pd.testing.assert_frame_equal(df, expected_df)
```

### Comparing `dynamicio-5.0.0rc1/tests/test_inject.py` & `dynamicio-5.0.0rc2/tests/test_inject.py`

 * *Files identical despite different names*

### Comparing `dynamicio-5.0.0rc1/tests/test_kafka.py` & `dynamicio-5.0.0rc2/tests/test_kafka.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 # flake8: noqa: I101
 
 from unittest.mock import MagicMock, call, patch
 
 import pytest
 
-from dynamicio import KafkaConfig, KafkaResource
+from dynamicio import KafkaResource
 
 
 @pytest.fixture
 def mocked_kafka_producer():
     mocked_kafka_producer = MagicMock()
     with patch("dynamicio.io.kafka.KafkaProducer") as kafka_producer:
         kafka_producer.return_value = mocked_kafka_producer
         yield mocked_kafka_producer
 
 
 @pytest.fixture
 def kafka_resource() -> KafkaResource:
-    config = KafkaConfig(topic="test_topic", server="test_server")
-    return KafkaResource(config)
+    return KafkaResource(topic="test_topic", server="test_server")
 
 
 def test_kafka_resource_write(sample_df, kafka_resource, mocked_kafka_producer):
     kafka_resource.write(sample_df)
     mocked_kafka_producer.send.assert_has_calls(
         [
             call("test_topic", key=0, value={"a": 1, "b": 4}),
```

### Comparing `dynamicio-5.0.0rc1/tests/test_postgres.py` & `dynamicio-5.0.0rc2/tests/test_postgres.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,49 +1,43 @@
 from unittest.mock import ANY, MagicMock, Mock, patch
 
 import pandas as pd
 import pytest
 
-from dynamicio import PostgresConfig, PostgresResource
+from dynamicio import PostgresResource
 from dynamicio.inject import InjectionError
 from dynamicio.io.postgres import ConfigurationError
 from tests import constants
 from tests.resources.schemas import PgSampleSchema
 
 sample_path = f"{constants.TEST_RESOURCES}/data/input/pg_parquet_sample.parquet"
 
 
-@pytest.fixture
-def postgres_table_config() -> PostgresConfig:
-    return PostgresConfig(
+@pytest.fixture()
+def postgres_table_resource() -> PostgresResource:
+    return PostgresResource(
         db_user="test_user",
         db_host="test_host",
         db_port=1234,
         db_name="test_db",
         db_schema="republic",
         table_name="test_table",
     )
 
 
 @pytest.fixture()
-def postgres_table_resource(postgres_table_config) -> PostgresResource:
-    return PostgresResource(postgres_table_config)
-
-
-@pytest.fixture()
 def postgres_query_resource() -> PostgresResource:
-    config = PostgresConfig(
+    return PostgresResource(
         db_user="test_user",
         db_host="test_host",
         db_port=1234,
         db_name="test_db",
         db_schema="republic",
         sql_query="SELECT * FROM other_table",
     )
-    return PostgresResource(config)
 
 
 @pytest.fixture
 def mock_cursor():
     return MagicMock()
 
 
@@ -81,18 +75,24 @@
 
 def test_postgres_resource_read(postgres_table_resource, postgres_df, read_sql_mock, mocked_session, mock_binding):
     df = postgres_table_resource.read()
     read_sql_mock.assert_called_once_with(sql="SELECT * FROM republic.test_table", con=mock_binding)
     pd.testing.assert_frame_equal(df, postgres_df)
 
 
-def test_postgres_resource_read_with_schema(
-    postgres_table_config, postgres_df, read_sql_mock, mocked_session, mock_binding
-):
-    resource = PostgresResource(postgres_table_config, pa_schema=PgSampleSchema)
+def test_postgres_resource_read_with_schema(postgres_df, read_sql_mock, mocked_session, mock_binding):
+    resource = PostgresResource(
+        db_user="test_user",
+        db_host="test_host",
+        db_port=1234,
+        db_name="test_db",
+        db_schema="republic",
+        table_name="test_table",
+        pa_schema=PgSampleSchema,
+    )
     df = resource.read()
     read_sql_mock.assert_called_once_with(sql="SELECT * FROM republic.test_table", con=mock_binding)
     pd.testing.assert_frame_equal(df, postgres_df)
 
 
 class PgFilterSampleSchema(PgSampleSchema):
     class Config:
@@ -131,95 +131,91 @@
         name="test_table", con=mock_binding, if_exists="replace", index=False, schema="republic"
     )
 
 
 def test_postgres_resource_write_truncate_and_append(
     postgres_table_resource, postgres_df, to_sql_mock, mocked_session, mock_binding, mock_cursor
 ):
-    postgres_table_resource.config.truncate_and_append = True
+    postgres_table_resource.truncate_and_append = True
     postgres_table_resource.write(postgres_df)
     mocked_session.execute.assert_called_once_with("TRUNCATE TABLE republic.test_table;")
     mock_cursor.execute.assert_called_once_with("SET search_path TO republic;")
     mock_cursor.copy_from.assert_called_once_with(ANY, "test_table", columns=postgres_df.columns, null="")
 
 
 def test_postgres_resource_inject_and_read(postgres_df, read_sql_mock, mocked_session, mock_binding):
-    config = PostgresConfig(
+    resource = PostgresResource(
         db_user="[[db_user]]",
         db_host="{db_host}",
         db_port=1234,
         db_name="that_{db_name}",
         db_schema="[[republic]]",
         table_name="[[table]]",
     )
-    config = config.inject(
+    resource = resource.inject(
         db_user="test_user", db_host="test_host", db_name="test_db", table="test_table", republic="republic"
     )
-    resource = PostgresResource(config)
     df = resource.read()
     read_sql_mock.assert_called_once_with(sql="SELECT * FROM republic.test_table", con=mock_binding)
     pd.testing.assert_frame_equal(df, postgres_df)
 
 
 def test_postgres_resource_inject_and_read_query(postgres_df, read_sql_mock, mocked_session, mock_binding):
-    config = PostgresConfig(
+    resource = PostgresResource(
         db_user="[[db_user]]",
         db_host="{db_host}",
         db_port=1234,
         db_name="that_{db_name}",
         db_schema="[[republic]]",
         sql_query="SELECT * FROM [[republic]].[[table]]",
     )
-    config = config.inject(
+    resource = resource.inject(
         db_user="test_user", db_host="test_host", db_name="test_db", table="test_table", republic="republic"
     )
-    resource = PostgresResource(config)
     df = resource.read()
     read_sql_mock.assert_called_once_with(sql="SELECT * FROM republic.test_table", con=mock_binding)
     pd.testing.assert_frame_equal(df, postgres_df)
 
 
 @pytest.mark.parametrize("arg_to_miss_out", ["db_user", "db_host", "db_name", "table"])
 def test_postgres_resource_check_raises_on_incomplete_injection(
     arg_to_miss_out, postgres_df, read_sql_mock, mocked_session, mock_binding
 ):
     args = {"db_user": "test_user", "db_host": "test_host", "db_name": "test_db", "table": "test_table"}
     args.pop(arg_to_miss_out)
-    config = PostgresConfig(
+    resource = PostgresResource(
         db_user="[[db_user]]",
         db_host="{db_host}",
         db_port=1234,
         db_name="that_{db_name}",
         table_name="[[table]]",
     )
-    config = config.inject(**args)
+    resource = resource.inject(**args)
     with pytest.raises(InjectionError):
-        config.check_injections()
+        resource.check_injections()
 
 
 def test_postgres_resource_raises_on_wrong_read_configuration(postgres_df, read_sql_mock, mocked_session, mock_binding):
-    config = PostgresConfig(
+    resource = PostgresResource(
         db_user="test_user",
         db_host="test_host",
         db_port=1234,
         db_name="test_db",
         table_name="test_table",
         sql_query="SELECT * FROM other_table",
     )
-    resource = PostgresResource(config)
     with pytest.raises(ConfigurationError):
         resource.read()
 
 
 def test_postgres_resource_raises_on_wrong_write_configuration(
     postgres_df, read_sql_mock, mocked_session, mock_binding, to_sql_mock, mock_cursor
 ):
-    config = PostgresConfig(
+    resource = PostgresResource(
         db_user="test_user",
         db_host="test_host",
         db_port=1234,
         db_name="test_db",
         sql_query="SELECT * FROM other_table",
     )
-    resource = PostgresResource(config)
     with pytest.raises(ConfigurationError):
         resource.write(postgres_df)
```

### Comparing `dynamicio-5.0.0rc1/tests/test_validations.py` & `dynamicio-5.0.0rc2/tests/test_validations.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,43 +1,41 @@
 import pandas as pd
 import pytest
 from pandera import Field, SchemaModel
 from pandera.errors import SchemaError
 from pandera.typing import Series
 
-from dynamicio import ParquetConfig, ParquetResource
+from dynamicio import ParquetResource
 from tests.constants import TEST_RESOURCES
 
 
 class ParquetSampleSchema(SchemaModel):
     """Schema for sample parquet file."""
 
     id: Series[int]
     foo_name: Series[str]
     bar: Series[int]
 
 
 def test_parquet_resource_read_with_schema():
     test_path = TEST_RESOURCES / "data/input/parquet_sample.parquet"
 
-    resource = ParquetConfig(path=test_path)
-    resource = ParquetResource(resource, ParquetSampleSchema)
+    resource = ParquetResource(path=test_path, pa_schema=ParquetSampleSchema)
     df = resource.read()
 
     target_df = pd.read_parquet(test_path)
     pd.testing.assert_frame_equal(df, target_df)
 
 
 def test_parquet_resource_write_with_schema(output_dir_path):
     input_path = TEST_RESOURCES / "data/input/parquet_sample.parquet"
     output_path = output_dir_path / "test_parquet_resource_write.parquet"
     in_memory_df = pd.read_parquet(input_path)
 
-    config = ParquetConfig(path=output_path)
-    resource = ParquetResource(config, ParquetSampleSchema)
+    resource = ParquetResource(path=output_path, pa_schema=ParquetSampleSchema)
     resource.write(in_memory_df)
 
     target_df = pd.read_parquet(output_path)
     pd.testing.assert_frame_equal(in_memory_df, target_df)
 
 
 def test_parquet_resource_read_with_schema_fails_validation():
@@ -45,16 +43,15 @@
         """Schema for sample parquet file."""
 
         id: Series[int] = Field(gt=3)
         foo_name: Series[str]
         bar: Series[int]
 
     test_path = TEST_RESOURCES / "data/input/parquet_sample.parquet"
-    config = ParquetConfig(path=test_path)
-    resource = ParquetResource(config, ParquetSampleSchema)
+    resource = ParquetResource(path=test_path, pa_schema=ParquetSampleSchema)
     with pytest.raises(SchemaError):
         resource.read()
 
 
 def test_parquet_resource_read_with_schema_pandera_config_is_applied():
     class ParquetSampleSchema(SchemaModel):
         """Schema for sample parquet file."""
@@ -62,11 +59,10 @@
         id: Series[int]
         foo_name: Series[str]
 
         class Config:
             strict = True
 
     test_path = TEST_RESOURCES / "data/input/parquet_sample.parquet"
-    config = ParquetConfig(path=test_path)
-    resource = ParquetResource(config, ParquetSampleSchema)
+    resource = ParquetResource(path=test_path, pa_schema=ParquetSampleSchema)
     with pytest.raises(SchemaError):
         resource.read()
```

