# Comparing `tmp/hot-fair-utilities-1.0.51.tar.gz` & `tmp/hot-fair-utilities-1.0.52.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hot-fair-utilities-1.0.51.tar", last modified: Wed Jun 14 09:13:45 2023, max compression
+gzip compressed data, was "hot-fair-utilities-1.0.52.tar", last modified: Tue Jun 20 05:16:44 2023, max compression
```

## Comparing `hot-fair-utilities-1.0.51.tar` & `hot-fair-utilities-1.0.52.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:13:45.565979 hot-fair-utilities-1.0.51/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-14 09:13:24.000000 hot-fair-utilities-1.0.51/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-14 09:13:24.000000 hot-fair-utilities-1.0.51/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    43175 2023-06-14 09:13:45.565979 hot-fair-utilities-1.0.51/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-06-14 09:13:24.000000 hot-fair-utilities-1.0.51/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:13:45.561979 hot-fair-utilities-1.0.51/hot_fair_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-14 09:13:24.000000 hot-fair-utilities-1.0.51/hot_fair_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-06-14 09:13:24.000000 hot-fair-utilities-1.0.51/hot_fair_utilities/georeferencing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:13:45.561979 hot-fair-utilities-1.0.51/hot_fair_utilities/inference/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-14 09:13:24.000000 hot-fair-utilities-1.0.51/hot_fair_utilities/inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-06-14 09:13:24.000000 hot-fair-utilities-1.0.51/hot_fair_utilities/inference/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-14 09:13:24.000000 hot-fair-utilities-1.0.51/hot_fair_utilities/inference/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:13:45.561979 hot-fair-utilities-1.0.51/hot_fair_utilities/postprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-14 09:13:24.000000 hot-fair-utilities-1.0.51/hot_fair_utilities/postprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-06-14 09:13:24.000000 hot-fair-utilities-1.0.51/hot_fair_utilities/postprocessing/building_footprint.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-14 09:13:24.000000 hot-fair-utilities-1.0.51/hot_fair_utilities/postprocessing/get_polygons.py
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-06-14 09:13:24.000000 hot-fair-utilities-1.0.51/hot_fair_utilities/postprocessing/merge_polygons.py
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-06-14 09:13:24.000000 hot-fair-utilities-1.0.51/hot_fair_utilities/postprocessing/polygonize.py
--rw-r--r--   0 runner    (1001) docker     (123)     8440 2023-06-14 09:13:24.000000 hot-fair-utilities-1.0.51/hot_fair_utilities/postprocessing/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-06-14 09:13:24.000000 hot-fair-utilities-1.0.51/hot_fair_utilities/postprocessing/vectorize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:13:45.561979 hot-fair-utilities-1.0.51/hot_fair_utilities/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-14 09:13:24.000000 hot-fair-utilities-1.0.51/hot_fair_utilities/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-06-14 09:13:24.000000 hot-fair-utilities-1.0.51/hot_fair_utilities/preprocessing/clip_labels.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-14 09:13:24.000000 hot-fair-utilities-1.0.51/hot_fair_utilities/preprocessing/fix_labels.py
--rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-06-14 09:13:24.000000 hot-fair-utilities-1.0.51/hot_fair_utilities/preprocessing/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-14 09:13:24.000000 hot-fair-utilities-1.0.51/hot_fair_utilities/preprocessing/reproject_labels.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:13:45.565979 hot-fair-utilities-1.0.51/hot_fair_utilities/training/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-14 09:13:24.000000 hot-fair-utilities-1.0.51/hot_fair_utilities/training/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-06-14 09:13:24.000000 hot-fair-utilities-1.0.51/hot_fair_utilities/training/cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-06-14 09:13:24.000000 hot-fair-utilities-1.0.51/hot_fair_utilities/training/prepare_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-06-14 09:13:24.000000 hot-fair-utilities-1.0.51/hot_fair_utilities/training/ramp_config_base.json
--rw-r--r--   0 runner    (1001) docker     (123)    12215 2023-06-14 09:13:24.000000 hot-fair-utilities-1.0.51/hot_fair_utilities/training/run_training.py
--rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-06-14 09:13:24.000000 hot-fair-utilities-1.0.51/hot_fair_utilities/training/train.py
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-06-14 09:13:24.000000 hot-fair-utilities-1.0.51/hot_fair_utilities/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:13:45.561979 hot-fair-utilities-1.0.51/hot_fair_utilities.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    43175 2023-06-14 09:13:45.000000 hot-fair-utilities-1.0.51/hot_fair_utilities.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-06-14 09:13:45.000000 hot-fair-utilities-1.0.51/hot_fair_utilities.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 09:13:45.000000 hot-fair-utilities-1.0.51/hot_fair_utilities.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-14 09:13:45.000000 hot-fair-utilities-1.0.51/hot_fair_utilities.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-14 09:13:45.000000 hot-fair-utilities-1.0.51/hot_fair_utilities.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-06-14 09:13:24.000000 hot-fair-utilities-1.0.51/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 09:13:45.565979 hot-fair-utilities-1.0.51/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 09:13:24.000000 hot-fair-utilities-1.0.51/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 05:16:44.770195 hot-fair-utilities-1.0.52/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-20 05:16:31.000000 hot-fair-utilities-1.0.52/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-20 05:16:31.000000 hot-fair-utilities-1.0.52/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    43175 2023-06-20 05:16:44.770195 hot-fair-utilities-1.0.52/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-06-20 05:16:31.000000 hot-fair-utilities-1.0.52/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 05:16:44.762195 hot-fair-utilities-1.0.52/hot_fair_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-20 05:16:31.000000 hot-fair-utilities-1.0.52/hot_fair_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-06-20 05:16:31.000000 hot-fair-utilities-1.0.52/hot_fair_utilities/georeferencing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 05:16:44.762195 hot-fair-utilities-1.0.52/hot_fair_utilities/inference/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-20 05:16:31.000000 hot-fair-utilities-1.0.52/hot_fair_utilities/inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-06-20 05:16:31.000000 hot-fair-utilities-1.0.52/hot_fair_utilities/inference/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-20 05:16:31.000000 hot-fair-utilities-1.0.52/hot_fair_utilities/inference/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 05:16:44.766195 hot-fair-utilities-1.0.52/hot_fair_utilities/postprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-20 05:16:31.000000 hot-fair-utilities-1.0.52/hot_fair_utilities/postprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-06-20 05:16:31.000000 hot-fair-utilities-1.0.52/hot_fair_utilities/postprocessing/building_footprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-20 05:16:31.000000 hot-fair-utilities-1.0.52/hot_fair_utilities/postprocessing/get_polygons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-06-20 05:16:31.000000 hot-fair-utilities-1.0.52/hot_fair_utilities/postprocessing/merge_polygons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-06-20 05:16:31.000000 hot-fair-utilities-1.0.52/hot_fair_utilities/postprocessing/polygonize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8440 2023-06-20 05:16:31.000000 hot-fair-utilities-1.0.52/hot_fair_utilities/postprocessing/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-06-20 05:16:31.000000 hot-fair-utilities-1.0.52/hot_fair_utilities/postprocessing/vectorize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 05:16:44.766195 hot-fair-utilities-1.0.52/hot_fair_utilities/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-20 05:16:31.000000 hot-fair-utilities-1.0.52/hot_fair_utilities/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-06-20 05:16:31.000000 hot-fair-utilities-1.0.52/hot_fair_utilities/preprocessing/clip_labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-20 05:16:31.000000 hot-fair-utilities-1.0.52/hot_fair_utilities/preprocessing/fix_labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-06-20 05:16:31.000000 hot-fair-utilities-1.0.52/hot_fair_utilities/preprocessing/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-20 05:16:31.000000 hot-fair-utilities-1.0.52/hot_fair_utilities/preprocessing/reproject_labels.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 05:16:44.770195 hot-fair-utilities-1.0.52/hot_fair_utilities/training/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-20 05:16:31.000000 hot-fair-utilities-1.0.52/hot_fair_utilities/training/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-06-20 05:16:31.000000 hot-fair-utilities-1.0.52/hot_fair_utilities/training/cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-06-20 05:16:31.000000 hot-fair-utilities-1.0.52/hot_fair_utilities/training/prepare_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-06-20 05:16:31.000000 hot-fair-utilities-1.0.52/hot_fair_utilities/training/ramp_config_base.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12215 2023-06-20 05:16:31.000000 hot-fair-utilities-1.0.52/hot_fair_utilities/training/run_training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-06-20 05:16:31.000000 hot-fair-utilities-1.0.52/hot_fair_utilities/training/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8751 2023-06-20 05:16:31.000000 hot-fair-utilities-1.0.52/hot_fair_utilities/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 05:16:44.762195 hot-fair-utilities-1.0.52/hot_fair_utilities.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    43175 2023-06-20 05:16:44.000000 hot-fair-utilities-1.0.52/hot_fair_utilities.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-06-20 05:16:44.000000 hot-fair-utilities-1.0.52/hot_fair_utilities.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 05:16:44.000000 hot-fair-utilities-1.0.52/hot_fair_utilities.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-20 05:16:44.000000 hot-fair-utilities-1.0.52/hot_fair_utilities.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-20 05:16:44.000000 hot-fair-utilities-1.0.52/hot_fair_utilities.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-06-20 05:16:31.000000 hot-fair-utilities-1.0.52/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 05:16:44.770195 hot-fair-utilities-1.0.52/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 05:16:31.000000 hot-fair-utilities-1.0.52/setup.py
```

### Comparing `hot-fair-utilities-1.0.51/LICENSE` & `hot-fair-utilities-1.0.52/LICENSE`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.0.51/PKG-INFO` & `hot-fair-utilities-1.0.52/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hot-fair-utilities
-Version: 1.0.51
+Version: 1.0.52
 Summary: Utilities for AI - Assisted Mapping fAIr
 Author-email: Omdena <project@omdena.com>, Hot Tech Team <sysadmin@hotosm.org>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `hot-fair-utilities-1.0.51/README.md` & `hot-fair-utilities-1.0.52/README.md`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.0.51/hot_fair_utilities/georeferencing.py` & `hot-fair-utilities-1.0.52/hot_fair_utilities/georeferencing.py`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.0.51/hot_fair_utilities/inference/predict.py` & `hot-fair-utilities-1.0.52/hot_fair_utilities/inference/predict.py`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.0.51/hot_fair_utilities/inference/utils.py` & `hot-fair-utilities-1.0.52/hot_fair_utilities/inference/utils.py`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.0.51/hot_fair_utilities/postprocessing/building_footprint.py` & `hot-fair-utilities-1.0.52/hot_fair_utilities/postprocessing/building_footprint.py`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.0.51/hot_fair_utilities/postprocessing/get_polygons.py` & `hot-fair-utilities-1.0.52/hot_fair_utilities/postprocessing/get_polygons.py`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.0.51/hot_fair_utilities/postprocessing/merge_polygons.py` & `hot-fair-utilities-1.0.52/hot_fair_utilities/postprocessing/merge_polygons.py`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.0.51/hot_fair_utilities/postprocessing/polygonize.py` & `hot-fair-utilities-1.0.52/hot_fair_utilities/postprocessing/polygonize.py`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.0.51/hot_fair_utilities/postprocessing/utils.py` & `hot-fair-utilities-1.0.52/hot_fair_utilities/postprocessing/utils.py`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.0.51/hot_fair_utilities/postprocessing/vectorize.py` & `hot-fair-utilities-1.0.52/hot_fair_utilities/postprocessing/vectorize.py`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.0.51/hot_fair_utilities/preprocessing/clip_labels.py` & `hot-fair-utilities-1.0.52/hot_fair_utilities/preprocessing/clip_labels.py`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.0.51/hot_fair_utilities/preprocessing/fix_labels.py` & `hot-fair-utilities-1.0.52/hot_fair_utilities/preprocessing/fix_labels.py`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.0.51/hot_fair_utilities/preprocessing/preprocess.py` & `hot-fair-utilities-1.0.52/hot_fair_utilities/preprocessing/preprocess.py`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.0.51/hot_fair_utilities/preprocessing/reproject_labels.py` & `hot-fair-utilities-1.0.52/hot_fair_utilities/preprocessing/reproject_labels.py`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.0.51/hot_fair_utilities/training/cleanup.py` & `hot-fair-utilities-1.0.52/hot_fair_utilities/training/cleanup.py`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.0.51/hot_fair_utilities/training/prepare_data.py` & `hot-fair-utilities-1.0.52/hot_fair_utilities/training/prepare_data.py`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.0.51/hot_fair_utilities/training/ramp_config_base.json` & `hot-fair-utilities-1.0.52/hot_fair_utilities/training/ramp_config_base.json`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.0.51/hot_fair_utilities/training/run_training.py` & `hot-fair-utilities-1.0.52/hot_fair_utilities/training/run_training.py`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.0.51/hot_fair_utilities/training/train.py` & `hot-fair-utilities-1.0.52/hot_fair_utilities/training/train.py`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.0.51/hot_fair_utilities.egg-info/PKG-INFO` & `hot-fair-utilities-1.0.52/hot_fair_utilities.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hot-fair-utilities
-Version: 1.0.51
+Version: 1.0.52
 Summary: Utilities for AI - Assisted Mapping fAIr
 Author-email: Omdena <project@omdena.com>, Hot Tech Team <sysadmin@hotosm.org>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `hot-fair-utilities-1.0.51/hot_fair_utilities.egg-info/SOURCES.txt` & `hot-fair-utilities-1.0.52/hot_fair_utilities.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hot-fair-utilities-1.0.51/pyproject.toml` & `hot-fair-utilities-1.0.52/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hot-fair-utilities"
-version = "1.0.51"
+version = "1.0.52"
 description = "Utilities for AI - Assisted Mapping fAIr"
 readme = "README.md"
 authors = [{ name = "Omdena", email = "project@omdena.com" },{ name = "Hot Tech Team", email = "sysadmin@hotosm.org" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: BSD License",
     "Programming Language :: Python :: 3",
```

