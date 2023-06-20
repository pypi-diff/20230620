# Comparing `tmp/csnlp-1.5.5.tar.gz` & `tmp/csnlp-1.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csnlp-1.5.5.tar", last modified: Fri Jun  2 17:17:48 2023, max compression
+gzip compressed data, was "csnlp-1.5.6.tar", last modified: Tue Jun 20 15:28:23 2023, max compression
```

## Comparing `csnlp-1.5.5.tar` & `csnlp-1.5.6.tar`

### file list

```diff
@@ -1,52 +1,51 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 17:17:48.983255 csnlp-1.5.5/
--rw-rw-rw-   0        0        0     1093 2022-11-02 20:11:46.000000 csnlp-1.5.5/LICENSE
--rw-rw-rw-   0        0        0     7069 2023-06-02 17:17:48.982580 csnlp-1.5.5/PKG-INFO
--rw-rw-rw-   0        0        0     6267 2023-02-24 10:22:25.000000 csnlp-1.5.5/README.md
--rw-rw-rw-   0        0        0     1155 2023-06-02 17:13:58.000000 csnlp-1.5.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-02 17:17:48.984358 csnlp-1.5.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-02 17:17:48.822631 csnlp-1.5.5/src/
-drwxrwxrwx   0        0        0        0 2023-06-02 17:17:48.847830 csnlp-1.5.5/src/csnlp/
--rw-rw-rw-   0        0        0      210 2023-04-04 11:47:09.000000 csnlp-1.5.5/src/csnlp/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-02 17:17:48.885464 csnlp-1.5.5/src/csnlp/core/
--rw-rw-rw-   0        0        0     3267 2023-01-02 20:43:22.000000 csnlp-1.5.5/src/csnlp/core/cache.py
--rw-rw-rw-   0        0        0     3186 2023-04-04 11:47:09.000000 csnlp-1.5.5/src/csnlp/core/data.py
--rw-rw-rw-   0        0        0     6057 2023-03-24 10:24:25.000000 csnlp-1.5.5/src/csnlp/core/debug.py
--rw-rw-rw-   0        0        0     2085 2023-02-16 10:35:36.000000 csnlp-1.5.5/src/csnlp/core/derivatives.py
--rw-rw-rw-   0        0        0     5241 2023-02-16 10:40:42.000000 csnlp-1.5.5/src/csnlp/core/scaling.py
--rw-rw-rw-   0        0        0     6426 2023-03-23 22:24:06.000000 csnlp-1.5.5/src/csnlp/core/solutions.py
-drwxrwxrwx   0        0        0        0 2023-06-02 17:17:48.896386 csnlp-1.5.5/src/csnlp/multistart/
--rw-rw-rw-   0        0        0      425 2023-03-20 12:01:22.000000 csnlp-1.5.5/src/csnlp/multistart/__init__.py
--rw-rw-rw-   0        0        0    15829 2023-06-02 17:10:40.000000 csnlp-1.5.5/src/csnlp/multistart/multistart_nlp.py
--rw-rw-rw-   0        0        0     3831 2023-03-20 12:48:12.000000 csnlp-1.5.5/src/csnlp/multistart/startpoints.py
-drwxrwxrwx   0        0        0        0 2023-06-02 17:17:48.911677 csnlp-1.5.5/src/csnlp/nlps/
--rw-rw-rw-   0        0        0    12295 2023-04-05 14:05:07.000000 csnlp-1.5.5/src/csnlp/nlps/constraints.py
--rw-rw-rw-   0        0        0     9068 2023-04-05 14:05:07.000000 csnlp-1.5.5/src/csnlp/nlps/nlp.py
--rw-rw-rw-   0        0        0     9584 2023-06-02 17:10:40.000000 csnlp-1.5.5/src/csnlp/nlps/objective.py
--rw-rw-rw-   0        0        0     2039 2023-03-25 14:04:48.000000 csnlp-1.5.5/src/csnlp/nlps/parameters.py
--rw-rw-rw-   0        0        0     2030 2023-03-25 14:01:54.000000 csnlp-1.5.5/src/csnlp/nlps/variables.py
-drwxrwxrwx   0        0        0        0 2023-06-02 17:17:48.929036 csnlp-1.5.5/src/csnlp/util/
--rw-rw-rw-   0        0        0     5231 2023-03-26 20:40:12.000000 csnlp-1.5.5/src/csnlp/util/docs.py
--rw-rw-rw-   0        0        0    11398 2023-03-25 13:36:29.000000 csnlp-1.5.5/src/csnlp/util/io.py
--rw-rw-rw-   0        0        0     5187 2023-04-05 14:05:07.000000 csnlp-1.5.5/src/csnlp/util/math.py
--rw-rw-rw-   0        0        0     3455 2023-03-24 17:58:30.000000 csnlp-1.5.5/src/csnlp/util/plot.py
--rw-rw-rw-   0        0        0      920 2023-03-17 16:33:38.000000 csnlp-1.5.5/src/csnlp/util/random.py
-drwxrwxrwx   0        0        0        0 2023-06-02 17:17:48.946460 csnlp-1.5.5/src/csnlp/wrappers/
--rw-rw-rw-   0        0        0      294 2023-03-29 19:05:51.000000 csnlp-1.5.5/src/csnlp/wrappers/__init__.py
--rw-rw-rw-   0        0        0    16506 2023-03-25 14:29:46.000000 csnlp-1.5.5/src/csnlp/wrappers/mpc.py
--rw-rw-rw-   0        0        0     7474 2023-02-16 10:51:07.000000 csnlp-1.5.5/src/csnlp/wrappers/scaling.py
--rw-rw-rw-   0        0        0    16282 2023-04-04 11:47:09.000000 csnlp-1.5.5/src/csnlp/wrappers/sensitivity.py
--rw-rw-rw-   0        0        0     3644 2023-01-07 17:14:55.000000 csnlp-1.5.5/src/csnlp/wrappers/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-06-02 17:17:48.865631 csnlp-1.5.5/src/csnlp.egg-info/
--rw-rw-rw-   0        0        0     7069 2023-06-02 17:17:48.000000 csnlp-1.5.5/src/csnlp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1040 2023-06-02 17:17:48.000000 csnlp-1.5.5/src/csnlp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 17:17:48.000000 csnlp-1.5.5/src/csnlp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       87 2023-06-02 17:17:48.000000 csnlp-1.5.5/src/csnlp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-02 17:17:48.000000 csnlp-1.5.5/src/csnlp.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-02 17:17:48.978647 csnlp-1.5.5/tests/
--rw-rw-rw-   0        0        0    13201 2023-03-29 19:49:44.000000 csnlp-1.5.5/tests/test_core.py
--rw-rw-rw-   0        0        0    10172 2023-04-05 14:05:07.000000 csnlp-1.5.5/tests/test_examples.py
--rw-rw-rw-   0        0        0     7610 2023-03-22 17:16:32.000000 csnlp-1.5.5/tests/test_multistart.py
--rw-rw-rw-   0        0        0    25071 2023-04-05 14:05:07.000000 csnlp-1.5.5/tests/test_nlps.py
--rw-rw-rw-   0        0        0    27469 2023-03-17 16:39:02.000000 csnlp-1.5.5/tests/test_quadrotor_mpc.py
--rw-rw-rw-   0        0        0     8655 2023-04-05 13:15:57.000000 csnlp-1.5.5/tests/test_util.py
--rw-rw-rw-   0        0        0    28699 2023-04-05 14:05:07.000000 csnlp-1.5.5/tests/test_wrappers.py
+drwxrwxrwx   0        0        0        0 2023-06-20 15:28:23.141423 csnlp-1.5.6/
+-rw-rw-rw-   0        0        0     1093 2022-11-02 20:11:46.000000 csnlp-1.5.6/LICENSE
+-rw-rw-rw-   0        0        0     7065 2023-06-20 15:28:23.139434 csnlp-1.5.6/PKG-INFO
+-rw-rw-rw-   0        0        0     6263 2023-06-20 12:25:01.000000 csnlp-1.5.6/README.md
+-rw-rw-rw-   0        0        0     1155 2023-06-20 12:25:08.000000 csnlp-1.5.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-20 15:28:23.142065 csnlp-1.5.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-20 15:28:23.006753 csnlp-1.5.6/src/
+drwxrwxrwx   0        0        0        0 2023-06-20 15:28:23.029001 csnlp-1.5.6/src/csnlp/
+-rw-rw-rw-   0        0        0      210 2023-04-04 11:47:09.000000 csnlp-1.5.6/src/csnlp/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 15:28:23.069034 csnlp-1.5.6/src/csnlp/core/
+-rw-rw-rw-   0        0        0     3267 2023-01-02 20:43:22.000000 csnlp-1.5.6/src/csnlp/core/cache.py
+-rw-rw-rw-   0        0        0     3186 2023-04-04 11:47:09.000000 csnlp-1.5.6/src/csnlp/core/data.py
+-rw-rw-rw-   0        0        0     6057 2023-03-24 10:24:25.000000 csnlp-1.5.6/src/csnlp/core/debug.py
+-rw-rw-rw-   0        0        0     2085 2023-02-16 10:35:36.000000 csnlp-1.5.6/src/csnlp/core/derivatives.py
+-rw-rw-rw-   0        0        0     5241 2023-02-16 10:40:42.000000 csnlp-1.5.6/src/csnlp/core/scaling.py
+-rw-rw-rw-   0        0        0     6426 2023-03-23 22:24:06.000000 csnlp-1.5.6/src/csnlp/core/solutions.py
+drwxrwxrwx   0        0        0        0 2023-06-20 15:28:23.077428 csnlp-1.5.6/src/csnlp/multistart/
+-rw-rw-rw-   0        0        0      425 2023-03-20 12:01:22.000000 csnlp-1.5.6/src/csnlp/multistart/__init__.py
+-rw-rw-rw-   0        0        0    15829 2023-06-20 15:25:08.000000 csnlp-1.5.6/src/csnlp/multistart/multistart_nlp.py
+-rw-rw-rw-   0        0        0     3800 2023-06-20 15:25:49.000000 csnlp-1.5.6/src/csnlp/multistart/startpoints.py
+drwxrwxrwx   0        0        0        0 2023-06-20 15:28:23.091469 csnlp-1.5.6/src/csnlp/nlps/
+-rw-rw-rw-   0        0        0    12297 2023-06-20 12:25:40.000000 csnlp-1.5.6/src/csnlp/nlps/constraints.py
+-rw-rw-rw-   0        0        0     9068 2023-04-05 14:05:07.000000 csnlp-1.5.6/src/csnlp/nlps/nlp.py
+-rw-rw-rw-   0        0        0     9584 2023-06-20 15:25:08.000000 csnlp-1.5.6/src/csnlp/nlps/objective.py
+-rw-rw-rw-   0        0        0     2039 2023-03-25 14:04:48.000000 csnlp-1.5.6/src/csnlp/nlps/parameters.py
+-rw-rw-rw-   0        0        0     2030 2023-03-25 14:01:54.000000 csnlp-1.5.6/src/csnlp/nlps/variables.py
+drwxrwxrwx   0        0        0        0 2023-06-20 15:28:23.103237 csnlp-1.5.6/src/csnlp/util/
+-rw-rw-rw-   0        0        0     5231 2023-03-26 20:40:12.000000 csnlp-1.5.6/src/csnlp/util/docs.py
+-rw-rw-rw-   0        0        0    11398 2023-03-25 13:36:29.000000 csnlp-1.5.6/src/csnlp/util/io.py
+-rw-rw-rw-   0        0        0     5187 2023-04-05 14:05:07.000000 csnlp-1.5.6/src/csnlp/util/math.py
+-rw-rw-rw-   0        0        0     3455 2023-03-24 17:58:30.000000 csnlp-1.5.6/src/csnlp/util/plot.py
+drwxrwxrwx   0        0        0        0 2023-06-20 15:28:23.117443 csnlp-1.5.6/src/csnlp/wrappers/
+-rw-rw-rw-   0        0        0      294 2023-03-29 19:05:51.000000 csnlp-1.5.6/src/csnlp/wrappers/__init__.py
+-rw-rw-rw-   0        0        0    16506 2023-03-25 14:29:46.000000 csnlp-1.5.6/src/csnlp/wrappers/mpc.py
+-rw-rw-rw-   0        0        0     7474 2023-02-16 10:51:07.000000 csnlp-1.5.6/src/csnlp/wrappers/scaling.py
+-rw-rw-rw-   0        0        0    16282 2023-04-04 11:47:09.000000 csnlp-1.5.6/src/csnlp/wrappers/sensitivity.py
+-rw-rw-rw-   0        0        0     3644 2023-01-07 17:14:55.000000 csnlp-1.5.6/src/csnlp/wrappers/wrapper.py
+drwxrwxrwx   0        0        0        0 2023-06-20 15:28:23.044057 csnlp-1.5.6/src/csnlp.egg-info/
+-rw-rw-rw-   0        0        0     7065 2023-06-20 15:28:22.000000 csnlp-1.5.6/src/csnlp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1015 2023-06-20 15:28:22.000000 csnlp-1.5.6/src/csnlp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 15:28:22.000000 csnlp-1.5.6/src/csnlp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       87 2023-06-20 15:28:22.000000 csnlp-1.5.6/src/csnlp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-20 15:28:22.000000 csnlp-1.5.6/src/csnlp.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-20 15:28:23.137180 csnlp-1.5.6/tests/
+-rw-rw-rw-   0        0        0    13201 2023-03-29 19:49:44.000000 csnlp-1.5.6/tests/test_core.py
+-rw-rw-rw-   0        0        0    10143 2023-06-20 15:25:49.000000 csnlp-1.5.6/tests/test_examples.py
+-rw-rw-rw-   0        0        0     7610 2023-03-22 17:16:32.000000 csnlp-1.5.6/tests/test_multistart.py
+-rw-rw-rw-   0        0        0    25071 2023-04-05 14:05:07.000000 csnlp-1.5.6/tests/test_nlps.py
+-rw-rw-rw-   0        0        0    27440 2023-06-20 15:25:49.000000 csnlp-1.5.6/tests/test_quadrotor_mpc.py
+-rw-rw-rw-   0        0        0     8151 2023-06-20 15:25:49.000000 csnlp-1.5.6/tests/test_util.py
+-rw-rw-rw-   0        0        0    28699 2023-04-05 14:05:07.000000 csnlp-1.5.6/tests/test_wrappers.py
```

### Comparing `csnlp-1.5.5/LICENSE` & `csnlp-1.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.5/PKG-INFO` & `csnlp-1.5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csnlp
-Version: 1.5.5
+Version: 1.5.6
 Summary: Nonlinear Progamming with CasADi
 Author-email: Filippo Airaldi <filippoairaldi@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/FilippoAiraldi/casadi-nlp
 Project-URL: Bug Tracker, https://github.com/FilippoAiraldi/casadi-nlp/issues
 Keywords: nonlinear-optimization,casadi,sensitivity-analysis
 Classifier: Programming Language :: Python :: 3.8
@@ -21,15 +21,15 @@
 # Nonlinear Programming with CasADi
 
 **csnlp** provides classes and utilities to model, solve and analyse nonlinear programmes (NLPs) in optimization.
 
 In particular, it makes use of the [CasADi](https://web.casadi.org/) framework [[1]](#1) to model the optimization problems and perform symbolic differentiation, as well as the [IPOPT](https://github.com/coin-or/Ipopt) solver [[2]](#2) (though the package can be adapted to other solvers pretty easily). The package offers also tools for the sensitivity analysis of NLPs, solving them with multiple initial conditions, as well as for building MPC controllers.
 
 [![PyPI version](https://badge.fury.io/py/csnlp.svg)](https://badge.fury.io/py/csnlp)
-[![Source Code License](https://img.shields.io/badge/license-MIT-blueviolet)](https://github.com/FilippoAiraldi/casadi-nlp/blob/release/LICENSE)
+[![Source Code License](https://img.shields.io/badge/license-MIT-blueviolet)](https://github.com/FilippoAiraldi/casadi-nlp/blob/dev/LICENSE)
 ![Python 3.8](https://img.shields.io/badge/python->=3.8-green.svg)
 
 [![Tests](https://github.com/FilippoAiraldi/casadi-nlp/actions/workflows/ci.yml/badge.svg)](https://github.com/FilippoAiraldi/casadi-nlp/actions/workflows/ci.yml)
 [![Downloads](https://pepy.tech/badge/csnlp)](https://pepy.tech/project/csnlp)
 [![Maintainability](https://api.codeclimate.com/v1/badges/d1cf537cff6af1a08508/maintainability)](https://codeclimate.com/github/FilippoAiraldi/casadi-nlp/maintainability)
 [![Test Coverage](https://api.codeclimate.com/v1/badges/d1cf537cff6af1a08508/test_coverage)](https://codeclimate.com/github/FilippoAiraldi/casadi-nlp/test_coverage)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
```

### Comparing `csnlp-1.5.5/README.md` & `csnlp-1.5.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Nonlinear Programming with CasADi
 
 **csnlp** provides classes and utilities to model, solve and analyse nonlinear programmes (NLPs) in optimization.
 
 In particular, it makes use of the [CasADi](https://web.casadi.org/) framework [[1]](#1) to model the optimization problems and perform symbolic differentiation, as well as the [IPOPT](https://github.com/coin-or/Ipopt) solver [[2]](#2) (though the package can be adapted to other solvers pretty easily). The package offers also tools for the sensitivity analysis of NLPs, solving them with multiple initial conditions, as well as for building MPC controllers.
 
 [![PyPI version](https://badge.fury.io/py/csnlp.svg)](https://badge.fury.io/py/csnlp)
-[![Source Code License](https://img.shields.io/badge/license-MIT-blueviolet)](https://github.com/FilippoAiraldi/casadi-nlp/blob/release/LICENSE)
+[![Source Code License](https://img.shields.io/badge/license-MIT-blueviolet)](https://github.com/FilippoAiraldi/casadi-nlp/blob/dev/LICENSE)
 ![Python 3.8](https://img.shields.io/badge/python->=3.8-green.svg)
 
 [![Tests](https://github.com/FilippoAiraldi/casadi-nlp/actions/workflows/ci.yml/badge.svg)](https://github.com/FilippoAiraldi/casadi-nlp/actions/workflows/ci.yml)
 [![Downloads](https://pepy.tech/badge/csnlp)](https://pepy.tech/project/csnlp)
 [![Maintainability](https://api.codeclimate.com/v1/badges/d1cf537cff6af1a08508/maintainability)](https://codeclimate.com/github/FilippoAiraldi/casadi-nlp/maintainability)
 [![Test Coverage](https://api.codeclimate.com/v1/badges/d1cf537cff6af1a08508/test_coverage)](https://codeclimate.com/github/FilippoAiraldi/casadi-nlp/test_coverage)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
```

### Comparing `csnlp-1.5.5/pyproject.toml` & `csnlp-1.5.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "csnlp"
-version = "1.5.5"
+version = "1.5.6"
 authors = [
   { name="Filippo Airaldi", email="filippoairaldi@gmail.com" },
 ]
 description = "Nonlinear Progamming with CasADi"
 readme = "README.md"
 requires-python = ">=3.8"
 license = { text = "MIT" }
```

### Comparing `csnlp-1.5.5/src/csnlp/core/cache.py` & `csnlp-1.5.6/src/csnlp/core/cache.py`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.5/src/csnlp/core/data.py` & `csnlp-1.5.6/src/csnlp/core/data.py`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.5/src/csnlp/core/debug.py` & `csnlp-1.5.6/src/csnlp/core/debug.py`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.5/src/csnlp/core/derivatives.py` & `csnlp-1.5.6/src/csnlp/core/derivatives.py`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.5/src/csnlp/core/scaling.py` & `csnlp-1.5.6/src/csnlp/core/scaling.py`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.5/src/csnlp/core/solutions.py` & `csnlp-1.5.6/src/csnlp/core/solutions.py`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.5/src/csnlp/multistart/multistart_nlp.py` & `csnlp-1.5.6/src/csnlp/multistart/multistart_nlp.py`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.5/src/csnlp/multistart/startpoints.py` & `csnlp-1.5.6/src/csnlp/multistart/startpoints.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 from typing import Any, Dict, Generator, NamedTuple, Optional
 
 import numpy as np
 import numpy.typing as npt
 
-from csnlp.util.random import np_random
-
 
 class RandomStartPoint:
     """Class containing all the information to guide the random generation of this
     point."""
 
     __slots__ = ("method", "args", "kwargs")
 
@@ -50,15 +48,15 @@
         multistarts : int
             The number of multiple start points.
         seed : int, optional
             RNG seed.
         """
         self.points = points
         self.multistarts = multistarts
-        self.np_random = np_random(seed)
+        self.np_random = np.random.default_rng(seed)
 
     def __iter__(self) -> Generator[Dict[str, npt.ArrayLike], None, None]:
         """Iterates over the random start points, yielding each time a different set."""
         points = self.points.items()
         yield from (
             {
                 n: getattr(self.np_random, p.method)(*p.args, **p.kwargs)
```

### Comparing `csnlp-1.5.5/src/csnlp/nlps/constraints.py` & `csnlp-1.5.6/src/csnlp/nlps/constraints.py`

 * *Files 0% similar despite different names*

```diff
@@ -214,20 +214,21 @@
         Raises
         ------
         ValueError
             Raises if there is already another variable with the same name; or if any
             element of the lower bound is larger than the corresponding lower bound
             element.
         """
-        var = super().variable(name, shape)
-
         lb = np.broadcast_to(lb, shape).reshape(-1, order="F")
         ub = np.broadcast_to(ub, shape).reshape(-1, order="F")
         if np.any(lb > ub):
             raise ValueError("Improper variable bounds.")
+
+        var = super().variable(name, shape)
+
         mlb: np.ma.MaskedArray = np.ma.masked_array(lb, np.ma.nomask)
         mub: np.ma.MaskedArray = np.ma.masked_array(ub, np.ma.nomask)
         if self._remove_redundant_x_bounds:
             mlb.mask = lb == -np.inf
             mub.mask = ub == +np.inf
 
         self._lbx = np.ma.concatenate((self._lbx, mlb))
```

### Comparing `csnlp-1.5.5/src/csnlp/nlps/nlp.py` & `csnlp-1.5.6/src/csnlp/nlps/nlp.py`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.5/src/csnlp/nlps/objective.py` & `csnlp-1.5.6/src/csnlp/nlps/objective.py`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.5/src/csnlp/nlps/parameters.py` & `csnlp-1.5.6/src/csnlp/nlps/parameters.py`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.5/src/csnlp/nlps/variables.py` & `csnlp-1.5.6/src/csnlp/nlps/variables.py`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.5/src/csnlp/util/docs.py` & `csnlp-1.5.6/src/csnlp/util/docs.py`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.5/src/csnlp/util/io.py` & `csnlp-1.5.6/src/csnlp/util/io.py`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.5/src/csnlp/util/math.py` & `csnlp-1.5.6/src/csnlp/util/math.py`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.5/src/csnlp/util/plot.py` & `csnlp-1.5.6/src/csnlp/util/plot.py`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.5/src/csnlp/wrappers/mpc.py` & `csnlp-1.5.6/src/csnlp/wrappers/mpc.py`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.5/src/csnlp/wrappers/scaling.py` & `csnlp-1.5.6/src/csnlp/wrappers/scaling.py`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.5/src/csnlp/wrappers/sensitivity.py` & `csnlp-1.5.6/src/csnlp/wrappers/sensitivity.py`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.5/src/csnlp/wrappers/wrapper.py` & `csnlp-1.5.6/src/csnlp/wrappers/wrapper.py`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.5/src/csnlp.egg-info/PKG-INFO` & `csnlp-1.5.6/src/csnlp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csnlp
-Version: 1.5.5
+Version: 1.5.6
 Summary: Nonlinear Progamming with CasADi
 Author-email: Filippo Airaldi <filippoairaldi@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/FilippoAiraldi/casadi-nlp
 Project-URL: Bug Tracker, https://github.com/FilippoAiraldi/casadi-nlp/issues
 Keywords: nonlinear-optimization,casadi,sensitivity-analysis
 Classifier: Programming Language :: Python :: 3.8
@@ -21,15 +21,15 @@
 # Nonlinear Programming with CasADi
 
 **csnlp** provides classes and utilities to model, solve and analyse nonlinear programmes (NLPs) in optimization.
 
 In particular, it makes use of the [CasADi](https://web.casadi.org/) framework [[1]](#1) to model the optimization problems and perform symbolic differentiation, as well as the [IPOPT](https://github.com/coin-or/Ipopt) solver [[2]](#2) (though the package can be adapted to other solvers pretty easily). The package offers also tools for the sensitivity analysis of NLPs, solving them with multiple initial conditions, as well as for building MPC controllers.
 
 [![PyPI version](https://badge.fury.io/py/csnlp.svg)](https://badge.fury.io/py/csnlp)
-[![Source Code License](https://img.shields.io/badge/license-MIT-blueviolet)](https://github.com/FilippoAiraldi/casadi-nlp/blob/release/LICENSE)
+[![Source Code License](https://img.shields.io/badge/license-MIT-blueviolet)](https://github.com/FilippoAiraldi/casadi-nlp/blob/dev/LICENSE)
 ![Python 3.8](https://img.shields.io/badge/python->=3.8-green.svg)
 
 [![Tests](https://github.com/FilippoAiraldi/casadi-nlp/actions/workflows/ci.yml/badge.svg)](https://github.com/FilippoAiraldi/casadi-nlp/actions/workflows/ci.yml)
 [![Downloads](https://pepy.tech/badge/csnlp)](https://pepy.tech/project/csnlp)
 [![Maintainability](https://api.codeclimate.com/v1/badges/d1cf537cff6af1a08508/maintainability)](https://codeclimate.com/github/FilippoAiraldi/casadi-nlp/maintainability)
 [![Test Coverage](https://api.codeclimate.com/v1/badges/d1cf537cff6af1a08508/test_coverage)](https://codeclimate.com/github/FilippoAiraldi/casadi-nlp/test_coverage)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
```

### Comparing `csnlp-1.5.5/src/csnlp.egg-info/SOURCES.txt` & `csnlp-1.5.6/src/csnlp.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 src/csnlp/nlps/objective.py
 src/csnlp/nlps/parameters.py
 src/csnlp/nlps/variables.py
 src/csnlp/util/docs.py
 src/csnlp/util/io.py
 src/csnlp/util/math.py
 src/csnlp/util/plot.py
-src/csnlp/util/random.py
 src/csnlp/wrappers/__init__.py
 src/csnlp/wrappers/mpc.py
 src/csnlp/wrappers/scaling.py
 src/csnlp/wrappers/sensitivity.py
 src/csnlp/wrappers/wrapper.py
 tests/test_core.py
 tests/test_examples.py
```

### Comparing `csnlp-1.5.5/tests/test_core.py` & `csnlp-1.5.6/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.5/tests/test_examples.py` & `csnlp-1.5.6/tests/test_examples.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import numpy as np
 from parameterized import parameterized, parameterized_class
 from scipy import io
 
 from csnlp import Nlp, Solution, scaling, wrappers
 from csnlp.multistart import ParallelMultistartNlp, StackedMultistartNlp
 from csnlp.multistart.multistart_nlp import MultistartNlp
-from csnlp.util.random import np_random
 
 OPTS = {
     "expand": True,
     "print_time": False,
     "ipopt": {
         "max_iter": 500,
         "sb": "yes",
@@ -212,15 +211,15 @@
         K = 3
         dt = T / N
         m0 = 500000
         yT = 100000
         g = 9.81
         alpha = 1 / (300 * g)
         seed = 69
-        rng = np_random(seed)
+        rng = np.random.default_rng(seed)
         kwargs = {"n_jobs": -1} if multinlp_cls is ParallelMultistartNlp else {}
         nlp = multinlp_cls(sym_type="SX", starts=K, **kwargs)
 
         y_nom = 1e5
         v_nom = 2e3
         m_nom = 3e5
         x_nom = cs.vertcat(y_nom, v_nom, m_nom)
```

### Comparing `csnlp-1.5.5/tests/test_multistart.py` & `csnlp-1.5.6/tests/test_multistart.py`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.5/tests/test_nlps.py` & `csnlp-1.5.6/tests/test_nlps.py`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.5/tests/test_quadrotor_mpc.py` & `csnlp-1.5.6/tests/test_quadrotor_mpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
 import casadi as cs
 import numpy as np
 from parameterized import parameterized
 
 from csnlp import Nlp, Solution
 from csnlp.util.math import quad_form
-from csnlp.util.random import np_random
 from csnlp.wrappers import Mpc
 
 
 @dataclass
 class QuadRotorEnvConfig:
     T: float = 0.1
     g: float = 9.81
@@ -129,15 +128,15 @@
             assert alt.ndim == 1, "Altitudes must be a vector"
 
         return np.vstack([np.exp(-np.square(alt - h)) for h in self.config.winds])
 
     def reset(
         self, seed: int = None, x0: np.ndarray = None, xf: np.ndarray = None
     ) -> np.ndarray:
-        self.np_random = np_random(seed)
+        self.np_random = np.random.default_rng(seed)
         if x0 is None:
             x0 = self.config.x0
         if xf is None:
             xf = self.config.xf
         self.x = x0
         self.config.x0 = x0
         self.config.xf = xf
```

### Comparing `csnlp-1.5.5/tests/test_util.py` & `csnlp-1.5.6/tests/test_util.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 import casadi as cs
 import numpy as np
 from parameterized import parameterized
 from scipy.stats import norm
 
 from csnlp.core.solutions import subsevalf
-from csnlp.util import io, math, random
+from csnlp.util import io, math
 
 TMPFILENAME: str = ""
 
 
 class EmptyClass(io.SupportsDeepcopyAndPickle):
     ...
 
@@ -231,22 +231,9 @@
         ]
     )
     def test_repeat(self, inputs, expected):
         actual = math.repeat(*inputs)
         np.testing.assert_array_equal(actual, expected)
 
 
-class TestRandom(unittest.TestCase):
-    def test_np_random__raises__with_invalid_seed(self):
-        with self.assertRaisesRegex(
-            ValueError, "Seed must be a non-negative integer or omitted, not -1."
-        ):
-            random.np_random(-1)
-
-    @parameterized.expand([(69,), (None,)])
-    def test_np_random__initializes_rng_with_correct_seed(self, seed: Optional[int]):
-        rng = random.np_random(seed)
-        self.assertIsInstance(rng, np.random.Generator)
-
-
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `csnlp-1.5.5/tests/test_wrappers.py` & `csnlp-1.5.6/tests/test_wrappers.py`

 * *Files identical despite different names*

