# Comparing `tmp/nanolsap-0.0.1.tar.gz` & `tmp/nanolsap-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanolsap-0.0.1.tar", last modified: Tue Jun 20 12:30:11 2023, max compression
+gzip compressed data, was "nanolsap-0.1.0.tar", last modified: Tue Jun 20 12:41:32 2023, max compression
```

## Comparing `nanolsap-0.0.1.tar` & `nanolsap-0.1.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 hz        (1000) hz        (1000)        0 2023-06-20 12:30:11.875722 nanolsap-0.0.1/
-drwxrwxr-x   0 hz        (1000) hz        (1000)        0 2023-06-20 12:30:11.871722 nanolsap-0.0.1/.github/
-drwxrwxr-x   0 hz        (1000) hz        (1000)        0 2023-06-20 12:30:11.871722 nanolsap-0.0.1/.github/workflows/
--rw-rw-r--   0 hz        (1000) hz        (1000)     1813 2023-06-20 11:57:55.000000 nanolsap-0.0.1/.github/workflows/python-publish.yml
--rw-rw-r--   0 hz        (1000) hz        (1000)     3078 2023-06-18 09:37:25.000000 nanolsap-0.0.1/.gitignore
--rw-rw-r--   0 hz        (1000) hz        (1000)     1494 2023-06-18 09:37:25.000000 nanolsap-0.0.1/LICENSE
--rw-rw-r--   0 hz        (1000) hz        (1000)     3607 2023-06-20 12:30:11.875722 nanolsap-0.0.1/PKG-INFO
--rw-rw-r--   0 hz        (1000) hz        (1000)     3032 2023-06-20 09:06:56.000000 nanolsap-0.0.1/README.md
--rw-rw-r--   0 hz        (1000) hz        (1000)     1158 2023-06-20 11:45:29.000000 nanolsap-0.0.1/pyproject.toml
--rw-rw-r--   0 hz        (1000) hz        (1000)       75 2023-06-20 12:30:11.875722 nanolsap-0.0.1/setup.cfg
--rw-rw-r--   0 hz        (1000) hz        (1000)     1154 2023-06-18 11:51:40.000000 nanolsap-0.0.1/setup.py
-drwxrwxr-x   0 hz        (1000) hz        (1000)        0 2023-06-20 12:30:11.871722 nanolsap-0.0.1/src/
-drwxrwxr-x   0 hz        (1000) hz        (1000)        0 2023-06-20 12:30:11.871722 nanolsap-0.0.1/src/nanolsap/
--rw-rw-r--   0 hz        (1000) hz        (1000)       84 2023-06-18 13:17:04.000000 nanolsap-0.0.1/src/nanolsap/__init__.py
--rw-rw-r--   0 hz        (1000) hz        (1000)    10488 2023-06-19 11:26:00.000000 nanolsap-0.0.1/src/nanolsap/_lsap.c
--rw-rw-r--   0 hz        (1000) hz        (1000)      305 2023-06-19 00:42:14.000000 nanolsap-0.0.1/src/nanolsap/_lsap.pyi
--rw-rw-r--   0 hz        (1000) hz        (1000)        0 2023-06-19 00:50:46.000000 nanolsap-0.0.1/src/nanolsap/py.typed
-drwxrwxr-x   0 hz        (1000) hz        (1000)        0 2023-06-20 12:30:11.875722 nanolsap-0.0.1/src/nanolsap/rectangular_lsap/
--rw-rw-r--   0 hz        (1000) hz        (1000)    12229 2023-06-20 11:36:31.000000 nanolsap-0.0.1/src/nanolsap/rectangular_lsap/rectangular_lsap.cpp
--rw-rw-r--   0 hz        (1000) hz        (1000)     2510 2023-06-18 23:03:33.000000 nanolsap-0.0.1/src/nanolsap/rectangular_lsap/rectangular_lsap.h
-drwxrwxr-x   0 hz        (1000) hz        (1000)        0 2023-06-20 12:30:11.871722 nanolsap-0.0.1/src/nanolsap.egg-info/
--rw-rw-r--   0 hz        (1000) hz        (1000)     3607 2023-06-20 12:30:11.000000 nanolsap-0.0.1/src/nanolsap.egg-info/PKG-INFO
--rw-rw-r--   0 hz        (1000) hz        (1000)      545 2023-06-20 12:30:11.000000 nanolsap-0.0.1/src/nanolsap.egg-info/SOURCES.txt
--rw-rw-r--   0 hz        (1000) hz        (1000)        1 2023-06-20 12:30:11.000000 nanolsap-0.0.1/src/nanolsap.egg-info/dependency_links.txt
--rw-rw-r--   0 hz        (1000) hz        (1000)       60 2023-06-20 12:30:11.000000 nanolsap-0.0.1/src/nanolsap.egg-info/requires.txt
--rw-rw-r--   0 hz        (1000) hz        (1000)        9 2023-06-20 12:30:11.000000 nanolsap-0.0.1/src/nanolsap.egg-info/top_level.txt
-drwxrwxr-x   0 hz        (1000) hz        (1000)        0 2023-06-20 12:30:11.875722 nanolsap-0.0.1/tests/
--rw-rw-r--   0 hz        (1000) hz        (1000)     4042 2023-06-20 12:04:54.000000 nanolsap-0.0.1/tests/test_linear_assignment.py
--rw-rw-r--   0 hz        (1000) hz        (1000)     2010 2023-06-19 06:34:44.000000 nanolsap-0.0.1/tests/test_solve.py
--rw-rw-r--   0 hz        (1000) hz        (1000)     1543 2023-06-19 09:13:03.000000 nanolsap-0.0.1/tests/test_subrowcol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:41:32.255155 nanolsap-0.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:41:32.251155 nanolsap-0.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:41:32.255155 nanolsap-0.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-06-20 12:41:15.000000 nanolsap-0.1.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-06-20 12:41:15.000000 nanolsap-0.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-20 12:41:15.000000 nanolsap-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-06-20 12:41:32.255155 nanolsap-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-06-20 12:41:15.000000 nanolsap-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-06-20 12:41:15.000000 nanolsap-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-20 12:41:32.259155 nanolsap-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-20 12:41:15.000000 nanolsap-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:41:32.251155 nanolsap-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:41:32.255155 nanolsap-0.1.0/src/nanolsap/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-20 12:41:15.000000 nanolsap-0.1.0/src/nanolsap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10488 2023-06-20 12:41:15.000000 nanolsap-0.1.0/src/nanolsap/_lsap.c
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-20 12:41:15.000000 nanolsap-0.1.0/src/nanolsap/_lsap.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 12:41:15.000000 nanolsap-0.1.0/src/nanolsap/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:41:32.255155 nanolsap-0.1.0/src/nanolsap/rectangular_lsap/
+-rw-r--r--   0 runner    (1001) docker     (123)    12229 2023-06-20 12:41:15.000000 nanolsap-0.1.0/src/nanolsap/rectangular_lsap/rectangular_lsap.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-06-20 12:41:15.000000 nanolsap-0.1.0/src/nanolsap/rectangular_lsap/rectangular_lsap.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:41:32.255155 nanolsap-0.1.0/src/nanolsap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-06-20 12:41:32.000000 nanolsap-0.1.0/src/nanolsap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-20 12:41:32.000000 nanolsap-0.1.0/src/nanolsap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 12:41:32.000000 nanolsap-0.1.0/src/nanolsap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-20 12:41:32.000000 nanolsap-0.1.0/src/nanolsap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-20 12:41:32.000000 nanolsap-0.1.0/src/nanolsap.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:41:32.255155 nanolsap-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-06-20 12:41:15.000000 nanolsap-0.1.0/tests/test_linear_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-06-20 12:41:15.000000 nanolsap-0.1.0/tests/test_solve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-06-20 12:41:15.000000 nanolsap-0.1.0/tests/test_subrowcol.py
```

### Comparing `nanolsap-0.0.1/.github/workflows/python-publish.yml` & `nanolsap-0.1.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `nanolsap-0.0.1/.gitignore` & `nanolsap-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `nanolsap-0.0.1/LICENSE` & `nanolsap-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nanolsap-0.0.1/PKG-INFO` & `nanolsap-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanolsap
-Version: 0.0.1
+Version: 0.1.0
 Summary: Python module to solve the linear sum assignment problem (LSAP) low memory friendly
 Author-email: hzqmwne <huangzhengqmwne@sina.cn>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/hzqmwne/nanolsap
 Keywords: lsap,munkres,kuhn-munkres,linear sum assignment problem
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `nanolsap-0.0.1/README.md` & `nanolsap-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `nanolsap-0.0.1/pyproject.toml` & `nanolsap-0.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nanolsap-0.0.1/setup.py` & `nanolsap-0.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `nanolsap-0.0.1/src/nanolsap/_lsap.c` & `nanolsap-0.1.0/src/nanolsap/_lsap.c`

 * *Files identical despite different names*

### Comparing `nanolsap-0.0.1/src/nanolsap/rectangular_lsap/rectangular_lsap.cpp` & `nanolsap-0.1.0/src/nanolsap/rectangular_lsap/rectangular_lsap.cpp`

 * *Files identical despite different names*

### Comparing `nanolsap-0.0.1/src/nanolsap/rectangular_lsap/rectangular_lsap.h` & `nanolsap-0.1.0/src/nanolsap/rectangular_lsap/rectangular_lsap.h`

 * *Files identical despite different names*

### Comparing `nanolsap-0.0.1/src/nanolsap.egg-info/PKG-INFO` & `nanolsap-0.1.0/src/nanolsap.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanolsap
-Version: 0.0.1
+Version: 0.1.0
 Summary: Python module to solve the linear sum assignment problem (LSAP) low memory friendly
 Author-email: hzqmwne <huangzhengqmwne@sina.cn>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/hzqmwne/nanolsap
 Keywords: lsap,munkres,kuhn-munkres,linear sum assignment problem
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `nanolsap-0.0.1/src/nanolsap.egg-info/SOURCES.txt` & `nanolsap-0.1.0/src/nanolsap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nanolsap-0.0.1/tests/test_linear_assignment.py` & `nanolsap-0.1.0/tests/test_linear_assignment.py`

 * *Files identical despite different names*

### Comparing `nanolsap-0.0.1/tests/test_solve.py` & `nanolsap-0.1.0/tests/test_solve.py`

 * *Files identical despite different names*

### Comparing `nanolsap-0.0.1/tests/test_subrowcol.py` & `nanolsap-0.1.0/tests/test_subrowcol.py`

 * *Files identical despite different names*

