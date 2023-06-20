# Comparing `tmp/titan-iris-0.4.0a0.tar.gz` & `tmp/titan-iris-0.5.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "titan-iris-0.4.0a0.tar", last modified: Tue Jun 20 08:29:12 2023, max compression
+gzip compressed data, was "titan-iris-0.5.0a0.tar", last modified: Tue Jun 20 14:20:38 2023, max compression
```

## Comparing `titan-iris-0.4.0a0.tar` & `titan-iris-0.5.0a0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:29:12.171455 titan-iris-0.4.0a0/
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-06-20 08:29:01.000000 titan-iris-0.4.0a0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-20 08:29:01.000000 titan-iris-0.4.0a0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-20 08:29:01.000000 titan-iris-0.4.0a0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-06-20 08:29:12.171455 titan-iris-0.4.0a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-06-20 08:29:01.000000 titan-iris-0.4.0a0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-20 08:29:01.000000 titan-iris-0.4.0a0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-20 08:29:01.000000 titan-iris-0.4.0a0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-20 08:29:01.000000 titan-iris-0.4.0a0/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-20 08:29:12.171455 titan-iris-0.4.0a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-20 08:29:01.000000 titan-iris-0.4.0a0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:29:12.159454 titan-iris-0.4.0a0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:29:12.163454 titan-iris-0.4.0a0/src/iris/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-20 08:29:01.000000 titan-iris-0.4.0a0/src/iris/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-20 08:29:01.000000 titan-iris-0.4.0a0/src/iris/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:29:12.167454 titan-iris-0.4.0a0/src/iris/gradio/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-20 08:29:01.000000 titan-iris-0.4.0a0/src/iris/gradio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-06-20 08:29:01.000000 titan-iris-0.4.0a0/src/iris/gradio/run.py
--rw-r--r--   0 runner    (1001) docker     (123)    23635 2023-06-20 08:29:01.000000 titan-iris-0.4.0a0/src/iris/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:29:12.167454 titan-iris-0.4.0a0/src/iris/sdk/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-20 08:29:01.000000 titan-iris-0.4.0a0/src/iris/sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11319 2023-06-20 08:29:01.000000 titan-iris-0.4.0a0/src/iris/sdk/auth_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-06-20 08:29:01.000000 titan-iris-0.4.0a0/src/iris/sdk/conf_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     6405 2023-06-20 08:29:01.000000 titan-iris-0.4.0a0/src/iris/sdk/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)    27387 2023-06-20 08:29:01.000000 titan-iris-0.4.0a0/src/iris/sdk/iris_sdk.py
--rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-06-20 08:29:01.000000 titan-iris-0.4.0a0/src/iris/sdk/safe_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)    16225 2023-06-20 08:29:01.000000 titan-iris-0.4.0a0/src/iris/sdk/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:29:12.171455 titan-iris-0.4.0a0/src/titan_iris.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-06-20 08:29:12.000000 titan-iris-0.4.0a0/src/titan_iris.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-20 08:29:12.000000 titan-iris-0.4.0a0/src/titan_iris.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 08:29:12.000000 titan-iris-0.4.0a0/src/titan_iris.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-20 08:29:12.000000 titan-iris-0.4.0a0/src/titan_iris.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-20 08:29:12.000000 titan-iris-0.4.0a0/src/titan_iris.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-20 08:29:12.000000 titan-iris-0.4.0a0/src/titan_iris.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:29:12.171455 titan-iris-0.4.0a0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9591 2023-06-20 08:29:01.000000 titan-iris-0.4.0a0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-06-20 08:29:01.000000 titan-iris-0.4.0a0/tests/test_sdk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:20:38.209332 titan-iris-0.5.0a0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-06-20 14:20:23.000000 titan-iris-0.5.0a0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-20 14:20:23.000000 titan-iris-0.5.0a0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-20 14:20:23.000000 titan-iris-0.5.0a0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-06-20 14:20:38.209332 titan-iris-0.5.0a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-06-20 14:20:23.000000 titan-iris-0.5.0a0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-20 14:20:23.000000 titan-iris-0.5.0a0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-20 14:20:23.000000 titan-iris-0.5.0a0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-20 14:20:23.000000 titan-iris-0.5.0a0/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-20 14:20:38.209332 titan-iris-0.5.0a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-20 14:20:23.000000 titan-iris-0.5.0a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:20:38.201332 titan-iris-0.5.0a0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:20:38.205332 titan-iris-0.5.0a0/src/iris/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-20 14:20:23.000000 titan-iris-0.5.0a0/src/iris/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-20 14:20:23.000000 titan-iris-0.5.0a0/src/iris/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:20:38.205332 titan-iris-0.5.0a0/src/iris/gradio/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-20 14:20:23.000000 titan-iris-0.5.0a0/src/iris/gradio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-06-20 14:20:23.000000 titan-iris-0.5.0a0/src/iris/gradio/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23635 2023-06-20 14:20:23.000000 titan-iris-0.5.0a0/src/iris/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:20:38.205332 titan-iris-0.5.0a0/src/iris/sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-20 14:20:23.000000 titan-iris-0.5.0a0/src/iris/sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11319 2023-06-20 14:20:23.000000 titan-iris-0.5.0a0/src/iris/sdk/auth_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-06-20 14:20:23.000000 titan-iris-0.5.0a0/src/iris/sdk/conf_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6405 2023-06-20 14:20:23.000000 titan-iris-0.5.0a0/src/iris/sdk/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27387 2023-06-20 14:20:23.000000 titan-iris-0.5.0a0/src/iris/sdk/iris_sdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-06-20 14:20:23.000000 titan-iris-0.5.0a0/src/iris/sdk/safe_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16225 2023-06-20 14:20:23.000000 titan-iris-0.5.0a0/src/iris/sdk/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:20:38.205332 titan-iris-0.5.0a0/src/titan_iris.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-06-20 14:20:38.000000 titan-iris-0.5.0a0/src/titan_iris.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-20 14:20:38.000000 titan-iris-0.5.0a0/src/titan_iris.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 14:20:38.000000 titan-iris-0.5.0a0/src/titan_iris.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-20 14:20:38.000000 titan-iris-0.5.0a0/src/titan_iris.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-20 14:20:38.000000 titan-iris-0.5.0a0/src/titan_iris.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-20 14:20:38.000000 titan-iris-0.5.0a0/src/titan_iris.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:20:38.205332 titan-iris-0.5.0a0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9591 2023-06-20 14:20:23.000000 titan-iris-0.5.0a0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-06-20 14:20:23.000000 titan-iris-0.5.0a0/tests/test_sdk.py
```

### Comparing `titan-iris-0.4.0a0/.gitignore` & `titan-iris-0.5.0a0/.gitignore`

 * *Files identical despite different names*

### Comparing `titan-iris-0.4.0a0/Dockerfile` & `titan-iris-0.5.0a0/Dockerfile`

 * *Files identical despite different names*

### Comparing `titan-iris-0.4.0a0/PKG-INFO` & `titan-iris-0.5.0a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: titan-iris
-Version: 0.4.0a0
+Version: 0.5.0a0
 Description-Content-Type: text/markdown
 
 # IRIS CLI Package.
 
 ## Description
 
 Iris is your portal to the TitanML platform. Using Iris, you can launch jobs to run on TitanML servers, run your own models and datasets through our compression algorithms, and explore and download the optimised models from the Titan Store.
```

### Comparing `titan-iris-0.4.0a0/README.md` & `titan-iris-0.5.0a0/README.md`

 * *Files identical despite different names*

### Comparing `titan-iris-0.4.0a0/setup.py` & `titan-iris-0.5.0a0/setup.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.4.0a0/src/iris/config.yaml` & `titan-iris-0.5.0a0/src/iris/config.yaml`

 * *Files identical despite different names*

### Comparing `titan-iris-0.4.0a0/src/iris/gradio/run.py` & `titan-iris-0.5.0a0/src/iris/gradio/run.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.4.0a0/src/iris/main.py` & `titan-iris-0.5.0a0/src/iris/main.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.4.0a0/src/iris/sdk/auth_utils.py` & `titan-iris-0.5.0a0/src/iris/sdk/auth_utils.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.4.0a0/src/iris/sdk/conf_manager.py` & `titan-iris-0.5.0a0/src/iris/sdk/conf_manager.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.4.0a0/src/iris/sdk/exception.py` & `titan-iris-0.5.0a0/src/iris/sdk/exception.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.4.0a0/src/iris/sdk/iris_sdk.py` & `titan-iris-0.5.0a0/src/iris/sdk/iris_sdk.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.4.0a0/src/iris/sdk/safe_convert.py` & `titan-iris-0.5.0a0/src/iris/sdk/safe_convert.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.4.0a0/src/iris/sdk/utils.py` & `titan-iris-0.5.0a0/src/iris/sdk/utils.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.4.0a0/src/titan_iris.egg-info/PKG-INFO` & `titan-iris-0.5.0a0/src/titan_iris.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: titan-iris
-Version: 0.4.0a0
+Version: 0.5.0a0
 Description-Content-Type: text/markdown
 
 # IRIS CLI Package.
 
 ## Description
 
 Iris is your portal to the TitanML platform. Using Iris, you can launch jobs to run on TitanML servers, run your own models and datasets through our compression algorithms, and explore and download the optimised models from the Titan Store.
```

### Comparing `titan-iris-0.4.0a0/src/titan_iris.egg-info/SOURCES.txt` & `titan-iris-0.5.0a0/src/titan_iris.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `titan-iris-0.4.0a0/tests/test_cli.py` & `titan-iris-0.5.0a0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.4.0a0/tests/test_sdk.py` & `titan-iris-0.5.0a0/tests/test_sdk.py`

 * *Files identical despite different names*

