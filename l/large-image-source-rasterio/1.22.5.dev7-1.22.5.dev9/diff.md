# Comparing `tmp/large-image-source-rasterio-1.22.5.dev7.tar.gz` & `tmp/large-image-source-rasterio-1.22.5.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "large-image-source-rasterio-1.22.5.dev7.tar", last modified: Fri Jun 16 21:01:34 2023, max compression
+gzip compressed data, was "large-image-source-rasterio-1.22.5.dev9.tar", last modified: Fri Jun 16 21:21:33 2023, max compression
```

## Comparing `large-image-source-rasterio-1.22.5.dev7.tar` & `large-image-source-rasterio-1.22.5.dev9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 21:01:34.586655 large-image-source-rasterio-1.22.5.dev7/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2023-06-16 21:01:34.000000 large-image-source-rasterio-1.22.5.dev7/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)      845 2023-06-16 21:01:34.586655 large-image-source-rasterio-1.22.5.dev7/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8267 2023-06-16 21:01:34.000000 large-image-source-rasterio-1.22.5.dev7/README.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 21:01:34.586655 large-image-source-rasterio-1.22.5.dev7/large_image_source_rasterio/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    43289 2023-06-16 20:59:30.000000 large-image-source-rasterio-1.22.5.dev7/large_image_source_rasterio/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1444 2023-06-16 20:59:30.000000 large-image-source-rasterio-1.22.5.dev7/large_image_source_rasterio/girder_source.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 21:01:34.586655 large-image-source-rasterio-1.22.5.dev7/large_image_source_rasterio.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      845 2023-06-16 21:01:34.000000 large-image-source-rasterio-1.22.5.dev7/large_image_source_rasterio.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      420 2023-06-16 21:01:34.000000 large-image-source-rasterio-1.22.5.dev7/large_image_source_rasterio.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-16 21:01:34.000000 large-image-source-rasterio-1.22.5.dev7/large_image_source_rasterio.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      190 2023-06-16 21:01:34.000000 large-image-source-rasterio-1.22.5.dev7/large_image_source_rasterio.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      108 2023-06-16 21:01:34.000000 large-image-source-rasterio-1.22.5.dev7/large_image_source_rasterio.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       28 2023-06-16 21:01:34.000000 large-image-source-rasterio-1.22.5.dev7/large_image_source_rasterio.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-06-16 21:01:34.586655 large-image-source-rasterio-1.22.5.dev7/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2564 2023-06-16 20:59:30.000000 large-image-source-rasterio-1.22.5.dev7/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 21:21:33.899934 large-image-source-rasterio-1.22.5.dev9/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2023-06-16 21:21:33.000000 large-image-source-rasterio-1.22.5.dev9/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      845 2023-06-16 21:21:33.899934 large-image-source-rasterio-1.22.5.dev9/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8267 2023-06-16 21:21:33.000000 large-image-source-rasterio-1.22.5.dev9/README.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 21:21:33.899934 large-image-source-rasterio-1.22.5.dev9/large_image_source_rasterio/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    43289 2023-06-16 21:20:05.000000 large-image-source-rasterio-1.22.5.dev9/large_image_source_rasterio/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1444 2023-06-16 21:20:05.000000 large-image-source-rasterio-1.22.5.dev9/large_image_source_rasterio/girder_source.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 21:21:33.899934 large-image-source-rasterio-1.22.5.dev9/large_image_source_rasterio.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      845 2023-06-16 21:21:33.000000 large-image-source-rasterio-1.22.5.dev9/large_image_source_rasterio.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      420 2023-06-16 21:21:33.000000 large-image-source-rasterio-1.22.5.dev9/large_image_source_rasterio.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-16 21:21:33.000000 large-image-source-rasterio-1.22.5.dev9/large_image_source_rasterio.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      190 2023-06-16 21:21:33.000000 large-image-source-rasterio-1.22.5.dev9/large_image_source_rasterio.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      108 2023-06-16 21:21:33.000000 large-image-source-rasterio-1.22.5.dev9/large_image_source_rasterio.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       28 2023-06-16 21:21:33.000000 large-image-source-rasterio-1.22.5.dev9/large_image_source_rasterio.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-06-16 21:21:33.899934 large-image-source-rasterio-1.22.5.dev9/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2564 2023-06-16 21:20:05.000000 large-image-source-rasterio-1.22.5.dev9/setup.py
```

### Comparing `large-image-source-rasterio-1.22.5.dev7/LICENSE` & `large-image-source-rasterio-1.22.5.dev9/LICENSE`

 * *Files identical despite different names*

### Comparing `large-image-source-rasterio-1.22.5.dev7/PKG-INFO` & `large-image-source-rasterio-1.22.5.dev9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-rasterio
-Version: 1.22.5.dev7
+Version: 1.22.5.dev9
 Summary: A rasterio tilesource for large_image.
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `large-image-source-rasterio-1.22.5.dev7/README.rst` & `large-image-source-rasterio-1.22.5.dev9/README.rst`

 * *Files identical despite different names*

### Comparing `large-image-source-rasterio-1.22.5.dev7/large_image_source_rasterio/__init__.py` & `large-image-source-rasterio-1.22.5.dev9/large_image_source_rasterio/__init__.py`

 * *Files identical despite different names*

### Comparing `large-image-source-rasterio-1.22.5.dev7/large_image_source_rasterio/girder_source.py` & `large-image-source-rasterio-1.22.5.dev9/large_image_source_rasterio/girder_source.py`

 * *Files identical despite different names*

### Comparing `large-image-source-rasterio-1.22.5.dev7/large_image_source_rasterio.egg-info/PKG-INFO` & `large-image-source-rasterio-1.22.5.dev9/large_image_source_rasterio.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-rasterio
-Version: 1.22.5.dev7
+Version: 1.22.5.dev9
 Summary: A rasterio tilesource for large_image.
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `large-image-source-rasterio-1.22.5.dev7/setup.py` & `large-image-source-rasterio-1.22.5.dev9/setup.py`

 * *Files identical despite different names*

