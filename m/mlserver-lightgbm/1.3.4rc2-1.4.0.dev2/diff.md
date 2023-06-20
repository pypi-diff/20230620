# Comparing `tmp/mlserver-lightgbm-1.3.4rc2.tar.gz` & `tmp/mlserver-lightgbm-1.4.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlserver-lightgbm-1.3.4rc2.tar", last modified: Tue Jun 20 09:09:33 2023, max compression
+gzip compressed data, was "mlserver-lightgbm-1.4.0.dev2.tar", last modified: Thu May  4 09:30:40 2023, max compression
```

## Comparing `mlserver-lightgbm-1.3.4rc2.tar` & `mlserver-lightgbm-1.4.0.dev2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:09:33.649520 mlserver-lightgbm-1.3.4rc2/
--rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-06-20 09:08:51.000000 mlserver-lightgbm-1.3.4rc2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-06-20 09:09:33.649520 mlserver-lightgbm-1.3.4rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-20 09:08:51.000000 mlserver-lightgbm-1.3.4rc2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:09:33.649520 mlserver-lightgbm-1.3.4rc2/mlserver_lightgbm/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-20 09:08:51.000000 mlserver-lightgbm-1.3.4rc2/mlserver_lightgbm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-20 09:08:51.000000 mlserver-lightgbm-1.3.4rc2/mlserver_lightgbm/lightgbm.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-20 09:08:51.000000 mlserver-lightgbm-1.3.4rc2/mlserver_lightgbm/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:09:33.649520 mlserver-lightgbm-1.3.4rc2/mlserver_lightgbm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-06-20 09:09:33.000000 mlserver-lightgbm-1.3.4rc2/mlserver_lightgbm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-20 09:09:33.000000 mlserver-lightgbm-1.3.4rc2/mlserver_lightgbm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 09:09:33.000000 mlserver-lightgbm-1.3.4rc2/mlserver_lightgbm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-20 09:09:33.000000 mlserver-lightgbm-1.3.4rc2/mlserver_lightgbm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-20 09:09:33.000000 mlserver-lightgbm-1.3.4rc2/mlserver_lightgbm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 09:09:33.649520 mlserver-lightgbm-1.3.4rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-20 09:08:51.000000 mlserver-lightgbm-1.3.4rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:40.245904 mlserver-lightgbm-1.4.0.dev2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-05-04 09:30:00.000000 mlserver-lightgbm-1.4.0.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-04 09:30:40.245904 mlserver-lightgbm-1.4.0.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-04 09:30:00.000000 mlserver-lightgbm-1.4.0.dev2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:40.241904 mlserver-lightgbm-1.4.0.dev2/mlserver_lightgbm/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-04 09:30:00.000000 mlserver-lightgbm-1.4.0.dev2/mlserver_lightgbm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-05-04 09:30:00.000000 mlserver-lightgbm-1.4.0.dev2/mlserver_lightgbm/lightgbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-04 09:30:00.000000 mlserver-lightgbm-1.4.0.dev2/mlserver_lightgbm/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:40.245904 mlserver-lightgbm-1.4.0.dev2/mlserver_lightgbm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-04 09:30:40.000000 mlserver-lightgbm-1.4.0.dev2/mlserver_lightgbm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-04 09:30:40.000000 mlserver-lightgbm-1.4.0.dev2/mlserver_lightgbm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 09:30:40.000000 mlserver-lightgbm-1.4.0.dev2/mlserver_lightgbm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-04 09:30:40.000000 mlserver-lightgbm-1.4.0.dev2/mlserver_lightgbm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-04 09:30:40.000000 mlserver-lightgbm-1.4.0.dev2/mlserver_lightgbm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 09:30:40.245904 mlserver-lightgbm-1.4.0.dev2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-04 09:30:00.000000 mlserver-lightgbm-1.4.0.dev2/setup.py
```

### Comparing `mlserver-lightgbm-1.3.4rc2/LICENSE` & `mlserver-lightgbm-1.4.0.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `mlserver-lightgbm-1.3.4rc2/PKG-INFO` & `mlserver-lightgbm-1.4.0.dev2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlserver-lightgbm
-Version: 1.3.4rc2
+Version: 1.4.0.dev2
 Summary: LightGBM runtime for MLServer
 Home-page: https://github.com/SeldonIO/MLServer.git
 Author: Seldon Technologies Ltd.
 Author-email: hello@seldon.io
 License: Apache 2.0
 Description: # LightGBM runtime for MLServer
```

### Comparing `mlserver-lightgbm-1.3.4rc2/README.md` & `mlserver-lightgbm-1.4.0.dev2/README.md`

 * *Files identical despite different names*

### Comparing `mlserver-lightgbm-1.3.4rc2/mlserver_lightgbm/lightgbm.py` & `mlserver-lightgbm-1.4.0.dev2/mlserver_lightgbm/lightgbm.py`

 * *Files identical despite different names*

### Comparing `mlserver-lightgbm-1.3.4rc2/mlserver_lightgbm.egg-info/PKG-INFO` & `mlserver-lightgbm-1.4.0.dev2/mlserver_lightgbm.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlserver-lightgbm
-Version: 1.3.4rc2
+Version: 1.4.0.dev2
 Summary: LightGBM runtime for MLServer
 Home-page: https://github.com/SeldonIO/MLServer.git
 Author: Seldon Technologies Ltd.
 Author-email: hello@seldon.io
 License: Apache 2.0
 Description: # LightGBM runtime for MLServer
```

### Comparing `mlserver-lightgbm-1.3.4rc2/setup.py` & `mlserver-lightgbm-1.4.0.dev2/setup.py`

 * *Files identical despite different names*

