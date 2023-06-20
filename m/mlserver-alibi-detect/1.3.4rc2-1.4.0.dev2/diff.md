# Comparing `tmp/mlserver-alibi-detect-1.3.4rc2.tar.gz` & `tmp/mlserver-alibi-detect-1.4.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlserver-alibi-detect-1.3.4rc2.tar", last modified: Tue Jun 20 09:09:27 2023, max compression
+gzip compressed data, was "mlserver-alibi-detect-1.4.0.dev2.tar", last modified: Thu May  4 09:30:37 2023, max compression
```

## Comparing `mlserver-alibi-detect-1.3.4rc2.tar` & `mlserver-alibi-detect-1.4.0.dev2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:09:27.498269 mlserver-alibi-detect-1.3.4rc2/
--rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-06-20 09:08:48.000000 mlserver-alibi-detect-1.3.4rc2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-06-20 09:09:27.498269 mlserver-alibi-detect-1.3.4rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-06-20 09:08:48.000000 mlserver-alibi-detect-1.3.4rc2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:09:27.498269 mlserver-alibi-detect-1.3.4rc2/mlserver_alibi_detect/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-20 09:08:48.000000 mlserver-alibi-detect-1.3.4rc2/mlserver_alibi_detect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7503 2023-06-20 09:08:48.000000 mlserver-alibi-detect-1.3.4rc2/mlserver_alibi_detect/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-20 09:08:48.000000 mlserver-alibi-detect-1.3.4rc2/mlserver_alibi_detect/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:09:27.498269 mlserver-alibi-detect-1.3.4rc2/mlserver_alibi_detect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-06-20 09:09:27.000000 mlserver-alibi-detect-1.3.4rc2/mlserver_alibi_detect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-20 09:09:27.000000 mlserver-alibi-detect-1.3.4rc2/mlserver_alibi_detect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 09:09:27.000000 mlserver-alibi-detect-1.3.4rc2/mlserver_alibi_detect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-20 09:09:27.000000 mlserver-alibi-detect-1.3.4rc2/mlserver_alibi_detect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-20 09:09:27.000000 mlserver-alibi-detect-1.3.4rc2/mlserver_alibi_detect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 09:09:27.498269 mlserver-alibi-detect-1.3.4rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-06-20 09:08:48.000000 mlserver-alibi-detect-1.3.4rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:37.811358 mlserver-alibi-detect-1.4.0.dev2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-05-04 09:29:58.000000 mlserver-alibi-detect-1.4.0.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-05-04 09:30:37.811358 mlserver-alibi-detect-1.4.0.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-05-04 09:29:58.000000 mlserver-alibi-detect-1.4.0.dev2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:37.811358 mlserver-alibi-detect-1.4.0.dev2/mlserver_alibi_detect/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-04 09:29:58.000000 mlserver-alibi-detect-1.4.0.dev2/mlserver_alibi_detect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7503 2023-05-04 09:29:58.000000 mlserver-alibi-detect-1.4.0.dev2/mlserver_alibi_detect/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-04 09:29:58.000000 mlserver-alibi-detect-1.4.0.dev2/mlserver_alibi_detect/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:37.811358 mlserver-alibi-detect-1.4.0.dev2/mlserver_alibi_detect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-05-04 09:30:37.000000 mlserver-alibi-detect-1.4.0.dev2/mlserver_alibi_detect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-04 09:30:37.000000 mlserver-alibi-detect-1.4.0.dev2/mlserver_alibi_detect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 09:30:37.000000 mlserver-alibi-detect-1.4.0.dev2/mlserver_alibi_detect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-04 09:30:37.000000 mlserver-alibi-detect-1.4.0.dev2/mlserver_alibi_detect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-04 09:30:37.000000 mlserver-alibi-detect-1.4.0.dev2/mlserver_alibi_detect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 09:30:37.811358 mlserver-alibi-detect-1.4.0.dev2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-05-04 09:29:58.000000 mlserver-alibi-detect-1.4.0.dev2/setup.py
```

### Comparing `mlserver-alibi-detect-1.3.4rc2/LICENSE` & `mlserver-alibi-detect-1.4.0.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `mlserver-alibi-detect-1.3.4rc2/PKG-INFO` & `mlserver-alibi-detect-1.4.0.dev2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlserver-alibi-detect
-Version: 1.3.4rc2
+Version: 1.4.0.dev2
 Summary: Alibi-Detect runtime for MLServer
 Home-page: https://github.com/SeldonIO/MLServer.git
 Author: Seldon Technologies Ltd.
 Author-email: hello@seldon.io
 License: Apache 2.0
 Description: # Alibi-Detect runtime for MLServer
```

### Comparing `mlserver-alibi-detect-1.3.4rc2/README.md` & `mlserver-alibi-detect-1.4.0.dev2/README.md`

 * *Files identical despite different names*

### Comparing `mlserver-alibi-detect-1.3.4rc2/mlserver_alibi_detect/runtime.py` & `mlserver-alibi-detect-1.4.0.dev2/mlserver_alibi_detect/runtime.py`

 * *Files identical despite different names*

### Comparing `mlserver-alibi-detect-1.3.4rc2/mlserver_alibi_detect.egg-info/PKG-INFO` & `mlserver-alibi-detect-1.4.0.dev2/mlserver_alibi_detect.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlserver-alibi-detect
-Version: 1.3.4rc2
+Version: 1.4.0.dev2
 Summary: Alibi-Detect runtime for MLServer
 Home-page: https://github.com/SeldonIO/MLServer.git
 Author: Seldon Technologies Ltd.
 Author-email: hello@seldon.io
 License: Apache 2.0
 Description: # Alibi-Detect runtime for MLServer
```

### Comparing `mlserver-alibi-detect-1.3.4rc2/setup.py` & `mlserver-alibi-detect-1.4.0.dev2/setup.py`

 * *Files identical despite different names*

