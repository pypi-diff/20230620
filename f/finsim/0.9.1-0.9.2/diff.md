# Comparing `tmp/finsim-0.9.1.tar.gz` & `tmp/finsim-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/finsim-0.9.1.tar", last modified: Mon Apr  4 14:24:47 2022, max compression
+gzip compressed data, was "dist/finsim-0.9.2.tar", last modified: Fri Sep 30 02:05:57 2022, max compression
```

## Comparing `finsim-0.9.1.tar` & `finsim-0.9.2.tar`

### file list

```diff
@@ -1,62 +1,63 @@
-drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2022-04-04 14:24:47.641466 finsim-0.9.1/
--rw-r--r--   0 stephenhky   (501) staff       (20)    26433 2020-09-28 01:25:03.000000 finsim-0.9.1/LICENSE
--rw-r--r--   0 stephenhky   (501) staff       (20)      353 2022-04-03 21:48:56.000000 finsim-0.9.1/MANIFEST.in
--rw-r--r--   0 stephenhky   (501) staff       (20)     1115 2022-04-04 14:24:47.640956 finsim-0.9.1/PKG-INFO
--rw-r--r--   0 stephenhky   (501) staff       (20)     1083 2022-04-03 21:48:56.000000 finsim-0.9.1/README.md
-drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2022-04-04 14:24:47.591685 finsim-0.9.1/finsim/
--rw-r--r--   0 stephenhky   (501) staff       (20)       17 2021-01-05 19:13:37.000000 finsim-0.9.1/finsim/__init__.py
-drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2022-04-04 14:24:47.601927 finsim-0.9.1/finsim/data/
--rw-r--r--   0 stephenhky   (501) staff       (20)      117 2020-09-26 16:53:01.000000 finsim-0.9.1/finsim/data/__init__.py
--rw-r--r--   0 stephenhky   (501) staff       (20)     1373 2020-09-20 16:38:34.000000 finsim-0.9.1/finsim/data/finnhub.py
--rw-r--r--   0 stephenhky   (501) staff       (20)    10942 2022-04-03 21:48:56.000000 finsim-0.9.1/finsim/data/preader.py
--rw-r--r--   0 stephenhky   (501) staff       (20)      578 2020-09-24 20:48:13.000000 finsim-0.9.1/finsim/data/quandl.py
-drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2022-04-04 14:24:47.606615 finsim-0.9.1/finsim/estimate/
--rw-r--r--   0 stephenhky   (501) staff       (20)        0 2020-09-24 20:53:37.000000 finsim-0.9.1/finsim/estimate/__init__.py
--rw-r--r--   0 stephenhky   (501) staff       (20)      149 2020-11-19 04:09:58.000000 finsim-0.9.1/finsim/estimate/constants.py
--rw-r--r--   0 stephenhky   (501) staff       (20)     3248 2022-04-03 21:48:56.000000 finsim-0.9.1/finsim/estimate/fit.py
-drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2022-04-04 14:24:47.616603 finsim-0.9.1/finsim/estimate/native/
--rw-r--r--   0 stephenhky   (501) staff       (20)        0 2022-04-04 14:24:02.000000 finsim-0.9.1/finsim/estimate/native/__init__.py
--rw-r--r--   0 stephenhky   (501) staff       (20)   289188 2022-04-04 14:24:45.000000 finsim-0.9.1/finsim/estimate/native/cythonfit.c
--rw-r--r--   0 stephenhky   (501) staff       (20)     1261 2022-04-03 21:48:56.000000 finsim-0.9.1/finsim/estimate/native/cythonfit.pyx
--rw-r--r--   0 stephenhky   (501) staff       (20)   244242 2022-04-03 21:49:04.000000 finsim-0.9.1/finsim/estimate/native/cythonrisk.c
--rw-r--r--   0 stephenhky   (501) staff       (20)     1194 2022-02-09 20:10:49.000000 finsim-0.9.1/finsim/estimate/native/cythonrisk.pyx
--rw-r--r--   0 stephenhky   (501) staff       (20)      589 2022-04-03 21:48:56.000000 finsim-0.9.1/finsim/estimate/native/pyfit.py
--rw-r--r--   0 stephenhky   (501) staff       (20)      746 2022-02-09 20:10:49.000000 finsim-0.9.1/finsim/estimate/native/pyrisk.py
--rw-r--r--   0 stephenhky   (501) staff       (20)     2125 2022-04-03 21:49:05.000000 finsim-0.9.1/finsim/estimate/risk.py
-drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2022-04-04 14:24:47.621800 finsim-0.9.1/finsim/portfolio/
--rw-r--r--   0 stephenhky   (501) staff       (20)      388 2022-02-09 20:10:49.000000 finsim-0.9.1/finsim/portfolio/__init__.py
--rw-r--r--   0 stephenhky   (501) staff       (20)     4303 2022-04-03 21:48:56.000000 finsim-0.9.1/finsim/portfolio/create.py
--rw-r--r--   0 stephenhky   (501) staff       (20)    10448 2022-02-09 20:10:49.000000 finsim-0.9.1/finsim/portfolio/dynamic.py
--rw-r--r--   0 stephenhky   (501) staff       (20)     1013 2022-04-03 21:48:56.000000 finsim-0.9.1/finsim/portfolio/helper.py
-drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2022-04-04 14:24:47.625161 finsim-0.9.1/finsim/portfolio/optimize/
--rw-r--r--   0 stephenhky   (501) staff       (20)        0 2020-11-18 04:11:27.000000 finsim-0.9.1/finsim/portfolio/optimize/__init__.py
--rw-r--r--   0 stephenhky   (501) staff       (20)     1453 2022-04-03 21:48:56.000000 finsim-0.9.1/finsim/portfolio/optimize/metrics.py
-drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2022-04-04 14:24:47.629591 finsim-0.9.1/finsim/portfolio/optimize/native/
--rw-r--r--   0 stephenhky   (501) staff       (20)        1 2022-04-04 14:24:02.000000 finsim-0.9.1/finsim/portfolio/optimize/native/__init__.py
--rw-r--r--   0 stephenhky   (501) staff       (20)   318037 2022-04-04 14:24:45.000000 finsim-0.9.1/finsim/portfolio/optimize/native/cythonmetrics.c
--rw-r--r--   0 stephenhky   (501) staff       (20)     1606 2022-04-03 21:48:56.000000 finsim-0.9.1/finsim/portfolio/optimize/native/cythonmetrics.pyx
--rw-r--r--   0 stephenhky   (501) staff       (20)     1011 2022-02-09 20:10:49.000000 finsim-0.9.1/finsim/portfolio/optimize/native/pymetrics.py
--rw-r--r--   0 stephenhky   (501) staff       (20)    10107 2022-04-03 21:48:56.000000 finsim-0.9.1/finsim/portfolio/optimize/numerics.py
--rw-r--r--   0 stephenhky   (501) staff       (20)     8314 2021-09-16 04:37:30.000000 finsim-0.9.1/finsim/portfolio/optimize/policy.py
--rw-r--r--   0 stephenhky   (501) staff       (20)     7700 2022-04-03 21:48:56.000000 finsim-0.9.1/finsim/portfolio/portfolio.py
-drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2022-04-04 14:24:47.630952 finsim-0.9.1/finsim/simulation/
--rw-r--r--   0 stephenhky   (501) staff       (20)        0 2020-09-09 13:49:43.000000 finsim-0.9.1/finsim/simulation/__init__.py
--rw-r--r--   0 stephenhky   (501) staff       (20)     4210 2022-04-03 21:48:56.000000 finsim-0.9.1/finsim/simulation/stock.py
-drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2022-04-04 14:24:47.597783 finsim-0.9.1/finsim.egg-info/
--rw-r--r--   0 stephenhky   (501) staff       (20)     1115 2022-04-04 14:24:47.000000 finsim-0.9.1/finsim.egg-info/PKG-INFO
--rw-r--r--   0 stephenhky   (501) staff       (20)     1381 2022-04-04 14:24:47.000000 finsim-0.9.1/finsim.egg-info/SOURCES.txt
--rw-r--r--   0 stephenhky   (501) staff       (20)        1 2022-04-04 14:24:47.000000 finsim-0.9.1/finsim.egg-info/dependency_links.txt
--rw-r--r--   0 stephenhky   (501) staff       (20)        1 2020-10-01 04:33:45.000000 finsim-0.9.1/finsim.egg-info/not-zip-safe
--rw-r--r--   0 stephenhky   (501) staff       (20)      147 2022-04-04 14:24:47.000000 finsim-0.9.1/finsim.egg-info/requires.txt
--rw-r--r--   0 stephenhky   (501) staff       (20)        7 2022-04-04 14:24:47.000000 finsim-0.9.1/finsim.egg-info/top_level.txt
--rw-r--r--   0 stephenhky   (501) staff       (20)      147 2022-04-03 21:48:56.000000 finsim-0.9.1/requirements.txt
--rw-r--r--   0 stephenhky   (501) staff       (20)       38 2022-04-04 14:24:47.641626 finsim-0.9.1/setup.cfg
--rw-r--r--   0 stephenhky   (501) staff       (20)     2861 2022-04-04 14:12:37.000000 finsim-0.9.1/setup.py
-drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2022-04-04 14:24:47.639724 finsim-0.9.1/test/
--rw-r--r--   0 stephenhky   (501) staff       (20)      720 2022-04-03 21:48:56.000000 finsim-0.9.1/test/test_data.py
--rw-r--r--   0 stephenhky   (501) staff       (20)     2551 2022-02-09 20:10:49.000000 finsim-0.9.1/test/test_dynamic.py
--rw-r--r--   0 stephenhky   (501) staff       (20)     1333 2022-04-03 21:48:56.000000 finsim-0.9.1/test/test_fit.py
--rw-r--r--   0 stephenhky   (501) staff       (20)     2858 2022-04-03 21:48:56.000000 finsim-0.9.1/test/test_metrics.py
--rw-r--r--   0 stephenhky   (501) staff       (20)     3553 2022-04-03 21:48:56.000000 finsim-0.9.1/test/test_portfolio.py
--rw-r--r--   0 stephenhky   (501) staff       (20)     2504 2022-04-04 13:33:34.000000 finsim-0.9.1/test/test_risk.py
--rw-r--r--   0 stephenhky   (501) staff       (20)     3798 2022-04-03 21:48:56.000000 finsim-0.9.1/test/test_stock_simulations.py
+drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2022-09-30 02:05:57.906965 finsim-0.9.2/
+-rw-r--r--   0 stephenhky   (501) staff       (20)    26433 2020-09-28 01:25:03.000000 finsim-0.9.2/LICENSE
+-rw-r--r--   0 stephenhky   (501) staff       (20)      376 2022-09-30 02:05:19.000000 finsim-0.9.2/MANIFEST.in
+-rw-r--r--   0 stephenhky   (501) staff       (20)     1115 2022-09-30 02:05:57.906305 finsim-0.9.2/PKG-INFO
+-rw-r--r--   0 stephenhky   (501) staff       (20)     1083 2022-04-03 21:48:56.000000 finsim-0.9.2/README.md
+drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2022-09-30 02:05:57.863842 finsim-0.9.2/finsim/
+-rw-r--r--   0 stephenhky   (501) staff       (20)       17 2021-01-05 19:13:37.000000 finsim-0.9.2/finsim/__init__.py
+drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2022-09-30 02:05:57.871963 finsim-0.9.2/finsim/data/
+-rw-r--r--   0 stephenhky   (501) staff       (20)      117 2020-09-26 16:53:01.000000 finsim-0.9.2/finsim/data/__init__.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)     1373 2020-09-20 16:38:34.000000 finsim-0.9.2/finsim/data/finnhub.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)    10942 2022-04-03 21:48:56.000000 finsim-0.9.2/finsim/data/preader.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)      578 2020-09-24 20:48:13.000000 finsim-0.9.2/finsim/data/quandl.py
+drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2022-09-30 02:05:57.876500 finsim-0.9.2/finsim/estimate/
+-rw-r--r--   0 stephenhky   (501) staff       (20)        0 2020-09-24 20:53:37.000000 finsim-0.9.2/finsim/estimate/__init__.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)      149 2020-11-19 04:09:58.000000 finsim-0.9.2/finsim/estimate/constants.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)     3248 2022-04-03 21:48:56.000000 finsim-0.9.2/finsim/estimate/fit.py
+drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2022-09-30 02:05:57.887077 finsim-0.9.2/finsim/estimate/native/
+-rw-r--r--   0 stephenhky   (501) staff       (20)        0 2022-04-04 14:24:02.000000 finsim-0.9.2/finsim/estimate/native/__init__.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)   289188 2022-04-04 14:24:45.000000 finsim-0.9.2/finsim/estimate/native/cythonfit.c
+-rw-r--r--   0 stephenhky   (501) staff       (20)     1261 2022-04-03 21:48:56.000000 finsim-0.9.2/finsim/estimate/native/cythonfit.pyx
+-rw-r--r--   0 stephenhky   (501) staff       (20)   244242 2022-04-03 21:49:04.000000 finsim-0.9.2/finsim/estimate/native/cythonrisk.c
+-rw-r--r--   0 stephenhky   (501) staff       (20)     1194 2022-02-09 20:10:49.000000 finsim-0.9.2/finsim/estimate/native/cythonrisk.pyx
+-rw-r--r--   0 stephenhky   (501) staff       (20)      589 2022-04-03 21:48:56.000000 finsim-0.9.2/finsim/estimate/native/pyfit.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)      746 2022-02-09 20:10:49.000000 finsim-0.9.2/finsim/estimate/native/pyrisk.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)     2125 2022-04-03 21:49:05.000000 finsim-0.9.2/finsim/estimate/risk.py
+drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2022-09-30 02:05:57.890995 finsim-0.9.2/finsim/portfolio/
+-rw-r--r--   0 stephenhky   (501) staff       (20)      388 2022-02-09 20:10:49.000000 finsim-0.9.2/finsim/portfolio/__init__.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)     4303 2022-04-03 21:48:56.000000 finsim-0.9.2/finsim/portfolio/create.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)    10448 2022-02-09 20:10:49.000000 finsim-0.9.2/finsim/portfolio/dynamic.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)     1013 2022-04-03 21:48:56.000000 finsim-0.9.2/finsim/portfolio/helper.py
+drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2022-09-30 02:05:57.893524 finsim-0.9.2/finsim/portfolio/optimize/
+-rw-r--r--   0 stephenhky   (501) staff       (20)        0 2020-11-18 04:11:27.000000 finsim-0.9.2/finsim/portfolio/optimize/__init__.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)     1453 2022-04-03 21:48:56.000000 finsim-0.9.2/finsim/portfolio/optimize/metrics.py
+drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2022-09-30 02:05:57.898291 finsim-0.9.2/finsim/portfolio/optimize/native/
+-rw-r--r--   0 stephenhky   (501) staff       (20)        1 2022-04-04 14:24:02.000000 finsim-0.9.2/finsim/portfolio/optimize/native/__init__.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)   318037 2022-04-04 14:24:45.000000 finsim-0.9.2/finsim/portfolio/optimize/native/cythonmetrics.c
+-rw-r--r--   0 stephenhky   (501) staff       (20)     1606 2022-04-03 21:48:56.000000 finsim-0.9.2/finsim/portfolio/optimize/native/cythonmetrics.pyx
+-rw-r--r--   0 stephenhky   (501) staff       (20)     1011 2022-02-09 20:10:49.000000 finsim-0.9.2/finsim/portfolio/optimize/native/pymetrics.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)    10107 2022-04-03 21:48:56.000000 finsim-0.9.2/finsim/portfolio/optimize/numerics.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)     8305 2022-09-30 02:05:19.000000 finsim-0.9.2/finsim/portfolio/optimize/policy.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)     7700 2022-04-03 21:48:56.000000 finsim-0.9.2/finsim/portfolio/portfolio.py
+drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2022-09-30 02:05:57.899381 finsim-0.9.2/finsim/simulation/
+-rw-r--r--   0 stephenhky   (501) staff       (20)        0 2020-09-09 13:49:43.000000 finsim-0.9.2/finsim/simulation/__init__.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)     4210 2022-04-03 21:48:56.000000 finsim-0.9.2/finsim/simulation/stock.py
+drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2022-09-30 02:05:57.868198 finsim-0.9.2/finsim.egg-info/
+-rw-r--r--   0 stephenhky   (501) staff       (20)     1115 2022-09-30 02:05:57.000000 finsim-0.9.2/finsim.egg-info/PKG-INFO
+-rw-r--r--   0 stephenhky   (501) staff       (20)     1396 2022-09-30 02:05:57.000000 finsim-0.9.2/finsim.egg-info/SOURCES.txt
+-rw-r--r--   0 stephenhky   (501) staff       (20)        1 2022-09-30 02:05:57.000000 finsim-0.9.2/finsim.egg-info/dependency_links.txt
+-rw-r--r--   0 stephenhky   (501) staff       (20)        1 2020-10-01 04:33:45.000000 finsim-0.9.2/finsim.egg-info/not-zip-safe
+-rw-r--r--   0 stephenhky   (501) staff       (20)      147 2022-09-30 02:05:57.000000 finsim-0.9.2/finsim.egg-info/requires.txt
+-rw-r--r--   0 stephenhky   (501) staff       (20)        7 2022-09-30 02:05:57.000000 finsim-0.9.2/finsim.egg-info/top_level.txt
+-rw-r--r--   0 stephenhky   (501) staff       (20)       83 2022-09-30 02:05:19.000000 finsim-0.9.2/pyproject.toml
+-rw-r--r--   0 stephenhky   (501) staff       (20)      147 2022-04-03 21:48:56.000000 finsim-0.9.2/requirements.txt
+-rw-r--r--   0 stephenhky   (501) staff       (20)       38 2022-09-30 02:05:57.907131 finsim-0.9.2/setup.cfg
+-rw-r--r--   0 stephenhky   (501) staff       (20)     2247 2022-09-30 02:05:33.000000 finsim-0.9.2/setup.py
+drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2022-09-30 02:05:57.905415 finsim-0.9.2/test/
+-rw-r--r--   0 stephenhky   (501) staff       (20)      720 2022-04-03 21:48:56.000000 finsim-0.9.2/test/test_data.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)     2551 2022-02-09 20:10:49.000000 finsim-0.9.2/test/test_dynamic.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)     1333 2022-04-03 21:48:56.000000 finsim-0.9.2/test/test_fit.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)     2858 2022-04-03 21:48:56.000000 finsim-0.9.2/test/test_metrics.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)     3553 2022-04-03 21:48:56.000000 finsim-0.9.2/test/test_portfolio.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)     2504 2022-04-04 13:33:34.000000 finsim-0.9.2/test/test_risk.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)     3798 2022-04-03 21:48:56.000000 finsim-0.9.2/test/test_stock_simulations.py
```

### Comparing `finsim-0.9.1/LICENSE` & `finsim-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `finsim-0.9.1/PKG-INFO` & `finsim-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finsim
-Version: 0.9.1
+Version: 0.9.2
 Summary: Financial simulation and inference
 Home-page: https://github.com/stephenhky/FinanceSimulation
 Author: Kwan-Yuet Ho
 Author-email: stephenhky@yahoo.com.hk
 License: LGPL
 Description: ## Introduction
```

### Comparing `finsim-0.9.1/README.md` & `finsim-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `finsim-0.9.1/finsim/data/finnhub.py` & `finsim-0.9.2/finsim/data/finnhub.py`

 * *Files identical despite different names*

### Comparing `finsim-0.9.1/finsim/data/preader.py` & `finsim-0.9.2/finsim/data/preader.py`

 * *Files identical despite different names*

### Comparing `finsim-0.9.1/finsim/data/quandl.py` & `finsim-0.9.2/finsim/data/quandl.py`

 * *Files identical despite different names*

### Comparing `finsim-0.9.1/finsim/estimate/fit.py` & `finsim-0.9.2/finsim/estimate/fit.py`

 * *Files identical despite different names*

### Comparing `finsim-0.9.1/finsim/estimate/native/cythonfit.c` & `finsim-0.9.2/finsim/estimate/native/cythonfit.c`

 * *Files identical despite different names*

### Comparing `finsim-0.9.1/finsim/estimate/native/cythonfit.pyx` & `finsim-0.9.2/finsim/estimate/native/cythonfit.pyx`

 * *Files identical despite different names*

### Comparing `finsim-0.9.1/finsim/estimate/native/cythonrisk.c` & `finsim-0.9.2/finsim/estimate/native/cythonrisk.c`

 * *Files identical despite different names*

### Comparing `finsim-0.9.1/finsim/estimate/native/cythonrisk.pyx` & `finsim-0.9.2/finsim/estimate/native/cythonrisk.pyx`

 * *Files identical despite different names*

### Comparing `finsim-0.9.1/finsim/estimate/native/pyfit.py` & `finsim-0.9.2/finsim/estimate/native/pyfit.py`

 * *Files identical despite different names*

### Comparing `finsim-0.9.1/finsim/estimate/native/pyrisk.py` & `finsim-0.9.2/finsim/estimate/native/pyrisk.py`

 * *Files identical despite different names*

### Comparing `finsim-0.9.1/finsim/estimate/risk.py` & `finsim-0.9.2/finsim/estimate/risk.py`

 * *Files identical despite different names*

### Comparing `finsim-0.9.1/finsim/portfolio/create.py` & `finsim-0.9.2/finsim/portfolio/create.py`

 * *Files identical despite different names*

### Comparing `finsim-0.9.1/finsim/portfolio/dynamic.py` & `finsim-0.9.2/finsim/portfolio/dynamic.py`

 * *Files identical despite different names*

### Comparing `finsim-0.9.1/finsim/portfolio/helper.py` & `finsim-0.9.2/finsim/portfolio/helper.py`

 * *Files identical despite different names*

### Comparing `finsim-0.9.1/finsim/portfolio/optimize/metrics.py` & `finsim-0.9.2/finsim/portfolio/optimize/metrics.py`

 * *Files identical despite different names*

### Comparing `finsim-0.9.1/finsim/portfolio/optimize/native/cythonmetrics.c` & `finsim-0.9.2/finsim/portfolio/optimize/native/cythonmetrics.c`

 * *Files identical despite different names*

### Comparing `finsim-0.9.1/finsim/portfolio/optimize/native/cythonmetrics.pyx` & `finsim-0.9.2/finsim/portfolio/optimize/native/cythonmetrics.pyx`

 * *Files identical despite different names*

### Comparing `finsim-0.9.1/finsim/portfolio/optimize/native/pymetrics.py` & `finsim-0.9.2/finsim/portfolio/optimize/native/pymetrics.py`

 * *Files identical despite different names*

### Comparing `finsim-0.9.1/finsim/portfolio/optimize/numerics.py` & `finsim-0.9.2/finsim/portfolio/optimize/numerics.py`

 * *Files identical despite different names*

### Comparing `finsim-0.9.1/finsim/portfolio/optimize/policy.py` & `finsim-0.9.2/finsim/portfolio/optimize/policy.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,15 +103,15 @@
         super(OptimizedWeightingPolicyUsingMPTSharpeRatio, self).optimize(r, cov, symbols=symbols)
         self.optimized_sol = optimized_portfolio_on_sharperatio(r, cov, self.rf, minweight=self.minweight)
         self.optimized = True
 
         self.optimized_weights = self.optimized_sol.x
         self.optimized_sharpe_ratio = -self.optimized_sol.fun
         self.optimized_portfolio_yield = np.sum(self.optimized_weights * self.r)
-        sqweights = np.matmul(
+        sqweights = np.dot(
             np.expand_dims(self.optimized_weights, axis=1),
             np.expand_dims(self.optimized_weights, axis=0)
         )
         self.optimized_volatility = np.sqrt(np.sum(sqweights * self.cov))
 
     @property
     def weights(self):
@@ -154,15 +154,15 @@
         self.optimized_sol = optimized_portfolio_mpt_costfunction(r, cov, self.rf, self.lamb, V0=self.V0)
         self.optimized = True
 
         self.optimized_unnormalized_weights = self.optimized_sol.x
         self.optimized_weights = self.optimized_unnormalized_weights[:-1] / np.sum(self.optimized_unnormalized_weights[:-1])
         self.optimized_costfunction = -self.optimized_sol.fun
         self.optimized_portfolio_yield = np.sum(self.optimized_weights * self.r)
-        sqweights = np.matmul(
+        sqweights = np.dot(
             np.expand_dims(self.optimized_weights, axis=1),
             np.expand_dims(self.optimized_weights, axis=0)
         )
         self.optimized_volatility = np.sqrt(np.sum(sqweights * self.cov))
 
     @property
     def weights(self):
@@ -208,15 +208,15 @@
         self.optimized_sol = optimized_portfolio_mpt_entropy_costfunction(r, cov, self.rf, self.lamb0, self.lamb1, V=self.V)
         self.optimized = True
 
         self.optimized_unnormalized_weights = self.optimized_sol.x
         self.optimized_weights = self.optimized_unnormalized_weights[:-1] / np.sum(self.optimized_unnormalized_weights[:-1])
         self.optimized_costfunction = -self.optimized_sol.fun
         self.optimized_portfolio_yield = np.sum(self.optimized_weights * self.r)
-        sqweights = np.matmul(
+        sqweights = np.dot(
             np.expand_dims(self.optimized_weights, axis=1),
             np.expand_dims(self.optimized_weights, axis=0)
         )
         self.optimized_volatility = np.sqrt(np.sum(sqweights * self.cov))
 
     @property
     def weights(self):
```

### Comparing `finsim-0.9.1/finsim/portfolio/portfolio.py` & `finsim-0.9.2/finsim/portfolio/portfolio.py`

 * *Files identical despite different names*

### Comparing `finsim-0.9.1/finsim/simulation/stock.py` & `finsim-0.9.2/finsim/simulation/stock.py`

 * *Files identical despite different names*

### Comparing `finsim-0.9.1/finsim.egg-info/PKG-INFO` & `finsim-0.9.2/finsim.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finsim
-Version: 0.9.1
+Version: 0.9.2
 Summary: Financial simulation and inference
 Home-page: https://github.com/stephenhky/FinanceSimulation
 Author: Kwan-Yuet Ho
 Author-email: stephenhky@yahoo.com.hk
 License: LGPL
 Description: ## Introduction
```

### Comparing `finsim-0.9.1/finsim.egg-info/SOURCES.txt` & `finsim-0.9.2/finsim.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 MANIFEST.in
 README.md
+pyproject.toml
 requirements.txt
 setup.py
 finsim/__init__.py
 finsim.egg-info/PKG-INFO
 finsim.egg-info/SOURCES.txt
 finsim.egg-info/dependency_links.txt
 finsim.egg-info/not-zip-safe
```

### Comparing `finsim-0.9.1/setup.py` & `finsim-0.9.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,16 @@
 
-# Reference: https://stackoverflow.com/questions/7932028/setup-py-for-packages-that-depend-on-both-cython-and-f2py
-
 from setuptools import setup
-
-try:
-    from Cython.Build import cythonize
-    ext_modules = cythonize(['finsim/portfolio/optimize/native/cythonmetrics.pyx',
-                             'finsim/estimate/native/cythonfit.pyx',
-                             'finsim/estimate/native/cythonrisk.pyx'])
-except ImportError:
-    from setuptools import Extension
-    ext_modules = [
-        Extension('finsim.portfolio.optimize.native.cynthonmetrics',
-                  sources=['finsim/portfolio/optimize/native/cythonmetrics.c']),
-        Extension('finsim.estimate.native.cythonfit',
-                  sources=['finsim/estimate/native/cythonfit.c']),
-        Extension('finsim.estimate.native.cythonrisk',
-                  sources=['finsim/estimate/native/cythonrisk.c'])
-    ]
-
 import numpy as np
 
+from Cython.Build import cythonize
+ext_modules = cythonize(['finsim/portfolio/optimize/native/cythonmetrics.pyx',
+                         'finsim/estimate/native/cythonfit.pyx',
+                         'finsim/estimate/native/cythonrisk.pyx'])
+
 
 def readme():
     with open('README.md') as f:
         return f.read()
 
 
 def install_requirements():
@@ -35,15 +21,15 @@
     text = open('README.md', 'r').read()
     startpos = text.find('## Introduction')
     return text[startpos:]
 
 
 setup(
     name='finsim',
-    version="0.9.1",
+    version="0.9.2",
     description="Financial simulation and inference",
     long_description=package_description(),
     long_description_content_type='text/markdown',
     classifiers=[
       "Topic :: Scientific/Engineering :: Mathematics",
       "Topic :: Software Development :: Libraries :: Python Modules",
       "Topic :: Software Development :: Version Control :: Git",
```

### Comparing `finsim-0.9.1/test/test_data.py` & `finsim-0.9.2/test/test_data.py`

 * *Files identical despite different names*

### Comparing `finsim-0.9.1/test/test_dynamic.py` & `finsim-0.9.2/test/test_dynamic.py`

 * *Files identical despite different names*

### Comparing `finsim-0.9.1/test/test_fit.py` & `finsim-0.9.2/test/test_fit.py`

 * *Files identical despite different names*

### Comparing `finsim-0.9.1/test/test_metrics.py` & `finsim-0.9.2/test/test_metrics.py`

 * *Files identical despite different names*

### Comparing `finsim-0.9.1/test/test_portfolio.py` & `finsim-0.9.2/test/test_portfolio.py`

 * *Files identical despite different names*

### Comparing `finsim-0.9.1/test/test_risk.py` & `finsim-0.9.2/test/test_risk.py`

 * *Files identical despite different names*

### Comparing `finsim-0.9.1/test/test_stock_simulations.py` & `finsim-0.9.2/test/test_stock_simulations.py`

 * *Files identical despite different names*

