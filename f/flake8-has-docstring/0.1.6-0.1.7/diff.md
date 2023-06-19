# Comparing `tmp/flake8-has-docstring-0.1.6.tar.gz` & `tmp/flake8-has-docstring-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flake8-has-docstring-0.1.6.tar", last modified: Mon Jan 30 23:04:34 2023, max compression
+gzip compressed data, was "flake8-has-docstring-0.1.7.tar", last modified: Mon Jun 19 22:12:23 2023, max compression
```

## Comparing `flake8-has-docstring-0.1.6.tar` & `flake8-has-docstring-0.1.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 23:04:34.893652 flake8-has-docstring-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-01-30 23:04:32.000000 flake8-has-docstring-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-30 23:04:32.000000 flake8-has-docstring-0.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-01-30 23:04:34.893652 flake8-has-docstring-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-01-30 23:04:32.000000 flake8-has-docstring-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 23:04:34.893652 flake8-has-docstring-0.1.6/flake8_has_docstring.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-01-30 23:04:34.000000 flake8-has-docstring-0.1.6/flake8_has_docstring.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-01-30 23:04:34.000000 flake8-has-docstring-0.1.6/flake8_has_docstring.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-30 23:04:34.000000 flake8-has-docstring-0.1.6/flake8_has_docstring.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-01-30 23:04:34.000000 flake8-has-docstring-0.1.6/flake8_has_docstring.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-01-30 23:04:34.000000 flake8-has-docstring-0.1.6/flake8_has_docstring.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-01-30 23:04:34.000000 flake8-has-docstring-0.1.6/flake8_has_docstring.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-01-30 23:04:32.000000 flake8-has-docstring-0.1.6/flake8_has_docstring.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-01-30 23:04:32.000000 flake8-has-docstring-0.1.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-30 23:04:34.893652 flake8-has-docstring-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-01-30 23:04:32.000000 flake8-has-docstring-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:12:23.411202 flake8-has-docstring-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-19 22:12:22.000000 flake8-has-docstring-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-19 22:12:22.000000 flake8-has-docstring-0.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-06-19 22:12:23.411202 flake8-has-docstring-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-19 22:12:22.000000 flake8-has-docstring-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:12:23.411202 flake8-has-docstring-0.1.7/flake8_has_docstring.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-06-19 22:12:23.000000 flake8-has-docstring-0.1.7/flake8_has_docstring.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-19 22:12:23.000000 flake8-has-docstring-0.1.7/flake8_has_docstring.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 22:12:23.000000 flake8-has-docstring-0.1.7/flake8_has_docstring.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-19 22:12:23.000000 flake8-has-docstring-0.1.7/flake8_has_docstring.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-19 22:12:23.000000 flake8-has-docstring-0.1.7/flake8_has_docstring.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-19 22:12:23.000000 flake8-has-docstring-0.1.7/flake8_has_docstring.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-06-19 22:12:22.000000 flake8-has-docstring-0.1.7/flake8_has_docstring.py
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-19 22:12:22.000000 flake8-has-docstring-0.1.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 22:12:23.411202 flake8-has-docstring-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-19 22:12:22.000000 flake8-has-docstring-0.1.7/setup.py
```

### Comparing `flake8-has-docstring-0.1.6/LICENSE` & `flake8-has-docstring-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `flake8-has-docstring-0.1.6/PKG-INFO` & `flake8-has-docstring-0.1.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: flake8-has-docstring
-Version: 0.1.6
-Requires-Python: >=3.10,<3.11
+Version: 0.1.7
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # flake8-has-docstring
 
 A flake8 plugin that checks that functions have docstrings.
```

### Comparing `flake8-has-docstring-0.1.6/flake8_has_docstring.egg-info/PKG-INFO` & `flake8-has-docstring-0.1.7/flake8_has_docstring.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: flake8-has-docstring
-Version: 0.1.6
-Requires-Python: >=3.10,<3.11
+Version: 0.1.7
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # flake8-has-docstring
 
 A flake8 plugin that checks that functions have docstrings.
```

### Comparing `flake8-has-docstring-0.1.6/flake8_has_docstring.py` & `flake8-has-docstring-0.1.7/flake8_has_docstring.py`

 * *Files identical despite different names*

### Comparing `flake8-has-docstring-0.1.6/setup.py` & `flake8-has-docstring-0.1.7/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     install_requires = f.read().splitlines()
 
 with open("README.md") as f:
     long_description = f.read().strip()
 
 setup(
     name="flake8-has-docstring",
-    version="0.1.6",
-    python_requires=">=3.10,<3.11",
+    version="0.1.7",
+    python_requires=">=3.10",
     install_requires=install_requires,
     py_modules=["flake8_has_docstring"],
     entry_points={"flake8.extension": "DOC001 = flake8_has_docstring:Plugin"},
     long_description=long_description,
     long_description_content_type="text/markdown",
 )
```

