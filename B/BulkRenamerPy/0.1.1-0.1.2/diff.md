# Comparing `tmp/BulkRenamerPy-0.1.1.tar.gz` & `tmp/BulkRenamerPy-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BulkRenamerPy-0.1.1.tar", last modified: Tue Jun 20 19:59:18 2023, max compression
+gzip compressed data, was "BulkRenamerPy-0.1.2.tar", last modified: Tue Jun 20 20:14:07 2023, max compression
```

## Comparing `BulkRenamerPy-0.1.1.tar` & `BulkRenamerPy-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-06-20 19:59:18.600173 BulkRenamerPy-0.1.1/
--rw-r--r--   0 frost     (1000) frost     (1000)    35149 2023-06-20 05:50:54.000000 BulkRenamerPy-0.1.1/LICENSE
--rw-r--r--   0 frost     (1000) frost     (1000)     1720 2023-06-20 19:59:18.600173 BulkRenamerPy-0.1.1/PKG-INFO
--rw-r--r--   0 frost     (1000) frost     (1000)     1089 2023-06-20 19:53:55.000000 BulkRenamerPy-0.1.1/README.md
--rw-r--r--   0 frost     (1000) frost     (1000)      849 2023-06-20 19:56:51.000000 BulkRenamerPy-0.1.1/pyproject.toml
--rw-r--r--   0 frost     (1000) frost     (1000)       38 2023-06-20 19:59:18.600173 BulkRenamerPy-0.1.1/setup.cfg
-drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-06-20 19:59:18.600173 BulkRenamerPy-0.1.1/src/
-drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-06-20 19:59:18.600173 BulkRenamerPy-0.1.1/src/BulkRenamerPy.egg-info/
--rw-r--r--   0 frost     (1000) frost     (1000)     1720 2023-06-20 19:59:18.000000 BulkRenamerPy-0.1.1/src/BulkRenamerPy.egg-info/PKG-INFO
--rw-r--r--   0 frost     (1000) frost     (1000)      313 2023-06-20 19:59:18.000000 BulkRenamerPy-0.1.1/src/BulkRenamerPy.egg-info/SOURCES.txt
--rw-r--r--   0 frost     (1000) frost     (1000)        1 2023-06-20 19:59:18.000000 BulkRenamerPy-0.1.1/src/BulkRenamerPy.egg-info/dependency_links.txt
--rw-r--r--   0 frost     (1000) frost     (1000)       71 2023-06-20 19:59:18.000000 BulkRenamerPy-0.1.1/src/BulkRenamerPy.egg-info/requires.txt
--rw-r--r--   0 frost     (1000) frost     (1000)       30 2023-06-20 19:59:18.000000 BulkRenamerPy-0.1.1/src/BulkRenamerPy.egg-info/top_level.txt
--rw-r--r--   0 frost     (1000) frost     (1000)        0 2023-06-15 18:49:54.000000 BulkRenamerPy-0.1.1/src/__init__.py
--rw-r--r--   0 frost     (1000) frost     (1000)        0 2023-06-15 18:49:54.000000 BulkRenamerPy-0.1.1/src/__main__.py
--rw-r--r--   0 frost     (1000) frost     (1000)     2780 2023-06-20 17:54:27.000000 BulkRenamerPy-0.1.1/src/bulk_rename.py
-drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-06-20 19:59:18.600173 BulkRenamerPy-0.1.1/tests/
--rw-r--r--   0 frost     (1000) frost     (1000)     2283 2023-06-20 19:43:22.000000 BulkRenamerPy-0.1.1/tests/test_bulk_rename.py
+drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-06-20 20:14:07.864496 BulkRenamerPy-0.1.2/
+-rw-r--r--   0 frost     (1000) frost     (1000)    35149 2023-06-20 05:50:54.000000 BulkRenamerPy-0.1.2/LICENSE
+-rw-r--r--   0 frost     (1000) frost     (1000)     1720 2023-06-20 20:14:07.864496 BulkRenamerPy-0.1.2/PKG-INFO
+-rw-r--r--   0 frost     (1000) frost     (1000)     1089 2023-06-20 19:53:55.000000 BulkRenamerPy-0.1.2/README.md
+-rw-r--r--   0 frost     (1000) frost     (1000)      901 2023-06-20 20:13:55.000000 BulkRenamerPy-0.1.2/pyproject.toml
+-rw-r--r--   0 frost     (1000) frost     (1000)       38 2023-06-20 20:14:07.864496 BulkRenamerPy-0.1.2/setup.cfg
+drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-06-20 20:14:07.864496 BulkRenamerPy-0.1.2/src/
+drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-06-20 20:14:07.864496 BulkRenamerPy-0.1.2/src/BulkRenamerPy.egg-info/
+-rw-r--r--   0 frost     (1000) frost     (1000)     1720 2023-06-20 20:14:07.000000 BulkRenamerPy-0.1.2/src/BulkRenamerPy.egg-info/PKG-INFO
+-rw-r--r--   0 frost     (1000) frost     (1000)      357 2023-06-20 20:14:07.000000 BulkRenamerPy-0.1.2/src/BulkRenamerPy.egg-info/SOURCES.txt
+-rw-r--r--   0 frost     (1000) frost     (1000)        1 2023-06-20 20:14:07.000000 BulkRenamerPy-0.1.2/src/BulkRenamerPy.egg-info/dependency_links.txt
+-rw-r--r--   0 frost     (1000) frost     (1000)       49 2023-06-20 20:14:07.000000 BulkRenamerPy-0.1.2/src/BulkRenamerPy.egg-info/entry_points.txt
+-rw-r--r--   0 frost     (1000) frost     (1000)       71 2023-06-20 20:14:07.000000 BulkRenamerPy-0.1.2/src/BulkRenamerPy.egg-info/requires.txt
+-rw-r--r--   0 frost     (1000) frost     (1000)       30 2023-06-20 20:14:07.000000 BulkRenamerPy-0.1.2/src/BulkRenamerPy.egg-info/top_level.txt
+-rw-r--r--   0 frost     (1000) frost     (1000)        0 2023-06-15 18:49:54.000000 BulkRenamerPy-0.1.2/src/__init__.py
+-rw-r--r--   0 frost     (1000) frost     (1000)        0 2023-06-15 18:49:54.000000 BulkRenamerPy-0.1.2/src/__main__.py
+-rw-r--r--   0 frost     (1000) frost     (1000)     2780 2023-06-20 17:54:27.000000 BulkRenamerPy-0.1.2/src/bulk_rename.py
+drwxr-xr-x   0 frost     (1000) frost     (1000)        0 2023-06-20 20:14:07.864496 BulkRenamerPy-0.1.2/tests/
+-rw-r--r--   0 frost     (1000) frost     (1000)     2283 2023-06-20 19:43:22.000000 BulkRenamerPy-0.1.2/tests/test_bulk_rename.py
```

### Comparing `BulkRenamerPy-0.1.1/LICENSE` & `BulkRenamerPy-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `BulkRenamerPy-0.1.1/PKG-INFO` & `BulkRenamerPy-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BulkRenamerPy
-Version: 0.1.1
+Version: 0.1.2
 Summary: A simple tool to bulk rename files in a directory
 Author-email: Bruno Anesio <brunohanesio@gmail.com>
 Project-URL: Homepage, https://github.com/brunoanesio/bulk-rename
 Project-URL: Bug Tracker, https://github.com/brunoanesio/bulk-rename/issues
 Keywords: bulk rename,rename,rename files
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `BulkRenamerPy-0.1.1/README.md` & `BulkRenamerPy-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `BulkRenamerPy-0.1.1/pyproject.toml` & `BulkRenamerPy-0.1.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=68.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "BulkRenamerPy"
-version = "0.1.1"
+version = "0.1.2"
 authors = [{ name = "Bruno Anesio", email = "brunohanesio@gmail.com" }]
 description = "A simple tool to bulk rename files in a directory"
 keywords = ["bulk rename", "rename", "rename files"]
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
   "Programming Language :: Python :: 3",
@@ -24,10 +24,13 @@
   "rich",
   "rich-click",
 ]
 
 [project.optional-dependencies]
 test = ["pytest"]
 
+[project.scripts]
+bulk-rename = "bulk_rename:main"
+
 [project.urls]
 "Homepage" = "https://github.com/brunoanesio/bulk-rename"
 "Bug Tracker" = "https://github.com/brunoanesio/bulk-rename/issues"
```

### Comparing `BulkRenamerPy-0.1.1/src/BulkRenamerPy.egg-info/PKG-INFO` & `BulkRenamerPy-0.1.2/src/BulkRenamerPy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BulkRenamerPy
-Version: 0.1.1
+Version: 0.1.2
 Summary: A simple tool to bulk rename files in a directory
 Author-email: Bruno Anesio <brunohanesio@gmail.com>
 Project-URL: Homepage, https://github.com/brunoanesio/bulk-rename
 Project-URL: Bug Tracker, https://github.com/brunoanesio/bulk-rename/issues
 Keywords: bulk rename,rename,rename files
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `BulkRenamerPy-0.1.1/src/bulk_rename.py` & `BulkRenamerPy-0.1.2/src/bulk_rename.py`

 * *Files identical despite different names*

### Comparing `BulkRenamerPy-0.1.1/tests/test_bulk_rename.py` & `BulkRenamerPy-0.1.2/tests/test_bulk_rename.py`

 * *Files identical despite different names*

