# Comparing `tmp/netzip-0.2.tar.gz` & `tmp/netzip-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netzip-0.2.tar", last modified: Tue Jun 13 16:29:40 2023, max compression
+gzip compressed data, was "netzip-0.3.0.tar", last modified: Tue Jun 20 15:40:57 2023, max compression
```

## Comparing `netzip-0.2.tar` & `netzip-0.3.0.tar`

### file list

```diff
@@ -1,22 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:29:40.834752 netzip-0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-13 16:29:16.000000 netzip-0.2/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:29:40.834752 netzip-0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:29:40.834752 netzip-0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-13 16:29:16.000000 netzip-0.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-13 16:29:16.000000 netzip-0.2/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-13 16:29:16.000000 netzip-0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-13 16:29:16.000000 netzip-0.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-13 16:29:40.834752 netzip-0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-13 16:29:16.000000 netzip-0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-13 16:29:16.000000 netzip-0.2/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-13 16:29:16.000000 netzip-0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 16:29:40.834752 netzip-0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:29:40.834752 netzip-0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:29:40.834752 netzip-0.2/src/netzip.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-13 16:29:40.000000 netzip-0.2/src/netzip.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-13 16:29:40.000000 netzip-0.2/src/netzip.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 16:29:40.000000 netzip-0.2/src/netzip.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 16:29:40.000000 netzip-0.2/src/netzip.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    13702 2023-06-13 16:29:16.000000 netzip-0.2/src/netzip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:29:40.834752 netzip-0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-06-13 16:29:16.000000 netzip-0.2/tests/test_netzip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:40:57.508407 netzip-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-20 15:40:21.000000 netzip-0.3.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-20 15:40:57.508407 netzip-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-20 15:40:21.000000 netzip-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-20 15:40:21.000000 netzip-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 15:40:57.508407 netzip-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:40:57.504407 netzip-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:40:57.504407 netzip-0.3.0/src/netzip/
+-rw-r--r--   0 runner    (1001) docker     (123)    10405 2023-06-20 15:40:21.000000 netzip-0.3.0/src/netzip/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:40:57.508407 netzip-0.3.0/src/netzip.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-20 15:40:57.000000 netzip-0.3.0/src/netzip.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-20 15:40:57.000000 netzip-0.3.0/src/netzip.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 15:40:57.000000 netzip-0.3.0/src/netzip.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-20 15:40:57.000000 netzip-0.3.0/src/netzip.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:40:57.508407 netzip-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-06-20 15:40:21.000000 netzip-0.3.0/tests/test_netzip.py
```

### Comparing `netzip-0.2/LICENSE.txt` & `netzip-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `netzip-0.2/pyproject.toml` & `netzip-0.3.0/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,26 +1,33 @@
 [build-system]
-requires = ["setuptools", "setuptools-scm"]
+requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "netzip"
-authors = [
-    {name = "Emil Melnikov", email = "emilmelnikov@gmail.com"},
-]
+version = "0.3.0"
+authors = [{ name = "Emil Melnikov", email = "emilmelnikov@gmail.com" }]
 description = "ZIP file reader optimized for network access"
 readme = "README.md"
 requires-python = ">=3.8"
-license = {text = "MIT"}
-dynamic = ["version"]
+license = { text = "MIT" }
+
+[project.urls]
+"Homepage" = "https://github.com/emilmelnikov/netzip"
+"Bug Tracker" = "https://github.com/emilmelnikov/netzip/issues"
+"Source" = "https://github.com/emilmelnikov/netzip"
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
-[tool.setuptools_scm]
-
 [tool.pytest.ini_options]
 addopts = "-rfEP --quiet"
 testpaths = ["tests"]
 
 [tool.isort]
 profile = "black"
+
+[tool.pyright]
+include = ["src"]
+ignore = ["noxfile.py", "tests"]
+pythonVersion = "3.8"
+typeCheckingMode = "strict"
```

