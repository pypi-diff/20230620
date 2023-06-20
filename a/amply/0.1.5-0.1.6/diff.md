# Comparing `tmp/amply-0.1.5.tar.gz` & `tmp/amply-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amply-0.1.5.tar", last modified: Mon Apr 25 09:15:13 2022, max compression
+gzip compressed data, was "amply-0.1.6.tar", last modified: Tue Jun 20 15:42:57 2023, max compression
```

## Comparing `amply-0.1.5.tar` & `amply-0.1.6.tar`

### file list

```diff
@@ -1,27 +1,31 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-04-25 09:15:13.812560 amply-0.1.5/
--rw-rw-r--   0 travis    (2000) travis    (2000)       91 2022-04-25 09:13:14.000000 amply-0.1.5/.gitignore
--rw-rw-r--   0 travis    (2000) travis    (2000)      301 2022-04-25 09:13:14.000000 amply-0.1.5/.isort.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)      840 2022-04-25 09:13:14.000000 amply-0.1.5/.pre-commit-config.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)     1575 2022-04-25 09:13:14.000000 amply-0.1.5/.travis.yml
--rw-rw-r--   0 travis    (2000) travis    (2000)      233 2022-04-25 09:13:14.000000 amply-0.1.5/AUTHORS
--rw-rw-r--   0 travis    (2000) travis    (2000)      104 2022-04-25 09:13:14.000000 amply-0.1.5/INSTALL
--rw-rw-r--   0 travis    (2000) travis    (2000)    11320 2022-04-25 09:13:14.000000 amply-0.1.5/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)    15590 2022-04-25 09:15:13.812560 amply-0.1.5/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)    14786 2022-04-25 09:13:14.000000 amply-0.1.5/README.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      146 2022-04-25 09:13:14.000000 amply-0.1.5/pyproject.toml
--rw-rw-r--   0 travis    (2000) travis    (2000)       10 2022-04-25 09:13:14.000000 amply-0.1.5/requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2022-04-25 09:15:13.812560 amply-0.1.5/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1562 2022-04-25 09:13:14.000000 amply-0.1.5/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-04-25 09:15:13.812560 amply-0.1.5/src/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-04-25 09:15:13.812560 amply-0.1.5/src/amply/
--rw-rw-r--   0 travis    (2000) travis    (2000)       72 2022-04-25 09:13:14.000000 amply-0.1.5/src/amply/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22351 2022-04-25 09:13:14.000000 amply-0.1.5/src/amply/amply.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-04-25 09:15:13.812560 amply-0.1.5/src/amply.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)    15590 2022-04-25 09:15:13.000000 amply-0.1.5/src/amply.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      382 2022-04-25 09:15:13.000000 amply-0.1.5/src/amply.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2022-04-25 09:15:13.000000 amply-0.1.5/src/amply.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       24 2022-04-25 09:15:13.000000 amply-0.1.5/src/amply.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        6 2022-04-25 09:15:13.000000 amply-0.1.5/src/amply.egg-info/top_level.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-04-25 09:15:13.812560 amply-0.1.5/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)    21009 2022-04-25 09:13:14.000000 amply-0.1.5/tests/test_amply.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2220 2022-04-25 09:13:14.000000 amply-0.1.5/tests/travis_install.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:42:57.374627 amply-0.1.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:42:57.370627 amply-0.1.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:42:57.374627 amply-0.1.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-06-20 15:42:44.000000 amply-0.1.6/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-20 15:42:44.000000 amply-0.1.6/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-20 15:42:44.000000 amply-0.1.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-20 15:42:44.000000 amply-0.1.6/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-20 15:42:44.000000 amply-0.1.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-06-20 15:42:44.000000 amply-0.1.6/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-20 15:42:44.000000 amply-0.1.6/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-20 15:42:44.000000 amply-0.1.6/INSTALL
+-rw-r--r--   0 runner    (1001) docker     (123)    11320 2023-06-20 15:42:44.000000 amply-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15616 2023-06-20 15:42:57.374627 amply-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14832 2023-06-20 15:42:44.000000 amply-0.1.6/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-20 15:42:44.000000 amply-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-20 15:42:44.000000 amply-0.1.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 15:42:57.374627 amply-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-06-20 15:42:44.000000 amply-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:42:57.370627 amply-0.1.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:42:57.374627 amply-0.1.6/src/amply/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-20 15:42:44.000000 amply-0.1.6/src/amply/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22357 2023-06-20 15:42:44.000000 amply-0.1.6/src/amply/amply.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:42:57.374627 amply-0.1.6/src/amply.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15616 2023-06-20 15:42:57.000000 amply-0.1.6/src/amply.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-20 15:42:57.000000 amply-0.1.6/src/amply.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 15:42:57.000000 amply-0.1.6/src/amply.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-20 15:42:57.000000 amply-0.1.6/src/amply.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-20 15:42:57.000000 amply-0.1.6/src/amply.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:42:57.374627 amply-0.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    20994 2023-06-20 15:42:44.000000 amply-0.1.6/tests/test_amply.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-06-20 15:42:44.000000 amply-0.1.6/tests/travis_install.sh
```

### Comparing `amply-0.1.5/.pre-commit-config.yaml` & `amply-0.1.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `amply-0.1.5/.travis.yml` & `amply-0.1.6/.travis.yml`

 * *Files identical despite different names*

### Comparing `amply-0.1.5/LICENSE` & `amply-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `amply-0.1.5/PKG-INFO` & `amply-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: amply
-Version: 0.1.5
+Version: 0.1.6
 Summary: Amply allows you to load and manipulate AMPL/GLPK data as Python data structures
 Home-page: http://github.com/willu47/amply
 Author: Will Usher,Christophe-Marie Duquesne,Stuart Mitchell,Franco Peschiera,Stu,smit023,Q. Lim
 Author-email: wusher@kth.se
 License: Eclipse Public License 1.0 (EPL-1.0)
 Project-URL: Bug Tracker, http://github.com/willu47/amply/issues
 Project-URL: Documentation, http://github.com/willu47/amply/README.rst
 Project-URL: Source Code, http://github.com/willu47/amply
 Keywords: ampl gmpl
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Eclipse Public License 1.0 (EPL-1.0)
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS
 
 Amply
 ======
 
 .. image:: https://travis-ci.com/willu47/amply.svg?branch=master
     :target: https://travis-ci.com/willu47/amply
 .. image:: https://img.shields.io/pypi/v/amply?style=plastic
      :alt: PyPI
+     :target: https://pypi.org/project/amply/
 .. image:: https://coveralls.io/repos/github/willu47/amply/badge.svg?branch=master
     :target: https://coveralls.io/github/willu47/amply?branch=master
 
 
 Introduction
 ------------
 
@@ -516,9 +516,7 @@
     ~~~~~~~~~~~~~~
 
 Development Notes
 -----------------
 
 Many thanks to Johannes Ragam (@thet), former custodian of the "amply" project on PyPi.
 Johannes graciously transferred the project to this. Thanks!
-
-
```

### Comparing `amply-0.1.5/README.rst` & `amply-0.1.6/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Amply
 ======
 
 .. image:: https://travis-ci.com/willu47/amply.svg?branch=master
     :target: https://travis-ci.com/willu47/amply
 .. image:: https://img.shields.io/pypi/v/amply?style=plastic
      :alt: PyPI
+     :target: https://pypi.org/project/amply/
 .. image:: https://coveralls.io/repos/github/willu47/amply/badge.svg?branch=master
     :target: https://coveralls.io/github/willu47/amply?branch=master
 
 
 Introduction
 ------------
```

### Comparing `amply-0.1.5/setup.py` & `amply-0.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `amply-0.1.5/src/amply/amply.py` & `amply-0.1.6/src/amply/amply.py`

 * *Files 0% similar despite different names*

```diff
@@ -606,15 +606,15 @@
     tokens[0].setTransposed(True)
     return tokens
 
 
 # What follows is a Pyparsing description of the grammar
 
 index = Word(alphanums, exact=1)
-symbol = Word(alphanums, bodyChars=alphanums + "_", min=1)
+symbol = Word(alphanums + "_", bodyChars=alphanums + "_", min=1)
 sign = Optional(oneOf("+ -"))
 integer = Combine(sign + Word(nums)).setParseAction(lambda t: int(t[0]))
 number = Combine(
     Word("+-" + nums, nums)
     + Optional("." + Optional(Word(nums)))
     + Optional(oneOf("e E") + Word("+-" + nums, nums))
 ).setParseAction(lambda t: float(t[0]))
```

### Comparing `amply-0.1.5/src/amply.egg-info/PKG-INFO` & `amply-0.1.6/src/amply.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: amply
-Version: 0.1.5
+Version: 0.1.6
 Summary: Amply allows you to load and manipulate AMPL/GLPK data as Python data structures
 Home-page: http://github.com/willu47/amply
 Author: Will Usher,Christophe-Marie Duquesne,Stuart Mitchell,Franco Peschiera,Stu,smit023,Q. Lim
 Author-email: wusher@kth.se
 License: Eclipse Public License 1.0 (EPL-1.0)
 Project-URL: Bug Tracker, http://github.com/willu47/amply/issues
 Project-URL: Documentation, http://github.com/willu47/amply/README.rst
 Project-URL: Source Code, http://github.com/willu47/amply
 Keywords: ampl gmpl
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Eclipse Public License 1.0 (EPL-1.0)
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS
 
 Amply
 ======
 
 .. image:: https://travis-ci.com/willu47/amply.svg?branch=master
     :target: https://travis-ci.com/willu47/amply
 .. image:: https://img.shields.io/pypi/v/amply?style=plastic
      :alt: PyPI
+     :target: https://pypi.org/project/amply/
 .. image:: https://coveralls.io/repos/github/willu47/amply/badge.svg?branch=master
     :target: https://coveralls.io/github/willu47/amply?branch=master
 
 
 Introduction
 ------------
 
@@ -516,9 +516,7 @@
     ~~~~~~~~~~~~~~
 
 Development Notes
 -----------------
 
 Many thanks to Johannes Ragam (@thet), former custodian of the "amply" project on PyPi.
 Johannes graciously transferred the project to this. Thanks!
-
-
```

### Comparing `amply-0.1.5/tests/test_amply.py` & `amply-0.1.6/tests/test_amply.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
+import pytest
+
 import unittest
 from io import StringIO
 
-import pytest
-
 from amply import amply
 from amply.amply import (
     number,
     param_def_stmt,
     param_stmt,
     set_record,
     set_stmt,
@@ -75,15 +75,14 @@
 class TestSymbol:
     def test_not_symbol(self):
         fixture = """
         1.1
         0.234
         +1e-049
         skj!adfk
-        __12
         """
         result = symbol.runTests(fixture, failureTests=True)
         assert result[0]
 
     def test_symbol(self):
         fixture = """
         Jan
@@ -223,30 +222,30 @@
         result = amply.Amply("param T:= 4;").T
         assert result == 4
 
     def test_from_file(self):
         try:
             s = StringIO("param T:= 4;")
         except TypeError:
-            s = StringIO(u"param T:= 4;")
+            s = StringIO("param T:= 4;")
         assert amply.Amply.from_file(s).T == 4
 
     def test_load_string(self):
         a = amply.Amply("param T:= 4; param X{foo};")
         a.load_string("param S := 6; param X := 1 2;")
         assert a.T == 4
         assert a.S == 6
         assert a.X[1] == 2
 
     def test_load_file(self):
         a = amply.Amply("param T:= 4; param X{foo};")
         try:
             s = StringIO("param S := 6; param X := 1 2;")
         except TypeError:
-            s = StringIO(u"param S := 6; param X := 1 2;")
+            s = StringIO("param S := 6; param X := 1 2;")
         a.load_file(s)
         assert a.T == 4
         assert a.S == 6
         assert a.X[1] == 2
 
     def test_empty_init(self):
         a = amply.Amply()
```

### Comparing `amply-0.1.5/tests/travis_install.sh` & `amply-0.1.6/tests/travis_install.sh`

 * *Files identical despite different names*

