# Comparing `tmp/handyman-0.3.5.tar.gz` & `tmp/handyman-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "handyman-0.3.5.tar", last modified: Wed Feb 15 08:13:56 2023, max compression
+gzip compressed data, was "handyman-0.3.6.tar", last modified: Tue Jun 20 05:52:12 2023, max compression
```

## Comparing `handyman-0.3.5.tar` & `handyman-0.3.6.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 deepankaragrawal   (502) staff       (20)        0 2023-02-15 08:13:56.396871 handyman-0.3.5/
--rw-r--r--   0 deepankaragrawal   (502) staff       (20)        1 2023-02-15 07:57:39.000000 handyman-0.3.5/LICENSE
--rw-r--r--   0 deepankaragrawal   (502) staff       (20)       24 2023-02-15 07:57:39.000000 handyman-0.3.5/MANIFEST.in
--rw-r--r--   0 deepankaragrawal   (502) staff       (20)     4490 2023-02-15 08:13:56.397004 handyman-0.3.5/PKG-INFO
--rw-r--r--   0 deepankaragrawal   (502) staff       (20)     3646 2023-02-15 08:04:23.000000 handyman-0.3.5/README.md
-drwxr-xr-x   0 deepankaragrawal   (502) staff       (20)        0 2023-02-15 08:13:56.393531 handyman-0.3.5/handyman/
--rw-r--r--   0 deepankaragrawal   (502) staff       (20)      172 2023-02-15 07:57:39.000000 handyman-0.3.5/handyman/__init__.py
--rw-r--r--   0 deepankaragrawal   (502) staff       (20)     1015 2023-02-15 07:57:39.000000 handyman-0.3.5/handyman/__main__.py
-drwxr-xr-x   0 deepankaragrawal   (502) staff       (20)        0 2023-02-15 08:13:56.394743 handyman-0.3.5/handyman/cli/
--rw-r--r--   0 deepankaragrawal   (502) staff       (20)        0 2023-02-15 07:57:39.000000 handyman-0.3.5/handyman/cli/__init__.py
--rw-r--r--   0 deepankaragrawal   (502) staff       (20)      915 2023-02-15 07:57:39.000000 handyman-0.3.5/handyman/cli/proto_gen.py
-drwxr-xr-x   0 deepankaragrawal   (502) staff       (20)        0 2023-02-15 08:13:56.395629 handyman-0.3.5/handyman/crypto/
--rw-r--r--   0 deepankaragrawal   (502) staff       (20)      543 2023-02-15 07:57:39.000000 handyman-0.3.5/handyman/crypto/__init__.py
--rw-r--r--   0 deepankaragrawal   (502) staff       (20)     1317 2023-02-15 07:57:39.000000 handyman-0.3.5/handyman/crypto/cache.py
--rw-r--r--   0 deepankaragrawal   (502) staff       (20)    10481 2023-02-15 07:57:39.000000 handyman-0.3.5/handyman/crypto/crypto.py
--rw-r--r--   0 deepankaragrawal   (502) staff       (20)     2805 2023-02-15 07:57:39.000000 handyman-0.3.5/handyman/crypto/exceptions.py
--rw-r--r--   0 deepankaragrawal   (502) staff       (20)     8389 2023-02-15 07:57:39.000000 handyman-0.3.5/handyman/crypto/vault.py
-drwxr-xr-x   0 deepankaragrawal   (502) staff       (20)        0 2023-02-15 08:13:56.396465 handyman-0.3.5/handyman/events/
--rw-r--r--   0 deepankaragrawal   (502) staff       (20)      290 2023-02-15 07:57:39.000000 handyman-0.3.5/handyman/events/__init__.py
--rw-r--r--   0 deepankaragrawal   (502) staff       (20)      601 2023-02-15 08:00:46.000000 handyman-0.3.5/handyman/events/event_types.py
--rw-r--r--   0 deepankaragrawal   (502) staff       (20)      361 2023-02-15 07:57:39.000000 handyman-0.3.5/handyman/events/exceptions.py
--rw-r--r--   0 deepankaragrawal   (502) staff       (20)      986 2023-02-15 07:57:39.000000 handyman-0.3.5/handyman/events/goroutine.py
--rw-r--r--   0 deepankaragrawal   (502) staff       (20)     8130 2023-02-15 08:02:54.000000 handyman-0.3.5/handyman/events/sqs.py
-drwxr-xr-x   0 deepankaragrawal   (502) staff       (20)        0 2023-02-15 08:13:56.396712 handyman-0.3.5/handyman/exceptions/
--rw-r--r--   0 deepankaragrawal   (502) staff       (20)     2972 2023-02-15 07:57:39.000000 handyman-0.3.5/handyman/exceptions/__init__.py
--rw-r--r--   0 deepankaragrawal   (502) staff       (20)      390 2023-02-15 07:57:39.000000 handyman-0.3.5/handyman/grpc_utils.py
--rw-r--r--   0 deepankaragrawal   (502) staff       (20)     1197 2023-02-15 07:57:39.000000 handyman-0.3.5/handyman/helpers.py
--rw-r--r--   0 deepankaragrawal   (502) staff       (20)     2452 2023-02-15 07:57:39.000000 handyman-0.3.5/handyman/io.py
--rw-r--r--   0 deepankaragrawal   (502) staff       (20)     2125 2023-02-15 07:57:39.000000 handyman-0.3.5/handyman/json_utils.py
--rw-r--r--   0 deepankaragrawal   (502) staff       (20)     2488 2023-02-15 07:57:39.000000 handyman-0.3.5/handyman/log.py
--rw-r--r--   0 deepankaragrawal   (502) staff       (20)     9375 2023-02-15 07:57:39.000000 handyman-0.3.5/handyman/prometheus.py
--rw-r--r--   0 deepankaragrawal   (502) staff       (20)      751 2023-02-15 07:57:39.000000 handyman-0.3.5/handyman/sentry.py
-drwxr-xr-x   0 deepankaragrawal   (502) staff       (20)        0 2023-02-15 08:13:56.394490 handyman-0.3.5/handyman.egg-info/
--rw-r--r--   0 deepankaragrawal   (502) staff       (20)     4490 2023-02-15 08:13:56.000000 handyman-0.3.5/handyman.egg-info/PKG-INFO
--rw-r--r--   0 deepankaragrawal   (502) staff       (20)      835 2023-02-15 08:13:56.000000 handyman-0.3.5/handyman.egg-info/SOURCES.txt
--rw-r--r--   0 deepankaragrawal   (502) staff       (20)        1 2023-02-15 08:13:56.000000 handyman-0.3.5/handyman.egg-info/dependency_links.txt
--rw-r--r--   0 deepankaragrawal   (502) staff       (20)        9 2023-02-15 08:13:56.000000 handyman-0.3.5/handyman.egg-info/namespace_packages.txt
--rw-r--r--   0 deepankaragrawal   (502) staff       (20)        1 2023-02-15 08:13:56.000000 handyman-0.3.5/handyman.egg-info/not-zip-safe
--rw-r--r--   0 deepankaragrawal   (502) staff       (20)      195 2023-02-15 08:13:56.000000 handyman-0.3.5/handyman.egg-info/requires.txt
--rw-r--r--   0 deepankaragrawal   (502) staff       (20)        9 2023-02-15 08:13:56.000000 handyman-0.3.5/handyman.egg-info/top_level.txt
--rw-r--r--   0 deepankaragrawal   (502) staff       (20)      195 2023-02-15 07:57:39.000000 handyman-0.3.5/requirements.txt
--rw-r--r--   0 deepankaragrawal   (502) staff       (20)      149 2023-02-15 08:13:56.399317 handyman-0.3.5/setup.cfg
--rw-r--r--   0 deepankaragrawal   (502) staff       (20)     1994 2023-02-15 08:03:43.000000 handyman-0.3.5/setup.py
+drwxr-xr-x   0 deepankaragrawal   (502) staff       (20)        0 2023-06-20 05:52:12.643173 handyman-0.3.6/
+-rw-r--r--   0 deepankaragrawal   (502) staff       (20)        1 2023-02-15 07:57:39.000000 handyman-0.3.6/LICENSE
+-rw-r--r--   0 deepankaragrawal   (502) staff       (20)       24 2023-02-15 07:57:39.000000 handyman-0.3.6/MANIFEST.in
+-rw-r--r--   0 deepankaragrawal   (502) staff       (20)     4490 2023-06-20 05:52:12.643238 handyman-0.3.6/PKG-INFO
+-rw-r--r--   0 deepankaragrawal   (502) staff       (20)     3646 2023-02-15 09:38:04.000000 handyman-0.3.6/README.md
+drwxr-xr-x   0 deepankaragrawal   (502) staff       (20)        0 2023-06-20 05:52:12.639608 handyman-0.3.6/handyman/
+-rw-r--r--   0 deepankaragrawal   (502) staff       (20)      172 2023-02-15 07:57:39.000000 handyman-0.3.6/handyman/__init__.py
+-rw-r--r--   0 deepankaragrawal   (502) staff       (20)     1015 2023-02-15 07:57:39.000000 handyman-0.3.6/handyman/__main__.py
+drwxr-xr-x   0 deepankaragrawal   (502) staff       (20)        0 2023-06-20 05:52:12.641119 handyman-0.3.6/handyman/cli/
+-rw-r--r--   0 deepankaragrawal   (502) staff       (20)        0 2023-02-15 07:57:39.000000 handyman-0.3.6/handyman/cli/__init__.py
+-rw-r--r--   0 deepankaragrawal   (502) staff       (20)      915 2023-02-15 07:57:39.000000 handyman-0.3.6/handyman/cli/proto_gen.py
+drwxr-xr-x   0 deepankaragrawal   (502) staff       (20)        0 2023-06-20 05:52:12.641861 handyman-0.3.6/handyman/crypto/
+-rw-r--r--   0 deepankaragrawal   (502) staff       (20)      543 2023-02-15 07:57:39.000000 handyman-0.3.6/handyman/crypto/__init__.py
+-rw-r--r--   0 deepankaragrawal   (502) staff       (20)     1317 2023-02-15 07:57:39.000000 handyman-0.3.6/handyman/crypto/cache.py
+-rw-r--r--   0 deepankaragrawal   (502) staff       (20)    10481 2023-02-15 07:57:39.000000 handyman-0.3.6/handyman/crypto/crypto.py
+-rw-r--r--   0 deepankaragrawal   (502) staff       (20)     2805 2023-02-15 07:57:39.000000 handyman-0.3.6/handyman/crypto/exceptions.py
+-rw-r--r--   0 deepankaragrawal   (502) staff       (20)     8389 2023-02-15 07:57:39.000000 handyman-0.3.6/handyman/crypto/vault.py
+drwxr-xr-x   0 deepankaragrawal   (502) staff       (20)        0 2023-06-20 05:52:12.642686 handyman-0.3.6/handyman/events/
+-rw-r--r--   0 deepankaragrawal   (502) staff       (20)      290 2023-02-15 07:57:39.000000 handyman-0.3.6/handyman/events/__init__.py
+-rw-r--r--   0 deepankaragrawal   (502) staff       (20)      601 2023-02-15 09:38:04.000000 handyman-0.3.6/handyman/events/event_types.py
+-rw-r--r--   0 deepankaragrawal   (502) staff       (20)      361 2023-02-15 07:57:39.000000 handyman-0.3.6/handyman/events/exceptions.py
+-rw-r--r--   0 deepankaragrawal   (502) staff       (20)      986 2023-02-15 07:57:39.000000 handyman-0.3.6/handyman/events/goroutine.py
+-rw-r--r--   0 deepankaragrawal   (502) staff       (20)     8130 2023-02-15 09:38:04.000000 handyman-0.3.6/handyman/events/sqs.py
+drwxr-xr-x   0 deepankaragrawal   (502) staff       (20)        0 2023-06-20 05:52:12.643034 handyman-0.3.6/handyman/exceptions/
+-rw-r--r--   0 deepankaragrawal   (502) staff       (20)     2972 2023-02-15 07:57:39.000000 handyman-0.3.6/handyman/exceptions/__init__.py
+-rw-r--r--   0 deepankaragrawal   (502) staff       (20)      390 2023-02-15 07:57:39.000000 handyman-0.3.6/handyman/grpc_utils.py
+-rw-r--r--   0 deepankaragrawal   (502) staff       (20)     1197 2023-02-15 07:57:39.000000 handyman-0.3.6/handyman/helpers.py
+-rw-r--r--   0 deepankaragrawal   (502) staff       (20)     2452 2023-02-15 07:57:39.000000 handyman-0.3.6/handyman/io.py
+-rw-r--r--   0 deepankaragrawal   (502) staff       (20)     2125 2023-02-15 07:57:39.000000 handyman-0.3.6/handyman/json_utils.py
+-rw-r--r--   0 deepankaragrawal   (502) staff       (20)     2488 2023-02-15 07:57:39.000000 handyman-0.3.6/handyman/log.py
+-rw-r--r--   0 deepankaragrawal   (502) staff       (20)     9375 2023-02-15 07:57:39.000000 handyman-0.3.6/handyman/prometheus.py
+-rw-r--r--   0 deepankaragrawal   (502) staff       (20)      751 2023-02-15 07:57:39.000000 handyman-0.3.6/handyman/sentry.py
+drwxr-xr-x   0 deepankaragrawal   (502) staff       (20)        0 2023-06-20 05:52:12.640776 handyman-0.3.6/handyman.egg-info/
+-rw-r--r--   0 deepankaragrawal   (502) staff       (20)     4490 2023-06-20 05:52:12.000000 handyman-0.3.6/handyman.egg-info/PKG-INFO
+-rw-r--r--   0 deepankaragrawal   (502) staff       (20)      835 2023-06-20 05:52:12.000000 handyman-0.3.6/handyman.egg-info/SOURCES.txt
+-rw-r--r--   0 deepankaragrawal   (502) staff       (20)        1 2023-06-20 05:52:12.000000 handyman-0.3.6/handyman.egg-info/dependency_links.txt
+-rw-r--r--   0 deepankaragrawal   (502) staff       (20)        9 2023-06-20 05:52:12.000000 handyman-0.3.6/handyman.egg-info/namespace_packages.txt
+-rw-r--r--   0 deepankaragrawal   (502) staff       (20)        1 2023-02-15 08:13:56.000000 handyman-0.3.6/handyman.egg-info/not-zip-safe
+-rw-r--r--   0 deepankaragrawal   (502) staff       (20)      196 2023-06-20 05:52:12.000000 handyman-0.3.6/handyman.egg-info/requires.txt
+-rw-r--r--   0 deepankaragrawal   (502) staff       (20)        9 2023-06-20 05:52:12.000000 handyman-0.3.6/handyman.egg-info/top_level.txt
+-rw-r--r--   0 deepankaragrawal   (502) staff       (20)      196 2023-06-20 05:51:04.000000 handyman-0.3.6/requirements.txt
+-rw-r--r--   0 deepankaragrawal   (502) staff       (20)      149 2023-06-20 05:52:12.643434 handyman-0.3.6/setup.cfg
+-rw-r--r--   0 deepankaragrawal   (502) staff       (20)     1994 2023-06-20 05:51:04.000000 handyman-0.3.6/setup.py
```

### Comparing `handyman-0.3.5/PKG-INFO` & `handyman-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: handyman
-Version: 0.3.5
+Version: 0.3.6
 Summary: Skit utils package for ML Services
 Home-page: https://gitlab.com/vernacularai/tools/handyman
 Author: Skit.ai
 Author-email: deepankar@vernacular.ai
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `handyman-0.3.5/README.md` & `handyman-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `handyman-0.3.5/handyman/__main__.py` & `handyman-0.3.6/handyman/__main__.py`

 * *Files identical despite different names*

### Comparing `handyman-0.3.5/handyman/cli/proto_gen.py` & `handyman-0.3.6/handyman/cli/proto_gen.py`

 * *Files identical despite different names*

### Comparing `handyman-0.3.5/handyman/crypto/__init__.py` & `handyman-0.3.6/handyman/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `handyman-0.3.5/handyman/crypto/cache.py` & `handyman-0.3.6/handyman/crypto/cache.py`

 * *Files identical despite different names*

### Comparing `handyman-0.3.5/handyman/crypto/crypto.py` & `handyman-0.3.6/handyman/crypto/crypto.py`

 * *Files identical despite different names*

### Comparing `handyman-0.3.5/handyman/crypto/exceptions.py` & `handyman-0.3.6/handyman/crypto/exceptions.py`

 * *Files identical despite different names*

### Comparing `handyman-0.3.5/handyman/crypto/vault.py` & `handyman-0.3.6/handyman/crypto/vault.py`

 * *Files identical despite different names*

### Comparing `handyman-0.3.5/handyman/events/event_types.py` & `handyman-0.3.6/handyman/events/event_types.py`

 * *Files identical despite different names*

### Comparing `handyman-0.3.5/handyman/events/goroutine.py` & `handyman-0.3.6/handyman/events/goroutine.py`

 * *Files identical despite different names*

### Comparing `handyman-0.3.5/handyman/events/sqs.py` & `handyman-0.3.6/handyman/events/sqs.py`

 * *Files identical despite different names*

### Comparing `handyman-0.3.5/handyman/exceptions/__init__.py` & `handyman-0.3.6/handyman/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `handyman-0.3.5/handyman/helpers.py` & `handyman-0.3.6/handyman/helpers.py`

 * *Files identical despite different names*

### Comparing `handyman-0.3.5/handyman/io.py` & `handyman-0.3.6/handyman/io.py`

 * *Files identical despite different names*

### Comparing `handyman-0.3.5/handyman/json_utils.py` & `handyman-0.3.6/handyman/json_utils.py`

 * *Files identical despite different names*

### Comparing `handyman-0.3.5/handyman/log.py` & `handyman-0.3.6/handyman/log.py`

 * *Files identical despite different names*

### Comparing `handyman-0.3.5/handyman/prometheus.py` & `handyman-0.3.6/handyman/prometheus.py`

 * *Files identical despite different names*

### Comparing `handyman-0.3.5/handyman/sentry.py` & `handyman-0.3.6/handyman/sentry.py`

 * *Files identical despite different names*

### Comparing `handyman-0.3.5/handyman.egg-info/PKG-INFO` & `handyman-0.3.6/handyman.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: handyman
-Version: 0.3.5
+Version: 0.3.6
 Summary: Skit utils package for ML Services
 Home-page: https://gitlab.com/vernacularai/tools/handyman
 Author: Skit.ai
 Author-email: deepankar@vernacular.ai
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `handyman-0.3.5/handyman.egg-info/SOURCES.txt` & `handyman-0.3.6/handyman.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `handyman-0.3.5/setup.py` & `handyman-0.3.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 
 from setuptools import setup
 
 
 name = "handyman"
 description = "Skit utils package for ML Services"
-version = "0.3.5"
+version = "0.3.6"
 
 package_root = os.path.abspath(os.path.dirname(__file__))
 
 dependencies_filename = os.path.join(package_root, "requirements.txt")
 with io.open(dependencies_filename, "r") as dependencies_file:
     dependencies = dependencies_file.readlines()
```

