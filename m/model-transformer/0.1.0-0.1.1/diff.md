# Comparing `tmp/model_transformer-0.1.0.tar.gz` & `tmp/model_transformer-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "model_transformer-0.1.0.tar", max compression
+gzip compressed data, was "model_transformer-0.1.1.tar", max compression
```

## Comparing `model_transformer-0.1.0.tar` & `model_transformer-0.1.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      988 2023-06-20 13:31:05.803724 model_transformer-0.1.0/README.md
--rw-r--r--   0        0        0     2030 2023-06-20 13:12:52.933951 model_transformer-0.1.0/model_transformer/__init__.py
--rw-r--r--   0        0        0      384 2023-06-20 13:08:01.224013 model_transformer-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1290 1970-01-01 00:00:00.000000 model_transformer-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      989 2023-06-20 13:55:39.433417 model_transformer-0.1.1/README.md
+-rw-r--r--   0        0        0     2030 2023-06-20 13:12:52.933951 model_transformer-0.1.1/model_transformer/__init__.py
+-rw-r--r--   0        0        0      384 2023-06-20 13:55:35.223418 model_transformer-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1291 1970-01-01 00:00:00.000000 model_transformer-0.1.1/PKG-INFO
```

### Comparing `model_transformer-0.1.0/README.md` & `model_transformer-0.1.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from datetime import datetime
 
 from model_transformer import Transformer, Field
 
 class SampleTransformer(Transformer):
     name = Field("name") # This field will extract name from input data.
 
-    def get_age(self, row: dict) -> int
+    def get_age(self, row: dict) -> int:
         birth = datetime.fromisoformat(row.get("birth"))
 
         diff = datetime.now() - birth
 
         return diff.days // 365
 
 data = [
```

### Comparing `model_transformer-0.1.0/model_transformer/__init__.py` & `model_transformer-0.1.1/model_transformer/__init__.py`

 * *Files identical despite different names*

### Comparing `model_transformer-0.1.0/PKG-INFO` & `model_transformer-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: model-transformer
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Giancarlo Rocha
 Author-email: giancarloiff@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
@@ -27,15 +27,15 @@
 from datetime import datetime
 
 from model_transformer import Transformer, Field
 
 class SampleTransformer(Transformer):
     name = Field("name") # This field will extract name from input data.
 
-    def get_age(self, row: dict) -> int
+    def get_age(self, row: dict) -> int:
         birth = datetime.fromisoformat(row.get("birth"))
 
         diff = datetime.now() - birth
 
         return diff.days // 365
 
 data = [
```

