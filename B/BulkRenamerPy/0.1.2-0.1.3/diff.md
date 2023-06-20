# Comparing `tmp/BulkRenamerPy-0.1.2.tar.gz` & `tmp/BulkRenamerPy-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BulkRenamerPy-0.1.2.tar", last modified: Tue Jun 20 20:14:07 2023, max compression
+gzip compressed data, was "BulkRenamerPy-0.1.3.tar", last modified: Tue Jun 20 20:17:25 2023, max compression
```

## Comparing `BulkRenamerPy-0.1.2.tar` & `BulkRenamerPy-0.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-06-20 20:14:07.864496 BulkRenamerPy-0.1.2/
--rw-r--r--   0 frost     (1000) frost     (1000)    35149 2023-06-20 05:50:54.000000 BulkRenamerPy-0.1.2/LICENSE
--rw-r--r--   0 frost     (1000) frost     (1000)     1720 2023-06-20 20:14:07.864496 BulkRenamerPy-0.1.2/PKG-INFO
--rw-r--r--   0 frost     (1000) frost     (1000)     1089 2023-06-20 19:53:55.000000 BulkRenamerPy-0.1.2/README.md
--rw-r--r--   0 frost     (1000) frost     (1000)      901 2023-06-20 20:13:55.000000 BulkRenamerPy-0.1.2/pyproject.toml
--rw-r--r--   0 frost     (1000) frost     (1000)       38 2023-06-20 20:14:07.864496 BulkRenamerPy-0.1.2/setup.cfg
-drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-06-20 20:14:07.864496 BulkRenamerPy-0.1.2/src/
-drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-06-20 20:14:07.864496 BulkRenamerPy-0.1.2/src/BulkRenamerPy.egg-info/
--rw-r--r--   0 frost     (1000) frost     (1000)     1720 2023-06-20 20:14:07.000000 BulkRenamerPy-0.1.2/src/BulkRenamerPy.egg-info/PKG-INFO
--rw-r--r--   0 frost     (1000) frost     (1000)      357 2023-06-20 20:14:07.000000 BulkRenamerPy-0.1.2/src/BulkRenamerPy.egg-info/SOURCES.txt
--rw-r--r--   0 frost     (1000) frost     (1000)        1 2023-06-20 20:14:07.000000 BulkRenamerPy-0.1.2/src/BulkRenamerPy.egg-info/dependency_links.txt
--rw-r--r--   0 frost     (1000) frost     (1000)       49 2023-06-20 20:14:07.000000 BulkRenamerPy-0.1.2/src/BulkRenamerPy.egg-info/entry_points.txt
--rw-r--r--   0 frost     (1000) frost     (1000)       71 2023-06-20 20:14:07.000000 BulkRenamerPy-0.1.2/src/BulkRenamerPy.egg-info/requires.txt
--rw-r--r--   0 frost     (1000) frost     (1000)       30 2023-06-20 20:14:07.000000 BulkRenamerPy-0.1.2/src/BulkRenamerPy.egg-info/top_level.txt
--rw-r--r--   0 frost     (1000) frost     (1000)        0 2023-06-15 18:49:54.000000 BulkRenamerPy-0.1.2/src/__init__.py
--rw-r--r--   0 frost     (1000) frost     (1000)        0 2023-06-15 18:49:54.000000 BulkRenamerPy-0.1.2/src/__main__.py
--rw-r--r--   0 frost     (1000) frost     (1000)     2780 2023-06-20 17:54:27.000000 BulkRenamerPy-0.1.2/src/bulk_rename.py
-drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-06-20 20:14:07.864496 BulkRenamerPy-0.1.2/tests/
--rw-r--r--   0 frost     (1000) frost     (1000)     2283 2023-06-20 19:43:22.000000 BulkRenamerPy-0.1.2/tests/test_bulk_rename.py
+drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-06-20 20:17:25.840252 BulkRenamerPy-0.1.3/
+-rw-r--r--   0 frost     (1000) frost     (1000)    35149 2023-06-20 05:50:54.000000 BulkRenamerPy-0.1.3/LICENSE
+-rw-r--r--   0 frost     (1000) frost     (1000)     1720 2023-06-20 20:17:25.840252 BulkRenamerPy-0.1.3/PKG-INFO
+-rw-r--r--   0 frost     (1000) frost     (1000)     1089 2023-06-20 19:53:55.000000 BulkRenamerPy-0.1.3/README.md
+-rw-r--r--   0 frost     (1000) frost     (1000)      908 2023-06-20 20:17:08.000000 BulkRenamerPy-0.1.3/pyproject.toml
+-rw-r--r--   0 frost     (1000) frost     (1000)       38 2023-06-20 20:17:25.840252 BulkRenamerPy-0.1.3/setup.cfg
+drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-06-20 20:17:25.840252 BulkRenamerPy-0.1.3/src/
+drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-06-20 20:17:25.840252 BulkRenamerPy-0.1.3/src/BulkRenamerPy.egg-info/
+-rw-r--r--   0 frost     (1000) frost     (1000)     1720 2023-06-20 20:17:25.000000 BulkRenamerPy-0.1.3/src/BulkRenamerPy.egg-info/PKG-INFO
+-rw-r--r--   0 frost     (1000) frost     (1000)      357 2023-06-20 20:17:25.000000 BulkRenamerPy-0.1.3/src/BulkRenamerPy.egg-info/SOURCES.txt
+-rw-r--r--   0 frost     (1000) frost     (1000)        1 2023-06-20 20:17:25.000000 BulkRenamerPy-0.1.3/src/BulkRenamerPy.egg-info/dependency_links.txt
+-rw-r--r--   0 frost     (1000) frost     (1000)       56 2023-06-20 20:17:25.000000 BulkRenamerPy-0.1.3/src/BulkRenamerPy.egg-info/entry_points.txt
+-rw-r--r--   0 frost     (1000) frost     (1000)       71 2023-06-20 20:17:25.000000 BulkRenamerPy-0.1.3/src/BulkRenamerPy.egg-info/requires.txt
+-rw-r--r--   0 frost     (1000) frost     (1000)       30 2023-06-20 20:17:25.000000 BulkRenamerPy-0.1.3/src/BulkRenamerPy.egg-info/top_level.txt
+-rw-r--r--   0 frost     (1000) frost     (1000)        0 2023-06-15 18:49:54.000000 BulkRenamerPy-0.1.3/src/__init__.py
+-rw-r--r--   0 frost     (1000) frost     (1000)        0 2023-06-15 18:49:54.000000 BulkRenamerPy-0.1.3/src/__main__.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     2780 2023-06-20 17:54:27.000000 BulkRenamerPy-0.1.3/src/bulk_rename.py
+drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-06-20 20:17:25.840252 BulkRenamerPy-0.1.3/tests/
+-rw-r--r--   0 frost     (1000) frost     (1000)     2283 2023-06-20 19:43:22.000000 BulkRenamerPy-0.1.3/tests/test_bulk_rename.py
```

### Comparing `BulkRenamerPy-0.1.2/LICENSE` & `BulkRenamerPy-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `BulkRenamerPy-0.1.2/PKG-INFO` & `BulkRenamerPy-0.1.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BulkRenamerPy
-Version: 0.1.2
+Version: 0.1.3
 Summary: A simple tool to bulk rename files in a directory
 Author-email: Bruno Anesio <brunohanesio@gmail.com>
 Project-URL: Homepage, https://github.com/brunoanesio/bulk-rename
 Project-URL: Bug Tracker, https://github.com/brunoanesio/bulk-rename/issues
 Keywords: bulk rename,rename,rename files
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `BulkRenamerPy-0.1.2/README.md` & `BulkRenamerPy-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `BulkRenamerPy-0.1.2/pyproject.toml` & `BulkRenamerPy-0.1.3/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=68.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "BulkRenamerPy"
-version = "0.1.2"
+version = "0.1.3"
 authors = [{ name = "Bruno Anesio", email = "brunohanesio@gmail.com" }]
 description = "A simple tool to bulk rename files in a directory"
 keywords = ["bulk rename", "rename", "rename files"]
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
   "Programming Language :: Python :: 3",
@@ -25,12 +25,12 @@
   "rich-click",
 ]
 
 [project.optional-dependencies]
 test = ["pytest"]
 
 [project.scripts]
-bulk-rename = "bulk_rename:main"
+bulk_rename = "bulk_rename:bulk_rename"
 
 [project.urls]
 "Homepage" = "https://github.com/brunoanesio/bulk-rename"
 "Bug Tracker" = "https://github.com/brunoanesio/bulk-rename/issues"
```

### Comparing `BulkRenamerPy-0.1.2/src/BulkRenamerPy.egg-info/PKG-INFO` & `BulkRenamerPy-0.1.3/src/BulkRenamerPy.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BulkRenamerPy
-Version: 0.1.2
+Version: 0.1.3
 Summary: A simple tool to bulk rename files in a directory
 Author-email: Bruno Anesio <brunohanesio@gmail.com>
 Project-URL: Homepage, https://github.com/brunoanesio/bulk-rename
 Project-URL: Bug Tracker, https://github.com/brunoanesio/bulk-rename/issues
 Keywords: bulk rename,rename,rename files
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `BulkRenamerPy-0.1.2/src/bulk_rename.py` & `BulkRenamerPy-0.1.3/src/bulk_rename.py`

 * *Files identical despite different names*

### Comparing `BulkRenamerPy-0.1.2/tests/test_bulk_rename.py` & `BulkRenamerPy-0.1.3/tests/test_bulk_rename.py`

 * *Files identical despite different names*

