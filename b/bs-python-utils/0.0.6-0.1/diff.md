# Comparing `tmp/bs_python_utils-0.0.6.tar.gz` & `tmp/bs_python_utils-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bs_python_utils-0.0.6.tar", max compression
+gzip compressed data, was "bs_python_utils-0.1.tar", max compression
```

## Comparing `bs_python_utils-0.0.6.tar` & `bs_python_utils-0.1.tar`

### file list

```diff
@@ -1,28 +1,30 @@
--rw-r--r--   0        0        0     1073 2023-04-21 14:06:07.415664 bs_python_utils-0.0.6/LICENSE
--rw-r--r--   0        0        0     1414 2023-05-09 18:12:28.311148 bs_python_utils-0.0.6/README.md
--rw-r--r--   0        0        0     1799 2023-04-24 19:42:58.427840 bs_python_utils-0.0.6/bs_python_utils/Timer.py
--rw-r--r--   0        0        0        0 2023-04-24 19:42:58.429294 bs_python_utils-0.0.6/bs_python_utils/__init__.py
--rw-r--r--   0        0        0    28473 2023-04-24 22:57:44.859499 bs_python_utils-0.0.6/bs_python_utils/bs_altair.py
--rw-r--r--   0        0        0     2976 2023-04-24 20:25:24.489951 bs_python_utils-0.0.6/bs_python_utils/bs_logging.py
--rw-r--r--   0        0        0     3577 2023-04-24 19:42:58.433666 bs_python_utils-0.0.6/bs_python_utils/bs_mathstr.py
--rw-r--r--   0        0        0     4338 2023-04-24 21:45:53.142922 bs_python_utils-0.0.6/bs_python_utils/bs_mem.py
--rw-r--r--   0        0        0    13696 2023-04-24 22:48:26.403984 bs_python_utils-0.0.6/bs_python_utils/bs_opt.py
--rw-r--r--   0        0        0       36 2023-04-24 19:42:58.438686 bs_python_utils-0.0.6/bs_python_utils/bs_plots.py
--rw-r--r--   0        0        0     4507 2023-04-24 20:32:13.556809 bs_python_utils-0.0.6/bs_python_utils/bs_seaborn.py
--rw-r--r--   0        0        0     1391 2023-04-24 22:48:26.302214 bs_python_utils-0.0.6/bs_python_utils/bs_sparse_gaussian.py
--rw-r--r--   0        0        0      905 2023-04-24 19:42:58.441367 bs_python_utils-0.0.6/bs_python_utils/bsmplutils.py
--rw-r--r--   0        0        0    31244 2023-05-09 18:04:48.974809 bs_python_utils-0.0.6/bs_python_utils/bsnputils.py
--rw-r--r--   0        0        0     2132 2023-04-24 20:25:24.253141 bs_python_utils-0.0.6/bs_python_utils/bssputils.py
--rw-r--r--   0        0        0    15489 2023-04-24 20:25:24.644930 bs_python_utils-0.0.6/bs_python_utils/bsstats.py
--rw-r--r--   0        0        0     9471 2023-05-08 18:43:13.753098 bs_python_utils-0.0.6/bs_python_utils/bsutils.py
--rw-r--r--   0        0        0     7801 2023-04-24 21:45:53.165270 bs_python_utils-0.0.6/bs_python_utils/distance_covariances.py
--rw-r--r--   0        0        0     1350 2023-04-24 22:36:28.733299 bs_python_utils-0.0.6/bs_python_utils/example_opt.py
--rw-r--r--   0        0        0     3833 2023-04-24 22:48:26.344134 bs_python_utils-0.0.6/bs_python_utils/examples_altair.py
--rw-r--r--   0        0        0     1013 2023-04-24 22:36:28.733372 bs_python_utils-0.0.6/bs_python_utils/examples_distance_covariances.py
--rw-r--r--   0        0        0      552 2023-04-24 22:36:28.733335 bs_python_utils-0.0.6/bs_python_utils/examples_mem.py
--rw-r--r--   0        0        0      771 2023-04-24 21:45:53.146924 bs_python_utils-0.0.6/bs_python_utils/examples_seaborn.py
--rw-r--r--   0        0        0      786 2023-04-24 22:36:28.733292 bs_python_utils-0.0.6/bs_python_utils/examples_sklearn.py
--rw-r--r--   0        0        0     7426 2023-04-24 20:25:24.576148 bs_python_utils-0.0.6/bs_python_utils/pandas_utils.py
--rw-r--r--   0        0        0     1872 2023-04-24 21:46:50.361114 bs_python_utils-0.0.6/bs_python_utils/sklearn_utils.py
--rw-r--r--   0        0        0     1871 2023-05-09 18:13:15.166890 bs_python_utils-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     2386 1970-01-01 00:00:00.000000 bs_python_utils-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-04-21 14:06:07.415664 bs_python_utils-0.1/LICENSE
+-rw-r--r--   0        0        0     1490 2023-06-20 20:42:14.388128 bs_python_utils-0.1/README.md
+-rw-r--r--   0        0        0     1799 2023-04-24 19:42:58.427840 bs_python_utils-0.1/bs_python_utils/Timer.py
+-rw-r--r--   0        0        0        0 2023-04-24 19:42:58.429294 bs_python_utils-0.1/bs_python_utils/__init__.py
+-rw-r--r--   0        0        0    28473 2023-04-24 22:57:44.859499 bs_python_utils-0.1/bs_python_utils/bs_altair.py
+-rw-r--r--   0        0        0     2976 2023-04-24 20:25:24.489951 bs_python_utils-0.1/bs_python_utils/bs_logging.py
+-rw-r--r--   0        0        0     3577 2023-04-24 19:42:58.433666 bs_python_utils-0.1/bs_python_utils/bs_mathstr.py
+-rw-r--r--   0        0        0     4338 2023-04-24 21:45:53.142922 bs_python_utils-0.1/bs_python_utils/bs_mem.py
+-rw-r--r--   0        0        0    13696 2023-04-24 22:48:26.403984 bs_python_utils-0.1/bs_python_utils/bs_opt.py
+-rw-r--r--   0        0        0       36 2023-04-24 19:42:58.438686 bs_python_utils-0.1/bs_python_utils/bs_plots.py
+-rw-r--r--   0        0        0     4507 2023-04-24 20:32:13.556809 bs_python_utils-0.1/bs_python_utils/bs_seaborn.py
+-rw-r--r--   0        0        0     1391 2023-04-24 22:48:26.302214 bs_python_utils-0.1/bs_python_utils/bs_sparse_gaussian.py
+-rw-r--r--   0        0        0      905 2023-04-24 19:42:58.441367 bs_python_utils-0.1/bs_python_utils/bsmplutils.py
+-rw-r--r--   0        0        0    32084 2023-06-20 20:51:26.724318 bs_python_utils-0.1/bs_python_utils/bsnputils.py
+-rw-r--r--   0        0        0     2132 2023-04-24 20:25:24.253141 bs_python_utils-0.1/bs_python_utils/bssputils.py
+-rw-r--r--   0        0        0    15489 2023-04-24 20:25:24.644930 bs_python_utils-0.1/bs_python_utils/bsstats.py
+-rw-r--r--   0        0        0     9471 2023-05-08 18:43:13.753098 bs_python_utils-0.1/bs_python_utils/bsutils.py
+-rw-r--r--   0        0        0    14016 2023-06-20 20:58:35.021722 bs_python_utils-0.1/bs_python_utils/chebyshev.py
+-rw-r--r--   0        0        0     7801 2023-04-24 21:45:53.165270 bs_python_utils-0.1/bs_python_utils/distance_covariances.py
+-rw-r--r--   0        0        0     1350 2023-04-24 22:36:28.733299 bs_python_utils-0.1/bs_python_utils/example_opt.py
+-rw-r--r--   0        0        0     3833 2023-04-24 22:48:26.344134 bs_python_utils-0.1/bs_python_utils/examples_altair.py
+-rw-r--r--   0        0        0     1013 2023-04-24 22:36:28.733372 bs_python_utils-0.1/bs_python_utils/examples_distance_covariances.py
+-rw-r--r--   0        0        0      552 2023-04-24 22:36:28.733335 bs_python_utils-0.1/bs_python_utils/examples_mem.py
+-rw-r--r--   0        0        0      771 2023-04-24 21:45:53.146924 bs_python_utils-0.1/bs_python_utils/examples_seaborn.py
+-rw-r--r--   0        0        0      786 2023-04-24 22:36:28.733292 bs_python_utils-0.1/bs_python_utils/examples_sklearn.py
+-rw-r--r--   0        0        0     7426 2023-04-24 20:25:24.576148 bs_python_utils-0.1/bs_python_utils/pandas_utils.py
+-rw-r--r--   0        0        0     1872 2023-04-24 21:46:50.361114 bs_python_utils-0.1/bs_python_utils/sklearn_utils.py
+-rw-r--r--   0        0        0     1455 2023-05-27 22:42:00.768780 bs_python_utils-0.1/bs_python_utils/tests
+-rw-r--r--   0        0        0     1868 2023-06-20 20:59:29.194874 bs_python_utils-0.1/pyproject.toml
+-rw-r--r--   0        0        0     2459 1970-01-01 00:00:00.000000 bs_python_utils-0.1/PKG-INFO
```

### Comparing `bs_python_utils-0.0.6/LICENSE` & `bs_python_utils-0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.6/README.md` & `bs_python_utils-0.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 My Python utilities.
 
 -   **Github repository**: <https://github.com/bsalanie/bs-python-utils/>
 -   **Documentation** <https://bsalanie.github.io/bs-python-utils/>
 
 ### Release notes
 
+#### 0.1 (June 20, 2023)
+Added `grid_function` and the `chebyshev` module. 
 
 #### 0.0.6 (May 9, 2023)
 
 Improved docs.
 
 #### 0.0.5 (May 8, 2023)
```

### Comparing `bs_python_utils-0.0.6/bs_python_utils/Timer.py` & `bs_python_utils-0.1/bs_python_utils/Timer.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.6/bs_python_utils/bs_altair.py` & `bs_python_utils-0.1/bs_python_utils/bs_altair.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.6/bs_python_utils/bs_logging.py` & `bs_python_utils-0.1/bs_python_utils/bs_logging.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.6/bs_python_utils/bs_mathstr.py` & `bs_python_utils-0.1/bs_python_utils/bs_mathstr.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.6/bs_python_utils/bs_mem.py` & `bs_python_utils-0.1/bs_python_utils/bs_mem.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.6/bs_python_utils/bs_opt.py` & `bs_python_utils-0.1/bs_python_utils/bs_opt.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.6/bs_python_utils/bs_seaborn.py` & `bs_python_utils-0.1/bs_python_utils/bs_seaborn.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.6/bs_python_utils/bs_sparse_gaussian.py` & `bs_python_utils-0.1/bs_python_utils/bs_sparse_gaussian.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.6/bs_python_utils/bsmplutils.py` & `bs_python_utils-0.1/bs_python_utils/bsmplutils.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.6/bs_python_utils/bsnputils.py` & `bs_python_utils-0.1/bs_python_utils/bsnputils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 """
 Contains various `numpy` utility programs.
 """
 
 import sys
 from math import cos, exp, floor, log, pi, sqrt
-from typing import Any, Callable, Iterable, cast
+from typing import Any, Callable, Iterable, Union, cast
 
 import numpy as np
 from numpy.polynomial import Polynomial
 
 from bs_python_utils.bsutils import bs_error_abort, print_stars
 
 # some useful types
 TwoArrays = tuple[np.ndarray, np.ndarray]
 ThreeArrays = tuple[np.ndarray, np.ndarray, np.ndarray]
 FourArrays = tuple[np.ndarray, np.ndarray, np.ndarray, np.ndarray]
 SixArrays = tuple[
     np.ndarray, np.ndarray, np.ndarray, np.ndarray, np.ndarray, np.ndarray
 ]
+FloatOrArray = Union[float, np.ndarray]
+Function_x = Callable[[np.ndarray], float]
+Function_xa = Callable[[np.ndarray, int], float]
+Function_xargs = Callable[[np.ndarray, list], float]
+ArrayFunctionOfArray = Callable[[np.ndarray], np.ndarray]
 
 
 def check_vector(v: Any, fun_name: str = None) -> int:
     """
     test that `v` is a vector; aborts otherwise
 
     Args:
@@ -125,14 +130,36 @@
     ndims_x = x.ndim
     if ndims_x != n_dims:
         bs_error_abort(f"{fun_str} x should have {n_dims} dimensions, not {ndims_x}")
         return (0,)  # for mypy
     return cast(tuple[int, ...], x.shape)
 
 
+def grid_function(
+    fun: Callable[[np.ndarray, np.ndarray], np.ndarray],
+    x_points: np.ndarray,
+    y_points: np.ndarray,
+) -> np.ndarray:
+    """apply a function f(x, y) on a lattice grid
+
+    Args:
+        fun: should return a matrix `(m, n)`  when called with two matrices `(m, n)`
+        x_points: an `m`-vector
+        y_points: an `n`-vector
+
+    Returns:
+        the `(m, n)` matrix of values of `fun` on the grid
+    """
+    _ = check_vector(x_points)
+    _ = check_vector(y_points)
+    X1, Y1 = np.meshgrid(x_points, y_points)
+    z_grid = fun(X1, Y1).T
+    return z_grid
+
+
 # Numpy parallel RNG
 def generate_RNG_streams(
     nsim: int, initial_seed: int = 13091962
 ) -> list[np.random.Generator]:
     """
     return `nsim` RNGs
```

### Comparing `bs_python_utils-0.0.6/bs_python_utils/bssputils.py` & `bs_python_utils-0.1/bs_python_utils/bssputils.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.6/bs_python_utils/bsstats.py` & `bs_python_utils-0.1/bs_python_utils/bsstats.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.6/bs_python_utils/bsutils.py` & `bs_python_utils-0.1/bs_python_utils/bsutils.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.6/bs_python_utils/distance_covariances.py` & `bs_python_utils-0.1/bs_python_utils/distance_covariances.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.6/bs_python_utils/example_opt.py` & `bs_python_utils-0.1/bs_python_utils/example_opt.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.6/bs_python_utils/examples_altair.py` & `bs_python_utils-0.1/bs_python_utils/examples_altair.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.6/bs_python_utils/examples_distance_covariances.py` & `bs_python_utils-0.1/bs_python_utils/examples_distance_covariances.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.6/bs_python_utils/examples_mem.py` & `bs_python_utils-0.1/bs_python_utils/examples_mem.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.6/bs_python_utils/examples_seaborn.py` & `bs_python_utils-0.1/bs_python_utils/examples_seaborn.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.6/bs_python_utils/examples_sklearn.py` & `bs_python_utils-0.1/bs_python_utils/examples_sklearn.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.6/bs_python_utils/pandas_utils.py` & `bs_python_utils-0.1/bs_python_utils/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.6/bs_python_utils/sklearn_utils.py` & `bs_python_utils-0.1/bs_python_utils/sklearn_utils.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.6/pyproject.toml` & `bs_python_utils-0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "bs_python_utils"
-version = "0.0.6"
+version = "0.1"
 description = "my Python utilities"
-authors = ["Bernard Salanie <fbsalanie@columbia.edu>"]
+authors = ["Bernard Salanie <bsalanie@columbia.edu>"]
 repository = "https://github.com/bsalanie/bs-python-utils"
 documentation = "https://bsalanie.github.io/bs-python-utils/"
 readme = "README.md"
 packages = [
   {include = "bs_python_utils"}
 ]
```

### Comparing `bs_python_utils-0.0.6/PKG-INFO` & `bs_python_utils-0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: bs-python-utils
-Version: 0.0.6
+Version: 0.1
 Summary: my Python utilities
 Home-page: https://github.com/bsalanie/bs-python-utils
 Author: Bernard Salanie
-Author-email: fbsalanie@columbia.edu
+Author-email: bsalanie@columbia.edu
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: altair (>=4.2.2,<5.0.0)
@@ -33,14 +33,16 @@
 My Python utilities.
 
 -   **Github repository**: <https://github.com/bsalanie/bs-python-utils/>
 -   **Documentation** <https://bsalanie.github.io/bs-python-utils/>
 
 ### Release notes
 
+#### 0.1 (June 20, 2023)
+Added `grid_function` and the `chebyshev` module. 
 
 #### 0.0.6 (May 9, 2023)
 
 Improved docs.
 
 #### 0.0.5 (May 8, 2023)
```

