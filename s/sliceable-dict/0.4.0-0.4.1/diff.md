# Comparing `tmp/sliceable_dict-0.4.0-4.tar.gz` & `tmp/sliceable_dict-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sliceable_dict-0.4.0.tar", last modified: Mon Jun 19 10:42:12 2023, max compression
+gzip compressed data, was "sliceable_dict-0.4.1.tar", last modified: Tue Jun 20 08:57:35 2023, max compression
```

## Comparing `sliceable_dict-0.4.0-4.tar` & `sliceable_dict-0.4.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 palmb     (1000) palmb     (1000)        0 2023-06-19 10:42:12.539038 sliceable_dict-0.4.0/
--rw-rw-r--   0 palmb     (1000) palmb     (1000)    35149 2022-12-16 23:31:45.000000 sliceable_dict-0.4.0/LICENSE
--rw-rw-r--   0 palmb     (1000) palmb     (1000)     1781 2023-06-19 10:42:12.539038 sliceable_dict-0.4.0/PKG-INFO
--rw-rw-r--   0 palmb     (1000) palmb     (1000)     1218 2023-06-19 09:54:41.000000 sliceable_dict-0.4.0/README.md
--rw-rw-r--   0 palmb     (1000) palmb     (1000)      680 2023-06-19 10:38:13.000000 sliceable_dict-0.4.0/pyproject.toml
--rw-rw-r--   0 palmb     (1000) palmb     (1000)       38 2023-06-19 10:42:12.539038 sliceable_dict-0.4.0/setup.cfg
-drwxrwxr-x   0 palmb     (1000) palmb     (1000)        0 2023-06-19 10:42:12.539038 sliceable_dict-0.4.0/sliceable_dict/
--rw-rw-r--   0 palmb     (1000) palmb     (1000)       67 2023-02-08 13:50:27.000000 sliceable_dict-0.4.0/sliceable_dict/__init__.py
--rw-rw-r--   0 palmb     (1000) palmb     (1000)     9321 2023-06-19 10:13:49.000000 sliceable_dict-0.4.0/sliceable_dict/core.py
--rw-rw-r--   0 palmb     (1000) palmb     (1000)     4773 2023-03-14 20:25:45.000000 sliceable_dict-0.4.0/sliceable_dict/lib.py
-drwxrwxr-x   0 palmb     (1000) palmb     (1000)        0 2023-06-19 10:42:12.539038 sliceable_dict-0.4.0/sliceable_dict.egg-info/
--rw-rw-r--   0 palmb     (1000) palmb     (1000)     1781 2023-06-19 10:42:12.000000 sliceable_dict-0.4.0/sliceable_dict.egg-info/PKG-INFO
--rw-rw-r--   0 palmb     (1000) palmb     (1000)      363 2023-06-19 10:42:12.000000 sliceable_dict-0.4.0/sliceable_dict.egg-info/SOURCES.txt
--rw-rw-r--   0 palmb     (1000) palmb     (1000)        1 2023-06-19 10:42:12.000000 sliceable_dict-0.4.0/sliceable_dict.egg-info/dependency_links.txt
--rw-rw-r--   0 palmb     (1000) palmb     (1000)       18 2023-06-19 10:42:12.000000 sliceable_dict-0.4.0/sliceable_dict.egg-info/requires.txt
--rw-rw-r--   0 palmb     (1000) palmb     (1000)       15 2023-06-19 10:42:12.000000 sliceable_dict-0.4.0/sliceable_dict.egg-info/top_level.txt
-drwxrwxr-x   0 palmb     (1000) palmb     (1000)        0 2023-06-19 10:42:12.539038 sliceable_dict-0.4.0/tests/
--rw-rw-r--   0 palmb     (1000) palmb     (1000)     6211 2023-02-20 17:58:12.000000 sliceable_dict-0.4.0/tests/test_SimpleIdex.py
--rw-rw-r--   0 palmb     (1000) palmb     (1000)     6090 2023-06-19 09:55:38.000000 sliceable_dict-0.4.0/tests/test_SliceDict.py
--rw-rw-r--   0 palmb     (1000) palmb     (1000)      683 2023-06-19 10:14:01.000000 sliceable_dict-0.4.0/tests/test_pickle.py
+drwxrwxr-x   0 palmb     (1000) palmb     (1000)        0 2023-06-20 08:57:35.936647 sliceable_dict-0.4.1/
+-rw-rw-r--   0 palmb     (1000) palmb     (1000)    35149 2022-12-16 23:31:45.000000 sliceable_dict-0.4.1/LICENSE
+-rw-rw-r--   0 palmb     (1000) palmb     (1000)     1781 2023-06-20 08:57:35.936647 sliceable_dict-0.4.1/PKG-INFO
+-rw-rw-r--   0 palmb     (1000) palmb     (1000)     1218 2023-06-19 09:54:41.000000 sliceable_dict-0.4.1/README.md
+-rw-rw-r--   0 palmb     (1000) palmb     (1000)      680 2023-06-20 08:56:03.000000 sliceable_dict-0.4.1/pyproject.toml
+-rw-rw-r--   0 palmb     (1000) palmb     (1000)       38 2023-06-20 08:57:35.936647 sliceable_dict-0.4.1/setup.cfg
+drwxrwxr-x   0 palmb     (1000) palmb     (1000)        0 2023-06-20 08:57:35.932647 sliceable_dict-0.4.1/sliceable_dict/
+-rw-rw-r--   0 palmb     (1000) palmb     (1000)       67 2023-02-08 13:50:27.000000 sliceable_dict-0.4.1/sliceable_dict/__init__.py
+-rw-rw-r--   0 palmb     (1000) palmb     (1000)     9321 2023-06-19 10:13:49.000000 sliceable_dict-0.4.1/sliceable_dict/core.py
+-rw-rw-r--   0 palmb     (1000) palmb     (1000)     4773 2023-03-14 20:25:45.000000 sliceable_dict-0.4.1/sliceable_dict/lib.py
+drwxrwxr-x   0 palmb     (1000) palmb     (1000)        0 2023-06-20 08:57:35.936647 sliceable_dict-0.4.1/sliceable_dict.egg-info/
+-rw-rw-r--   0 palmb     (1000) palmb     (1000)     1781 2023-06-20 08:57:35.000000 sliceable_dict-0.4.1/sliceable_dict.egg-info/PKG-INFO
+-rw-rw-r--   0 palmb     (1000) palmb     (1000)      363 2023-06-20 08:57:35.000000 sliceable_dict-0.4.1/sliceable_dict.egg-info/SOURCES.txt
+-rw-rw-r--   0 palmb     (1000) palmb     (1000)        1 2023-06-20 08:57:35.000000 sliceable_dict-0.4.1/sliceable_dict.egg-info/dependency_links.txt
+-rw-rw-r--   0 palmb     (1000) palmb     (1000)       18 2023-06-20 08:57:35.000000 sliceable_dict-0.4.1/sliceable_dict.egg-info/requires.txt
+-rw-rw-r--   0 palmb     (1000) palmb     (1000)       15 2023-06-20 08:57:35.000000 sliceable_dict-0.4.1/sliceable_dict.egg-info/top_level.txt
+drwxrwxr-x   0 palmb     (1000) palmb     (1000)        0 2023-06-20 08:57:35.936647 sliceable_dict-0.4.1/tests/
+-rw-rw-r--   0 palmb     (1000) palmb     (1000)     6211 2023-02-20 17:58:12.000000 sliceable_dict-0.4.1/tests/test_SimpleIdex.py
+-rw-rw-r--   0 palmb     (1000) palmb     (1000)     6090 2023-06-19 09:55:38.000000 sliceable_dict-0.4.1/tests/test_SliceDict.py
+-rw-rw-r--   0 palmb     (1000) palmb     (1000)      683 2023-06-19 10:14:01.000000 sliceable_dict-0.4.1/tests/test_pickle.py
```

### Comparing `sliceable_dict-0.4.0/LICENSE` & `sliceable_dict-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sliceable_dict-0.4.0/PKG-INFO` & `sliceable_dict-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sliceable_dict
-Version: 0.4.0
+Version: 0.4.1
 Summary: Dictionary that support slicing and multiple key selection
 Author-email: Bert Palm <bert.palm.home@gmail.com>
 Project-URL: Homepage, https://github.com/palmb/slice-dict
 Project-URL: Bug Tracker, https://github.com/palmb/slice-dict/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `sliceable_dict-0.4.0/README.md` & `sliceable_dict-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `sliceable_dict-0.4.0/pyproject.toml` & `sliceable_dict-0.4.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sliceable_dict"
-version = "0.4.0"
+version = "0.4.1"
 authors = [
   { name="Bert Palm", email="bert.palm.home@gmail.com" },
 ]
 description = "Dictionary that support slicing and multiple key selection"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `sliceable_dict-0.4.0/sliceable_dict/core.py` & `sliceable_dict-0.4.1/sliceable_dict/core.py`

 * *Files identical despite different names*

### Comparing `sliceable_dict-0.4.0/sliceable_dict/lib.py` & `sliceable_dict-0.4.1/sliceable_dict/lib.py`

 * *Files identical despite different names*

### Comparing `sliceable_dict-0.4.0/sliceable_dict.egg-info/PKG-INFO` & `sliceable_dict-0.4.1/sliceable_dict.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sliceable-dict
-Version: 0.4.0
+Version: 0.4.1
 Summary: Dictionary that support slicing and multiple key selection
 Author-email: Bert Palm <bert.palm.home@gmail.com>
 Project-URL: Homepage, https://github.com/palmb/slice-dict
 Project-URL: Bug Tracker, https://github.com/palmb/slice-dict/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `sliceable_dict-0.4.0/tests/test_SimpleIdex.py` & `sliceable_dict-0.4.1/tests/test_SimpleIdex.py`

 * *Files identical despite different names*

### Comparing `sliceable_dict-0.4.0/tests/test_SliceDict.py` & `sliceable_dict-0.4.1/tests/test_SliceDict.py`

 * *Files identical despite different names*

### Comparing `sliceable_dict-0.4.0/tests/test_pickle.py` & `sliceable_dict-0.4.1/tests/test_pickle.py`

 * *Files identical despite different names*

