# Comparing `tmp/asset_extraction_framework-0.9.0.tar.gz` & `tmp/asset_extraction_framework-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asset_extraction_framework-0.9.0.tar", last modified: Mon Jun 19 21:59:36 2023, max compression
+gzip compressed data, was "asset_extraction_framework-0.9.1.tar", last modified: Tue Jun 20 21:49:45 2023, max compression
```

## Comparing `asset_extraction_framework-0.9.0.tar` & `asset_extraction_framework-0.9.1.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:59:36.104088 asset_extraction_framework-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-19 21:59:25.000000 asset_extraction_framework-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-06-19 21:59:36.104088 asset_extraction_framework-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-19 21:59:25.000000 asset_extraction_framework-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:59:36.100088 asset_extraction_framework-0.9.0/asset_extraction_framework.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-06-19 21:59:36.000000 asset_extraction_framework-0.9.0/asset_extraction_framework.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-19 21:59:36.000000 asset_extraction_framework-0.9.0/asset_extraction_framework.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 21:59:36.000000 asset_extraction_framework-0.9.0/asset_extraction_framework.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-19 21:59:36.000000 asset_extraction_framework-0.9.0/asset_extraction_framework.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:59:36.100088 asset_extraction_framework-0.9.0/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     7937 2023-06-19 21:59:25.000000 asset_extraction_framework-0.9.0/assets/Application.py
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-06-19 21:59:25.000000 asset_extraction_framework-0.9.0/assets/Asserts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:59:36.104088 asset_extraction_framework-0.9.0/assets/Asset/
--rw-r--r--   0 runner    (1001) docker     (123)    15501 2023-06-19 21:59:25.000000 asset_extraction_framework-0.9.0/assets/Asset/Animation.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-19 21:59:25.000000 asset_extraction_framework-0.9.0/assets/Asset/Asset.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-19 21:59:25.000000 asset_extraction_framework-0.9.0/assets/Asset/BoundingBox.py
--rw-r--r--   0 runner    (1001) docker     (123)    11081 2023-06-19 21:59:25.000000 asset_extraction_framework-0.9.0/assets/Asset/Image.py
--rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-06-19 21:59:25.000000 asset_extraction_framework-0.9.0/assets/Asset/Palette.py
--rw-r--r--   0 runner    (1001) docker     (123)     6506 2023-06-19 21:59:25.000000 asset_extraction_framework-0.9.0/assets/Asset/Sound.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 21:59:25.000000 asset_extraction_framework-0.9.0/assets/Asset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-06-19 21:59:25.000000 asset_extraction_framework-0.9.0/assets/CommandLine.py
--rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-06-19 21:59:25.000000 asset_extraction_framework-0.9.0/assets/File.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 21:59:25.000000 asset_extraction_framework-0.9.0/assets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-19 21:59:25.000000 asset_extraction_framework-0.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 21:59:36.104088 asset_extraction_framework-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 21:59:25.000000 asset_extraction_framework-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:49:45.447320 asset_extraction_framework-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-20 21:49:34.000000 asset_extraction_framework-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-06-20 21:49:45.447320 asset_extraction_framework-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-20 21:49:34.000000 asset_extraction_framework-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:49:45.443320 asset_extraction_framework-0.9.1/asset_extraction_framework.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-06-20 21:49:45.000000 asset_extraction_framework-0.9.1/asset_extraction_framework.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-20 21:49:45.000000 asset_extraction_framework-0.9.1/asset_extraction_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 21:49:45.000000 asset_extraction_framework-0.9.1/asset_extraction_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-20 21:49:45.000000 asset_extraction_framework-0.9.1/asset_extraction_framework.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-20 21:49:45.000000 asset_extraction_framework-0.9.1/asset_extraction_framework.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:49:45.447320 asset_extraction_framework-0.9.1/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     7937 2023-06-20 21:49:34.000000 asset_extraction_framework-0.9.1/assets/Application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-06-20 21:49:34.000000 asset_extraction_framework-0.9.1/assets/Asserts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:49:45.447320 asset_extraction_framework-0.9.1/assets/Asset/
+-rw-r--r--   0 runner    (1001) docker     (123)    15501 2023-06-20 21:49:34.000000 asset_extraction_framework-0.9.1/assets/Asset/Animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-20 21:49:34.000000 asset_extraction_framework-0.9.1/assets/Asset/Asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-20 21:49:34.000000 asset_extraction_framework-0.9.1/assets/Asset/BoundingBox.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11081 2023-06-20 21:49:34.000000 asset_extraction_framework-0.9.1/assets/Asset/Image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-06-20 21:49:34.000000 asset_extraction_framework-0.9.1/assets/Asset/Palette.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6506 2023-06-20 21:49:34.000000 asset_extraction_framework-0.9.1/assets/Asset/Sound.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 21:49:34.000000 asset_extraction_framework-0.9.1/assets/Asset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-06-20 21:49:34.000000 asset_extraction_framework-0.9.1/assets/CommandLine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-06-20 21:49:34.000000 asset_extraction_framework-0.9.1/assets/File.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 21:49:34.000000 asset_extraction_framework-0.9.1/assets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-20 21:49:34.000000 asset_extraction_framework-0.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 21:49:45.447320 asset_extraction_framework-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 21:49:34.000000 asset_extraction_framework-0.9.1/setup.py
```

### Comparing `asset_extraction_framework-0.9.0/LICENSE` & `asset_extraction_framework-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `asset_extraction_framework-0.9.0/PKG-INFO` & `asset_extraction_framework-0.9.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: asset_extraction_framework
-Version: 0.9.0
-Summary: Makes the Python struct library more self-documenting.
+Version: 0.9.1
+Summary: Extract multimedia assets from legacy software
 Author: npjg
 License: MIT License
         
         Copyright (c) 2022 Nathanael Gentry
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `asset_extraction_framework-0.9.0/README.md` & `asset_extraction_framework-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `asset_extraction_framework-0.9.0/asset_extraction_framework.egg-info/PKG-INFO` & `asset_extraction_framework-0.9.1/asset_extraction_framework.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: asset-extraction-framework
-Version: 0.9.0
-Summary: Makes the Python struct library more self-documenting.
+Version: 0.9.1
+Summary: Extract multimedia assets from legacy software
 Author: npjg
 License: MIT License
         
         Copyright (c) 2022 Nathanael Gentry
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `asset_extraction_framework-0.9.0/assets/Application.py` & `asset_extraction_framework-0.9.1/assets/Application.py`

 * *Files identical despite different names*

### Comparing `asset_extraction_framework-0.9.0/assets/Asserts.py` & `asset_extraction_framework-0.9.1/assets/Asserts.py`

 * *Files identical despite different names*

### Comparing `asset_extraction_framework-0.9.0/assets/Asset/Animation.py` & `asset_extraction_framework-0.9.1/assets/Asset/Animation.py`

 * *Files identical despite different names*

### Comparing `asset_extraction_framework-0.9.0/assets/Asset/BoundingBox.py` & `asset_extraction_framework-0.9.1/assets/Asset/BoundingBox.py`

 * *Files identical despite different names*

### Comparing `asset_extraction_framework-0.9.0/assets/Asset/Image.py` & `asset_extraction_framework-0.9.1/assets/Asset/Image.py`

 * *Files identical despite different names*

### Comparing `asset_extraction_framework-0.9.0/assets/Asset/Palette.py` & `asset_extraction_framework-0.9.1/assets/Asset/Palette.py`

 * *Files identical despite different names*

### Comparing `asset_extraction_framework-0.9.0/assets/Asset/Sound.py` & `asset_extraction_framework-0.9.1/assets/Asset/Sound.py`

 * *Files identical despite different names*

### Comparing `asset_extraction_framework-0.9.0/assets/CommandLine.py` & `asset_extraction_framework-0.9.1/assets/CommandLine.py`

 * *Files identical despite different names*

### Comparing `asset_extraction_framework-0.9.0/assets/File.py` & `asset_extraction_framework-0.9.1/assets/File.py`

 * *Files identical despite different names*

### Comparing `asset_extraction_framework-0.9.0/pyproject.toml` & `asset_extraction_framework-0.9.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "asset_extraction_framework"
-version = "0.9.0"
-description = "Makes the Python struct library more self-documenting."
+version = "0.9.1"
+description = "Extract multimedia assets from legacy software"
 readme = "README.md"
 authors = [{ name = "npjg" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["struct", "reverse-engineering", "self-document"]
 requires-python = ">=3.9"
 
+dependencies = [
+    "Pillow>=9.2.0",
+    "numpy>=1.23.0",
+    "jsons>=1.6.2"
+]
+
 [project.urls]
 Homepage = "https://github.com/npjg/asset_extraction_framework"
```

