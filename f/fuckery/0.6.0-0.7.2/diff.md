# Comparing `tmp/fuckery-0.6.0.tar.gz` & `tmp/fuckery-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fuckery-0.6.0.tar", last modified: Sun Jan 22 21:07:37 2023, max compression
+gzip compressed data, was "fuckery-0.7.2.tar", last modified: Tue Jun 20 01:40:26 2023, max compression
```

## Comparing `fuckery-0.6.0.tar` & `fuckery-0.7.2.tar`

### file list

```diff
@@ -1,66 +1,29 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-01-22 21:07:37.789937 fuckery-0.6.0/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      200 2023-01-22 21:07:25.000000 fuckery-0.6.0/.bumpversion.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1856 2023-01-22 21:07:25.000000 fuckery-0.6.0/.cookiecutterrc
--rw-r--r--   0 circleci  (3434) circleci  (3434)      149 2023-01-22 21:07:25.000000 fuckery-0.6.0/.coveragerc
--rw-r--r--   0 circleci  (3434) circleci  (3434)      215 2023-01-22 21:07:25.000000 fuckery-0.6.0/.editorconfig
--rw-r--r--   0 circleci  (3434) circleci  (3434)       67 2023-01-22 21:07:25.000000 fuckery-0.6.0/AUTHORS.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2629 2023-01-22 21:07:25.000000 fuckery-0.6.0/CHANGELOG.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2853 2023-01-22 21:07:25.000000 fuckery-0.6.0/CONTRIBUTING.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1057 2023-01-22 21:07:25.000000 fuckery-0.6.0/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)      397 2023-01-22 21:07:25.000000 fuckery-0.6.0/MANIFEST.in
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4162 2023-01-22 21:07:37.789937 fuckery-0.6.0/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2919 2023-01-22 21:07:25.000000 fuckery-0.6.0/README.rst
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-01-22 21:07:37.789937 fuckery-0.6.0/docs/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       28 2023-01-22 21:07:25.000000 fuckery-0.6.0/docs/authors.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)       30 2023-01-22 21:07:25.000000 fuckery-0.6.0/docs/changelog.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1381 2023-01-22 21:07:25.000000 fuckery-0.6.0/docs/conf.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       33 2023-01-22 21:07:25.000000 fuckery-0.6.0/docs/contributing.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)      245 2023-01-22 21:07:25.000000 fuckery-0.6.0/docs/index.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)       87 2023-01-22 21:07:25.000000 fuckery-0.6.0/docs/installation.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)       27 2023-01-22 21:07:25.000000 fuckery-0.6.0/docs/readme.rst
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-01-22 21:07:37.789937 fuckery-0.6.0/docs/reference/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      124 2023-01-22 21:07:25.000000 fuckery-0.6.0/docs/reference/fuckery.cli.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)      142 2023-01-22 21:07:25.000000 fuckery-0.6.0/docs/reference/fuckery.constants.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)      124 2023-01-22 21:07:25.000000 fuckery-0.6.0/docs/reference/fuckery.exc.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)      133 2023-01-22 21:07:25.000000 fuckery-0.6.0/docs/reference/fuckery.memory.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)      133 2023-01-22 21:07:25.000000 fuckery-0.6.0/docs/reference/fuckery.parser.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)      254 2023-01-22 21:07:25.000000 fuckery-0.6.0/docs/reference/fuckery.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)      121 2023-01-22 21:07:25.000000 fuckery-0.6.0/docs/reference/fuckery.vm.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)       59 2023-01-22 21:07:25.000000 fuckery-0.6.0/docs/reference/index.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)       58 2023-01-22 21:07:25.000000 fuckery-0.6.0/docs/reference/modules.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)       34 2023-01-22 21:07:25.000000 fuckery-0.6.0/docs/requirements.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      109 2023-01-22 21:07:25.000000 fuckery-0.6.0/docs/spelling_wordlist.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      771 2023-01-22 21:07:25.000000 fuckery-0.6.0/docs/usage.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)      655 2023-01-22 21:07:37.793937 fuckery-0.6.0/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2895 2023-01-22 21:07:25.000000 fuckery-0.6.0/setup.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-01-22 21:07:37.785937 fuckery-0.6.0/src/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-01-22 21:07:37.789937 fuckery-0.6.0/src/fuckery/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      211 2023-01-22 21:07:25.000000 fuckery-0.6.0/src/fuckery/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      418 2023-01-22 21:07:25.000000 fuckery-0.6.0/src/fuckery/__main__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2582 2023-01-22 21:07:25.000000 fuckery-0.6.0/src/fuckery/cli.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1772 2023-01-22 21:07:25.000000 fuckery-0.6.0/src/fuckery/constants.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      562 2023-01-22 21:07:25.000000 fuckery-0.6.0/src/fuckery/exc.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3553 2023-01-22 21:07:25.000000 fuckery-0.6.0/src/fuckery/memory.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1737 2023-01-22 21:07:25.000000 fuckery-0.6.0/src/fuckery/parser.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8282 2023-01-22 21:07:25.000000 fuckery-0.6.0/src/fuckery/vm.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-01-22 21:07:37.789937 fuckery-0.6.0/src/fuckery.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4162 2023-01-22 21:07:37.000000 fuckery-0.6.0/src/fuckery.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1256 2023-01-22 21:07:37.000000 fuckery-0.6.0/src/fuckery.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-01-22 21:07:37.000000 fuckery-0.6.0/src/fuckery.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       47 2023-01-22 21:07:37.000000 fuckery-0.6.0/src/fuckery.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-01-22 21:07:33.000000 fuckery-0.6.0/src/fuckery.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (3434) circleci  (3434)       48 2023-01-22 21:07:37.000000 fuckery-0.6.0/src/fuckery.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        8 2023-01-22 21:07:37.000000 fuckery-0.6.0/src/fuckery.egg-info/top_level.txt
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-01-22 21:07:37.789937 fuckery-0.6.0/tests/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-01-22 21:07:25.000000 fuckery-0.6.0/tests/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-01-22 21:07:37.789937 fuckery-0.6.0/tests/assets/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      409 2023-01-22 21:07:25.000000 fuckery-0.6.0/tests/assets/add.bf
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2208 2023-01-22 21:07:25.000000 fuckery-0.6.0/tests/assets/hello_world.bf
--rw-r--r--   0 circleci  (3434) circleci  (3434)      729 2023-01-22 21:07:25.000000 fuckery-0.6.0/tests/assets/real_adder.bf
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2253 2023-01-22 21:07:25.000000 fuckery-0.6.0/tests/assets/rot13.bf
--rw-r--r--   0 circleci  (3434) circleci  (3434)      375 2023-01-22 21:07:25.000000 fuckery-0.6.0/tests/common.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2656 2023-01-22 21:07:25.000000 fuckery-0.6.0/tests/test_memory.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1402 2023-01-22 21:07:25.000000 fuckery-0.6.0/tests/test_parser.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      310 2023-01-22 21:07:25.000000 fuckery-0.6.0/tests/test_pyfuckery.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6693 2023-01-22 21:07:25.000000 fuckery-0.6.0/tests/test_vm.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2136 2023-01-22 21:07:25.000000 fuckery-0.6.0/tox.ini
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 01:40:26.009681 fuckery-0.7.2/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       67 2023-06-20 01:40:05.000000 fuckery-0.7.2/AUTHORS.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1057 2023-06-20 01:40:05.000000 fuckery-0.7.2/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4042 2023-06-20 01:40:26.009681 fuckery-0.7.2/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2907 2023-06-20 01:40:05.000000 fuckery-0.7.2/README.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1382 2023-06-20 01:40:05.000000 fuckery-0.7.2/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      657 2023-06-20 01:40:26.009681 fuckery-0.7.2/setup.cfg
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 01:40:26.005681 fuckery-0.7.2/src/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 01:40:26.005681 fuckery-0.7.2/src/fuckery/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      211 2023-06-20 01:40:05.000000 fuckery-0.7.2/src/fuckery/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      418 2023-06-20 01:40:05.000000 fuckery-0.7.2/src/fuckery/__main__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2582 2023-06-20 01:40:05.000000 fuckery-0.7.2/src/fuckery/cli.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1772 2023-06-20 01:40:05.000000 fuckery-0.7.2/src/fuckery/constants.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      562 2023-06-20 01:40:05.000000 fuckery-0.7.2/src/fuckery/exc.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3553 2023-06-20 01:40:05.000000 fuckery-0.7.2/src/fuckery/memory.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1737 2023-06-20 01:40:05.000000 fuckery-0.7.2/src/fuckery/parser.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8282 2023-06-20 01:40:05.000000 fuckery-0.7.2/src/fuckery/vm.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 01:40:26.005681 fuckery-0.7.2/src/fuckery.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4042 2023-06-20 01:40:25.000000 fuckery-0.7.2/src/fuckery.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      523 2023-06-20 01:40:26.000000 fuckery-0.7.2/src/fuckery.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-20 01:40:25.000000 fuckery-0.7.2/src/fuckery.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       46 2023-06-20 01:40:25.000000 fuckery-0.7.2/src/fuckery.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       48 2023-06-20 01:40:25.000000 fuckery-0.7.2/src/fuckery.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        8 2023-06-20 01:40:26.000000 fuckery-0.7.2/src/fuckery.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-20 01:40:26.009681 fuckery-0.7.2/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2656 2023-06-20 01:40:05.000000 fuckery-0.7.2/tests/test_memory.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1402 2023-06-20 01:40:05.000000 fuckery-0.7.2/tests/test_parser.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      310 2023-06-20 01:40:05.000000 fuckery-0.7.2/tests/test_pyfuckery.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6693 2023-06-20 01:40:05.000000 fuckery-0.7.2/tests/test_vm.py
```

### Comparing `fuckery-0.6.0/LICENSE` & `fuckery-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fuckery-0.6.0/README.rst` & `fuckery-0.7.2/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     * - docs
       - |docs|
     * - tests
       - | |appveyor| |circleci| |requires|
         | |codecov|
         | |codeclimate|
     * - package
-      - | |version| |downloads| |wheel| |supported-versions| |supported-implementations|
+      - | |version| |wheel| |supported-versions| |supported-implementations|
         | |commits-since|
 
 .. |docs| image:: https://readthedocs.org/projects/pyfuckery/badge/?style=flat
     :target: https://readthedocs.org/projects/pyfuckery
     :alt: Documentation Status
 
 .. |appveyor| image:: https://ci.appveyor.com/api/projects/status/github/williamgibb/pyFuckery?branch=master&svg=true
@@ -41,17 +41,17 @@
    :target: https://codeclimate.com/github/williamgibb/pyFuckery/maintainability
    :alt: Maintainability
 
 .. |version| image:: https://img.shields.io/pypi/v/fuckery.svg
     :alt: PyPI Package latest release
     :target: https://pypi.python.org/pypi/fuckery
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/williamgibb/pyFuckery/v0.6.0.svg
+.. |commits-since| image:: https://img.shields.io/github/commits-since/williamgibb/pyFuckery/v0.7.2.svg
     :alt: Commits since latest release
-    :target: https://github.com/williamgibb/pyFuckery/compare/v0.6.0...master
+    :target: https://github.com/williamgibb/pyFuckery/compare/v0.7.2...master
 
 .. |wheel| image:: https://img.shields.io/pypi/wheel/fuckery.svg
     :alt: PyPI Wheel
     :target: https://pypi.python.org/pypi/fuckery
 
 .. |supported-versions| image:: https://img.shields.io/pypi/pyversions/fuckery.svg
     :alt: Supported versions
```

### Comparing `fuckery-0.6.0/setup.cfg` & `fuckery-0.7.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bdist_wheel]
-python-tag = py3
+python-tag = py311
 
 [flake8]
 max-line-length = 140
 exclude = tests/*,*/migrations/*,*/south_migrations/*
 
 [tool:pytest]
 norecursedirs =
```

### Comparing `fuckery-0.6.0/src/fuckery/cli.py` & `fuckery-0.7.2/src/fuckery/cli.py`

 * *Files identical despite different names*

### Comparing `fuckery-0.6.0/src/fuckery/constants.py` & `fuckery-0.7.2/src/fuckery/constants.py`

 * *Files identical despite different names*

### Comparing `fuckery-0.6.0/src/fuckery/exc.py` & `fuckery-0.7.2/src/fuckery/exc.py`

 * *Files identical despite different names*

### Comparing `fuckery-0.6.0/src/fuckery/memory.py` & `fuckery-0.7.2/src/fuckery/memory.py`

 * *Files identical despite different names*

### Comparing `fuckery-0.6.0/src/fuckery/parser.py` & `fuckery-0.7.2/src/fuckery/parser.py`

 * *Files identical despite different names*

### Comparing `fuckery-0.6.0/src/fuckery/vm.py` & `fuckery-0.7.2/src/fuckery/vm.py`

 * *Files identical despite different names*

### Comparing `fuckery-0.6.0/tests/test_memory.py` & `fuckery-0.7.2/tests/test_memory.py`

 * *Files identical despite different names*

### Comparing `fuckery-0.6.0/tests/test_parser.py` & `fuckery-0.7.2/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `fuckery-0.6.0/tests/test_vm.py` & `fuckery-0.7.2/tests/test_vm.py`

 * *Files identical despite different names*

