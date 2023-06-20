# Comparing `tmp/bgstools-0.1.7.tar.gz` & `tmp/bgstools-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bgstools-0.1.7.tar", max compression
+gzip compressed data, was "bgstools-0.1.8.tar", max compression
```

## Comparing `bgstools-0.1.7.tar` & `bgstools-0.1.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0       72 2023-06-11 05:11:36.804060 bgstools-0.1.7/README.md
--rw-r--r--   0        0        0        0 2023-06-11 05:11:36.804060 bgstools-0.1.7/bgstools/__init__.py
--rw-r--r--   0        0        0       64 2023-06-11 05:11:36.804060 bgstools-0.1.7/bgstools/datastorage/__init__.py
--rw-r--r--   0        0        0     5014 2023-06-11 05:11:36.804060 bgstools-0.1.7/bgstools/datastorage/datastorage.py
--rw-r--r--   0        0        0      165 2023-06-11 05:11:36.804060 bgstools-0.1.7/bgstools/io/__init__.py
--rw-r--r--   0        0        0     4617 2023-06-12 19:14:12.497334 bgstools-0.1.7/bgstools/io/io.py
--rw-r--r--   0        0        0     3770 2023-06-11 05:11:36.804060 bgstools-0.1.7/bgstools/io/media.py
--rw-r--r--   0        0        0      122 2023-06-11 05:11:36.804060 bgstools-0.1.7/bgstools/spatial/__init__.py
--rw-r--r--   0        0        0     2654 2023-06-11 05:11:36.804060 bgstools-0.1.7/bgstools/spatial/spatial.py
--rw-r--r--   0        0        0       54 2023-06-12 20:06:53.761372 bgstools-0.1.7/bgstools/stt/__init__.py
--rw-r--r--   0        0        0     3641 2023-06-12 19:12:06.833881 bgstools-0.1.7/bgstools/stt/stt.py
--rw-r--r--   0        0        0       99 2023-06-11 05:11:36.804060 bgstools-0.1.7/bgstools/utils/__init__.py
--rw-r--r--   0        0        0     2971 2023-06-11 05:11:36.804060 bgstools-0.1.7/bgstools/utils/utils.py
--rw-r--r--   0        0        0      433 2023-06-12 20:26:52.960120 bgstools-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      630 1970-01-01 00:00:00.000000 bgstools-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0       72 2023-06-11 05:11:36.804060 bgstools-0.1.8/README.md
+-rw-r--r--   0        0        0        0 2023-06-11 05:11:36.804060 bgstools-0.1.8/bgstools/__init__.py
+-rw-r--r--   0        0        0       64 2023-06-11 05:11:36.804060 bgstools-0.1.8/bgstools/datastorage/__init__.py
+-rw-r--r--   0        0        0     5014 2023-06-11 05:11:36.804060 bgstools-0.1.8/bgstools/datastorage/datastorage.py
+-rw-r--r--   0        0        0      165 2023-06-11 05:11:36.804060 bgstools-0.1.8/bgstools/io/__init__.py
+-rw-r--r--   0        0        0     5088 2023-06-20 12:54:32.302600 bgstools-0.1.8/bgstools/io/io.py
+-rw-r--r--   0        0        0     3770 2023-06-11 05:11:36.804060 bgstools-0.1.8/bgstools/io/media.py
+-rw-r--r--   0        0        0      122 2023-06-11 05:11:36.804060 bgstools-0.1.8/bgstools/spatial/__init__.py
+-rw-r--r--   0        0        0     2654 2023-06-11 05:11:36.804060 bgstools-0.1.8/bgstools/spatial/spatial.py
+-rw-r--r--   0        0        0       54 2023-06-12 20:06:53.761372 bgstools-0.1.8/bgstools/stt/__init__.py
+-rw-r--r--   0        0        0     3641 2023-06-12 19:12:06.833881 bgstools-0.1.8/bgstools/stt/stt.py
+-rw-r--r--   0        0        0       99 2023-06-11 05:11:36.804060 bgstools-0.1.8/bgstools/utils/__init__.py
+-rw-r--r--   0        0        0     2971 2023-06-11 05:11:36.804060 bgstools-0.1.8/bgstools/utils/utils.py
+-rw-r--r--   0        0        0      433 2023-06-20 12:57:02.436828 bgstools-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      630 1970-01-01 00:00:00.000000 bgstools-0.1.8/PKG-INFO
```

### Comparing `bgstools-0.1.7/bgstools/datastorage/datastorage.py` & `bgstools-0.1.8/bgstools/datastorage/datastorage.py`

 * *Files identical despite different names*

### Comparing `bgstools-0.1.7/bgstools/io/io.py` & `bgstools-0.1.8/bgstools/io/io.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,31 @@
 import os
 import yaml
 from collections import OrderedDict
 import requests
+import toml
+
+
+def load_toml_variables(file_path):
+    """
+    Load variables from a .toml file into a dictionary.
+
+    Args:
+        file_path (str): Path to the .toml file.
+
+    Returns:
+        dict: Dictionary containing the loaded variables.
+    """
+    try:
+        with open(file_path, "r") as file:
+            data = toml.load(file)
+            return data
+    except IOError:
+        print(f"Error: Unable to load .toml file from {file_path}")
+        return {}
 
 
 def load_yaml(filepath: str) -> dict:
     """
     Loads a YAML file.
 
     Can be used as stand-alone script by providing a command-line argument:
```

### Comparing `bgstools-0.1.7/bgstools/io/media.py` & `bgstools-0.1.8/bgstools/io/media.py`

 * *Files identical despite different names*

### Comparing `bgstools-0.1.7/bgstools/spatial/spatial.py` & `bgstools-0.1.8/bgstools/spatial/spatial.py`

 * *Files identical despite different names*

### Comparing `bgstools-0.1.7/bgstools/stt/stt.py` & `bgstools-0.1.8/bgstools/stt/stt.py`

 * *Files identical despite different names*

### Comparing `bgstools-0.1.7/bgstools/utils/utils.py` & `bgstools-0.1.8/bgstools/utils/utils.py`

 * *Files identical despite different names*

### Comparing `bgstools-0.1.7/PKG-INFO` & `bgstools-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bgstools
-Version: 0.1.7
+Version: 0.1.8
 Summary: BeGeoSpatial Development Tools
 Author: José Beltrán
 Author-email: 102664984+jose-begeospatial@users.noreply.github.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyYAML (>=6.0,<7.0)
```

