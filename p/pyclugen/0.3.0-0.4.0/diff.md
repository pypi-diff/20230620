# Comparing `tmp/pyclugen-0.3.0.tar.gz` & `tmp/pyclugen-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyclugen-0.3.0.tar", last modified: Sun Jun 11 18:15:43 2023, max compression
+gzip compressed data, was "pyclugen-0.4.0.tar", last modified: Tue Jun 20 18:27:34 2023, max compression
```

## Comparing `pyclugen-0.3.0.tar` & `pyclugen-0.4.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:15:43.897245 pyclugen-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-11 18:15:33.000000 pyclugen-0.3.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-06-11 18:15:43.897245 pyclugen-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-06-11 18:15:33.000000 pyclugen-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:15:43.897245 pyclugen-0.3.0/pyclugen/
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-06-11 18:15:33.000000 pyclugen-0.3.0/pyclugen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6385 2023-06-11 18:15:33.000000 pyclugen-0.3.0/pyclugen/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     8472 2023-06-11 18:15:33.000000 pyclugen-0.3.0/pyclugen/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    19955 2023-06-11 18:15:33.000000 pyclugen-0.3.0/pyclugen/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    12041 2023-06-11 18:15:33.000000 pyclugen-0.3.0/pyclugen/module.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-11 18:15:33.000000 pyclugen-0.3.0/pyclugen/shared.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:15:43.897245 pyclugen-0.3.0/pyclugen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-06-11 18:15:43.000000 pyclugen-0.3.0/pyclugen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-11 18:15:43.000000 pyclugen-0.3.0/pyclugen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 18:15:43.000000 pyclugen-0.3.0/pyclugen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-11 18:15:43.000000 pyclugen-0.3.0/pyclugen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-11 18:15:43.000000 pyclugen-0.3.0/pyclugen.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-06-11 18:15:33.000000 pyclugen-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 18:15:43.897245 pyclugen-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 18:15:43.897245 pyclugen-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-06-11 18:15:33.000000 pyclugen-0.3.0/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     7949 2023-06-11 18:15:33.000000 pyclugen-0.3.0/tests/test_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    22816 2023-06-11 18:15:33.000000 pyclugen-0.3.0/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-06-11 18:15:33.000000 pyclugen-0.3.0/tests/test_module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:27:34.290877 pyclugen-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-20 18:27:26.000000 pyclugen-0.4.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-06-20 18:27:34.290877 pyclugen-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-06-20 18:27:26.000000 pyclugen-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:27:34.286877 pyclugen-0.4.0/pyclugen/
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-06-20 18:27:26.000000 pyclugen-0.4.0/pyclugen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6385 2023-06-20 18:27:26.000000 pyclugen-0.4.0/pyclugen/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8472 2023-06-20 18:27:26.000000 pyclugen-0.4.0/pyclugen/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27822 2023-06-20 18:27:26.000000 pyclugen-0.4.0/pyclugen/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12041 2023-06-20 18:27:26.000000 pyclugen-0.4.0/pyclugen/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-20 18:27:26.000000 pyclugen-0.4.0/pyclugen/shared.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:27:34.286877 pyclugen-0.4.0/pyclugen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-06-20 18:27:34.000000 pyclugen-0.4.0/pyclugen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-20 18:27:34.000000 pyclugen-0.4.0/pyclugen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 18:27:34.000000 pyclugen-0.4.0/pyclugen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-20 18:27:34.000000 pyclugen-0.4.0/pyclugen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-20 18:27:34.000000 pyclugen-0.4.0/pyclugen.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-06-20 18:27:26.000000 pyclugen-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 18:27:34.290877 pyclugen-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:27:34.290877 pyclugen-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-06-20 18:27:26.000000 pyclugen-0.4.0/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7949 2023-06-20 18:27:26.000000 pyclugen-0.4.0/tests/test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30706 2023-06-20 18:27:26.000000 pyclugen-0.4.0/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-06-20 18:27:26.000000 pyclugen-0.4.0/tests/test_module.py
```

### Comparing `pyclugen-0.3.0/LICENSE.txt` & `pyclugen-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyclugen-0.3.0/PKG-INFO` & `pyclugen-0.4.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyclugen
-Version: 0.3.0
+Version: 0.4.0
 Summary: Multidimensional cluster generation in Python
 Author-email: Nuno Fachada <faken@fakenmc.com>
 License: MIT
 Project-URL: Bug Reports, https://github.com/clugen/pyclugen/issues
 Project-URL: Documentation, https://clugen.github.io/pyclugen/
 Project-URL: Source, https://github.com/clugen/pyclugen/
 Keywords: multidimensional data,synthetic clusters,synthetic data generation,synthetic data generator,multidimensional clusters,clustering
@@ -25,19 +25,21 @@
 [![PyPI](https://img.shields.io/pypi/v/pyclugen)](https://pypi.org/project/pyclugen/)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/pyclugen?color=blueviolet)
 [![MIT](https://img.shields.io/badge/license-MIT-yellowgreen.svg)](https://tldrlegal.com/license/mit-license)
 
 # pyclugen
 
 **pyclugen** is a Python implementation of the *clugen* algorithm for
-generating multidimensional clusters. Each cluster is supported by a line
-segment, the position, orientation and length of which guide where the
-respective points are placed.
-
-See the [documentation](https://clugen.github.io/pyclugen/) for more details.
+generating multidimensional clusters with arbitrary distributions. Each cluster
+is supported by a line segment, the position, orientation and length of which
+guide where the respective points are placed.
+
+See the [documentation](https://clugen.github.io/pyclugen/) and
+[examples](https://clugen.github.io/pyclugen/generated/gallery/) for more
+details.
 
 ## Installation
 
 Install from PyPI:
 
 ```sh
 pip install --upgrade pip
```

### Comparing `pyclugen-0.3.0/README.md` & `pyclugen-0.4.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -4,19 +4,21 @@
 [![PyPI](https://img.shields.io/pypi/v/pyclugen)](https://pypi.org/project/pyclugen/)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/pyclugen?color=blueviolet)
 [![MIT](https://img.shields.io/badge/license-MIT-yellowgreen.svg)](https://tldrlegal.com/license/mit-license)
 
 # pyclugen
 
 **pyclugen** is a Python implementation of the *clugen* algorithm for
-generating multidimensional clusters. Each cluster is supported by a line
-segment, the position, orientation and length of which guide where the
-respective points are placed.
-
-See the [documentation](https://clugen.github.io/pyclugen/) for more details.
+generating multidimensional clusters with arbitrary distributions. Each cluster
+is supported by a line segment, the position, orientation and length of which
+guide where the respective points are placed.
+
+See the [documentation](https://clugen.github.io/pyclugen/) and
+[examples](https://clugen.github.io/pyclugen/generated/gallery/) for more
+details.
 
 ## Installation
 
 Install from PyPI:
 
 ```sh
 pip install --upgrade pip
```

### Comparing `pyclugen-0.3.0/pyclugen/__init__.py` & `pyclugen-0.4.0/pyclugen/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,15 @@
    [`Generator`][numpy.random.Generator] initialized with the same seed.
 """
 
 
 __all__ = [
     "Clusters",
     "clugen",
+    "clumerge",
     "points_on_line",
     "rand_ortho_vector",
     "rand_unit_vector",
     "rand_vector_at_angle",
     "angle_deltas",
     "angle_btw",
     "clupoints_n_1_template",
@@ -37,15 +38,15 @@
 from pyclugen.core import (
     points_on_line,
     rand_ortho_vector,
     rand_unit_vector,
     rand_vector_at_angle,
 )
 from pyclugen.helper import angle_btw, clupoints_n_1_template, fix_empty, fix_num_points
-from pyclugen.main import Clusters, clugen
+from pyclugen.main import Clusters, clugen, clumerge
 from pyclugen.module import (
     angle_deltas,
     clucenters,
     clupoints_n,
     clupoints_n_1,
     clusizes,
     llengths,
```

### Comparing `pyclugen-0.3.0/pyclugen/core.py` & `pyclugen-0.4.0/pyclugen/core.py`

 * *Files identical despite different names*

### Comparing `pyclugen-0.3.0/pyclugen/helper.py` & `pyclugen-0.4.0/pyclugen/helper.py`

 * *Files identical despite different names*

### Comparing `pyclugen-0.3.0/pyclugen/module.py` & `pyclugen-0.4.0/pyclugen/module.py`

 * *Files identical despite different names*

### Comparing `pyclugen-0.3.0/pyclugen.egg-info/PKG-INFO` & `pyclugen-0.4.0/pyclugen.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyclugen
-Version: 0.3.0
+Version: 0.4.0
 Summary: Multidimensional cluster generation in Python
 Author-email: Nuno Fachada <faken@fakenmc.com>
 License: MIT
 Project-URL: Bug Reports, https://github.com/clugen/pyclugen/issues
 Project-URL: Documentation, https://clugen.github.io/pyclugen/
 Project-URL: Source, https://github.com/clugen/pyclugen/
 Keywords: multidimensional data,synthetic clusters,synthetic data generation,synthetic data generator,multidimensional clusters,clustering
@@ -25,19 +25,21 @@
 [![PyPI](https://img.shields.io/pypi/v/pyclugen)](https://pypi.org/project/pyclugen/)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/pyclugen?color=blueviolet)
 [![MIT](https://img.shields.io/badge/license-MIT-yellowgreen.svg)](https://tldrlegal.com/license/mit-license)
 
 # pyclugen
 
 **pyclugen** is a Python implementation of the *clugen* algorithm for
-generating multidimensional clusters. Each cluster is supported by a line
-segment, the position, orientation and length of which guide where the
-respective points are placed.
-
-See the [documentation](https://clugen.github.io/pyclugen/) for more details.
+generating multidimensional clusters with arbitrary distributions. Each cluster
+is supported by a line segment, the position, orientation and length of which
+guide where the respective points are placed.
+
+See the [documentation](https://clugen.github.io/pyclugen/) and
+[examples](https://clugen.github.io/pyclugen/generated/gallery/) for more
+details.
 
 ## Installation
 
 Install from PyPI:
 
 ```sh
 pip install --upgrade pip
```

### Comparing `pyclugen-0.3.0/pyproject.toml` & `pyclugen-0.4.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyclugen"
 description = "Multidimensional cluster generation in Python"
-version = "0.3.0"
+version = "0.4.0"
 authors = [ { name = "Nuno Fachada", email = "faken@fakenmc.com" } ]
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = [
     "multidimensional data",
     "synthetic clusters",
     "synthetic data generation",
@@ -50,26 +50,28 @@
     "pandas",
     "pep8-naming",
     "pre-commit",
     "pytest >= 6.0",
     "coverage",
     "pytest-cov >= 3.0.0",
     "pytest-mypy",
+    "scikit-learn",
     "seaborn" ]
 
 [project.urls]
 "Bug Reports" = "https://github.com/clugen/pyclugen/issues"
 "Documentation" = "https://clugen.github.io/pyclugen/"
 "Source" = "https://github.com/clugen/pyclugen/"
 
 [tool.setuptools]
 packages = ["pyclugen"]
 
 [tool.mypy]
 python_version = 3.8
+warn_unused_ignores = true
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 addopts = "--mypy --doctest-modules"
 norecursedirs = [
     "hooks",
     "*.egg",
@@ -92,15 +94,19 @@
 line_length = 88
 skip_gitignore = "True"
 
 [tool.flake8]
 extend-select = ["B9", "C4"]
 max-line-length = 88
 max-doc-length = 88
-ignore = [ "B018", "SIM106", "W503" ]
+ignore = [
+    "B905",  # Force `strict` in zip(), but this requires Python 3.10
+    "E203",  # "whitespace before ':'"", but that's how black likes it
+    "W503" ] # "line break before binary operator", conflicts with black
+
 doctests = true
 exclude = [
     ".git",
     "__pycache__",
     ".*cache",
     "build",
     "dist",
```

### Comparing `pyclugen-0.3.0/tests/test_core.py` & `pyclugen-0.4.0/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `pyclugen-0.3.0/tests/test_helper.py` & `pyclugen-0.4.0/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `pyclugen-0.3.0/tests/test_module.py` & `pyclugen-0.4.0/tests/test_module.py`

 * *Files identical despite different names*

