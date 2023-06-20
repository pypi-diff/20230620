# Comparing `tmp/target_s3_delta-0.0.2.tar.gz` & `tmp/target_s3_delta-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "target_s3_delta-0.0.2.tar", max compression
+gzip compressed data, was "target_s3_delta-0.0.3.tar", max compression
```

## Comparing `target_s3_delta-0.0.2.tar` & `target_s3_delta-0.0.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      165 2023-05-11 21:51:01.799055 target_s3_delta-0.0.2/README.md
--rw-r--r--   0        0        0     1050 2023-05-11 21:51:32.792113 target_s3_delta-0.0.2/pyproject.toml
--rw-r--r--   0        0        0       27 2023-05-07 18:12:10.284812 target_s3_delta-0.0.2/target_s3_delta/__init__.py
--rw-r--r--   0        0        0     3810 2023-05-11 21:49:41.250236 target_s3_delta-0.0.2/target_s3_delta/sinks.py
--rw-r--r--   0        0        0      838 2023-05-11 20:29:50.089499 target_s3_delta-0.0.2/target_s3_delta/target.py
--rw-r--r--   0        0        0      921 1970-01-01 00:00:00.000000 target_s3_delta-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      165 2023-06-19 14:17:00.274933 target_s3_delta-0.0.3/README.md
+-rw-r--r--   0        0        0     1050 2023-06-20 07:42:14.377011 target_s3_delta-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0       27 2023-06-19 14:17:00.276362 target_s3_delta-0.0.3/target_s3_delta/__init__.py
+-rw-r--r--   0        0        0     3447 2023-06-19 20:19:07.448666 target_s3_delta-0.0.3/target_s3_delta/sinks.py
+-rw-r--r--   0        0        0     2141 2023-06-19 20:23:41.085928 target_s3_delta-0.0.3/target_s3_delta/target.py
+-rw-r--r--   0        0        0      921 1970-01-01 00:00:00.000000 target_s3_delta-0.0.3/PKG-INFO
```

### Comparing `target_s3_delta-0.0.2/pyproject.toml` & `target_s3_delta-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "target-s3-delta"
-version = "0.0.2"
+version = "0.0.3"
 description = "`target-s3-delta` is a Singer target for s3-delta, built with the Meltano Singer SDK."
 readme = "README.md"
 authors = ["resul yurttakalan"]
 keywords = [
     "ELT",
     "s3-delta",
 ]
```

### Comparing `target_s3_delta-0.0.2/target_s3_delta/sinks.py` & `target_s3_delta-0.0.3/target_s3_delta/sinks.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 """s3-delta target sink class, which handles writing streams."""
 
 from __future__ import annotations
 
+import os
+
 from dateutil import parser
 from deltalake import write_deltalake
 from singer_sdk.helpers._typing import (
     DatetimeErrorTreatmentEnum,
     get_datelike_property_type,
     handle_invalid_timestamp_in_record,
 )
 from singer_sdk.sinks import BatchSink
 import pandas as pd
 
 NOT_PROPER_DATETIME_FORMAT = "0000-00-00 00:00:00"
-
+TEMP_DATA_DIRECTORY = "/tmp/meltano_temp_data/"
 
 class S3DeltaSink(BatchSink):
     """s3-delta target sink class."""
 
     max_size = 10000  # Max records to write in one batch
 
     def process_record(self, record: dict, context: dict) -> None:
@@ -80,40 +82,24 @@
 
         Developers may optionally add additional markers to the `context` dict,
         which is unique to this batch.
 
         Args:
             context: Stream partition or context dictionary.
         """
-        # Sample:
-        # ------
-        # batch_key = context["batch_id"]
-        # context["file_path"] = f"{batch_key}.csv"
+        batch_key = context["batch_id"]
+        context["file_path"] = f"{batch_key}.parquet"
 
     def process_batch(self, context: dict) -> None:
         """Write out any prepped records and return once fully written.
 
         Args:
             context: Stream partition or context dictionary.
         """
-        df = pd.DataFrame(context["records"])
+        is_exist = os.path.exists(TEMP_DATA_DIRECTORY)
+        if not is_exist:
+            os.makedirs(TEMP_DATA_DIRECTORY)
 
-        storage_options = {
-            "AWS_ACCESS_KEY_ID": self.config.get("aws_access_key_id"),
-            "AWS_SECRET_ACCESS_KEY": self.config.get("aws_secret_access_key"),
-            "REGION": self.config.get("aws_region"),
-            "AWS_S3_ALLOW_UNSAFE_RENAME": "true",
-        }
-
-        path = self.config.get("s3_path")
-
-        write_deltalake(
-            path,
-            df,
-            storage_options=storage_options,
-            mode="overwrite",
-            overwrite_schema=True,
-        )
-
-        self.logger.info(f"Uploaded {len(context['records'])} rows.")
+        df = pd.DataFrame(context["records"])
+        df.to_parquet(f"{TEMP_DATA_DIRECTORY}{context.get('file_path')}")
 
         context["records"] = []
```

### Comparing `target_s3_delta-0.0.2/PKG-INFO` & `target_s3_delta-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: target-s3-delta
-Version: 0.0.2
+Version: 0.0.3
 Summary: `target-s3-delta` is a Singer target for s3-delta, built with the Meltano Singer SDK.
 License: Apache 2.0
 Keywords: ELT,s3-delta
 Author: resul yurttakalan
 Requires-Python: >=3.8,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

