# Comparing `tmp/mlserver-alibi-explain-1.3.4rc2.tar.gz` & `tmp/mlserver-alibi-explain-1.4.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlserver-alibi-explain-1.3.4rc2.tar", last modified: Tue Jun 20 09:09:36 2023, max compression
+gzip compressed data, was "mlserver-alibi-explain-1.4.0.dev2.tar", last modified: Thu May  4 09:30:33 2023, max compression
```

## Comparing `mlserver-alibi-explain-1.3.4rc2.tar` & `mlserver-alibi-explain-1.4.0.dev2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:09:36.487910 mlserver-alibi-explain-1.3.4rc2/
--rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-06-20 09:08:50.000000 mlserver-alibi-explain-1.3.4rc2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-20 09:09:36.487910 mlserver-alibi-explain-1.3.4rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-20 09:08:50.000000 mlserver-alibi-explain-1.3.4rc2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:09:36.483910 mlserver-alibi-explain-1.3.4rc2/mlserver_alibi_explain/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-20 09:08:50.000000 mlserver-alibi-explain-1.3.4rc2/mlserver_alibi_explain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-06-20 09:08:50.000000 mlserver-alibi-explain-1.3.4rc2/mlserver_alibi_explain/alibi_dependency_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-06-20 09:08:50.000000 mlserver-alibi-explain-1.3.4rc2/mlserver_alibi_explain/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-20 09:08:50.000000 mlserver-alibi-explain-1.3.4rc2/mlserver_alibi_explain/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:09:36.487910 mlserver-alibi-explain-1.3.4rc2/mlserver_alibi_explain/explainers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 09:08:50.000000 mlserver-alibi-explain-1.3.4rc2/mlserver_alibi_explain/explainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-06-20 09:08:50.000000 mlserver-alibi-explain-1.3.4rc2/mlserver_alibi_explain/explainers/black_box_runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-20 09:08:50.000000 mlserver-alibi-explain-1.3.4rc2/mlserver_alibi_explain/explainers/integrated_gradients.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-06-20 09:08:50.000000 mlserver-alibi-explain-1.3.4rc2/mlserver_alibi_explain/explainers/white_box_runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     5934 2023-06-20 09:08:50.000000 mlserver-alibi-explain-1.3.4rc2/mlserver_alibi_explain/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-20 09:08:50.000000 mlserver-alibi-explain-1.3.4rc2/mlserver_alibi_explain/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:09:36.483910 mlserver-alibi-explain-1.3.4rc2/mlserver_alibi_explain.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-20 09:09:36.000000 mlserver-alibi-explain-1.3.4rc2/mlserver_alibi_explain.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-06-20 09:09:36.000000 mlserver-alibi-explain-1.3.4rc2/mlserver_alibi_explain.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 09:09:36.000000 mlserver-alibi-explain-1.3.4rc2/mlserver_alibi_explain.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-20 09:09:36.000000 mlserver-alibi-explain-1.3.4rc2/mlserver_alibi_explain.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-20 09:09:36.000000 mlserver-alibi-explain-1.3.4rc2/mlserver_alibi_explain.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 09:09:36.487910 mlserver-alibi-explain-1.3.4rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-06-20 09:08:50.000000 mlserver-alibi-explain-1.3.4rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:33.211432 mlserver-alibi-explain-1.4.0.dev2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-05-04 09:29:57.000000 mlserver-alibi-explain-1.4.0.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-04 09:30:33.211432 mlserver-alibi-explain-1.4.0.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-04 09:29:57.000000 mlserver-alibi-explain-1.4.0.dev2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:33.207432 mlserver-alibi-explain-1.4.0.dev2/mlserver_alibi_explain/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-04 09:29:57.000000 mlserver-alibi-explain-1.4.0.dev2/mlserver_alibi_explain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-05-04 09:29:57.000000 mlserver-alibi-explain-1.4.0.dev2/mlserver_alibi_explain/alibi_dependency_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-05-04 09:29:57.000000 mlserver-alibi-explain-1.4.0.dev2/mlserver_alibi_explain/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-04 09:29:57.000000 mlserver-alibi-explain-1.4.0.dev2/mlserver_alibi_explain/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:33.211432 mlserver-alibi-explain-1.4.0.dev2/mlserver_alibi_explain/explainers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 09:29:57.000000 mlserver-alibi-explain-1.4.0.dev2/mlserver_alibi_explain/explainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-05-04 09:29:57.000000 mlserver-alibi-explain-1.4.0.dev2/mlserver_alibi_explain/explainers/black_box_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-04 09:29:57.000000 mlserver-alibi-explain-1.4.0.dev2/mlserver_alibi_explain/explainers/integrated_gradients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-04 09:29:57.000000 mlserver-alibi-explain-1.4.0.dev2/mlserver_alibi_explain/explainers/white_box_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5934 2023-05-04 09:29:57.000000 mlserver-alibi-explain-1.4.0.dev2/mlserver_alibi_explain/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-04 09:29:57.000000 mlserver-alibi-explain-1.4.0.dev2/mlserver_alibi_explain/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:33.207432 mlserver-alibi-explain-1.4.0.dev2/mlserver_alibi_explain.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-04 09:30:32.000000 mlserver-alibi-explain-1.4.0.dev2/mlserver_alibi_explain.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-04 09:30:33.000000 mlserver-alibi-explain-1.4.0.dev2/mlserver_alibi_explain.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 09:30:32.000000 mlserver-alibi-explain-1.4.0.dev2/mlserver_alibi_explain.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-04 09:30:32.000000 mlserver-alibi-explain-1.4.0.dev2/mlserver_alibi_explain.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-04 09:30:32.000000 mlserver-alibi-explain-1.4.0.dev2/mlserver_alibi_explain.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 09:30:33.211432 mlserver-alibi-explain-1.4.0.dev2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-05-04 09:29:57.000000 mlserver-alibi-explain-1.4.0.dev2/setup.py
```

### Comparing `mlserver-alibi-explain-1.3.4rc2/LICENSE` & `mlserver-alibi-explain-1.4.0.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `mlserver-alibi-explain-1.3.4rc2/PKG-INFO` & `mlserver-alibi-explain-1.4.0.dev2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlserver-alibi-explain
-Version: 1.3.4rc2
+Version: 1.4.0.dev2
 Summary: Alibi-Explain runtime for MLServer
 Home-page: https://github.com/SeldonIO/MLServer.git
 Author: Seldon Technologies Ltd.
 Author-email: hello@seldon.io
 License: Apache 2.0
 Description: # Alibi-Explain runtime for MLServer
```

### Comparing `mlserver-alibi-explain-1.3.4rc2/mlserver_alibi_explain/alibi_dependency_reference.py` & `mlserver-alibi-explain-1.4.0.dev2/mlserver_alibi_explain/alibi_dependency_reference.py`

 * *Files identical despite different names*

### Comparing `mlserver-alibi-explain-1.3.4rc2/mlserver_alibi_explain/common.py` & `mlserver-alibi-explain-1.4.0.dev2/mlserver_alibi_explain/common.py`

 * *Files identical despite different names*

### Comparing `mlserver-alibi-explain-1.3.4rc2/mlserver_alibi_explain/explainers/black_box_runtime.py` & `mlserver-alibi-explain-1.4.0.dev2/mlserver_alibi_explain/explainers/black_box_runtime.py`

 * *Files identical despite different names*

### Comparing `mlserver-alibi-explain-1.3.4rc2/mlserver_alibi_explain/explainers/integrated_gradients.py` & `mlserver-alibi-explain-1.4.0.dev2/mlserver_alibi_explain/explainers/integrated_gradients.py`

 * *Files identical despite different names*

### Comparing `mlserver-alibi-explain-1.3.4rc2/mlserver_alibi_explain/explainers/white_box_runtime.py` & `mlserver-alibi-explain-1.4.0.dev2/mlserver_alibi_explain/explainers/white_box_runtime.py`

 * *Files identical despite different names*

### Comparing `mlserver-alibi-explain-1.3.4rc2/mlserver_alibi_explain/runtime.py` & `mlserver-alibi-explain-1.4.0.dev2/mlserver_alibi_explain/runtime.py`

 * *Files identical despite different names*

### Comparing `mlserver-alibi-explain-1.3.4rc2/mlserver_alibi_explain.egg-info/PKG-INFO` & `mlserver-alibi-explain-1.4.0.dev2/mlserver_alibi_explain.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlserver-alibi-explain
-Version: 1.3.4rc2
+Version: 1.4.0.dev2
 Summary: Alibi-Explain runtime for MLServer
 Home-page: https://github.com/SeldonIO/MLServer.git
 Author: Seldon Technologies Ltd.
 Author-email: hello@seldon.io
 License: Apache 2.0
 Description: # Alibi-Explain runtime for MLServer
```

### Comparing `mlserver-alibi-explain-1.3.4rc2/mlserver_alibi_explain.egg-info/SOURCES.txt` & `mlserver-alibi-explain-1.4.0.dev2/mlserver_alibi_explain.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mlserver-alibi-explain-1.3.4rc2/setup.py` & `mlserver-alibi-explain-1.4.0.dev2/setup.py`

 * *Files identical despite different names*

