# Comparing `tmp/mlserver-mllib-1.3.4rc2.tar.gz` & `tmp/mlserver-mllib-1.4.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlserver-mllib-1.3.4rc2.tar", last modified: Tue Jun 20 09:09:39 2023, max compression
+gzip compressed data, was "mlserver-mllib-1.4.0.dev2.tar", last modified: Thu May  4 09:30:35 2023, max compression
```

## Comparing `mlserver-mllib-1.3.4rc2.tar` & `mlserver-mllib-1.4.0.dev2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:09:39.454200 mlserver-mllib-1.3.4rc2/
--rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-06-20 09:08:52.000000 mlserver-mllib-1.3.4rc2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-20 09:09:39.454200 mlserver-mllib-1.3.4rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-20 09:08:52.000000 mlserver-mllib-1.3.4rc2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:09:39.450199 mlserver-mllib-1.3.4rc2/mlserver_mllib/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-20 09:08:52.000000 mlserver-mllib-1.3.4rc2/mlserver_mllib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-20 09:08:52.000000 mlserver-mllib-1.3.4rc2/mlserver_mllib/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-06-20 09:08:52.000000 mlserver-mllib-1.3.4rc2/mlserver_mllib/mllib.py
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-06-20 09:08:52.000000 mlserver-mllib-1.3.4rc2/mlserver_mllib/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-20 09:08:52.000000 mlserver-mllib-1.3.4rc2/mlserver_mllib/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:09:39.454200 mlserver-mllib-1.3.4rc2/mlserver_mllib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-20 09:09:39.000000 mlserver-mllib-1.3.4rc2/mlserver_mllib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-20 09:09:39.000000 mlserver-mllib-1.3.4rc2/mlserver_mllib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 09:09:39.000000 mlserver-mllib-1.3.4rc2/mlserver_mllib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-20 09:09:39.000000 mlserver-mllib-1.3.4rc2/mlserver_mllib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-20 09:09:39.000000 mlserver-mllib-1.3.4rc2/mlserver_mllib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 09:09:39.454200 mlserver-mllib-1.3.4rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-06-20 09:08:52.000000 mlserver-mllib-1.3.4rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:35.714868 mlserver-mllib-1.4.0.dev2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-05-04 09:29:57.000000 mlserver-mllib-1.4.0.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-05-04 09:30:35.714868 mlserver-mllib-1.4.0.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-04 09:29:57.000000 mlserver-mllib-1.4.0.dev2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:35.710868 mlserver-mllib-1.4.0.dev2/mlserver_mllib/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-04 09:29:57.000000 mlserver-mllib-1.4.0.dev2/mlserver_mllib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-04 09:29:57.000000 mlserver-mllib-1.4.0.dev2/mlserver_mllib/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-05-04 09:29:57.000000 mlserver-mllib-1.4.0.dev2/mlserver_mllib/mllib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-05-04 09:29:57.000000 mlserver-mllib-1.4.0.dev2/mlserver_mllib/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-04 09:29:57.000000 mlserver-mllib-1.4.0.dev2/mlserver_mllib/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:35.714868 mlserver-mllib-1.4.0.dev2/mlserver_mllib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-05-04 09:30:35.000000 mlserver-mllib-1.4.0.dev2/mlserver_mllib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-04 09:30:35.000000 mlserver-mllib-1.4.0.dev2/mlserver_mllib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 09:30:35.000000 mlserver-mllib-1.4.0.dev2/mlserver_mllib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-04 09:30:35.000000 mlserver-mllib-1.4.0.dev2/mlserver_mllib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-04 09:30:35.000000 mlserver-mllib-1.4.0.dev2/mlserver_mllib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 09:30:35.714868 mlserver-mllib-1.4.0.dev2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-04 09:29:57.000000 mlserver-mllib-1.4.0.dev2/setup.py
```

### Comparing `mlserver-mllib-1.3.4rc2/LICENSE` & `mlserver-mllib-1.4.0.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `mlserver-mllib-1.3.4rc2/PKG-INFO` & `mlserver-mllib-1.4.0.dev2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlserver-mllib
-Version: 1.3.4rc2
+Version: 1.4.0.dev2
 Summary: Spark MLlib runtime for MLServer
 Home-page: https://github.com/SeldonIO/MLServer.git
 Author: Seldon Technologies Ltd.
 Author-email: hello@seldon.io
 License: Apache 2.0
 Description: # Spark MLlib runtime for MLServer
```

### Comparing `mlserver-mllib-1.3.4rc2/mlserver_mllib/mllib.py` & `mlserver-mllib-1.4.0.dev2/mlserver_mllib/mllib.py`

 * *Files identical despite different names*

### Comparing `mlserver-mllib-1.3.4rc2/mlserver_mllib/utils.py` & `mlserver-mllib-1.4.0.dev2/mlserver_mllib/utils.py`

 * *Files identical despite different names*

### Comparing `mlserver-mllib-1.3.4rc2/mlserver_mllib.egg-info/PKG-INFO` & `mlserver-mllib-1.4.0.dev2/mlserver_mllib.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlserver-mllib
-Version: 1.3.4rc2
+Version: 1.4.0.dev2
 Summary: Spark MLlib runtime for MLServer
 Home-page: https://github.com/SeldonIO/MLServer.git
 Author: Seldon Technologies Ltd.
 Author-email: hello@seldon.io
 License: Apache 2.0
 Description: # Spark MLlib runtime for MLServer
```

### Comparing `mlserver-mllib-1.3.4rc2/setup.py` & `mlserver-mllib-1.4.0.dev2/setup.py`

 * *Files identical despite different names*

