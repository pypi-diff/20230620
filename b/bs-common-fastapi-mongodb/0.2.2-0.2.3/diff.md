# Comparing `tmp/bs_common_fastapi_mongodb-0.2.2.tar.gz` & `tmp/bs_common_fastapi_mongodb-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bs_common_fastapi_mongodb-0.2.2.tar", max compression
+gzip compressed data, was "bs_common_fastapi_mongodb-0.2.3.tar", max compression
```

## Comparing `bs_common_fastapi_mongodb-0.2.2.tar` & `bs_common_fastapi_mongodb-0.2.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       27 2023-06-19 21:48:08.450249 bs_common_fastapi_mongodb-0.2.2/README.md
--rw-r--r--   0        0        0        0 2023-06-19 21:52:57.103108 bs_common_fastapi_mongodb-0.2.2/bs_common_fastapi_mongodb/__init__.py
--rw-r--r--   0        0        0        0 2023-06-19 21:55:09.317338 bs_common_fastapi_mongodb-0.2.2/bs_common_fastapi_mongodb/common/__init__.py
--rw-r--r--   0        0        0        0 2023-06-19 21:55:15.837448 bs_common_fastapi_mongodb-0.2.2/bs_common_fastapi_mongodb/common/application/__init__.py
--rw-r--r--   0        0        0     3693 2023-06-20 12:17:50.986458 bs_common_fastapi_mongodb-0.2.2/bs_common_fastapi_mongodb/common/application/base.py
--rw-r--r--   0        0        0        0 2023-06-19 22:06:14.214350 bs_common_fastapi_mongodb-0.2.2/bs_common_fastapi_mongodb/common/config/__init__.py
--rw-r--r--   0        0        0      549 2023-06-20 00:24:57.661356 bs_common_fastapi_mongodb-0.2.2/bs_common_fastapi_mongodb/common/config/base.py
--rw-r--r--   0        0        0        0 2023-06-19 22:04:33.818873 bs_common_fastapi_mongodb-0.2.2/bs_common_fastapi_mongodb/common/dependencies/__init__.py
--rw-r--r--   0        0        0      944 2023-06-20 00:31:39.821962 bs_common_fastapi_mongodb-0.2.2/bs_common_fastapi_mongodb/common/dependencies/base.py
--rw-r--r--   0        0        0        0 2023-06-20 00:09:45.267778 bs_common_fastapi_mongodb-0.2.2/bs_common_fastapi_mongodb/common/model/__init__.py
--rw-r--r--   0        0        0      682 2023-06-20 00:13:07.226705 bs_common_fastapi_mongodb-0.2.2/bs_common_fastapi_mongodb/common/model/base_default_model.py
--rw-r--r--   0        0        0      388 2023-06-20 12:18:35.417803 bs_common_fastapi_mongodb-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      423 1970-01-01 00:00:00.000000 bs_common_fastapi_mongodb-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0       27 2023-06-19 21:48:08.450249 bs_common_fastapi_mongodb-0.2.3/README.md
+-rw-r--r--   0        0        0        0 2023-06-19 21:52:57.103108 bs_common_fastapi_mongodb-0.2.3/bs_common_fastapi_mongodb/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-19 21:55:09.317338 bs_common_fastapi_mongodb-0.2.3/bs_common_fastapi_mongodb/common/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-19 21:55:15.837448 bs_common_fastapi_mongodb-0.2.3/bs_common_fastapi_mongodb/common/application/__init__.py
+-rw-r--r--   0        0        0     3693 2023-06-20 12:17:50.986458 bs_common_fastapi_mongodb-0.2.3/bs_common_fastapi_mongodb/common/application/base.py
+-rw-r--r--   0        0        0        0 2023-06-19 22:06:14.214350 bs_common_fastapi_mongodb-0.2.3/bs_common_fastapi_mongodb/common/config/__init__.py
+-rw-r--r--   0        0        0      549 2023-06-20 00:24:57.661356 bs_common_fastapi_mongodb-0.2.3/bs_common_fastapi_mongodb/common/config/base.py
+-rw-r--r--   0        0        0        0 2023-06-19 22:04:33.818873 bs_common_fastapi_mongodb-0.2.3/bs_common_fastapi_mongodb/common/dependencies/__init__.py
+-rw-r--r--   0        0        0      944 2023-06-20 00:31:39.821962 bs_common_fastapi_mongodb-0.2.3/bs_common_fastapi_mongodb/common/dependencies/base.py
+-rw-r--r--   0        0        0        0 2023-06-20 00:09:45.267778 bs_common_fastapi_mongodb-0.2.3/bs_common_fastapi_mongodb/common/model/__init__.py
+-rw-r--r--   0        0        0      682 2023-06-20 00:13:07.226705 bs_common_fastapi_mongodb-0.2.3/bs_common_fastapi_mongodb/common/model/base_default_model.py
+-rw-r--r--   0        0        0      388 2023-06-20 13:27:37.371571 bs_common_fastapi_mongodb-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      423 1970-01-01 00:00:00.000000 bs_common_fastapi_mongodb-0.2.3/PKG-INFO
```

### Comparing `bs_common_fastapi_mongodb-0.2.2/bs_common_fastapi_mongodb/common/application/base.py` & `bs_common_fastapi_mongodb-0.2.3/bs_common_fastapi_mongodb/common/application/base.py`

 * *Files identical despite different names*

### Comparing `bs_common_fastapi_mongodb-0.2.2/bs_common_fastapi_mongodb/common/config/base.py` & `bs_common_fastapi_mongodb-0.2.3/bs_common_fastapi_mongodb/common/config/base.py`

 * *Files identical despite different names*

### Comparing `bs_common_fastapi_mongodb-0.2.2/bs_common_fastapi_mongodb/common/dependencies/base.py` & `bs_common_fastapi_mongodb-0.2.3/bs_common_fastapi_mongodb/common/dependencies/base.py`

 * *Files identical despite different names*

### Comparing `bs_common_fastapi_mongodb-0.2.2/bs_common_fastapi_mongodb/common/model/base_default_model.py` & `bs_common_fastapi_mongodb-0.2.3/bs_common_fastapi_mongodb/common/model/base_default_model.py`

 * *Files identical despite different names*

