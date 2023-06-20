# Comparing `tmp/dbfpy3-4.2.1.tar.gz` & `tmp/dbfpy3-4.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbfpy3-4.2.1.tar", last modified: Tue Jun 20 15:33:09 2023, max compression
+gzip compressed data, was "dbfpy3-4.2.2.tar", last modified: Tue Jun 20 15:40:18 2023, max compression
```

## Comparing `dbfpy3-4.2.1.tar` & `dbfpy3-4.2.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:33:09.359517 dbfpy3-4.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-06-20 15:33:06.000000 dbfpy3-4.2.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-20 15:33:06.000000 dbfpy3-4.2.1/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-20 15:33:06.000000 dbfpy3-4.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-20 15:33:06.000000 dbfpy3-4.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-06-20 15:33:09.359517 dbfpy3-4.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-20 15:33:06.000000 dbfpy3-4.2.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:33:09.355517 dbfpy3-4.2.1/dbfpy3/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-20 15:33:06.000000 dbfpy3-4.2.1/dbfpy3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-06-20 15:33:06.000000 dbfpy3-4.2.1/dbfpy3/code_page.py
--rw-r--r--   0 runner    (1001) docker     (123)     7842 2023-06-20 15:33:06.000000 dbfpy3-4.2.1/dbfpy3/dbf.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-20 15:33:06.000000 dbfpy3-4.2.1/dbfpy3/dbfpy3.py
--rw-r--r--   0 runner    (1001) docker     (123)    15444 2023-06-20 15:33:06.000000 dbfpy3-4.2.1/dbfpy3/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)    12528 2023-06-20 15:33:06.000000 dbfpy3-4.2.1/dbfpy3/header.py
--rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-06-20 15:33:06.000000 dbfpy3-4.2.1/dbfpy3/memo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-06-20 15:33:06.000000 dbfpy3-4.2.1/dbfpy3/record.py
--rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-06-20 15:33:06.000000 dbfpy3-4.2.1/dbfpy3/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:33:09.355517 dbfpy3-4.2.1/dbfpy3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-06-20 15:33:09.000000 dbfpy3-4.2.1/dbfpy3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-20 15:33:09.000000 dbfpy3-4.2.1/dbfpy3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 15:33:09.000000 dbfpy3-4.2.1/dbfpy3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 15:33:09.000000 dbfpy3-4.2.1/dbfpy3.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-20 15:33:09.000000 dbfpy3-4.2.1/dbfpy3.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:33:09.355517 dbfpy3-4.2.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-20 15:33:06.000000 dbfpy3-4.2.1/docs/Makefile
--rwxr-xr-x   0 runner    (1001) docker     (123)     4753 2023-06-20 15:33:06.000000 dbfpy3-4.2.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-20 15:33:06.000000 dbfpy3-4.2.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-20 15:33:06.000000 dbfpy3-4.2.1/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-20 15:33:06.000000 dbfpy3-4.2.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-06-20 15:33:06.000000 dbfpy3-4.2.1/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-20 15:33:06.000000 dbfpy3-4.2.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-20 15:33:06.000000 dbfpy3-4.2.1/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-20 15:33:06.000000 dbfpy3-4.2.1/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-20 15:33:09.359517 dbfpy3-4.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-06-20 15:33:06.000000 dbfpy3-4.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:33:09.359517 dbfpy3-4.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-20 15:33:06.000000 dbfpy3-4.2.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-20 15:33:06.000000 dbfpy3-4.2.1/tests/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-20 15:33:06.000000 dbfpy3-4.2.1/tests/test_code_page.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-20 15:33:06.000000 dbfpy3-4.2.1/tests/test_dbfpy3.py
--rw-r--r--   0 runner    (1001) docker     (123)     6924 2023-06-20 15:33:06.000000 dbfpy3-4.2.1/tests/test_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-20 15:33:06.000000 dbfpy3-4.2.1/tests/test_memo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:40:18.905281 dbfpy3-4.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-06-20 15:40:15.000000 dbfpy3-4.2.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-20 15:40:15.000000 dbfpy3-4.2.2/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-20 15:40:15.000000 dbfpy3-4.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-20 15:40:15.000000 dbfpy3-4.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-06-20 15:40:18.905281 dbfpy3-4.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-20 15:40:15.000000 dbfpy3-4.2.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:40:18.901281 dbfpy3-4.2.2/dbfpy3/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-20 15:40:15.000000 dbfpy3-4.2.2/dbfpy3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-06-20 15:40:15.000000 dbfpy3-4.2.2/dbfpy3/code_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7842 2023-06-20 15:40:15.000000 dbfpy3-4.2.2/dbfpy3/dbf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-20 15:40:15.000000 dbfpy3-4.2.2/dbfpy3/dbfpy3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15444 2023-06-20 15:40:15.000000 dbfpy3-4.2.2/dbfpy3/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12528 2023-06-20 15:40:15.000000 dbfpy3-4.2.2/dbfpy3/header.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-06-20 15:40:15.000000 dbfpy3-4.2.2/dbfpy3/memo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-06-20 15:40:15.000000 dbfpy3-4.2.2/dbfpy3/record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-06-20 15:40:15.000000 dbfpy3-4.2.2/dbfpy3/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:40:18.901281 dbfpy3-4.2.2/dbfpy3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-06-20 15:40:18.000000 dbfpy3-4.2.2/dbfpy3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-20 15:40:18.000000 dbfpy3-4.2.2/dbfpy3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 15:40:18.000000 dbfpy3-4.2.2/dbfpy3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 15:40:18.000000 dbfpy3-4.2.2/dbfpy3.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-20 15:40:18.000000 dbfpy3-4.2.2/dbfpy3.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:40:18.905281 dbfpy3-4.2.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-20 15:40:15.000000 dbfpy3-4.2.2/docs/Makefile
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4753 2023-06-20 15:40:15.000000 dbfpy3-4.2.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-20 15:40:15.000000 dbfpy3-4.2.2/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-20 15:40:15.000000 dbfpy3-4.2.2/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-20 15:40:15.000000 dbfpy3-4.2.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-06-20 15:40:15.000000 dbfpy3-4.2.2/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-20 15:40:15.000000 dbfpy3-4.2.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-20 15:40:15.000000 dbfpy3-4.2.2/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-20 15:40:15.000000 dbfpy3-4.2.2/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-20 15:40:18.905281 dbfpy3-4.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-06-20 15:40:15.000000 dbfpy3-4.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:40:18.905281 dbfpy3-4.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-20 15:40:15.000000 dbfpy3-4.2.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-20 15:40:15.000000 dbfpy3-4.2.2/tests/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-20 15:40:15.000000 dbfpy3-4.2.2/tests/test_code_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-20 15:40:15.000000 dbfpy3-4.2.2/tests/test_dbfpy3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6924 2023-06-20 15:40:15.000000 dbfpy3-4.2.2/tests/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-20 15:40:15.000000 dbfpy3-4.2.2/tests/test_memo.py
```

### Comparing `dbfpy3-4.2.1/CONTRIBUTING.rst` & `dbfpy3-4.2.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dbfpy3-4.2.1/LICENSE` & `dbfpy3-4.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dbfpy3-4.2.1/PKG-INFO` & `dbfpy3-4.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbfpy3
-Version: 4.2.1
+Version: 4.2.2
 Summary: Port to Python 3. Dbfpy is a python-only module for reading and writing DBF-files.
 Home-page: https://github.com/frankyxhl/dbfpy3
 Author: Frank Xu
 Author-email: franky.xhl@gmail.com
 License: MIT license
 Keywords: dbfpy3
 Classifier: Intended Audience :: Developers
```

### Comparing `dbfpy3-4.2.1/README.rst` & `dbfpy3-4.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `dbfpy3-4.2.1/dbfpy3/code_page.py` & `dbfpy3-4.2.2/dbfpy3/code_page.py`

 * *Files identical despite different names*

### Comparing `dbfpy3-4.2.1/dbfpy3/dbf.py` & `dbfpy3-4.2.2/dbfpy3/dbf.py`

 * *Files identical despite different names*

### Comparing `dbfpy3-4.2.1/dbfpy3/fields.py` & `dbfpy3-4.2.2/dbfpy3/fields.py`

 * *Files identical despite different names*

### Comparing `dbfpy3-4.2.1/dbfpy3/header.py` & `dbfpy3-4.2.2/dbfpy3/header.py`

 * *Files identical despite different names*

### Comparing `dbfpy3-4.2.1/dbfpy3/memo.py` & `dbfpy3-4.2.2/dbfpy3/memo.py`

 * *Files identical despite different names*

### Comparing `dbfpy3-4.2.1/dbfpy3/record.py` & `dbfpy3-4.2.2/dbfpy3/record.py`

 * *Files identical despite different names*

### Comparing `dbfpy3-4.2.1/dbfpy3/utils.py` & `dbfpy3-4.2.2/dbfpy3/utils.py`

 * *Files identical despite different names*

### Comparing `dbfpy3-4.2.1/dbfpy3.egg-info/PKG-INFO` & `dbfpy3-4.2.2/dbfpy3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbfpy3
-Version: 4.2.1
+Version: 4.2.2
 Summary: Port to Python 3. Dbfpy is a python-only module for reading and writing DBF-files.
 Home-page: https://github.com/frankyxhl/dbfpy3
 Author: Frank Xu
 Author-email: franky.xhl@gmail.com
 License: MIT license
 Keywords: dbfpy3
 Classifier: Intended Audience :: Developers
```

### Comparing `dbfpy3-4.2.1/dbfpy3.egg-info/SOURCES.txt` & `dbfpy3-4.2.2/dbfpy3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbfpy3-4.2.1/docs/Makefile` & `dbfpy3-4.2.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dbfpy3-4.2.1/docs/conf.py` & `dbfpy3-4.2.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dbfpy3-4.2.1/docs/installation.rst` & `dbfpy3-4.2.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `dbfpy3-4.2.1/docs/make.bat` & `dbfpy3-4.2.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dbfpy3-4.2.1/setup.py` & `dbfpy3-4.2.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -42,10 +42,10 @@
     keywords='dbfpy3',
     name='dbfpy3',
     packages=find_packages(include=['dbfpy3', 'dbfpy3.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/frankyxhl/dbfpy3',
-    version='4.2.1',
+    version='4.2.2',
     zip_safe=False,
 )
```

### Comparing `dbfpy3-4.2.1/tests/test_code_page.py` & `dbfpy3-4.2.2/tests/test_code_page.py`

 * *Files identical despite different names*

### Comparing `dbfpy3-4.2.1/tests/test_fields.py` & `dbfpy3-4.2.2/tests/test_fields.py`

 * *Files identical despite different names*

