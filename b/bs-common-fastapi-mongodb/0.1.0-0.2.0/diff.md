# Comparing `tmp/bs_common_fastapi_mongodb-0.1.0.tar.gz` & `tmp/bs_common_fastapi_mongodb-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bs_common_fastapi_mongodb-0.1.0.tar", max compression
+gzip compressed data, was "bs_common_fastapi_mongodb-0.2.0.tar", max compression
```

## Comparing `bs_common_fastapi_mongodb-0.1.0.tar` & `bs_common_fastapi_mongodb-0.2.0.tar`

### file list

```diff
@@ -1,11 +1,13 @@
--rw-r--r--   0        0        0       27 2023-06-19 21:48:08.450249 bs_common_fastapi_mongodb-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-06-19 21:52:57.103108 bs_common_fastapi_mongodb-0.1.0/bs_common_fastapi_mongodb/__init__.py
--rw-r--r--   0        0        0        0 2023-06-19 21:55:09.317338 bs_common_fastapi_mongodb-0.1.0/bs_common_fastapi_mongodb/common/__init__.py
--rw-r--r--   0        0        0        0 2023-06-19 21:55:15.837448 bs_common_fastapi_mongodb-0.1.0/bs_common_fastapi_mongodb/common/application/__init__.py
--rw-r--r--   0        0        0     3665 2023-06-19 22:02:54.305191 bs_common_fastapi_mongodb-0.1.0/bs_common_fastapi_mongodb/common/application/base.py
--rw-r--r--   0        0        0        0 2023-06-19 22:06:14.214350 bs_common_fastapi_mongodb-0.1.0/bs_common_fastapi_mongodb/common/config/__init__.py
--rw-r--r--   0        0        0      516 2023-06-19 22:08:14.018068 bs_common_fastapi_mongodb-0.1.0/bs_common_fastapi_mongodb/common/config/base.py
--rw-r--r--   0        0        0        0 2023-06-19 22:04:33.818873 bs_common_fastapi_mongodb-0.1.0/bs_common_fastapi_mongodb/common/dependencies/__init__.py
--rw-r--r--   0        0        0      917 2023-06-19 23:50:05.543807 bs_common_fastapi_mongodb-0.1.0/bs_common_fastapi_mongodb/common/dependencies/base.py
--rw-r--r--   0        0        0      388 2023-06-19 23:56:12.889047 bs_common_fastapi_mongodb-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      423 1970-01-01 00:00:00.000000 bs_common_fastapi_mongodb-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       27 2023-06-19 21:48:08.450249 bs_common_fastapi_mongodb-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-19 21:52:57.103108 bs_common_fastapi_mongodb-0.2.0/bs_common_fastapi_mongodb/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-19 21:55:09.317338 bs_common_fastapi_mongodb-0.2.0/bs_common_fastapi_mongodb/common/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-19 21:55:15.837448 bs_common_fastapi_mongodb-0.2.0/bs_common_fastapi_mongodb/common/application/__init__.py
+-rw-r--r--   0        0        0     3665 2023-06-19 22:02:54.305191 bs_common_fastapi_mongodb-0.2.0/bs_common_fastapi_mongodb/common/application/base.py
+-rw-r--r--   0        0        0        0 2023-06-19 22:06:14.214350 bs_common_fastapi_mongodb-0.2.0/bs_common_fastapi_mongodb/common/config/__init__.py
+-rw-r--r--   0        0        0      516 2023-06-19 22:08:14.018068 bs_common_fastapi_mongodb-0.2.0/bs_common_fastapi_mongodb/common/config/base.py
+-rw-r--r--   0        0        0        0 2023-06-19 22:04:33.818873 bs_common_fastapi_mongodb-0.2.0/bs_common_fastapi_mongodb/common/dependencies/__init__.py
+-rw-r--r--   0        0        0      917 2023-06-19 23:50:05.543807 bs_common_fastapi_mongodb-0.2.0/bs_common_fastapi_mongodb/common/dependencies/base.py
+-rw-r--r--   0        0        0        0 2023-06-20 00:09:45.267778 bs_common_fastapi_mongodb-0.2.0/bs_common_fastapi_mongodb/common/model/__init__.py
+-rw-r--r--   0        0        0      682 2023-06-20 00:13:07.226705 bs_common_fastapi_mongodb-0.2.0/bs_common_fastapi_mongodb/common/model/base_default_model.py
+-rw-r--r--   0        0        0      388 2023-06-20 00:13:33.681189 bs_common_fastapi_mongodb-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      423 1970-01-01 00:00:00.000000 bs_common_fastapi_mongodb-0.2.0/PKG-INFO
```

### Comparing `bs_common_fastapi_mongodb-0.1.0/bs_common_fastapi_mongodb/common/application/base.py` & `bs_common_fastapi_mongodb-0.2.0/bs_common_fastapi_mongodb/common/application/base.py`

 * *Files identical despite different names*

### Comparing `bs_common_fastapi_mongodb-0.1.0/bs_common_fastapi_mongodb/common/config/base.py` & `bs_common_fastapi_mongodb-0.2.0/bs_common_fastapi_mongodb/common/config/base.py`

 * *Files identical despite different names*

### Comparing `bs_common_fastapi_mongodb-0.1.0/bs_common_fastapi_mongodb/common/dependencies/base.py` & `bs_common_fastapi_mongodb-0.2.0/bs_common_fastapi_mongodb/common/dependencies/base.py`

 * *Files identical despite different names*

