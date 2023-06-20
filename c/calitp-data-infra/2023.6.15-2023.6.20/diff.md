# Comparing `tmp/calitp_data_infra-2023.6.15.tar.gz` & `tmp/calitp_data_infra-2023.6.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calitp_data_infra-2023.6.15.tar", max compression
+gzip compressed data, was "calitp_data_infra-2023.6.20.tar", max compression
```

## Comparing `calitp_data_infra-2023.6.15.tar` & `calitp_data_infra-2023.6.20.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2023-06-14 15:20:22.416689 calitp_data_infra-2023.6.15/calitp_data_infra/__init__.py
--rw-r--r--   0        0        0     1154 2023-06-14 15:20:22.416792 calitp_data_infra-2023.6.15/calitp_data_infra/auth.py
--rw-r--r--   0        0        0    24480 2023-06-15 14:24:35.027870 calitp_data_infra-2023.6.15/calitp_data_infra/storage.py
--rw-r--r--   0        0        0      751 2023-06-15 16:03:04.797779 calitp_data_infra-2023.6.15/pyproject.toml
--rw-r--r--   0        0        0      763 1970-01-01 00:00:00.000000 calitp_data_infra-2023.6.15/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-14 15:20:22.416689 calitp_data_infra-2023.6.20/calitp_data_infra/__init__.py
+-rw-r--r--   0        0        0     1154 2023-06-14 15:20:22.416792 calitp_data_infra-2023.6.20/calitp_data_infra/auth.py
+-rw-r--r--   0        0        0    24488 2023-06-20 15:44:59.472390 calitp_data_infra-2023.6.20/calitp_data_infra/storage.py
+-rw-r--r--   0        0        0      752 2023-06-20 15:54:29.473732 calitp_data_infra-2023.6.20/pyproject.toml
+-rw-r--r--   0        0        0      763 1970-01-01 00:00:00.000000 calitp_data_infra-2023.6.20/PKG-INFO
```

### Comparing `calitp_data_infra-2023.6.15/calitp_data_infra/auth.py` & `calitp_data_infra-2023.6.20/calitp_data_infra/auth.py`

 * *Files identical despite different names*

### Comparing `calitp_data_infra-2023.6.15/calitp_data_infra/storage.py` & `calitp_data_infra-2023.6.20/calitp_data_infra/storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -172,30 +172,32 @@
         content_type,
         client,
     )
 
 
 # Is there a better pattern for making this retry optional by the caller?
 @backoff.on_exception(
-    backoff.expo(base=5),
+    backoff.expo,
+    base=5,
     exception=(Exception,),
     max_tries=3,
 )
 def upload_from_string_with_retry(*args, **kwargs):
     return upload_from_string(*args, **kwargs)
 
 
 def set_metadata(blob: storage.Blob, model: BaseModel, exclude=None):
     blob.metadata = {PARTITIONED_ARTIFACT_METADATA_KEY: model.json(exclude=exclude)}
     blob.patch()
 
 
 # Is there a better pattern for making this retry optional by the caller?
 @backoff.on_exception(
-    backoff.expo(base=5),
+    backoff.expo,
+    base=5,
     exception=(Exception,),
     max_tries=3,
 )
 def set_metadata_with_retry(*args, **kwargs):
     return set_metadata(*args, **kwargs)
```

### Comparing `calitp_data_infra-2023.6.15/pyproject.toml` & `calitp_data_infra-2023.6.20/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "calitp-data-infra"
-version = "2023.6.15"
+version = "2023.06.20"
 description = "Shared code for developing data pipelines that process Cal-ITP data."
 authors = ["Andrew Vaccaro <andrew.v@jarv.us>"]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.10"
 # Some of these are pinned oddly to play nicely with Composer
 pydantic = "~1.9"
```

### Comparing `calitp_data_infra-2023.6.15/PKG-INFO` & `calitp_data_infra-2023.6.20/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calitp-data-infra
-Version: 2023.6.15
+Version: 2023.6.20
 Summary: Shared code for developing data pipelines that process Cal-ITP data.
 Author: Andrew Vaccaro
 Author-email: andrew.v@jarv.us
 Requires-Python: >=3.8,<3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

