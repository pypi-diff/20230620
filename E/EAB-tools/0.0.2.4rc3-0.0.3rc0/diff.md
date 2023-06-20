# Comparing `tmp/EAB_tools-0.0.2.4rc3.tar.gz` & `tmp/EAB_tools-0.0.3rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EAB_tools-0.0.2.4rc3.tar", last modified: Thu Jan  5 00:23:09 2023, max compression
+gzip compressed data, was "EAB_tools-0.0.3rc0.tar", last modified: Tue Jun 20 16:15:47 2023, max compression
```

## Comparing `EAB_tools-0.0.2.4rc3.tar` & `EAB_tools-0.0.3rc0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 00:23:09.215802 EAB_tools-0.0.2.4rc3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 00:23:09.211801 EAB_tools-0.0.2.4rc3/EAB_tools/
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-01-05 00:22:57.000000 EAB_tools-0.0.2.4rc3/EAB_tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 00:23:09.215802 EAB_tools-0.0.2.4rc3/EAB_tools/_testing/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-01-05 00:22:57.000000 EAB_tools-0.0.2.4rc3/EAB_tools/_testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-01-05 00:22:57.000000 EAB_tools-0.0.2.4rc3/EAB_tools/_testing/io.py
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-01-05 00:22:57.000000 EAB_tools-0.0.2.4rc3/EAB_tools/_testing/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     7585 2023-01-05 00:22:57.000000 EAB_tools-0.0.2.4rc3/EAB_tools/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-01-05 00:22:57.000000 EAB_tools-0.0.2.4rc3/EAB_tools/eab_rc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 00:23:09.215802 EAB_tools-0.0.2.4rc3/EAB_tools/io/
--rw-r--r--   0 runner    (1001) docker     (123)    25155 2023-01-05 00:22:57.000000 EAB_tools-0.0.2.4rc3/EAB_tools/io/display.py
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-01-05 00:22:57.000000 EAB_tools-0.0.2.4rc3/EAB_tools/io/filenames.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 00:23:09.215802 EAB_tools-0.0.2.4rc3/EAB_tools/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-05 00:22:57.000000 EAB_tools-0.0.2.4rc3/EAB_tools/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 00:23:09.215802 EAB_tools-0.0.2.4rc3/EAB_tools/tests/io/
--rw-r--r--   0 runner    (1001) docker     (123)    21542 2023-01-05 00:22:57.000000 EAB_tools-0.0.2.4rc3/EAB_tools/tests/io/test_display.py
--rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-01-05 00:22:57.000000 EAB_tools-0.0.2.4rc3/EAB_tools/tests/io/test_filenames.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 00:23:09.215802 EAB_tools-0.0.2.4rc3/EAB_tools/tests/util/
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-01-05 00:22:57.000000 EAB_tools-0.0.2.4rc3/EAB_tools/tests/util/test_hashing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 00:23:09.215802 EAB_tools-0.0.2.4rc3/EAB_tools/util/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-01-05 00:22:57.000000 EAB_tools-0.0.2.4rc3/EAB_tools/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-01-05 00:22:57.000000 EAB_tools-0.0.2.4rc3/EAB_tools/util/hashing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 00:23:09.215802 EAB_tools-0.0.2.4rc3/EAB_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4350 2023-01-05 00:23:09.000000 EAB_tools-0.0.2.4rc3/EAB_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-01-05 00:23:09.000000 EAB_tools-0.0.2.4rc3/EAB_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-05 00:23:09.000000 EAB_tools-0.0.2.4rc3/EAB_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-01-05 00:23:09.000000 EAB_tools-0.0.2.4rc3/EAB_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-01-05 00:23:09.000000 EAB_tools-0.0.2.4rc3/EAB_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-01-05 00:22:57.000000 EAB_tools-0.0.2.4rc3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4350 2023-01-05 00:23:09.215802 EAB_tools-0.0.2.4rc3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-01-05 00:22:57.000000 EAB_tools-0.0.2.4rc3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-01-05 00:22:57.000000 EAB_tools-0.0.2.4rc3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-01-05 00:23:09.215802 EAB_tools-0.0.2.4rc3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-01-05 00:22:57.000000 EAB_tools-0.0.2.4rc3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:15:47.942732 EAB_tools-0.0.3rc0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:15:47.942732 EAB_tools-0.0.3rc0/EAB_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-20 16:15:34.000000 EAB_tools-0.0.3rc0/EAB_tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:15:47.942732 EAB_tools-0.0.3rc0/EAB_tools/_testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-20 16:15:34.000000 EAB_tools-0.0.3rc0/EAB_tools/_testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-20 16:15:34.000000 EAB_tools-0.0.3rc0/EAB_tools/_testing/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-20 16:15:34.000000 EAB_tools-0.0.3rc0/EAB_tools/_testing/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7585 2023-06-20 16:15:34.000000 EAB_tools-0.0.3rc0/EAB_tools/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-20 16:15:34.000000 EAB_tools-0.0.3rc0/EAB_tools/eab_rc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:15:47.942732 EAB_tools-0.0.3rc0/EAB_tools/io/
+-rw-r--r--   0 runner    (1001) docker     (123)    25155 2023-06-20 16:15:34.000000 EAB_tools-0.0.3rc0/EAB_tools/io/display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-06-20 16:15:34.000000 EAB_tools-0.0.3rc0/EAB_tools/io/filenames.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:15:47.942732 EAB_tools-0.0.3rc0/EAB_tools/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 16:15:34.000000 EAB_tools-0.0.3rc0/EAB_tools/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:15:47.942732 EAB_tools-0.0.3rc0/EAB_tools/tests/io/
+-rw-r--r--   0 runner    (1001) docker     (123)    21542 2023-06-20 16:15:34.000000 EAB_tools-0.0.3rc0/EAB_tools/tests/io/test_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-06-20 16:15:34.000000 EAB_tools-0.0.3rc0/EAB_tools/tests/io/test_filenames.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:15:47.942732 EAB_tools-0.0.3rc0/EAB_tools/tests/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-06-20 16:15:34.000000 EAB_tools-0.0.3rc0/EAB_tools/tests/util/test_hashing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:15:47.942732 EAB_tools-0.0.3rc0/EAB_tools/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-20 16:15:34.000000 EAB_tools-0.0.3rc0/EAB_tools/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-06-20 16:15:34.000000 EAB_tools-0.0.3rc0/EAB_tools/util/hashing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:15:47.942732 EAB_tools-0.0.3rc0/EAB_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4348 2023-06-20 16:15:47.000000 EAB_tools-0.0.3rc0/EAB_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-20 16:15:47.000000 EAB_tools-0.0.3rc0/EAB_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 16:15:47.000000 EAB_tools-0.0.3rc0/EAB_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-20 16:15:47.000000 EAB_tools-0.0.3rc0/EAB_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-20 16:15:47.000000 EAB_tools-0.0.3rc0/EAB_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-20 16:15:34.000000 EAB_tools-0.0.3rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4348 2023-06-20 16:15:47.942732 EAB_tools-0.0.3rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-06-20 16:15:34.000000 EAB_tools-0.0.3rc0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-06-20 16:15:34.000000 EAB_tools-0.0.3rc0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-20 16:15:47.946732 EAB_tools-0.0.3rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-20 16:15:34.000000 EAB_tools-0.0.3rc0/setup.py
```

### Comparing `EAB_tools-0.0.2.4rc3/EAB_tools/_testing/io.py` & `EAB_tools-0.0.3rc0/EAB_tools/_testing/io.py`

 * *Files identical despite different names*

### Comparing `EAB_tools-0.0.2.4rc3/EAB_tools/conftest.py` & `EAB_tools-0.0.3rc0/EAB_tools/conftest.py`

 * *Files identical despite different names*

### Comparing `EAB_tools-0.0.2.4rc3/EAB_tools/io/display.py` & `EAB_tools-0.0.3rc0/EAB_tools/io/display.py`

 * *Files identical despite different names*

### Comparing `EAB_tools-0.0.2.4rc3/EAB_tools/io/filenames.py` & `EAB_tools-0.0.3rc0/EAB_tools/io/filenames.py`

 * *Files identical despite different names*

### Comparing `EAB_tools-0.0.2.4rc3/EAB_tools/tests/io/test_display.py` & `EAB_tools-0.0.3rc0/EAB_tools/tests/io/test_display.py`

 * *Files identical despite different names*

### Comparing `EAB_tools-0.0.2.4rc3/EAB_tools/tests/io/test_filenames.py` & `EAB_tools-0.0.3rc0/EAB_tools/tests/io/test_filenames.py`

 * *Files identical despite different names*

### Comparing `EAB_tools-0.0.2.4rc3/EAB_tools/tests/util/test_hashing.py` & `EAB_tools-0.0.3rc0/EAB_tools/tests/util/test_hashing.py`

 * *Files identical despite different names*

### Comparing `EAB_tools-0.0.2.4rc3/EAB_tools/util/hashing.py` & `EAB_tools-0.0.3rc0/EAB_tools/util/hashing.py`

 * *Files identical despite different names*

### Comparing `EAB_tools-0.0.2.4rc3/EAB_tools.egg-info/PKG-INFO` & `EAB_tools-0.0.3rc0/EAB_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EAB-tools
-Version: 0.0.2.4rc3
+Version: 0.0.3rc0
 Summary: Tools for analyzing data exported from the EAB Navigate Student Success Management Software.
 Author: Moshe Rubin
 Author-email: Moshe Rubin <mosherubin137@gmail.com>
 License: MIT License
         
         Copyright 2022 Moshe Rubin https://github.com/moshemoshe137
```

### Comparing `EAB_tools-0.0.2.4rc3/EAB_tools.egg-info/SOURCES.txt` & `EAB_tools-0.0.3rc0/EAB_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `EAB_tools-0.0.2.4rc3/LICENSE` & `EAB_tools-0.0.3rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `EAB_tools-0.0.2.4rc3/PKG-INFO` & `EAB_tools-0.0.3rc0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EAB_tools
-Version: 0.0.2.4rc3
+Version: 0.0.3rc0
 Summary: Tools for analyzing data exported from the EAB Navigate Student Success Management Software.
 Author: Moshe Rubin
 Author-email: Moshe Rubin <mosherubin137@gmail.com>
 License: MIT License
         
         Copyright 2022 Moshe Rubin https://github.com/moshemoshe137
```

### Comparing `EAB_tools-0.0.2.4rc3/README.md` & `EAB_tools-0.0.3rc0/README.md`

 * *Files identical despite different names*

### Comparing `EAB_tools-0.0.2.4rc3/pyproject.toml` & `EAB_tools-0.0.3rc0/pyproject.toml`

 * *Files identical despite different names*

