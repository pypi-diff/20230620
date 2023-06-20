# Comparing `tmp/pysna-0.1.0.tar.gz` & `tmp/pysna-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysna-0.1.0.tar", last modified: Wed Mar 15 14:10:33 2023, max compression
+gzip compressed data, was "pysna-0.1.1.tar", last modified: Tue Jun 20 09:10:48 2023, max compression
```

## Comparing `pysna-0.1.0.tar` & `pysna-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-03-15 14:10:33.614472 pysna-0.1.0/
--rw-rw-rw-   0        0        0     1084 2022-12-21 10:40:25.000000 pysna-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     4038 2023-03-15 14:10:33.605832 pysna-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-03-15 14:10:33.510204 pysna-0.1.0/PySNA.egg-info/
--rw-rw-rw-   0        0        0     4038 2023-03-15 14:10:33.000000 pysna-0.1.0/PySNA.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      549 2023-03-15 14:10:33.000000 pysna-0.1.0/PySNA.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-15 14:10:33.000000 pysna-0.1.0/PySNA.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-03-15 14:10:33.000000 pysna-0.1.0/PySNA.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      103 2023-03-15 14:10:33.000000 pysna-0.1.0/PySNA.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-03-15 14:10:33.000000 pysna-0.1.0/PySNA.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3513 2023-03-15 13:51:55.000000 pysna-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-03-15 14:10:33.559023 pysna-0.1.0/pysna/
--rw-rw-rw-   0        0        0      383 2023-03-15 14:10:04.000000 pysna-0.1.0/pysna/__init__.py
--rw-rw-rw-   0        0        0    32340 2023-02-23 14:25:50.000000 pysna-0.1.0/pysna/api.py
--rw-rw-rw-   0        0        0    14055 2023-03-15 13:49:38.000000 pysna-0.1.0/pysna/cli.py
--rw-rw-rw-   0        0        0    21580 2023-03-15 13:49:38.000000 pysna-0.1.0/pysna/fetch.py
--rw-rw-rw-   0        0        0    12947 2023-03-15 13:49:38.000000 pysna-0.1.0/pysna/process.py
--rw-rw-rw-   0        0        0    11279 2023-03-15 13:51:05.000000 pysna-0.1.0/pysna/utils.py
--rw-rw-rw-   0        0        0       42 2023-03-15 14:10:33.615428 pysna-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1583 2023-03-14 20:31:07.000000 pysna-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-15 14:10:33.596279 pysna-0.1.0/tests/
--rw-rw-rw-   0        0        0     2510 2023-03-10 16:55:23.000000 pysna-0.1.0/tests/test_api.py
--rw-rw-rw-   0        0        0    18072 2023-03-10 17:02:53.000000 pysna-0.1.0/tests/test_fetch.py
--rw-rw-rw-   0        0        0     8254 2023-02-23 15:33:31.000000 pysna-0.1.0/tests/test_process.py
--rw-rw-rw-   0        0        0     1083 2023-02-19 17:05:43.000000 pysna-0.1.0/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-20 09:10:48.703758 pysna-0.1.1/
+-rw-rw-rw-   0        0        0     1084 2022-12-21 10:40:25.000000 pysna-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     4138 2023-06-20 09:10:48.703758 pysna-0.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-20 09:10:48.656481 pysna-0.1.1/PySNA.egg-info/
+-rw-rw-rw-   0        0        0     4138 2023-06-20 09:10:48.000000 pysna-0.1.1/PySNA.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      549 2023-06-20 09:10:48.000000 pysna-0.1.1/PySNA.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 09:10:48.000000 pysna-0.1.1/PySNA.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-06-20 09:10:48.000000 pysna-0.1.1/PySNA.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      103 2023-06-20 09:10:48.000000 pysna-0.1.1/PySNA.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-20 09:10:48.000000 pysna-0.1.1/PySNA.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3613 2023-03-15 14:43:39.000000 pysna-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-20 09:10:48.672098 pysna-0.1.1/pysna/
+-rw-rw-rw-   0        0        0      383 2023-06-20 09:05:39.000000 pysna-0.1.1/pysna/__init__.py
+-rw-rw-rw-   0        0        0    32340 2023-02-23 14:25:50.000000 pysna-0.1.1/pysna/api.py
+-rw-rw-rw-   0        0        0    14055 2023-03-15 13:49:38.000000 pysna-0.1.1/pysna/cli.py
+-rw-rw-rw-   0        0        0    21580 2023-03-15 13:49:38.000000 pysna-0.1.1/pysna/fetch.py
+-rw-rw-rw-   0        0        0    12947 2023-03-15 13:49:38.000000 pysna-0.1.1/pysna/process.py
+-rw-rw-rw-   0        0        0    11279 2023-03-15 13:51:05.000000 pysna-0.1.1/pysna/utils.py
+-rw-rw-rw-   0        0        0       42 2023-06-20 09:10:48.703758 pysna-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1583 2023-03-14 20:31:07.000000 pysna-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 09:10:48.703758 pysna-0.1.1/tests/
+-rw-rw-rw-   0        0        0     2510 2023-03-10 16:55:23.000000 pysna-0.1.1/tests/test_api.py
+-rw-rw-rw-   0        0        0    18072 2023-03-10 17:02:53.000000 pysna-0.1.1/tests/test_fetch.py
+-rw-rw-rw-   0        0        0     8254 2023-02-23 15:33:31.000000 pysna-0.1.1/tests/test_process.py
+-rw-rw-rw-   0        0        0     1083 2023-02-19 17:05:43.000000 pysna-0.1.1/tests/test_utils.py
```

### Comparing `pysna-0.1.0/LICENSE` & `pysna-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pysna-0.1.0/PKG-INFO` & `pysna-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: pysna
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python Package for Social Network Analytics
 Home-page: https://github.com/mathun3003/PySNA
 Author: Mathis Hunke
 Author-email: mathun3003@gmail.com
 License: MIT License
 Project-URL: Documentation, https://mathun3003.github.io/PySNA/
 Project-URL: Issue Tracker, https://github.com/mathun3003/PySNA/issues
 Project-URL: Source Code, https://github.com/mathun3003/PySNA
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PySNA
 
+[![PyPI Version](https://img.shields.io/pypi/v/pysna?label=PyPI)](https://pypi.org/project/pysna/)
 [![Twitter API v1.1](https://img.shields.io/endpoint?url=https%3A%2F%2Ftwbadges.glitch.me%2Fbadges%2Fstandard)](https://developer.twitter.com/en/docs/twitter-api/v1)
 [![Twitter API v2](https://img.shields.io/endpoint?url=https%3A%2F%2Ftwbadges.glitch.me%2Fbadges%2Fv2)](https://developer.twitter.com/en/docs/twitter-api)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 
 
 Python Package for Social Network Analytics
```

### Comparing `pysna-0.1.0/PySNA.egg-info/PKG-INFO` & `pysna-0.1.1/PySNA.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: pysna
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python Package for Social Network Analytics
 Home-page: https://github.com/mathun3003/PySNA
 Author: Mathis Hunke
 Author-email: mathun3003@gmail.com
 License: MIT License
 Project-URL: Documentation, https://mathun3003.github.io/PySNA/
 Project-URL: Issue Tracker, https://github.com/mathun3003/PySNA/issues
 Project-URL: Source Code, https://github.com/mathun3003/PySNA
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PySNA
 
+[![PyPI Version](https://img.shields.io/pypi/v/pysna?label=PyPI)](https://pypi.org/project/pysna/)
 [![Twitter API v1.1](https://img.shields.io/endpoint?url=https%3A%2F%2Ftwbadges.glitch.me%2Fbadges%2Fstandard)](https://developer.twitter.com/en/docs/twitter-api/v1)
 [![Twitter API v2](https://img.shields.io/endpoint?url=https%3A%2F%2Ftwbadges.glitch.me%2Fbadges%2Fv2)](https://developer.twitter.com/en/docs/twitter-api)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 
 
 Python Package for Social Network Analytics
```

### Comparing `pysna-0.1.0/PySNA.egg-info/SOURCES.txt` & `pysna-0.1.1/PySNA.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pysna-0.1.0/README.md` & `pysna-0.1.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # PySNA
 
+[![PyPI Version](https://img.shields.io/pypi/v/pysna?label=PyPI)](https://pypi.org/project/pysna/)
 [![Twitter API v1.1](https://img.shields.io/endpoint?url=https%3A%2F%2Ftwbadges.glitch.me%2Fbadges%2Fstandard)](https://developer.twitter.com/en/docs/twitter-api/v1)
 [![Twitter API v2](https://img.shields.io/endpoint?url=https%3A%2F%2Ftwbadges.glitch.me%2Fbadges%2Fv2)](https://developer.twitter.com/en/docs/twitter-api)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 
 
 Python Package for Social Network Analytics
```

### Comparing `pysna-0.1.0/pysna/api.py` & `pysna-0.1.1/pysna/api.py`

 * *Files identical despite different names*

### Comparing `pysna-0.1.0/pysna/cli.py` & `pysna-0.1.1/pysna/cli.py`

 * *Files identical despite different names*

### Comparing `pysna-0.1.0/pysna/fetch.py` & `pysna-0.1.1/pysna/fetch.py`

 * *Files identical despite different names*

### Comparing `pysna-0.1.0/pysna/process.py` & `pysna-0.1.1/pysna/process.py`

 * *Files identical despite different names*

### Comparing `pysna-0.1.0/pysna/utils.py` & `pysna-0.1.1/pysna/utils.py`

 * *Files identical despite different names*

### Comparing `pysna-0.1.0/setup.py` & `pysna-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `pysna-0.1.0/tests/test_api.py` & `pysna-0.1.1/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `pysna-0.1.0/tests/test_fetch.py` & `pysna-0.1.1/tests/test_fetch.py`

 * *Files identical despite different names*

### Comparing `pysna-0.1.0/tests/test_process.py` & `pysna-0.1.1/tests/test_process.py`

 * *Files identical despite different names*

### Comparing `pysna-0.1.0/tests/test_utils.py` & `pysna-0.1.1/tests/test_utils.py`

 * *Files identical despite different names*

