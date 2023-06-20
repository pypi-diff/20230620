# Comparing `tmp/meltanolabs_target_snowflake-0.2.1.tar.gz` & `tmp/meltanolabs_target_snowflake-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meltanolabs_target_snowflake-0.2.1.tar", max compression
+gzip compressed data, was "meltanolabs_target_snowflake-0.3.0.tar", max compression
```

## Comparing `meltanolabs_target_snowflake-0.2.1.tar` & `meltanolabs_target_snowflake-0.3.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     3860 2023-06-14 22:10:42.781383 meltanolabs_target_snowflake-0.2.1/LICENSE
--rw-r--r--   0        0        0     3924 2023-06-14 22:10:42.781383 meltanolabs_target_snowflake-0.2.1/README.md
--rw-r--r--   0        0        0     1282 2023-06-14 22:11:02.493650 meltanolabs_target_snowflake-0.2.1/pyproject.toml
--rw-r--r--   0        0        0       89 2023-06-14 22:11:02.493650 meltanolabs_target_snowflake-0.2.1/target_snowflake/__init__.py
--rw-r--r--   0        0        0    16397 2023-06-14 22:10:42.785383 meltanolabs_target_snowflake-0.2.1/target_snowflake/connector.py
--rw-r--r--   0        0        0     7060 2023-06-14 22:10:42.785383 meltanolabs_target_snowflake-0.2.1/target_snowflake/sinks.py
--rw-r--r--   0        0        0      724 2023-06-14 22:10:42.785383 meltanolabs_target_snowflake-0.2.1/target_snowflake/snowflake_types.py
--rw-r--r--   0        0        0     4057 2023-06-14 22:10:42.785383 meltanolabs_target_snowflake-0.2.1/target_snowflake/target.py
--rw-r--r--   0        0        0     4671 1970-01-01 00:00:00.000000 meltanolabs_target_snowflake-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     3860 2023-06-20 20:10:11.284209 meltanolabs_target_snowflake-0.3.0/LICENSE
+-rw-r--r--   0        0        0     3924 2023-06-20 20:10:11.284209 meltanolabs_target_snowflake-0.3.0/README.md
+-rw-r--r--   0        0        0     1282 2023-06-20 20:10:32.916325 meltanolabs_target_snowflake-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       89 2023-06-20 20:10:32.920325 meltanolabs_target_snowflake-0.3.0/target_snowflake/__init__.py
+-rw-r--r--   0        0        0    18228 2023-06-20 20:10:11.288209 meltanolabs_target_snowflake-0.3.0/target_snowflake/connector.py
+-rw-r--r--   0        0        0     7872 2023-06-20 20:10:11.288209 meltanolabs_target_snowflake-0.3.0/target_snowflake/sinks.py
+-rw-r--r--   0        0        0      724 2023-06-20 20:10:11.288209 meltanolabs_target_snowflake-0.3.0/target_snowflake/snowflake_types.py
+-rw-r--r--   0        0        0     4057 2023-06-20 20:10:11.288209 meltanolabs_target_snowflake-0.3.0/target_snowflake/target.py
+-rw-r--r--   0        0        0     4671 1970-01-01 00:00:00.000000 meltanolabs_target_snowflake-0.3.0/PKG-INFO
```

### Comparing `meltanolabs_target_snowflake-0.2.1/LICENSE` & `meltanolabs_target_snowflake-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_snowflake-0.2.1/README.md` & `meltanolabs_target_snowflake-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_snowflake-0.2.1/pyproject.toml` & `meltanolabs_target_snowflake-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "meltanolabs-target-snowflake"
-version = "0.2.1"
+version = "0.3.0"
 description = "`target-snowflake` is a Singer target for Snowflake, built with the Meltano SDK for Singer Targets."
 readme = "README.md"
 authors = ["Ken Payne"]
 keywords = [
     "ELT",
     "Snowflake",
 ]
```

### Comparing `meltanolabs_target_snowflake-0.2.1/target_snowflake/connector.py` & `meltanolabs_target_snowflake-0.3.0/target_snowflake/connector.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from operator import contains, eq
 from typing import Dict, List, Sequence, Tuple, Union, cast
 
+import snowflake.sqlalchemy.custom_types as sct
 import sqlalchemy
 from singer_sdk import typing as th
 from singer_sdk.connectors import SQLConnector
 from snowflake.sqlalchemy import URL
 from snowflake.sqlalchemy.base import SnowflakeIdentifierPreparer
 from snowflake.sqlalchemy.snowdialect import SnowflakeDialect
 from sqlalchemy.engine import Engine
@@ -31,23 +32,51 @@
 def evaluate_typemaps(type_maps, compare_value, unmatched_value):
     for type_map in type_maps:
         if type_map.match(compare_value):
             return type_map.map_value
     return unmatched_value
 
 
+def _jsonschema_type_check(jsonschema_type: dict, type_check: Tuple[str]) -> bool:
+    """Return True if the jsonschema_type supports the provided type.
+
+    Args:
+        jsonschema_type: The type dict.
+        type_check: A tuple of type strings to look for.
+
+    Returns:
+        True if the schema suports the type.
+    """
+    if "type" in jsonschema_type:
+        if isinstance(jsonschema_type["type"], (list, tuple)):
+            for schema_type in jsonschema_type["type"]:
+                if schema_type in type_check:
+                    return True
+        else:
+            if jsonschema_type.get("type") in type_check:  # noqa: PLR5501
+                return True
+
+    # TODO: remove following release of https://github.com/meltano/sdk/issues/1774
+    if any(
+        _jsonschema_type_check(t, type_check)
+        for t in jsonschema_type.get("anyOf", ())
+    ):
+        return True
+
+    return False
+
 class SnowflakeConnector(SQLConnector):
     """Snowflake Target Connector.
 
     This class handles all DDL and type conversions.
     """
 
     allow_column_add: bool = True  # Whether ADD COLUMN is supported.
     allow_column_rename: bool = True  # Whether RENAME COLUMN is supported.
-    allow_column_alter: bool = False  # Whether altering column types is supported.
+    allow_column_alter: bool = True  # Whether altering column types is supported.
     allow_merge_upsert: bool = False  # Whether MERGE UPSERT is supported.
     allow_temp_tables: bool = True  # Whether temp tables are supported.
 
     def __init__(self, *args, **kwargs) -> None:
         self.table_cache: dict = {}
         self.schema_cache: dict = {}
         super().__init__(*args, **kwargs)
@@ -66,18 +95,41 @@
         Returns:
             An ordered list of column objects.
         """
         # Cache these columns because they're frequently used.
         if full_table_name in self.table_cache:
             return self.table_cache[full_table_name]
         else:
-            parsed_columns = super().get_table_columns(full_table_name, column_names)
+            _, schema_name, table_name = self.parse_full_table_name(full_table_name)
+            inspector = sqlalchemy.inspect(self._engine)
+            columns = inspector.get_columns(table_name, schema_name)
+
+            parsed_columns = {
+                col_meta["name"]: sqlalchemy.Column(
+                    col_meta["name"],
+                    self._convert_type(col_meta["type"]),
+                    nullable=col_meta.get("nullable", False),
+                )
+                for col_meta in columns
+                if not column_names
+                or col_meta["name"].casefold() in {col.casefold() for col in column_names}
+            }
             self.table_cache[full_table_name] = parsed_columns
             return parsed_columns
 
+    def _convert_type(self, sql_type):
+        if isinstance(sql_type, sct.TIMESTAMP_NTZ):
+            return TIMESTAMP_NTZ
+        elif isinstance(sql_type, sct.NUMBER):
+            return NUMBER
+        elif isinstance(sql_type, sct.VARIANT):
+            return VARIANT
+        else:
+            return sql_type
+
     def get_sqlalchemy_url(self, config: dict) -> str:
         """Generates a SQLAlchemy URL for Snowflake.
 
         Args:
             config: The configuration for the connector.
         """
         params = {
@@ -200,20 +252,20 @@
         string_submaps = [
             TypeMap(eq, TIMESTAMP_NTZ(), "date-time"),
             TypeMap(contains, sqlalchemy.types.TIME(), "time"),
             TypeMap(eq, sqlalchemy.types.DATE(), "date"),
             TypeMap(eq, sqlalchemy.types.VARCHAR(maxlength), None),
         ]
         type_maps = [
-            TypeMap(th._jsonschema_type_check, NUMBER(), ("integer",)),
-            TypeMap(th._jsonschema_type_check, VARIANT(), ("object",)),
-            TypeMap(th._jsonschema_type_check, VARIANT(), ("array",)),
+            TypeMap(_jsonschema_type_check, NUMBER(), ("integer",)),
+            TypeMap(_jsonschema_type_check, VARIANT(), ("object",)),
+            TypeMap(_jsonschema_type_check, VARIANT(), ("array",)),
         ]
         # apply type maps
-        if th._jsonschema_type_check(jsonschema_type, ("string",)):
+        if _jsonschema_type_check(jsonschema_type, ("string",)):
             datelike_type = th.get_datelike_property_type(jsonschema_type)
             target_type = evaluate_typemaps(string_submaps, datelike_type, target_type)
         else:
             target_type = evaluate_typemaps(type_maps, jsonschema_type, target_type)
 
         return cast(sqlalchemy.types.TypeEngine, target_type)
 
@@ -300,15 +352,15 @@
         )
 
     def _get_file_format_statement(self, file_format):
         """Get Snowflake CREATE FILE FORMAT statement."""
         return (
             text(
                 f"create or replace file format {file_format}"
-                + "type = 'JSON' compression = 'GZIP'"
+                + "type = 'JSON' compression = 'AUTO'"
             ),
             {},
         )
 
     def _get_drop_file_format_statement(self, file_format):
         """Get Snowflake DROP FILE FORMAT statement."""
         return (
```

### Comparing `meltanolabs_target_snowflake-0.2.1/target_snowflake/sinks.py` & `meltanolabs_target_snowflake-0.3.0/target_snowflake/sinks.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,20 @@
 import os
 import typing as t
 from urllib.parse import urlparse
 from uuid import uuid4
 
 from singer_sdk import PluginBase, SQLConnector
 from singer_sdk.batch import JSONLinesBatcher
-from singer_sdk.helpers._batch import BatchConfig
+from singer_sdk.helpers._batch import (
+    BaseBatchFileEncoding,
+    BatchConfig,
+    BatchFileFormat,
+    StorageTarget,
+)
 from singer_sdk.helpers._typing import conform_record_data_types
 from singer_sdk.sinks import SQLSink
 from snowflake.sqlalchemy.base import SnowflakeIdentifierPreparer
 from snowflake.sqlalchemy.snowdialect import SnowflakeDialect
 
 from target_snowflake.connector import SnowflakeConnector
 
@@ -204,7 +209,29 @@
             self.connector.remove_staged_files(sync_id=sync_id)
             # clean up local files
             if self.config.get("clean_up_batch_files"):
                 for file_url in files:
                     file_path = urlparse(file_url).path
                     if os.path.exists(file_path):
                         os.remove(file_path)
+
+    def process_batch_files(
+        self, encoding: BaseBatchFileEncoding, files: t.Sequence[str]
+    ) -> None:
+        """Process a batch file with the given batch context.
+
+        Args:
+            encoding: The batch file encoding.
+            files: The batch files to process.
+
+        Raises:
+            NotImplementedError: If the batch file encoding is not supported.
+        """
+        if encoding.format == BatchFileFormat.JSONL:
+            self.insert_batch_files_via_internal_stage(
+                full_table_name=self.full_table_name,
+                files=files,
+            )
+        else:
+            raise NotImplementedError(
+                f"Unsupported batch file encoding: {encoding.format}"
+            )
```

### Comparing `meltanolabs_target_snowflake-0.2.1/target_snowflake/snowflake_types.py` & `meltanolabs_target_snowflake-0.3.0/target_snowflake/snowflake_types.py`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_snowflake-0.2.1/target_snowflake/target.py` & `meltanolabs_target_snowflake-0.3.0/target_snowflake/target.py`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_snowflake-0.2.1/PKG-INFO` & `meltanolabs_target_snowflake-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meltanolabs-target-snowflake
-Version: 0.2.1
+Version: 0.3.0
 Summary: `target-snowflake` is a Singer target for Snowflake, built with the Meltano SDK for Singer Targets.
 License: Apache 2.0
 Keywords: ELT,Snowflake
 Author: Ken Payne
 Requires-Python: >=3.7.1,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

