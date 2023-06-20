# Comparing `tmp/fx-bin-0.6.0.tar.gz` & `tmp/fx-bin-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fx-bin-0.6.0.tar", last modified: Tue Jun 20 15:51:04 2023, max compression
+gzip compressed data, was "fx-bin-0.6.1.tar", last modified: Tue Jun 20 16:02:17 2023, max compression
```

## Comparing `fx-bin-0.6.0.tar` & `fx-bin-0.6.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:51:04.164736 fx-bin-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-06-20 15:50:59.000000 fx-bin-0.6.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-20 15:50:59.000000 fx-bin-0.6.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-20 15:50:59.000000 fx-bin-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-06-20 15:51:04.164736 fx-bin-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-20 15:50:59.000000 fx-bin-0.6.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:51:04.160736 fx-bin-0.6.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-20 15:50:59.000000 fx-bin-0.6.0/docs/Makefile
--rwxr-xr-x   0 runner    (1001) docker     (123)     4845 2023-06-20 15:50:59.000000 fx-bin-0.6.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-20 15:50:59.000000 fx-bin-0.6.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-20 15:50:59.000000 fx-bin-0.6.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-20 15:50:59.000000 fx-bin-0.6.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-06-20 15:50:59.000000 fx-bin-0.6.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-06-20 15:50:59.000000 fx-bin-0.6.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-20 15:50:59.000000 fx-bin-0.6.0/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-20 15:50:59.000000 fx-bin-0.6.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:51:04.160736 fx-bin-0.6.0/fx_bin/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-20 15:50:59.000000 fx-bin-0.6.0/fx_bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-20 15:50:59.000000 fx-bin-0.6.0/fx_bin/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-06-20 15:50:59.000000 fx-bin-0.6.0/fx_bin/files.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-20 15:50:59.000000 fx-bin-0.6.0/fx_bin/find_files.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-06-20 15:50:59.000000 fx-bin-0.6.0/fx_bin/lib.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-06-20 15:50:59.000000 fx-bin-0.6.0/fx_bin/pd.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-20 15:50:59.000000 fx-bin-0.6.0/fx_bin/py_fx_bin.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-20 15:50:59.000000 fx-bin-0.6.0/fx_bin/replace.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-20 15:50:59.000000 fx-bin-0.6.0/fx_bin/run_upgrade_program.py
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-06-20 15:50:59.000000 fx-bin-0.6.0/fx_bin/size.py
--rw-r--r--   0 runner    (1001) docker     (123)    12017 2023-06-20 15:50:59.000000 fx-bin-0.6.0/fx_bin/upload_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:51:04.160736 fx-bin-0.6.0/fx_bin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-06-20 15:51:04.000000 fx-bin-0.6.0/fx_bin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-20 15:51:04.000000 fx-bin-0.6.0/fx_bin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 15:51:04.000000 fx-bin-0.6.0/fx_bin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-20 15:51:04.000000 fx-bin-0.6.0/fx_bin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 15:51:04.000000 fx-bin-0.6.0/fx_bin.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-20 15:51:04.000000 fx-bin-0.6.0/fx_bin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-20 15:51:04.000000 fx-bin-0.6.0/fx_bin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-20 15:50:59.000000 fx-bin-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-20 15:51:04.164736 fx-bin-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-06-20 15:50:59.000000 fx-bin-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:51:04.160736 fx-bin-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-20 15:50:59.000000 fx-bin-0.6.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-06-20 15:50:59.000000 fx-bin-0.6.0/tests/test_py_fx_bin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:02:17.318732 fx-bin-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-06-20 16:02:14.000000 fx-bin-0.6.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-20 16:02:14.000000 fx-bin-0.6.1/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-20 16:02:14.000000 fx-bin-0.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-20 16:02:17.318732 fx-bin-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-20 16:02:14.000000 fx-bin-0.6.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:02:17.314732 fx-bin-0.6.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-20 16:02:14.000000 fx-bin-0.6.1/docs/Makefile
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4845 2023-06-20 16:02:14.000000 fx-bin-0.6.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-20 16:02:14.000000 fx-bin-0.6.1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-20 16:02:14.000000 fx-bin-0.6.1/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-20 16:02:14.000000 fx-bin-0.6.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-06-20 16:02:14.000000 fx-bin-0.6.1/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-06-20 16:02:14.000000 fx-bin-0.6.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-20 16:02:14.000000 fx-bin-0.6.1/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-20 16:02:14.000000 fx-bin-0.6.1/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:02:17.314732 fx-bin-0.6.1/fx_bin/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-20 16:02:14.000000 fx-bin-0.6.1/fx_bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-20 16:02:14.000000 fx-bin-0.6.1/fx_bin/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-06-20 16:02:14.000000 fx-bin-0.6.1/fx_bin/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-20 16:02:14.000000 fx-bin-0.6.1/fx_bin/find_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-06-20 16:02:14.000000 fx-bin-0.6.1/fx_bin/lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-06-20 16:02:14.000000 fx-bin-0.6.1/fx_bin/pd.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-20 16:02:14.000000 fx-bin-0.6.1/fx_bin/py_fx_bin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-20 16:02:14.000000 fx-bin-0.6.1/fx_bin/replace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-20 16:02:14.000000 fx-bin-0.6.1/fx_bin/run_upgrade_program.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-06-20 16:02:14.000000 fx-bin-0.6.1/fx_bin/size.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12017 2023-06-20 16:02:14.000000 fx-bin-0.6.1/fx_bin/upload_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:02:17.318732 fx-bin-0.6.1/fx_bin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-20 16:02:17.000000 fx-bin-0.6.1/fx_bin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-20 16:02:17.000000 fx-bin-0.6.1/fx_bin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 16:02:17.000000 fx-bin-0.6.1/fx_bin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-20 16:02:17.000000 fx-bin-0.6.1/fx_bin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 16:02:17.000000 fx-bin-0.6.1/fx_bin.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-20 16:02:17.000000 fx-bin-0.6.1/fx_bin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-20 16:02:17.000000 fx-bin-0.6.1/fx_bin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-20 16:02:14.000000 fx-bin-0.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-20 16:02:17.318732 fx-bin-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-06-20 16:02:14.000000 fx-bin-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:02:17.318732 fx-bin-0.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-20 16:02:14.000000 fx-bin-0.6.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-06-20 16:02:14.000000 fx-bin-0.6.1/tests/test_py_fx_bin.py
```

### Comparing `fx-bin-0.6.0/CONTRIBUTING.rst` & `fx-bin-0.6.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `fx-bin-0.6.0/PKG-INFO` & `fx-bin-0.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,28 @@
 Metadata-Version: 2.1
 Name: fx-bin
-Version: 0.6.0
+Version: 0.6.1
 Summary: A common bin collection for my own usage
-Home-page: https://github.com/frankyxhl/py_fx_bin
+Home-page: https://github.com/frankyxhl/fx_bin
 Author: Frank Xu
 Author-email: frank@frankxu.me
 Keywords: fx_bin
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 
 =============
-Python FX bin
+FX bin
 =============
 
 
-
-
-
-
 A common bin collection for my own usage
 
 
 
 Features
 --------
```

### Comparing `fx-bin-0.6.0/docs/Makefile` & `fx-bin-0.6.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `fx-bin-0.6.0/docs/conf.py` & `fx-bin-0.6.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `fx-bin-0.6.0/docs/installation.rst` & `fx-bin-0.6.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `fx-bin-0.6.0/docs/make.bat` & `fx-bin-0.6.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `fx-bin-0.6.0/fx_bin/files.py` & `fx-bin-0.6.1/fx_bin/files.py`

 * *Files identical despite different names*

### Comparing `fx-bin-0.6.0/fx_bin/lib.py` & `fx-bin-0.6.1/fx_bin/lib.py`

 * *Files identical despite different names*

### Comparing `fx-bin-0.6.0/fx_bin/pd.py` & `fx-bin-0.6.1/fx_bin/pd.py`

 * *Files identical despite different names*

### Comparing `fx-bin-0.6.0/fx_bin/replace.py` & `fx-bin-0.6.1/fx_bin/replace.py`

 * *Files identical despite different names*

### Comparing `fx-bin-0.6.0/fx_bin/size.py` & `fx-bin-0.6.1/fx_bin/size.py`

 * *Files identical despite different names*

### Comparing `fx-bin-0.6.0/fx_bin/upload_server.py` & `fx-bin-0.6.1/fx_bin/upload_server.py`

 * *Files identical despite different names*

### Comparing `fx-bin-0.6.0/fx_bin.egg-info/PKG-INFO` & `fx-bin-0.6.1/fx_bin.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,28 @@
 Metadata-Version: 2.1
 Name: fx-bin
-Version: 0.6.0
+Version: 0.6.1
 Summary: A common bin collection for my own usage
-Home-page: https://github.com/frankyxhl/py_fx_bin
+Home-page: https://github.com/frankyxhl/fx_bin
 Author: Frank Xu
 Author-email: frank@frankxu.me
 Keywords: fx_bin
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 
 =============
-Python FX bin
+FX bin
 =============
 
 
-
-
-
-
 A common bin collection for my own usage
 
 
 
 Features
 --------
```

### Comparing `fx-bin-0.6.0/fx_bin.egg-info/SOURCES.txt` & `fx-bin-0.6.1/fx_bin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fx-bin-0.6.0/setup.py` & `fx-bin-0.6.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,11 +46,11 @@
     long_description=readme + '\n\n' + history,
     include_package_data=True,
     keywords='fx_bin',
     packages=find_packages(include=['fx_bin']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
-    url='https://github.com/frankyxhl/py_fx_bin',
-    version='0.6.0',
+    url='https://github.com/frankyxhl/fx_bin',
+    version='0.6.1',
     zip_safe=False,
 )
```

### Comparing `fx-bin-0.6.0/tests/test_py_fx_bin.py` & `fx-bin-0.6.1/tests/test_py_fx_bin.py`

 * *Files identical despite different names*

