# Comparing `tmp/bs_common_fastapi-0.3.1.tar.gz` & `tmp/bs_common_fastapi-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bs_common_fastapi-0.3.1.tar", max compression
+gzip compressed data, was "bs_common_fastapi-0.3.2.tar", max compression
```

## Comparing `bs_common_fastapi-0.3.1.tar` & `bs_common_fastapi-0.3.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      174 2023-06-19 14:46:25.417011 bs_common_fastapi-0.3.1/README.md
--rw-r--r--   0        0        0        0 2023-06-17 00:58:23.542317 bs_common_fastapi-0.3.1/bs_common_fastapi/__init__.py
--rw-r--r--   0        0        0        0 2023-06-17 01:21:20.232881 bs_common_fastapi-0.3.1/bs_common_fastapi/common/__init__.py
--rw-r--r--   0        0        0        0 2023-06-17 01:12:50.700330 bs_common_fastapi-0.3.1/bs_common_fastapi/common/config/__init__.py
--rw-r--r--   0        0        0     1173 2023-06-20 00:25:56.731497 bs_common_fastapi-0.3.1/bs_common_fastapi/common/config/base.py
--rw-r--r--   0        0        0      387 2023-06-19 13:00:52.405937 bs_common_fastapi-0.3.1/bs_common_fastapi/common/exception/__init__.py
--rw-r--r--   0        0        0        0 2023-06-17 00:59:12.863096 bs_common_fastapi-0.3.1/bs_common_fastapi/common/model/__init__.py
--rw-r--r--   0        0        0      797 2023-06-19 13:38:00.004819 bs_common_fastapi-0.3.1/bs_common_fastapi/common/model/base_default_model.py
--rw-r--r--   0        0        0      620 2023-06-20 00:26:27.952580 bs_common_fastapi-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      516 1970-01-01 00:00:00.000000 bs_common_fastapi-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      174 2023-06-19 14:46:25.417011 bs_common_fastapi-0.3.2/README.md
+-rw-r--r--   0        0        0        0 2023-06-17 00:58:23.542317 bs_common_fastapi-0.3.2/bs_common_fastapi/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-17 01:21:20.232881 bs_common_fastapi-0.3.2/bs_common_fastapi/common/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-17 01:12:50.700330 bs_common_fastapi-0.3.2/bs_common_fastapi/common/config/__init__.py
+-rw-r--r--   0        0        0      862 2023-06-20 13:11:29.154225 bs_common_fastapi-0.3.2/bs_common_fastapi/common/config/base.py
+-rw-r--r--   0        0        0      387 2023-06-19 13:00:52.405937 bs_common_fastapi-0.3.2/bs_common_fastapi/common/exception/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-17 00:59:12.863096 bs_common_fastapi-0.3.2/bs_common_fastapi/common/model/__init__.py
+-rw-r--r--   0        0        0      797 2023-06-19 13:38:00.004819 bs_common_fastapi-0.3.2/bs_common_fastapi/common/model/base_default_model.py
+-rw-r--r--   0        0        0      620 2023-06-20 13:12:13.234428 bs_common_fastapi-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      516 1970-01-01 00:00:00.000000 bs_common_fastapi-0.3.2/PKG-INFO
```

### Comparing `bs_common_fastapi-0.3.1/bs_common_fastapi/common/model/base_default_model.py` & `bs_common_fastapi-0.3.2/bs_common_fastapi/common/model/base_default_model.py`

 * *Files identical despite different names*

### Comparing `bs_common_fastapi-0.3.1/pyproject.toml` & `bs_common_fastapi-0.3.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bs-common-fastapi"
-version = "0.3.1"
+version = "0.3.2"
 description = ""
 authors = ["Bruno Segato <brunosegatoit@gmail.com>"]
 readme = "README.md"
 packages = [{include = "bs_common_fastapi"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `bs_common_fastapi-0.3.1/PKG-INFO` & `bs_common_fastapi-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bs-common-fastapi
-Version: 0.3.1
+Version: 0.3.2
 Summary: 
 Author: Bruno Segato
 Author-email: brunosegatoit@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: fastapi (>=0.97.0,<0.98.0)
```

