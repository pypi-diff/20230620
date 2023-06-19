# Comparing `tmp/flake8-unused-globals-0.1.8.tar.gz` & `tmp/flake8-unused-globals-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flake8-unused-globals-0.1.8.tar", last modified: Mon Jan  9 18:12:02 2023, max compression
+gzip compressed data, was "flake8-unused-globals-0.1.9.tar", last modified: Mon Jan  9 18:51:08 2023, max compression
```

## Comparing `flake8-unused-globals-0.1.8.tar` & `flake8-unused-globals-0.1.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 18:12:02.157668 flake8-unused-globals-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-01-09 18:12:00.000000 flake8-unused-globals-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-09 18:12:00.000000 flake8-unused-globals-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-01-09 18:12:02.157668 flake8-unused-globals-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-01-09 18:12:00.000000 flake8-unused-globals-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 18:12:02.157668 flake8-unused-globals-0.1.8/flake8_unused_globals.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-01-09 18:12:02.000000 flake8-unused-globals-0.1.8/flake8_unused_globals.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-01-09 18:12:02.000000 flake8-unused-globals-0.1.8/flake8_unused_globals.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-09 18:12:02.000000 flake8-unused-globals-0.1.8/flake8_unused_globals.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-01-09 18:12:02.000000 flake8-unused-globals-0.1.8/flake8_unused_globals.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-01-09 18:12:02.000000 flake8-unused-globals-0.1.8/flake8_unused_globals.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-01-09 18:12:02.000000 flake8-unused-globals-0.1.8/flake8_unused_globals.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-01-09 18:12:00.000000 flake8-unused-globals-0.1.8/flake8_unused_globals.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-01-09 18:12:00.000000 flake8-unused-globals-0.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-09 18:12:02.157668 flake8-unused-globals-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-01-09 18:12:00.000000 flake8-unused-globals-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 18:51:08.286677 flake8-unused-globals-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-01-09 18:51:07.000000 flake8-unused-globals-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-09 18:51:07.000000 flake8-unused-globals-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-01-09 18:51:08.286677 flake8-unused-globals-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-01-09 18:51:07.000000 flake8-unused-globals-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 18:51:08.286677 flake8-unused-globals-0.1.9/flake8_unused_globals.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-01-09 18:51:08.000000 flake8-unused-globals-0.1.9/flake8_unused_globals.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-01-09 18:51:08.000000 flake8-unused-globals-0.1.9/flake8_unused_globals.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-09 18:51:08.000000 flake8-unused-globals-0.1.9/flake8_unused_globals.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-01-09 18:51:08.000000 flake8-unused-globals-0.1.9/flake8_unused_globals.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-01-09 18:51:08.000000 flake8-unused-globals-0.1.9/flake8_unused_globals.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-01-09 18:51:08.000000 flake8-unused-globals-0.1.9/flake8_unused_globals.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-01-09 18:51:07.000000 flake8-unused-globals-0.1.9/flake8_unused_globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-01-09 18:51:07.000000 flake8-unused-globals-0.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-09 18:51:08.286677 flake8-unused-globals-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-01-09 18:51:07.000000 flake8-unused-globals-0.1.9/setup.py
```

### Comparing `flake8-unused-globals-0.1.8/LICENSE` & `flake8-unused-globals-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `flake8-unused-globals-0.1.8/flake8_unused_globals.py` & `flake8-unused-globals-0.1.9/flake8_unused_globals.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import ast
 from typing import Iterable, Any
 
 ERROR_CODE = "UUG001"
 CHECK = "unused global variable"
-VERSION = "0.1.8"
+VERSION = "0.1.9"
 
 
 class GlobalVariableLoadCounter(ast.NodeVisitor):
     def __init__(self, *args: Any, **kwargs: Any) -> None:
         super().__init__(*args, **kwargs)
         self.id_to_loads = {}
         self.id_to_store_info = {}
```

### Comparing `flake8-unused-globals-0.1.8/setup.py` & `flake8-unused-globals-0.1.9/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     install_requires = f.read().splitlines()
 
 with open("README.md") as f:
     long_description = f.read().strip()
 
 setup(
     name="flake8-unused-globals",
-    version="0.1.8",
+    version="0.1.9",
     python_requires=">=3.10,<3.11",
     install_requires=install_requires,
     py_modules=["flake8_unused_globals"],
     entry_points={"flake8.extension": "UUG001 = flake8_unused_globals:Plugin"},
     long_description=long_description,
     long_description_content_type="text/markdown",
 )
```

