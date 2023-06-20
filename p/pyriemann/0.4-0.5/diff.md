# Comparing `tmp/pyriemann-0.4.tar.gz` & `tmp/pyriemann-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyriemann-0.4.tar", last modified: Wed Feb 15 09:30:47 2023, max compression
+gzip compressed data, was "pyriemann-0.5.tar", last modified: Tue Jun 20 08:33:53 2023, max compression
```

## Comparing `pyriemann-0.4.tar` & `pyriemann-0.5.tar`

### file list

```diff
@@ -1,51 +1,77 @@
-drwxr-xr-x   0 agramfort   (501) staff       (20)        0 2023-02-15 09:30:47.554520 pyriemann-0.4/
--rw-r--r--   0 agramfort   (501) staff       (20)     1527 2023-02-15 09:25:27.000000 pyriemann-0.4/LICENSE
--rw-r--r--   0 agramfort   (501) staff       (20)       18 2022-11-12 16:58:51.000000 pyriemann-0.4/MANIFEST.in
--rw-r--r--   0 agramfort   (501) staff       (20)     7486 2023-02-15 09:30:47.554804 pyriemann-0.4/PKG-INFO
--rw-r--r--   0 agramfort   (501) staff       (20)     6902 2023-02-15 09:07:33.000000 pyriemann-0.4/README.md
-drwxr-xr-x   0 agramfort   (501) staff       (20)        0 2023-02-15 09:30:46.669335 pyriemann-0.4/pyriemann/
--rw-r--r--   0 agramfort   (501) staff       (20)      521 2022-11-12 16:58:51.000000 pyriemann-0.4/pyriemann/__init__.py
--rw-r--r--   0 agramfort   (501) staff       (20)       20 2023-02-15 09:09:39.000000 pyriemann-0.4/pyriemann/_version.py
--rw-r--r--   0 agramfort   (501) staff       (20)     6273 2022-11-28 12:50:02.000000 pyriemann-0.4/pyriemann/channelselection.py
--rw-r--r--   0 agramfort   (501) staff       (20)    36510 2022-12-15 08:43:19.000000 pyriemann-0.4/pyriemann/classification.py
--rw-r--r--   0 agramfort   (501) staff       (20)    27861 2022-11-28 12:50:02.000000 pyriemann-0.4/pyriemann/clustering.py
-drwxr-xr-x   0 agramfort   (501) staff       (20)        0 2023-02-15 09:30:46.865209 pyriemann-0.4/pyriemann/datasets/
--rw-r--r--   0 agramfort   (501) staff       (20)      452 2022-11-28 12:50:02.000000 pyriemann-0.4/pyriemann/datasets/__init__.py
--rwxr-xr-x   0 agramfort   (501) staff       (20)    19680 2022-11-28 12:50:02.000000 pyriemann-0.4/pyriemann/datasets/sampling.py
--rw-r--r--   0 agramfort   (501) staff       (20)    14064 2022-11-28 12:50:02.000000 pyriemann-0.4/pyriemann/datasets/simulated.py
--rw-r--r--   0 agramfort   (501) staff       (20)    13723 2022-11-28 12:50:02.000000 pyriemann-0.4/pyriemann/embedding.py
--rw-r--r--   0 agramfort   (501) staff       (20)    28705 2023-01-30 09:59:14.000000 pyriemann-0.4/pyriemann/estimation.py
--rw-r--r--   0 agramfort   (501) staff       (20)     7442 2022-11-12 16:58:51.000000 pyriemann-0.4/pyriemann/preprocessing.py
--rw-r--r--   0 agramfort   (501) staff       (20)     8497 2022-11-28 12:50:02.000000 pyriemann-0.4/pyriemann/regression.py
--rw-r--r--   0 agramfort   (501) staff       (20)    28997 2022-12-15 08:43:00.000000 pyriemann-0.4/pyriemann/spatialfilters.py
--rw-r--r--   0 agramfort   (501) staff       (20)    15089 2022-12-02 21:11:39.000000 pyriemann-0.4/pyriemann/stats.py
--rw-r--r--   0 agramfort   (501) staff       (20)    12756 2022-12-02 21:11:39.000000 pyriemann-0.4/pyriemann/tangentspace.py
-drwxr-xr-x   0 agramfort   (501) staff       (20)        0 2023-02-15 09:30:47.257006 pyriemann-0.4/pyriemann/transfer/
--rw-r--r--   0 agramfort   (501) staff       (20)      438 2022-11-28 12:50:03.000000 pyriemann-0.4/pyriemann/transfer/__init__.py
--rw-r--r--   0 agramfort   (501) staff       (20)    31348 2022-11-28 12:50:03.000000 pyriemann-0.4/pyriemann/transfer/_estimators.py
--rw-r--r--   0 agramfort   (501) staff       (20)     7664 2022-11-28 12:50:03.000000 pyriemann-0.4/pyriemann/transfer/_rotate.py
--rw-r--r--   0 agramfort   (501) staff       (20)     5031 2022-11-28 12:50:03.000000 pyriemann-0.4/pyriemann/transfer/_tools.py
-drwxr-xr-x   0 agramfort   (501) staff       (20)        0 2023-02-15 09:30:47.548297 pyriemann-0.4/pyriemann/utils/
--rw-r--r--   0 agramfort   (501) staff       (20)      745 2022-11-12 16:58:51.000000 pyriemann-0.4/pyriemann/utils/__init__.py
--rw-r--r--   0 agramfort   (501) staff       (20)    10256 2022-11-28 12:50:03.000000 pyriemann-0.4/pyriemann/utils/ajd.py
--rw-r--r--   0 agramfort   (501) staff       (20)     5905 2023-02-15 09:07:33.000000 pyriemann-0.4/pyriemann/utils/base.py
--rw-r--r--   0 agramfort   (501) staff       (20)    26664 2023-02-15 09:07:33.000000 pyriemann-0.4/pyriemann/utils/covariance.py
--rw-r--r--   0 agramfort   (501) staff       (20)    11450 2023-02-15 09:07:33.000000 pyriemann-0.4/pyriemann/utils/distance.py
--rw-r--r--   0 agramfort   (501) staff       (20)     2888 2022-11-12 16:58:51.000000 pyriemann-0.4/pyriemann/utils/docs.py
--rw-r--r--   0 agramfort   (501) staff       (20)     3439 2022-11-12 16:58:51.000000 pyriemann-0.4/pyriemann/utils/geodesic.py
--rw-r--r--   0 agramfort   (501) staff       (20)     7600 2023-01-30 09:59:14.000000 pyriemann-0.4/pyriemann/utils/kernel.py
--rw-r--r--   0 agramfort   (501) staff       (20)    24388 2022-11-28 12:50:03.000000 pyriemann-0.4/pyriemann/utils/mean.py
--rw-r--r--   0 agramfort   (501) staff       (20)     5764 2022-12-02 21:11:39.000000 pyriemann-0.4/pyriemann/utils/median.py
--rw-r--r--   0 agramfort   (501) staff       (20)    11128 2022-11-28 12:50:03.000000 pyriemann-0.4/pyriemann/utils/tangentspace.py
--rw-r--r--   0 agramfort   (501) staff       (20)     4370 2023-02-15 09:07:33.000000 pyriemann-0.4/pyriemann/utils/test.py
--rw-r--r--   0 agramfort   (501) staff       (20)     2008 2022-11-28 12:50:03.000000 pyriemann-0.4/pyriemann/utils/utils.py
--rw-r--r--   0 agramfort   (501) staff       (20)     8604 2022-11-28 12:50:03.000000 pyriemann-0.4/pyriemann/utils/viz.py
-drwxr-xr-x   0 agramfort   (501) staff       (20)        0 2023-02-15 09:30:46.751436 pyriemann-0.4/pyriemann.egg-info/
--rw-r--r--   0 agramfort   (501) staff       (20)     7486 2023-02-15 09:30:46.000000 pyriemann-0.4/pyriemann.egg-info/PKG-INFO
--rw-r--r--   0 agramfort   (501) staff       (20)     1124 2023-02-15 09:30:46.000000 pyriemann-0.4/pyriemann.egg-info/SOURCES.txt
--rw-r--r--   0 agramfort   (501) staff       (20)        1 2023-02-15 09:30:46.000000 pyriemann-0.4/pyriemann.egg-info/dependency_links.txt
--rw-r--r--   0 agramfort   (501) staff       (20)        1 2022-11-22 13:46:30.000000 pyriemann-0.4/pyriemann.egg-info/not-zip-safe
--rw-r--r--   0 agramfort   (501) staff       (20)      145 2023-02-15 09:30:46.000000 pyriemann-0.4/pyriemann.egg-info/requires.txt
--rw-r--r--   0 agramfort   (501) staff       (20)       10 2023-02-15 09:30:46.000000 pyriemann-0.4/pyriemann.egg-info/top_level.txt
--rw-r--r--   0 agramfort   (501) staff       (20)      182 2023-02-15 09:30:47.557399 pyriemann-0.4/setup.cfg
--rw-r--r--   0 agramfort   (501) staff       (20)     1714 2023-01-30 09:59:14.000000 pyriemann-0.4/setup.py
+drwxr-xr-x   0 plcrodrigues   (501) staff       (20)        0 2023-06-20 08:33:53.908144 pyriemann-0.5/
+-rw-r--r--   0 plcrodrigues   (501) staff       (20)     1527 2023-05-09 10:50:37.000000 pyriemann-0.5/LICENSE
+-rw-r--r--   0 plcrodrigues   (501) staff       (20)       18 2022-07-12 09:17:11.000000 pyriemann-0.5/MANIFEST.in
+-rw-r--r--   0 plcrodrigues   (501) staff       (20)     7514 2023-06-20 08:33:53.908227 pyriemann-0.5/PKG-INFO
+-rw-r--r--   0 plcrodrigues   (501) staff       (20)     6930 2023-06-16 09:10:00.000000 pyriemann-0.5/README.md
+drwxr-xr-x   0 plcrodrigues   (501) staff       (20)        0 2023-06-20 08:33:53.896208 pyriemann-0.5/pyriemann/
+-rw-r--r--   0 plcrodrigues   (501) staff       (20)      521 2023-06-19 12:13:12.000000 pyriemann-0.5/pyriemann/__init__.py
+-rw-r--r--   0 plcrodrigues   (501) staff       (20)       20 2023-06-20 08:28:01.000000 pyriemann-0.5/pyriemann/_version.py
+-rw-r--r--   0 plcrodrigues   (501) staff       (20)     6273 2023-02-15 09:15:26.000000 pyriemann-0.5/pyriemann/channelselection.py
+-rw-r--r--   0 plcrodrigues   (501) staff       (20)    36629 2023-06-19 13:13:37.000000 pyriemann-0.5/pyriemann/classification.py
+-rw-r--r--   0 plcrodrigues   (501) staff       (20)    27622 2023-06-16 09:10:00.000000 pyriemann-0.5/pyriemann/clustering.py
+drwxr-xr-x   0 plcrodrigues   (501) staff       (20)        0 2023-06-20 08:33:53.898133 pyriemann-0.5/pyriemann/datasets/
+-rw-r--r--   0 plcrodrigues   (501) staff       (20)      456 2023-06-16 09:10:00.000000 pyriemann-0.5/pyriemann/datasets/__init__.py
+-rwxr-xr-x   0 plcrodrigues   (501) staff       (20)    20032 2023-06-20 08:10:03.000000 pyriemann-0.5/pyriemann/datasets/sampling.py
+-rw-r--r--   0 plcrodrigues   (501) staff       (20)    17672 2023-06-19 13:13:37.000000 pyriemann-0.5/pyriemann/datasets/simulated.py
+-rw-r--r--   0 plcrodrigues   (501) staff       (20)    13538 2023-06-16 09:10:00.000000 pyriemann-0.5/pyriemann/embedding.py
+-rw-r--r--   0 plcrodrigues   (501) staff       (20)    28565 2023-06-16 09:10:00.000000 pyriemann-0.5/pyriemann/estimation.py
+-rw-r--r--   0 plcrodrigues   (501) staff       (20)     7442 2023-02-15 09:15:26.000000 pyriemann-0.5/pyriemann/preprocessing.py
+-rw-r--r--   0 plcrodrigues   (501) staff       (20)     8495 2023-06-16 09:10:00.000000 pyriemann-0.5/pyriemann/regression.py
+-rw-r--r--   0 plcrodrigues   (501) staff       (20)    28957 2023-06-19 13:13:37.000000 pyriemann-0.5/pyriemann/spatialfilters.py
+-rw-r--r--   0 plcrodrigues   (501) staff       (20)    15272 2023-06-19 13:13:37.000000 pyriemann-0.5/pyriemann/stats.py
+-rw-r--r--   0 plcrodrigues   (501) staff       (20)    12756 2023-02-15 09:15:26.000000 pyriemann-0.5/pyriemann/tangentspace.py
+drwxr-xr-x   0 plcrodrigues   (501) staff       (20)        0 2023-06-20 08:33:53.899166 pyriemann-0.5/pyriemann/transfer/
+-rw-r--r--   0 plcrodrigues   (501) staff       (20)      438 2023-02-15 09:15:26.000000 pyriemann-0.5/pyriemann/transfer/__init__.py
+-rw-r--r--   0 plcrodrigues   (501) staff       (20)    31390 2023-06-19 13:13:37.000000 pyriemann-0.5/pyriemann/transfer/_estimators.py
+-rw-r--r--   0 plcrodrigues   (501) staff       (20)     7662 2023-06-16 09:10:00.000000 pyriemann-0.5/pyriemann/transfer/_rotate.py
+-rw-r--r--   0 plcrodrigues   (501) staff       (20)     5025 2023-06-16 09:10:00.000000 pyriemann-0.5/pyriemann/transfer/_tools.py
+drwxr-xr-x   0 plcrodrigues   (501) staff       (20)        0 2023-06-20 08:33:53.902724 pyriemann-0.5/pyriemann/utils/
+-rw-r--r--   0 plcrodrigues   (501) staff       (20)      745 2023-02-15 09:15:26.000000 pyriemann-0.5/pyriemann/utils/__init__.py
+-rw-r--r--   0 plcrodrigues   (501) staff       (20)    10256 2023-02-15 09:15:26.000000 pyriemann-0.5/pyriemann/utils/ajd.py
+-rw-r--r--   0 plcrodrigues   (501) staff       (20)     6189 2023-06-16 09:10:00.000000 pyriemann-0.5/pyriemann/utils/base.py
+-rw-r--r--   0 plcrodrigues   (501) staff       (20)    26662 2023-06-16 09:10:00.000000 pyriemann-0.5/pyriemann/utils/covariance.py
+-rw-r--r--   0 plcrodrigues   (501) staff       (20)    16702 2023-06-19 13:13:37.000000 pyriemann-0.5/pyriemann/utils/distance.py
+-rw-r--r--   0 plcrodrigues   (501) staff       (20)     2888 2022-07-12 09:17:11.000000 pyriemann-0.5/pyriemann/utils/docs.py
+-rw-r--r--   0 plcrodrigues   (501) staff       (20)     3808 2023-06-16 09:10:00.000000 pyriemann-0.5/pyriemann/utils/geodesic.py
+-rw-r--r--   0 plcrodrigues   (501) staff       (20)     7687 2023-06-16 09:10:00.000000 pyriemann-0.5/pyriemann/utils/kernel.py
+-rw-r--r--   0 plcrodrigues   (501) staff       (20)    25249 2023-06-19 13:13:37.000000 pyriemann-0.5/pyriemann/utils/mean.py
+-rw-r--r--   0 plcrodrigues   (501) staff       (20)     5543 2023-06-19 13:13:37.000000 pyriemann-0.5/pyriemann/utils/median.py
+-rw-r--r--   0 plcrodrigues   (501) staff       (20)    10771 2023-06-16 09:10:00.000000 pyriemann-0.5/pyriemann/utils/tangentspace.py
+-rw-r--r--   0 plcrodrigues   (501) staff       (20)     5117 2023-06-16 09:10:00.000000 pyriemann-0.5/pyriemann/utils/test.py
+-rw-r--r--   0 plcrodrigues   (501) staff       (20)     2008 2023-06-16 09:10:00.000000 pyriemann-0.5/pyriemann/utils/utils.py
+-rw-r--r--   0 plcrodrigues   (501) staff       (20)     7624 2023-06-16 09:10:00.000000 pyriemann-0.5/pyriemann/utils/viz.py
+drwxr-xr-x   0 plcrodrigues   (501) staff       (20)        0 2023-06-20 08:33:53.897386 pyriemann-0.5/pyriemann.egg-info/
+-rw-r--r--   0 plcrodrigues   (501) staff       (20)     7514 2023-06-20 08:33:53.000000 pyriemann-0.5/pyriemann.egg-info/PKG-INFO
+-rw-r--r--   0 plcrodrigues   (501) staff       (20)     1783 2023-06-20 08:33:53.000000 pyriemann-0.5/pyriemann.egg-info/SOURCES.txt
+-rw-r--r--   0 plcrodrigues   (501) staff       (20)        1 2023-06-20 08:33:53.000000 pyriemann-0.5/pyriemann.egg-info/dependency_links.txt
+-rw-r--r--   0 plcrodrigues   (501) staff       (20)        1 2022-07-12 09:17:30.000000 pyriemann-0.5/pyriemann.egg-info/not-zip-safe
+-rw-r--r--   0 plcrodrigues   (501) staff       (20)      145 2023-06-20 08:33:53.000000 pyriemann-0.5/pyriemann.egg-info/requires.txt
+-rw-r--r--   0 plcrodrigues   (501) staff       (20)       10 2023-06-20 08:33:53.000000 pyriemann-0.5/pyriemann.egg-info/top_level.txt
+-rw-r--r--   0 plcrodrigues   (501) staff       (20)      182 2023-06-20 08:33:53.908509 pyriemann-0.5/setup.cfg
+-rw-r--r--   0 plcrodrigues   (501) staff       (20)     1719 2023-06-16 09:10:00.000000 pyriemann-0.5/setup.py
+drwxr-xr-x   0 plcrodrigues   (501) staff       (20)        0 2023-06-20 08:33:53.908008 pyriemann-0.5/tests/
+-rw-r--r--   0 plcrodrigues   (501) staff       (20)     1026 2022-07-12 09:17:11.000000 pyriemann-0.5/tests/test_channelselection.py
+-rw-r--r--   0 plcrodrigues   (501) staff       (20)    12791 2023-06-16 09:10:00.000000 pyriemann-0.5/tests/test_classification.py
+-rw-r--r--   0 plcrodrigues   (501) staff       (20)    11515 2023-06-16 09:10:00.000000 pyriemann-0.5/tests/test_clustering.py
+-rw-r--r--   0 plcrodrigues   (501) staff       (20)     6018 2023-06-16 09:10:00.000000 pyriemann-0.5/tests/test_embedding.py
+-rw-r--r--   0 plcrodrigues   (501) staff       (20)    11686 2023-02-15 09:15:26.000000 pyriemann-0.5/tests/test_estimation.py
+-rw-r--r--   0 plcrodrigues   (501) staff       (20)     3883 2023-06-16 09:10:00.000000 pyriemann-0.5/tests/test_preprocessing.py
+-rw-r--r--   0 plcrodrigues   (501) staff       (20)     7493 2023-06-16 09:10:00.000000 pyriemann-0.5/tests/test_regression.py
+-rw-r--r--   0 plcrodrigues   (501) staff       (20)     3426 2023-02-15 09:15:26.000000 pyriemann-0.5/tests/test_sampling.py
+-rw-r--r--   0 plcrodrigues   (501) staff       (20)     6457 2023-06-16 09:10:00.000000 pyriemann-0.5/tests/test_simulated.py
+-rw-r--r--   0 plcrodrigues   (501) staff       (20)    11694 2023-06-16 09:10:00.000000 pyriemann-0.5/tests/test_spatialfilters.py
+-rw-r--r--   0 plcrodrigues   (501) staff       (20)     2578 2022-07-12 09:17:11.000000 pyriemann-0.5/tests/test_stats.py
+-rw-r--r--   0 plcrodrigues   (501) staff       (20)     5039 2023-02-15 09:15:26.000000 pyriemann-0.5/tests/test_tangentspace.py
+-rw-r--r--   0 plcrodrigues   (501) staff       (20)    11477 2023-06-20 08:10:03.000000 pyriemann-0.5/tests/test_transfer.py
+-rw-r--r--   0 plcrodrigues   (501) staff       (20)     2630 2023-02-15 09:15:26.000000 pyriemann-0.5/tests/test_utils_ajd.py
+-rw-r--r--   0 plcrodrigues   (501) staff       (20)     4412 2023-06-16 09:10:00.000000 pyriemann-0.5/tests/test_utils_base.py
+-rw-r--r--   0 plcrodrigues   (501) staff       (20)    16131 2023-02-15 09:15:26.000000 pyriemann-0.5/tests/test_utils_covariance.py
+-rw-r--r--   0 plcrodrigues   (501) staff       (20)     9482 2023-06-19 13:13:37.000000 pyriemann-0.5/tests/test_utils_distance.py
+-rw-r--r--   0 plcrodrigues   (501) staff       (20)     3637 2023-06-16 09:10:00.000000 pyriemann-0.5/tests/test_utils_geodesic.py
+-rw-r--r--   0 plcrodrigues   (501) staff       (20)     3508 2023-06-16 09:10:00.000000 pyriemann-0.5/tests/test_utils_kernel.py
+-rw-r--r--   0 plcrodrigues   (501) staff       (20)    10391 2023-06-19 13:13:37.000000 pyriemann-0.5/tests/test_utils_mean.py
+-rw-r--r--   0 plcrodrigues   (501) staff       (20)     2765 2023-06-16 09:10:00.000000 pyriemann-0.5/tests/test_utils_median.py
+-rw-r--r--   0 plcrodrigues   (501) staff       (20)     4868 2023-06-16 09:10:00.000000 pyriemann-0.5/tests/test_utils_tangent_space.py
+-rw-r--r--   0 plcrodrigues   (501) staff       (20)     3420 2023-06-19 13:13:37.000000 pyriemann-0.5/tests/test_utils_test.py
+-rw-r--r--   0 plcrodrigues   (501) staff       (20)      908 2023-02-15 09:15:26.000000 pyriemann-0.5/tests/test_utils_utils.py
+-rw-r--r--   0 plcrodrigues   (501) staff       (20)     1451 2023-06-16 09:10:00.000000 pyriemann-0.5/tests/test_utils_viz.py
```

### Comparing `pyriemann-0.4/LICENSE` & `pyriemann-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyriemann-0.4/PKG-INFO` & `pyriemann-0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyriemann
-Version: 0.4
+Version: 0.5
 Summary: Biosignals classification with Riemannian geometry
 Home-page: https://pyriemann.readthedocs.io
 Author: Alexandre Barachant
 Author-email: alexandre.barachant@gmail.com
 License: BSD (3-clause)
 Project-URL: Documentation, https://pyriemann.readthedocs.io
 Project-URL: Source, https://github.com/pyRiemann/pyRiemann
@@ -52,29 +52,35 @@
 ```
 or using pip+git for the latest version of the code :
 
 ```
 pip install git+https://github.com/pyRiemann/pyRiemann
 ```
 
-Anaconda is not currently supported, if you want to use anaconda, you need to create a virtual environment in anaconda,
-activate it and use the above command to install it.
+#### Using conda
+
+The package is distributed via [conda-forge](https://conda-forge.org).
+You could install it in your working environment, with the following command:
+
+```shell
+conda install -c conda-forge pyriemann
+```
 
 #### From sources
 
-For the latest version, you can install the package from the sources using the setup.py script
+For the latest version, you can install the package from the sources using ``pip``:
 
-```
-python setup.py install
+```shell
+pip install .
 ```
 
-or in developer mode to be able to modify the sources.
+or in editable mode to be able to modify the sources:
 
-```
-python setup.py develop
+```shell
+pip install -e .
 ```
 
 ## How to use it
 
 Most of the functions mimic the scikit-learn API, and therefore can be directly used with sklearn.
 For example, for cross-validation classification of EEG signal using the MDM algorithm described in [[2]](#2), it is easy as:
```

### Comparing `pyriemann-0.4/README.md` & `pyriemann-0.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -34,29 +34,35 @@
 ```
 or using pip+git for the latest version of the code :
 
 ```
 pip install git+https://github.com/pyRiemann/pyRiemann
 ```
 
-Anaconda is not currently supported, if you want to use anaconda, you need to create a virtual environment in anaconda,
-activate it and use the above command to install it.
+#### Using conda
+
+The package is distributed via [conda-forge](https://conda-forge.org).
+You could install it in your working environment, with the following command:
+
+```shell
+conda install -c conda-forge pyriemann
+```
 
 #### From sources
 
-For the latest version, you can install the package from the sources using the setup.py script
+For the latest version, you can install the package from the sources using ``pip``:
 
-```
-python setup.py install
+```shell
+pip install .
 ```
 
-or in developer mode to be able to modify the sources.
+or in editable mode to be able to modify the sources:
 
-```
-python setup.py develop
+```shell
+pip install -e .
 ```
 
 ## How to use it
 
 Most of the functions mimic the scikit-learn API, and therefore can be directly used with sklearn.
 For example, for cross-validation classification of EEG signal using the MDM algorithm described in [[2]](#2), it is easy as:
```

### Comparing `pyriemann-0.4/pyriemann/__init__.py` & `pyriemann-0.5/pyriemann/__init__.py`

 * *Files identical despite different names*

### Comparing `pyriemann-0.4/pyriemann/channelselection.py` & `pyriemann-0.5/pyriemann/channelselection.py`

 * *Files identical despite different names*

### Comparing `pyriemann-0.4/pyriemann/classification.py` & `pyriemann-0.5/pyriemann/classification.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,15 +178,15 @@
 
     def fit_predict(self, X, y):
         """Fit and predict in one function."""
         self.fit(X, y)
         return self.predict(X)
 
     def predict_proba(self, X):
-        """Predict proba using softmax.
+        """Predict proba using softmax of negative squared distances.
 
         Parameters
         ----------
         X : ndarray, shape (n_matrices, n_channels, n_channels)
             Set of SPD matrices.
 
         Returns
@@ -814,15 +814,15 @@
         return self
 
     def _get_label(self, x, labs_unique):
         m = np.zeros((len(self.power_list), len(labs_unique)))
         for ip, p in enumerate(self.power_list):
             for ill, ll in enumerate(labs_unique):
                 m[ip, ill] = distance(
-                    x, self.covmeans_[p][ll], metric=self.metric) ** 2
+                    x, self.covmeans_[p][ll], metric=self.metric, squared=True)
 
         if self.method_label == 'sum_means':
             ipmin = np.argmin(np.sum(m, axis=1))
         elif self.method_label == 'inf_means':
             ipmin = np.where(m == np.min(m))[0][0]
         else:
             raise TypeError('method_label must be sum_means or inf_means')
@@ -857,16 +857,18 @@
         for x in X:
             m = {}
             for p in self.power_list:
                 m[p] = []
                 for ll in self.classes_:
                     m[p].append(
                         distance(
-                            x, self.covmeans_[p][ll], metric=self.metric
-                        ) ** 2
+                            x,
+                            self.covmeans_[p][ll],
+                            metric=self.metric,
+                        )
                     )
             pmin = min(m.items(), key=lambda x: np.sum(x[1]))[0]
             dist.append(np.array(m[pmin]))
 
         return np.stack(dist)
 
     def transform(self, X):
@@ -886,15 +888,15 @@
 
     def fit_predict(self, X, y):
         """Fit and predict in one function."""
         self.fit(X, y)
         return self.predict(X)
 
     def predict_proba(self, X):
-        """Predict proba using softmax.
+        """Predict proba using softmax of negative squared distances.
 
         Parameters
         ----------
         X : ndarray, shape (n_matrices, n_channels, n_channels)
             Set of SPD matrices.
 
         Returns
@@ -973,15 +975,15 @@
         True.
     denom : float
         Denominator value of class_dis. Returned only if return_num_denom is
         True.
 
     Notes
     -----
-    .. versionadded:: 0.3.1
+    .. versionadded:: 0.4
 
     References
     ----------
     .. [1] `Defining and quantifying users’ mental imagery-based
        BCI skills: a first step
        <https://hal.archives-ouvertes.fr/hal-01846434/>`_
        F. Lotte, and C. Jeunet. Journal of neural engineering,
```

### Comparing `pyriemann-0.4/pyriemann/clustering.py` & `pyriemann-0.5/pyriemann/clustering.py`

 * *Files 2% similar despite different names*

```diff
@@ -360,14 +360,17 @@
             self.metric
         )
 
         y_old = self._check_labels(X, y)
 
         for _ in range(self.n_iter_max):
             ix = (y_old == 1)
+            if not any(ix):
+                raise ValueError("Iterative outlier removal has rejected all "
+                                 "matrices. Choose a higher threshold.")
             self._mdm.fit(X[ix], y_old[ix])
             y = np.zeros(len(X))
             d = np.squeeze(np.log(self._mdm.transform(X[ix])))
             self._mean = np.mean(d)
             self._std = np.std(d)
             y[ix] = self._get_z_score(d) < self.threshold
 
@@ -520,14 +523,22 @@
 
     def _get_proba(self, z):
         """Get right-tailed proba from z-score."""
         proba = 1 - norm.cdf(z)
         return proba
 
 
+def _check_n_matrices(X, n_matrices):
+    """Check number of matrices in ndarray."""
+    if X.shape[0] != n_matrices:
+        raise ValueError(
+            'Unequal n_matrices between ndarray of X. Should be %d but'
+            ' got %d.' % (n_matrices, X.shape[0]))
+
+
 class PotatoField(BaseEstimator, TransformerMixin, ClassifierMixin):
     """Artefact detection with the Riemannian Potato Field.
 
     The Riemannian Potato Field [1]_ is a clustering method used to detect
     artifact in EEG signals. The algorithm combines several potatoes of low
     dimension, each one being designed to capture specific artifact typically
     affecting specific subsets of channels and/or specific frequency bands.
@@ -615,18 +626,15 @@
             metric=self.metric,
             threshold=self.z_threshold,
             n_iter_max=self.n_iter_max,
             pos_label=self.pos_label,
             neg_label=self.neg_label)
         self._potatoes = []
         for i in range(self.n_potatoes):
-            if X[i].shape[0] != n_matrices:
-                raise ValueError(
-                    'Unequal n_matrices between ndarray of X. Should be %d but'
-                    ' got %d.' % (n_matrices, X[i].shape[0]))
+            _check_n_matrices(X[i], n_matrices)
             self._potatoes.append(clone(pt))
             self._potatoes[i].fit(X[i], y)
 
         return self
 
     def partial_fit(self, X, y=None, alpha=0.1):
         """Partially fit the potato field from covariance matrices.
@@ -655,18 +663,15 @@
         self : PotatoField instance
             The PotatoField instance.
         """
         self._check_length(X)
         n_matrices = X[0].shape[0]
 
         for i in range(self.n_potatoes):
-            if X[i].shape[0] != n_matrices:
-                raise ValueError(
-                    'Unequal n_matrices between ndarray of X. Should be %d but'
-                    ' got %d.' % (n_matrices, X[i].shape[0]))
+            _check_n_matrices(X[i], n_matrices)
             self._potatoes[i].partial_fit(X[i], y, alpha=alpha)
         return self
 
     def transform(self, X):
         """Return the normalized log-distances to the centroids.
 
         Return the normalized log-distances to the centroids, ie geometric
@@ -687,18 +692,15 @@
             The normalized log-distances to the centroids.
         """
         self._check_length(X)
         n_matrices = X[0].shape[0]
 
         z = np.zeros((n_matrices, self.n_potatoes))
         for i in range(self.n_potatoes):
-            if X[i].shape[0] != n_matrices:
-                raise ValueError(
-                    'Unequal n_matrices between ndarray of X. Should be %d but'
-                    ' got %d.' % (n_matrices, X[i].shape[0]))
+            _check_n_matrices(X[i], n_matrices)
             z[:, i] = self._potatoes[i].transform(X[i])
         return z
 
     def predict(self, X):
         """Predict artefact from data.
 
         Parameters
@@ -744,18 +746,15 @@
             It is considered as abnormal/artifacted for low value of proba.
         """
         self._check_length(X)
         n_matrices = X[0].shape[0]
 
         p = np.zeros((self.n_potatoes, n_matrices))
         for i in range(self.n_potatoes):
-            if X[i].shape[0] != n_matrices:
-                raise ValueError(
-                    'Unequal n_matrices between ndarray of X. Should be %d but'
-                    ' got %d.' % (n_matrices, X[i].shape[0]))
+            _check_n_matrices(X[i], n_matrices)
             p[i] = self._potatoes[i].predict_proba(X[i])
         p[p < 1e-10] = 1e-10  # avoid trouble with log
         q = - 2 * np.sum(np.log(p), axis=0)
         proba = self._get_proba(q)
         return proba
 
     def _check_length(self, X):
```

### Comparing `pyriemann-0.4/pyriemann/datasets/sampling.py` & `pyriemann-0.5/pyriemann/datasets/sampling.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,27 +58,23 @@
     Returns
     -------
     p : float
         Probability of acceptation.
 
     Notes
     -----
-    .. versionadded:: 0.3.1
+    .. versionadded:: 0.4
 
     """
-    mu_a = np.array([sigma**2 / 2, -(sigma**2) / 2])
+    mu_a = np.array([-sigma**2 / 2, (sigma**2) / 2])
     cov_matrix = (sigma**2) * np.eye(2)
     m = np.pi * (sigma**2) * np.exp(sigma**2 / 4)
     if r_sample[0] >= r_sample[1]:
-        num = (
-            np.exp(-1 / (2 * sigma**2) * np.sum(r_sample**2))
-            * np.sinh((r_sample[0] - r_sample[1]) / 2)
-            / m
-        )
-        den = multivariate_normal.pdf(r_sample, mean=mu_a, cov=cov_matrix)
+        num = _pdf_r(r_sample, sigma)
+        den = multivariate_normal.pdf(r_sample, mean=mu_a, cov=cov_matrix)*m
         return num / den
     return 0
 
 
 def _rejection_sampling_2D_gfunction_minus(sigma, r_sample):
     """Auxiliary function for the 2D rejection sampling algorithm.
 
@@ -94,75 +90,87 @@
     Returns
     -------
     p : float
         Probability of acceptation.
 
     Notes
     -----
-    .. versionadded:: 0.3.1
+    .. versionadded:: 0.4
 
     """
-    mu_b = np.array([-(sigma**2) / 2, sigma**2 / 2])
+    mu_b = np.array([(sigma**2) / 2, -sigma**2 / 2])
     cov_matrix = (sigma**2) * np.eye(2)
     m = np.pi * (sigma**2) * np.exp(sigma**2 / 4)
     if r_sample[0] < r_sample[1]:
-        num = (
-            np.exp(-1 / (2 * sigma**2) * np.sum(r_sample**2))
-            * np.sinh((r_sample[1] - r_sample[0]) / 2)
-        )
+        num = _pdf_r(r_sample, sigma)
         den = multivariate_normal.pdf(r_sample, mean=mu_b, cov=cov_matrix) * m
         return num / den
     return 0
 
 
-def _rejection_sampling_2D(n_samples, sigma, random_state=None):
+def _rejection_sampling_2D(n_samples, sigma, random_state=None,
+                           return_acceptance_rate=False):
     """Rejection sampling algorithm for the 2D case.
 
     Implementation of a rejection sampling algorithm. The implementation
     follows the description given in page 528 of Christopher Bishop's book
     "Pattern recognition and Machine Learning" (2006).
 
     Parameters
     ----------
     n_samples : int
         Number of samples to get from the target distribution.
     sigma : float
         Dispersion of the Riemannian Gaussian distribution.
     random_state : int, RandomState instance or None, default=None
         Pass an int for reproducible output across multiple function calls.
+    return_acceptance_rate : boolean, default=False
+        Whether to return the acceptance rate with the sample (number of
+        samples obtained divided by the number of samples generated by
+        the algorithm).
+
+        .. versionadded:: 0.5
 
     Returns
     -------
     r_samples : ndarray, shape (n_samples, n_dim)
         Samples of the r parameters of the Riemannian Gaussian distribution.
+    acceptance_rate : float
+        Acceptance rate empirically computed for the generation of the sample.
+        Only returned if ``return_acceptance_rate=True``.
 
     Notes
     -----
-    .. versionadded:: 0.3.1
+    .. versionadded:: 0.4
 
     """
-    mu_a = np.array([sigma**2 / 2, -(sigma**2) / 2])
-    mu_b = np.array([-(sigma**2) / 2, sigma**2 / 2])
+    mu_a = np.array([-sigma**2 / 2, (sigma**2) / 2])
+    mu_b = np.array([(sigma**2) / 2, -sigma**2 / 2])
     cov_matrix = (sigma**2) * np.eye(2)
     r_samples = []
     cpt = 0
+    acc = 0
     rs = check_random_state(random_state)
     while cpt != n_samples:
-        if rs.binomial(1, 0.5, 1) == 1:
+        acc += 1
+        if (rs.binomial(1, 0.5, 1) == 1):
             r_sample = multivariate_normal.rvs(mu_a, cov_matrix, 1, rs)
             res = _rejection_sampling_2D_gfunction_plus(sigma, r_sample)
             if rs.rand(1) < res:
                 r_samples.append(r_sample)
                 cpt += 1
         else:
             r_sample = multivariate_normal.rvs(mu_b, cov_matrix, 1, rs)
             res = _rejection_sampling_2D_gfunction_minus(sigma, r_sample)
             if rs.rand(1) < res:
                 r_samples.append(r_sample)
                 cpt += 1
+
+    if return_acceptance_rate:
+        return np.array(r_samples), n_samples / acc
     return np.array(r_samples)
 
 
 def _slice_one_sample(ptarget, x0, w, rs):
     """Slice sampling for one sample
 
     Parameters
@@ -311,15 +319,15 @@
         each of the class centroid in parallel. If -1 all CPUs are used.
     sampling_method : str, default='auto'
         Name of the sampling method used to sample samples_r. It can be
         'auto', 'slice' or 'rejection'. If it is 'auto', the sampling_method
         will be equal to 'slice' for n_dim != 2 and equal to
         'rejection' for n_dim = 2.
 
-        .. versionadded:: 0.3.1
+        .. versionadded:: 0.4
 
     Returns
     -------
     r_samples : ndarray, shape (n_samples, n_dim)
         Samples of the r parameters of the Riemannian Gaussian distribution.
 
     References
@@ -409,15 +417,15 @@
         each of the class centroid in parallel. If -1 all CPUs are used.
     sampling_method : str, default='auto'
         Name of the sampling method used to sample samples_r. It can be
         'auto', 'slice' or 'rejection'. If it is 'auto', the sampling_method
         will be equal to 'slice' for n_dim != 2 and equal to
         'rejection' for n_dim = 2.
 
-        .. versionadded:: 0.3.1
+        .. versionadded:: 0.4
 
     Returns
     -------
     samples : ndarray, shape (n_matrices, n_dim, n_dim)
         Samples of the Riemannian Gaussian distribution.
 
     Notes
@@ -479,15 +487,15 @@
         each of the class centroid in parallel. If -1 all CPUs are used.
     sampling_method : str, default='auto'
         Sampling method to sample eigenvalues. It can be
         'auto', 'slice' or 'rejection'. If it is 'auto', the sampling_method
         will be equal to 'slice' for n_dim != 2 and equal to
         'rejection' for n_dim = 2.
 
-        .. versionadded:: 0.3.1
+        .. versionadded:: 0.4
 
     Returns
     -------
     samples : ndarray, shape (n_matrices, n_dim, n_dim)
         Samples of the Riemannian Gaussian distribution.
 
     Notes
```

### Comparing `pyriemann-0.4/pyriemann/datasets/simulated.py` & `pyriemann-0.5/pyriemann/datasets/simulated.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,16 +2,21 @@
 from sklearn.utils.validation import check_random_state
 
 from ..utils.mean import mean_riemann
 from ..utils.distance import distance_riemann
 from ..utils.base import invsqrtm, powm, sqrtm, expm
 from .sampling import generate_random_spd_matrix, sample_gaussian_spd
 from ..transfer import encode_domains
+from ..utils import deprecated
 
 
+@deprecated(
+    "make_covariances is deprecated and will be removed in 0.6.0; "
+    "please use make_matrices."
+)
 def make_covariances(n_matrices, n_channels, rs=None, return_params=False,
                      evals_mean=2.0, evals_std=0.1):
     """Generate a set of covariances matrices, with the same eigenvectors.
 
     Parameters
     ----------
     n_matrices : int
@@ -34,15 +39,14 @@
     evals : ndarray, shape (n_matrices, n_channels)
         Eigen values used for each covariance matrix.
         Only returned if ``return_params=True``.
     evecs : ndarray, shape (n_channels, n_channels)
         Eigen vectors used for all covariance matrices.
         Only returned if ``return_params=True``.
     """
-
     rs = check_random_state(rs)
 
     evals = np.abs(evals_mean + evals_std * rs.randn(n_matrices, n_channels))
     evecs, _ = np.linalg.qr(rs.randn(n_channels, n_channels))
 
     covmats = np.empty((n_matrices, n_channels, n_channels))
     for i in range(n_matrices):
@@ -50,14 +54,108 @@
 
     if return_params:
         return covmats, evals, evecs
     else:
         return covmats
 
 
+def make_matrices(n_matrices, n_dim, kind, rs=None, return_params=False,
+                  evals_low=0.5, evals_high=2.0, eigvecs_same=False):
+    """Generate a set of matrices, with specific properties.
+
+    Parameters
+    ----------
+    n_matrices : int
+        Number of matrices to generate.
+    n_dim : int
+        Dimension of square matrices to generate.
+    kind : {'real', 'comp', 'spd', 'spsd', 'hpd', 'hpsd'}
+        Kind of matrices to generate:
+
+        - 'real' for real-valued matrices;
+        - 'comp' for complex-valued matrices;
+        - 'spd' for symmetric positive-definite matrices;
+        - 'spsd' for symmetric positive semi-definite matrices;
+        - 'hpd' for Hermitian positive-definite matrices;
+        - 'hpsd' for Hermitian positive semi-definite matrices.
+    rs : RandomState instance, default=None
+        Random state for reproducible output across multiple function calls.
+    return_params : bool, default=False
+        If True, then returns evals and evecs for 'spd', 'spsd', 'hpd' and
+        'hpsd'.
+    evals_low : float, default=0.5
+        Lowest value of the uniform distribution to draw eigen values.
+    evals_high : float, default=2.0
+        Highest value of the uniform distribution to draw eigen values.
+    eigvecs_same : bool, default False
+        If True, then uses the same eigen vectors for all matrices.
+
+    Returns
+    -------
+    mats : ndarray, shape (n_matrices, n_dim, n_dim)
+        Generated matrices.
+    evals : ndarray, shape (n_matrices, n_dim)
+        Eigen values used for 'spd', 'spsd', 'hpd' and 'hpsd'.
+        Only returned if ``return_params=True``.
+    evecs : ndarray, shape (n_matrices, n_dim, n_dim) or (n_dim, n_dim)
+        Eigen vectors used for 'spd', 'spsd', 'hpd' and 'hpsd'.
+        Only returned if ``return_params=True``.
+
+    Notes
+    -----
+    .. versionadded:: 0.5
+    """
+    if kind not in ("real", "comp", "spd", "spsd", "hpd", "hpsd"):
+        raise ValueError(f"Unsupported matrix kind: {kind}")
+
+    rs = check_random_state(rs)
+    X = rs.randn(n_matrices, n_dim, n_dim)
+    if kind == "real":
+        return X
+
+    if kind in ("comp", "hpd", "hpsd"):
+        X = X + 1j * rs.randn(n_matrices, n_dim, n_dim)
+        if kind == "comp":
+            return X
+
+    # eigen values
+    if evals_low <= 0.0:
+        raise ValueError(
+            f"Lowest value must be strictly positive (Got {evals_low}).")
+    if evals_high <= evals_low:
+        raise ValueError(
+            "Highest value must be superior to lowest value "
+            f"(Got {evals_high} and {evals_low}).")
+    evals = rs.uniform(evals_low, evals_high, size=(n_matrices, n_dim))
+    if kind in ("spsd", "hpsd"):
+        evals[..., -1] = 1e-10  # last eigen value set to almost zero
+
+    # eigen vectors
+    if eigvecs_same:
+        X = X[0]
+    if np.__version__ < '1.22.0' and X.ndim > 2:
+        evecs = np.array([np.linalg.qr(x)[0] for x in X])
+    else:
+        evecs = np.linalg.qr(X)[0]
+
+    # conjugation
+    if eigvecs_same:
+        mats = np.empty((n_matrices, n_dim, n_dim), dtype=X.dtype)
+        for i in range(n_matrices):
+            mats[i] = (evecs * evals[i]) @ evecs.conj().T
+    else:
+        mats = (evecs * evals[:, np.newaxis, :]) @ np.swapaxes(evecs.conj(),
+                                                               -2, -1)
+
+    if return_params:
+        return mats, evals, evecs
+    else:
+        return mats
+
+
 def make_masks(n_masks, n_dim0, n_dim1_min, rs=None):
     """Generate a set of masks, defined as semi-orthogonal matrices.
 
     Parameters
     ----------
     n_masks : int
         Number of masks to generate.
@@ -69,16 +167,19 @@
         Random state for reproducible output across multiple function calls.
 
     Returns
     -------
     masks : list of n_masks ndarray of shape (n_dim0, n_dim1_i), \
             with different n_dim1_i, such that n_dim1_min <= n_dim1_i <= n_dim0
         Masks.
-    """
 
+    Notes
+    -----
+    .. versionadded:: 0.3
+    """
     rs = check_random_state(rs)
 
     masks = []
     for _ in range(n_masks):
         n_dim1 = rs.randint(n_dim1_min, n_dim0, size=1)[0]
         mask, _ = np.linalg.qr(rs.randn(n_dim0, n_dim1))
         masks.append(mask)
@@ -121,15 +222,15 @@
         each of the class centroid in parallel. If -1 all CPUs are used.
     sampling_method : str, default='auto'
         Name of the sampling method used to sample samples_r. It can be
         'auto', 'slice' or 'rejection'. If it is 'auto', the sampling_method
         will be equal to 'slice' for n_dim != 2 and equal to
         'rejection' for n_dim = 2.
 
-        .. versionadded:: 0.3.1
+        .. versionadded:: 0.4
 
     Returns
     -------
     X : ndarray, shape (2*n_matrices, n_dim, n_dim)
         Set of SPD matrices.
     y : ndarray, shape (2*n_matrices,)
         Labels corresponding to each matrix.
@@ -138,15 +239,15 @@
 
     Notes
     -----
     .. versionadded:: 0.3
 
     """
     if not isinstance(class_sep, float):
-        raise ValueError(f'class_sep must be a float (Got {class_sep})')
+        raise ValueError(f"class_sep must be a float (Got {class_sep})")
 
     rs = check_random_state(random_state)
     seeds = rs.randint(100, size=2)
 
     if centers is None:
         C0_in = np.eye(n_dim)  # first class mean at Identity at first
         Pv = rs.randn(n_dim, n_dim)  # create random tangent vector
@@ -249,15 +350,15 @@
     n_dim = mean.shape[1]
     mean_sqrt = sqrtm(mean)
 
     outliers = np.zeros((n_matrices, n_dim, n_dim))
     for i in range(n_matrices):
         Oi = generate_random_spd_matrix(n_dim=n_dim, random_state=random_state)
         epsilon_num = outlier_coeff * sigma * n_dim
-        epsilon_den = distance_riemann(Oi, np.eye(n_dim))**2
+        epsilon_den = distance_riemann(Oi, np.eye(n_dim), squared=True)
         epsilon = np.sqrt(epsilon_num / epsilon_den)
         outliers[i] = mean_sqrt @ powm(Oi, epsilon) @ mean_sqrt
 
     return outliers
 
 
 def make_classification_transfer(n_matrices, class_sep=3.0, class_disp=1.0,
@@ -298,15 +399,15 @@
     X_enc : ndarray, shape (4*n_matrices, 2, 2)
         Set of SPD matrices.
     y_enc : ndarray, shape (4*n_matrices,)
         Extended labels for each data point.
 
     Notes
     -----
-    .. versionadded:: 0.3.1
+    .. versionadded:: 0.4
     """
 
     rs = check_random_state(random_state)
     seeds = rs.randint(100, size=4)
 
     # the examples considered here are always for 2x2 matrices
     n_dim = 2
```

### Comparing `pyriemann-0.4/pyriemann/embedding.py` & `pyriemann-0.5/pyriemann/embedding.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,27 +3,18 @@
 import numpy as np
 from scipy.linalg import solve, eigh
 from scipy.sparse import csr_matrix
 
 from sklearn.base import BaseEstimator, TransformerMixin
 from sklearn.manifold import spectral_embedding
 
-from .utils import deprecated
 from .utils.kernel import kernel
 from .utils.distance import pairwise_distance
 
 
-@deprecated(
-    "Embedding is deprecated and will be removed in 0.4.0; "
-    "please use SpectralEmbedding."
-)
-class Embedding(BaseEstimator):
-    pass
-
-
 class SpectralEmbedding(BaseEstimator):
     """Spectral embedding of SPD matrices into an Euclidean space.
 
     It uses Laplacian Eigenmaps [1]_ to embed SPD matrices into an Euclidean
     space of smaller dimension. The basic hypothesis is that high-dimensional
     data lives in a low-dimensional manifold, whose intrinsic geometry can be
     described via the Laplacian matrix of a graph. The vertices of this graph
```

### Comparing `pyriemann-0.4/pyriemann/estimation.py` & `pyriemann-0.5/pyriemann/estimation.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     Perform a simple covariance matrix estimation for each given input.
 
     Parameters
     ----------
     estimator : string, default='scm'
         Covariance matrix estimator, see
         :func:`pyriemann.utils.covariance.covariances`.
-    **kwds : optional keyword parameters
+    **kwds : dict
         Any further parameters are passed directly to the covariance estimator.
 
     See Also
     --------
     ERPCovariances
     XdawnCovariances
     CospCovariances
@@ -107,15 +107,15 @@
         If None, all classes will be accounted.
     estimator : string, default='scm'
         Covariance matrix estimator, see
         :func:`pyriemann.utils.covariance.covariances`.
     svd : int | None, default=None
         If not None, number of components of SVD used to reduce prototype
         responses.
-    **kwds : optional keyword parameters
+    **kwds : dict
         Any further parameters are passed directly to the covariance estimator.
 
     Attributes
     ----------
     P_ : ndarray, shape (n_components, n_times)
         If fit, prototyped responses for each class, where `n_components` is
         equal to `n_classes x n_channels` if `svd` is None,
@@ -248,15 +248,15 @@
     xdawn_estimator : string, default='scm'
         Covariance matrix estimator for `Xdawn` spatial filtering.
         Should be regularized using 'lwf' or 'oas', see
         :func:`pyriemann.utils.covariance.covariances`.
     baseline_cov : array, shape (n_channels, n_channels) | None, default=None
         Baseline covariance for `Xdawn` spatial filtering,
         see :class:`pyriemann.spatialfilters.Xdawn`.
-    **kwds : optional keyword parameters
+    **kwds : dict
         Any further parameters are passed directly to the covariance estimator.
 
     Attributes
     ----------
     P_ : ndarray, shape (n_classes x min(n_channels, n_filters), n_times)
         If fit, the evoked response for each event type, concatenated.
 
@@ -362,15 +362,15 @@
     ----------
     block_size : int | list of int
         Sizes of individual blocks given as int for same-size block, or list
         for varying block sizes.
     estimator : string, default='scm'
         Covariance matrix estimator, see
         :func:`pyriemann.utils.covariance.covariances`.
-    **kwds : optional keyword parameters
+    **kwds : dict
         Any further parameters are passed directly to the covariance estimator.
 
     Notes
     -----
     .. versionadded:: 0.3
 
     See Also
@@ -649,15 +649,15 @@
     ----------
     delays : int | list of int, default=4
         The delays to apply for the Hankel matrices. If `int`, it use a range
         of delays up to the given value. A list of int can be given.
     estimator : string, default='scm'
         Covariance matrix estimator, see
         :func:`pyriemann.utils.covariance.covariances`.
-    **kwds : optional keyword parameters
+    **kwds : dict
         Any further parameters are passed directly to the covariance estimator.
 
     See Also
     --------
     Covariances
     ERPCovariances
     CospCovariances
@@ -756,24 +756,24 @@
     metric : string, default='linear'
         The metric to use when computing kernel function between channels [2]_:
         'linear', 'poly', 'polynomial', 'rbf', 'laplacian', 'cosine'.
     n_jobs : int, default=None
         The number of jobs to use for the computation [2]_. This works by
         breaking down the pairwise matrix into n_jobs even slices and computing
         them in parallel.
-    **kwds : optional keyword parameters
+    **kwds : dict
         Any further parameters are passed directly to the kernel function [2]_.
 
     See Also
     --------
     Covariances
 
     Notes
     -----
-    .. versionadded:: 0.3.1
+    .. versionadded:: 0.4
 
     References
     ----------
     .. [1] `Beyond Covariance: Feature Representation with Nonlinear Kernel
         Matrices
         <https://www.cv-foundation.org/openaccess/content_iccv_2015/papers/Wang_Beyond_Covariance_Feature_ICCV_2015_paper.pdf>`_
         L. Wang, J. Zhang, L. Zhou, C. Tang, W Li. ICCV, 2015.
```

### Comparing `pyriemann-0.4/pyriemann/preprocessing.py` & `pyriemann-0.5/pyriemann/preprocessing.py`

 * *Files identical despite different names*

### Comparing `pyriemann-0.4/pyriemann/regression.py` & `pyriemann-0.5/pyriemann/regression.py`

 * *Files 0% similar despite different names*

```diff
@@ -252,11 +252,11 @@
         Returns
         -------
         score : float
             R2 of self.predict(X) wrt. y.
 
         Notes
         -----
-        .. versionadded:: 0.3.1
+        .. versionadded:: 0.4
         """
         y_pred = self.predict(X)
         return r2_score(y, y_pred)
```

### Comparing `pyriemann-0.4/pyriemann/spatialfilters.py` & `pyriemann-0.5/pyriemann/spatialfilters.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import numpy as np
 from scipy.linalg import eigh, inv
 from sklearn.base import BaseEstimator, TransformerMixin
 
 from .utils.covariance import _check_est, normalize, get_nondiag_weight
 from .utils.mean import mean_covariance
 from .utils.ajd import ajd_pham
-from .utils.mean import _check_mean_method
 from . import estimation as est
 from .preprocessing import Whitening
 
 
 class Xdawn(BaseEstimator, TransformerMixin):
     """Xdawn algorithm.
 
@@ -100,16 +99,17 @@
         n_trials, n_channels, n_times = X.shape
 
         self.classes_ = (np.unique(y) if self.classes is None else
                          self.classes)
 
         Cx = self.baseline_cov
         if Cx is None:
+            tmp = X.transpose((1, 2, 0))
             Cx = np.asarray(self.estimator_fn(
-                X.reshape(n_channels, n_times * n_trials)
+                tmp.reshape(n_channels, n_times * n_trials)
             ))
 
         self.evokeds_ = []
         self.filters_ = []
         self.patterns_ = []
         for c in self.classes_:
             # Prototyped response for each class
@@ -314,15 +314,14 @@
         Returns
         -------
         self : CSP instance
             The CSP instance.
         """
         if not isinstance(self.nfilter, int):
             raise TypeError('nfilter must be an integer')
-        _check_mean_method(self.metric)
         if not isinstance(self.log, bool):
             raise TypeError('log must be a boolean')
 
         if not isinstance(X, (np.ndarray, list)):
             raise TypeError('X must be an array.')
         if not isinstance(y, (np.ndarray, list)):
             raise TypeError('y must be an array.')
```

### Comparing `pyriemann-0.4/pyriemann/stats.py` & `pyriemann-0.5/pyriemann/stats.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,15 +167,15 @@
 
         - None, to use the default 3-fold cross validation;
         - integer, to specify the number of folds in a `(Stratified)KFold`;
         - an object to be used as a cross-validation generator;
         - an iterable yielding train, test splits.
 
         For integer/None inputs, if the estimator is a classifier and `y` is
-        either binary or multiclass, :class:`StratifiedKFold` is used. In all
+        either binary or multiclass, `StratifiedKFold` is used. In all
         other cases, `KFold` is used.
     scoring : string or callable or None, default=None
         A string (see model evaluation documentation) or
         a scorer callable object / function with signature
         `scorer(estimator, X, y)`.
     n_jobs : integer, default=1
         The number of CPUs to use to do the computation. -1 means
@@ -355,37 +355,44 @@
         self.mdm = MDM(metric=self.metric, n_jobs=self.n_jobs)
         self.mdm.metric_mean, self.mdm.metric_dist = _check_metric(
             self.metric
         )
         if self.mode == 'ftest':
             self.global_mean = mean_covariance(X, metric=self.mdm.metric_mean)
         elif self.mode == 'pairwise':
-            X = pairwise_distance(X, metric=self.mdm.metric_dist)**2
+            X = pairwise_distance(X, metric=self.mdm.metric_dist, squared=True)
         return X
 
     def _score_ftest(self, X, y):
         """Get the score"""
         mdm = self.mdm.fit(X, y)
         covmeans = np.array(mdm.covmeans_)
 
         # estimates between classes variability
         n_classes = len(covmeans)
         between = 0
         for ix, classe in enumerate(mdm.classes_):
             di = distance(
-                covmeans[ix], self.global_mean, metric=mdm.metric_dist)**2
+                covmeans[ix],
+                self.global_mean,
+                metric=mdm.metric_dist,
+                squared=True,
+            )
             between += np.sum(y == classe) * di
         between /= (n_classes - 1)
 
         # estimates within class variability
         within = 0
         for ix, classe in enumerate(mdm.classes_):
-            within += (distance(
-                X[y == classe], covmeans[ix], metric=mdm.metric_dist)
-                ** 2).sum()
+            within += distance(
+                X[y == classe],
+                covmeans[ix],
+                metric=mdm.metric_dist,
+                squared=True,
+            ).sum()
         within /= (len(y) - n_classes)
 
         score = between / within
         return score
 
     def _score_ttest(self, X, y):
         """Get the score"""
@@ -396,17 +403,20 @@
         n_classes = len(covmeans)
         pairs = pairwise_distance(covmeans, metric=mdm.metric_dist)
         mean_dist = np.triu(pairs).sum()
         mean_dist /= (n_classes * (n_classes - 1)) / 2.0
 
         dist = 0
         for ix, classe in enumerate(mdm.classes_):
-            di = (distance(
-                X[y == classe], covmeans[ix], metric=mdm.metric_dist)
-                ** 2).mean()
+            di = distance(
+                X[y == classe],
+                covmeans[ix],
+                metric=mdm.metric_dist,
+                squared=True,
+            ).mean()
             dist += (di / np.sum(y == classe))
         score = mean_dist / np.sqrt(dist)
         return score
 
     def _score_pairwise(self, X, y):
         """Score for the pairwise distance test."""
         classes = np.unique(y)
```

### Comparing `pyriemann-0.4/pyriemann/tangentspace.py` & `pyriemann-0.5/pyriemann/tangentspace.py`

 * *Files identical despite different names*

### Comparing `pyriemann-0.4/pyriemann/transfer/_estimators.py` & `pyriemann-0.5/pyriemann/transfer/_estimators.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     """No transformation on data for transfer learning.
 
     No transformation of the data points between the domains.
     This is what we call the Direct Center Transfer (DCT) method.
 
     Notes
     -----
-    .. versionadded:: 0.3.1
+    .. versionadded:: 0.4
     """
 
     def __init__(self):
         pass
 
     def fit(self, X, y_enc):
         """Do nothing.
@@ -121,15 +121,15 @@
         Applications to Brain–Computer Interfaces
         <https://hal.archives-ouvertes.fr/hal-01923278/>`_
         P Zanini et al, IEEE Transactions on Biomedical Engineering, vol. 65,
         no. 5, pp. 1107-1116, August, 2017
 
     Notes
     -----
-    .. versionadded:: 0.3.1
+    .. versionadded:: 0.4
     """
 
     def __init__(self, target_domain, metric='riemann'):
         """Init"""
         self.target_domain = target_domain
         self.metric = metric
 
@@ -244,15 +244,15 @@
         brain-computer interfaces
         <https://hal.archives-ouvertes.fr/hal-01971856>`_
         PLC Rodrigues et al, IEEE Transactions on Biomedical Engineering,
         vol. 66, no. 8, pp. 2390-2401, December, 2018
 
     Notes
     -----
-    .. versionadded:: 0.3.1
+    .. versionadded:: 0.4
     """
 
     def __init__(self, target_domain, final_dispersion=1.0,
                  centered_data=False, metric='riemann'):
         """Init"""
         self.target_domain = target_domain
         self.final_dispersion = final_dispersion
@@ -282,17 +282,20 @@
         self._means = {}
         self.dispersions_ = {}
         for d in np.unique(domains):
             if self.centered_data:
                 self._means[d] = np.eye(n_dim)
             else:
                 self._means[d] = mean_riemann(X[domains == d])
-            disp_domain = np.sum(distance(
-                X[domains == d], self._means[d], metric=self.metric
-            )**2)
+            disp_domain = distance(
+                X[domains == d],
+                self._means[d],
+                metric=self.metric,
+                squared=True,
+            ).sum()
             self.dispersions_[d] = disp_domain
 
         return self
 
     def _center(self, X, mean):
         Mean_isqrt = invsqrtm(mean)
         return Mean_isqrt @ X @ Mean_isqrt
@@ -433,15 +436,15 @@
         vol. 66, no. 8, pp. 2390-2401, December, 2018
     .. [2] `An introduction to optimization on smooth manifolds
         <https://www.nicolasboumal.net/book/>`_
         N. Boumal. To appear with Cambridge University Press. June, 2022
 
     Notes
     -----
-    .. versionadded:: 0.3.1
+    .. versionadded:: 0.4
     """
 
     def __init__(self, target_domain, weights=None, metric='euclid', n_jobs=1):
         """Init"""
         self.target_domain = target_domain
         self.weights = weights
         self.metric = metric
@@ -570,15 +573,15 @@
     domain_weight : None | dict, default=None
         Weights to combine matrices from each domain to train the estimator.
         The dict contains key=domain_name and value=weight_to_assign.
         If None, it uses equal weights.
 
     Notes
     -----
-    .. versionadded:: 0.3.1
+    .. versionadded:: 0.4
     """
 
     def __init__(self, target_domain, estimator, domain_weight=None):
         """Init."""
         self.target_domain = target_domain
         self.domain_weight = domain_weight
         self.estimator = estimator
@@ -657,15 +660,15 @@
     domain_weight : None | dict, default=None
         Weights to combine matrices from each domain to train the classifier.
         The dict contains key=domain_name and value=weight_to_assign.
         If None, it uses equal weights.
 
     Notes
     -----
-    .. versionadded:: 0.3.1
+    .. versionadded:: 0.4
     """
 
     def fit(self, X, y_enc):
         """Fit TLClassifier.
 
         Parameters
         ----------
@@ -734,15 +737,15 @@
     domain_weight : None | dict, default=None
         Weights to combine matrices from each domain to train the regressor.
         The dict contains key=domain_name and value=weight_to_assign.
         If None, it uses equal weights.
 
     Notes
     -----
-    .. versionadded:: 0.3.1
+    .. versionadded:: 0.4
     """
 
     def fit(self, X, y_enc):
         """Fit TLRegressor.
 
         Parameters
         ----------
@@ -842,15 +845,15 @@
         <https://hal.archives-ouvertes.fr/hal-03202360/>`_
         S. Khazem, S. Chevallier, Q. Barthelemy, K. Haroun and C. Nous, 10th
         International IEEE/EMBS Conference on Neural Engineering (NER), pp.
         523-526. IEEE, 2021.
 
     Notes
     -----
-    .. versionadded:: 0.3.1
+    .. versionadded:: 0.4
     """
 
     def __init__(
             self,
             domain_tradeoff,
             target_domain,
             metric='riemann',
```

### Comparing `pyriemann-0.4/pyriemann/transfer/_rotate.py` & `pyriemann-0.5/pyriemann/transfer/_rotate.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,15 +184,15 @@
         vol. 66, no. 8, pp. 2390-2401, December, 2018
     .. [2] `An introduction to optimization on smooth manifolds
         <https://www.nicolasboumal.net/book/>`_
         N. Boumal. To appear with Cambridge University Press. June, 2022
 
     Notes
     -----
-    .. versionadded:: 0.3.1
+    .. versionadded:: 0.4
     """
 
     if M_source.shape[0] != M_target.shape[0]:
         raise ValueError("The number of classes in each domain don't match")
     if M_source.shape[1:] != M_target.shape[1:]:
         raise ValueError("The number of channels in each domain don't match")
```

### Comparing `pyriemann-0.4/pyriemann/transfer/_tools.py` & `pyriemann-0.5/pyriemann/transfer/_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
     See Also
     --------
     decode_domains
 
     Notes
     -----
-    .. versionadded:: 0.3.1
+    .. versionadded:: 0.4
     """
     if len(y) != len(domain):
         raise ValueError("Input lengths don't match")
 
     y_enc = [str(d_) + '/' + str(y_) for (d_, y_) in zip(domain, y)]
     return X, np.array(y_enc)
 
@@ -68,15 +68,15 @@
 
     See Also
     --------
     encode_domains
 
     Notes
     -----
-    .. versionadded:: 0.3.1
+    .. versionadded:: 0.4
     """
     y, domain = [], []
     for y_enc_ in y_enc:
         y_dec_ = y_enc_.split('/')
         domain.append(y_dec_[-2])
         y.append(y_dec_[-1])
     return X_enc, np.array(y), np.array(domain)
@@ -100,15 +100,15 @@
 
     References
     ----------
     .. [1] https://scikit-learn.org/stable/modules/cross_validation.html#cross-validation-iterators
 
     Notes
     -----
-    .. versionadded:: 0.3.1
+    .. versionadded:: 0.4
     """  # noqa
     def __init__(self, target_domain, cv):
 
         self.target_domain = target_domain
         self.cv = cv
 
     def split(self, X, y):
```

### Comparing `pyriemann-0.4/pyriemann/utils/__init__.py` & `pyriemann-0.5/pyriemann/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyriemann-0.4/pyriemann/utils/ajd.py` & `pyriemann-0.5/pyriemann/utils/ajd.py`

 * *Files identical despite different names*

### Comparing `pyriemann-0.4/pyriemann/utils/base.py` & `pyriemann-0.5/pyriemann/utils/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,156 +1,164 @@
-"""Base functions for SPD matrices."""
+"""Base functions for SPD/HPD matrices."""
 
 import numpy as np
 from numpy.core.numerictypes import typecodes
 from .test import is_pos_def
 
 
 def _matrix_operator(C, operator):
     """Matrix function."""
     if not isinstance(C, np.ndarray) or C.ndim < 2:
-        raise ValueError('Input must be at least a 2D ndarray')
+        raise ValueError("Input must be at least a 2D ndarray")
     if C.dtype.char in typecodes['AllFloat'] and (
             np.isinf(C).any() or np.isnan(C).any()):
         raise ValueError(
             "Matrices must be positive definite. Add "
             "regularization to avoid this error.")
     eigvals, eigvecs = np.linalg.eigh(C)
     eigvals = operator(eigvals)
     if C.ndim >= 3:
         eigvals = np.expand_dims(eigvals, -2)
     D = (eigvecs * eigvals) @ np.swapaxes(eigvecs.conj(), -2, -1)
     return D
 
 
-def sqrtm(C):
-    r"""Square root of SPD matrices.
+def expm(C):
+    r"""Exponential of SPD/HPD matrices.
 
-    The matrix square root of a SPD matrix C is defined by:
+    The symmetric matrix exponential of a SPD/HPD matrix
+    :math:`\mathbf{C}` is defined by:
 
     .. math::
-        \mathbf{D} =
-        \mathbf{V} \left( \mathbf{\Lambda} \right)^{1/2} \mathbf{V}^\top
+        \mathbf{D} = \mathbf{V} \exp{(\mathbf{\Lambda})} \mathbf{V}^H
 
     where :math:`\mathbf{\Lambda}` is the diagonal matrix of eigenvalues
     and :math:`\mathbf{V}` the eigenvectors of :math:`\mathbf{C}`.
 
     Parameters
     ----------
     C : ndarray, shape (..., n, n)
-        SPD matrices, at least 2D ndarray.
+        SPD/HPD matrices, at least 2D ndarray.
 
     Returns
     -------
     D : ndarray, shape (..., n, n)
-        Matrix square root of C.
+        Matrix exponential of C.
     """
-    return _matrix_operator(C, np.sqrt)
+    return _matrix_operator(C, np.exp)
 
 
-def logm(C):
-    r"""Logarithm of SPD matrices.
+def invsqrtm(C):
+    r"""Inverse square root of SPD/HPD matrices.
 
-    The matrix logarithm of a SPD matrix C is defined by:
+    The symmetric matrix inverse square root of a SPD/HPD matrix
+    :math:`\mathbf{C}` is defined by:
 
     .. math::
-        \mathbf{D} = \mathbf{V} \log{(\mathbf{\Lambda})} \mathbf{V}^\top
+        \mathbf{D} =
+        \mathbf{V} \left( \mathbf{\Lambda} \right)^{-1/2} \mathbf{V}^H
 
     where :math:`\mathbf{\Lambda}` is the diagonal matrix of eigenvalues
     and :math:`\mathbf{V}` the eigenvectors of :math:`\mathbf{C}`.
 
     Parameters
     ----------
     C : ndarray, shape (..., n, n)
-        SPD matrices, at least 2D ndarray.
+        SPD/HPD matrices, at least 2D ndarray.
 
     Returns
     -------
     D : ndarray, shape (..., n, n)
-        Matrix logarithm of C.
+        Matrix inverse square root of C.
     """
-    return _matrix_operator(C, np.log)
+    def isqrt(x): return 1. / np.sqrt(x)
+    return _matrix_operator(C, isqrt)
 
 
-def expm(C):
-    r"""Exponential of SPD matrices.
+def logm(C):
+    r"""Logarithm of SPD/HPD matrices.
 
-    The matrix exponential of a SPD matrix C is defined by:
+    The symmetric matrix logarithm of a SPD/HPD matrix
+    :math:`\mathbf{C}` is defined by:
 
     .. math::
-        \mathbf{D} = \mathbf{V} \exp{(\mathbf{\Lambda})} \mathbf{V}^\top
+        \mathbf{D} = \mathbf{V} \log{(\mathbf{\Lambda})} \mathbf{V}^H
 
     where :math:`\mathbf{\Lambda}` is the diagonal matrix of eigenvalues
     and :math:`\mathbf{V}` the eigenvectors of :math:`\mathbf{C}`.
 
     Parameters
     ----------
     C : ndarray, shape (..., n, n)
-        SPD matrices, at least 2D ndarray.
+        SPD/HPD matrices, at least 2D ndarray.
 
     Returns
     -------
     D : ndarray, shape (..., n, n)
-        Matrix exponential of C.
+        Matrix logarithm of C.
     """
-    return _matrix_operator(C, np.exp)
+    return _matrix_operator(C, np.log)
 
 
-def invsqrtm(C):
-    r"""Inverse square root of SPD matrices.
+def powm(C, alpha):
+    r"""Power of SPD/HPD matrices.
 
-    The matrix inverse square root of a SPD matrix C is defined by:
+    The symmetric matrix power :math:`\alpha` of a SPD/HPD matrix
+    :math:`\mathbf{C}` is defined by:
 
     .. math::
         \mathbf{D} =
-        \mathbf{V} \left( \mathbf{\Lambda} \right)^{-1/2} \mathbf{V}^\top
+        \mathbf{V} \left( \mathbf{\Lambda} \right)^{\alpha} \mathbf{V}^H
 
     where :math:`\mathbf{\Lambda}` is the diagonal matrix of eigenvalues
     and :math:`\mathbf{V}` the eigenvectors of :math:`\mathbf{C}`.
 
     Parameters
     ----------
     C : ndarray, shape (..., n, n)
-        SPD matrices, at least 2D ndarray.
+        SPD/HPD matrices, at least 2D ndarray.
+    alpha : float
+        The power to apply.
 
     Returns
     -------
     D : ndarray, shape (..., n, n)
-        Matrix inverse square root of C.
+        Matrix power of C.
     """
-    def isqrt(x): return 1. / np.sqrt(x)
-    return _matrix_operator(C, isqrt)
+    def power(x): return x**alpha
+    return _matrix_operator(C, power)
 
 
-def powm(C, alpha):
-    r"""Power of SPD matrices.
+def sqrtm(C):
+    r"""Square root of SPD/HPD matrices.
 
-    The matrix power :math:`\alpha` of a SPD matrix C is defined by:
+    The symmetric matrix square root of a SPD/HPD matrix
+    :math:`\mathbf{C}` is defined by:
 
     .. math::
         \mathbf{D} =
-        \mathbf{V} \left( \mathbf{\Lambda} \right)^{\alpha} \mathbf{V}^\top
+        \mathbf{V} \left( \mathbf{\Lambda} \right)^{1/2} \mathbf{V}^H
 
     where :math:`\mathbf{\Lambda}` is the diagonal matrix of eigenvalues
     and :math:`\mathbf{V}` the eigenvectors of :math:`\mathbf{C}`.
 
     Parameters
     ----------
     C : ndarray, shape (..., n, n)
-        SPD matrices, at least 2D ndarray.
-    alpha : float
-        The power to apply.
+        SPD/HPD matrices, at least 2D ndarray.
 
     Returns
     -------
     D : ndarray, shape (..., n, n)
-        Matrix power of C.
+        Matrix square root of C.
     """
-    def power(x): return x**alpha
-    return _matrix_operator(C, power)
+    return _matrix_operator(C, np.sqrt)
+
+
+###############################################################################
 
 
 def _nearest_sym_pos_def(S, reg=1e-6):
     """Find the nearest SPD matrix.
 
     Parameters
     ----------
@@ -208,15 +216,15 @@
     Returns
     -------
     P : ndarray, shape (..., n, n)
         Nearest SPD matrices.
 
     Notes
     -----
-    .. versionadded:: 0.3.1
+    .. versionadded:: 0.4
 
     References
     ----------
     .. [1] `nearestSPD
         <https://www.mathworks.com/matlabcentral/fileexchange/42885-nearestspd>`_
         J. D'Errico, MATLAB Central File Exchange
     .. [2] `Computing a nearest symmetric positive semidefinite matrix
```

### Comparing `pyriemann-0.4/pyriemann/utils/covariance.py` & `pyriemann-0.5/pyriemann/utils/covariance.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,15 @@
     Returns
     -------
     cov : ndarray, shape (n_channels, n_channels)
         Robust M-estimator based covariance matrix.
 
     Notes
     -----
-    .. versionadded:: 0.3.1
+    .. versionadded:: 0.4
 
     References
     ----------
     .. [1] `Complex Elliptically Symmetric Distributions: Survey, New Results
         and Applications
         <https://www.researchgate.net/profile/H-Vincent-Poor/publication/258658018_Complex_Elliptically_Symmetric_Distributions_Survey_New_Results_and_Applications/links/550480100cf24cee3a0150e2/Complex-Elliptically-Symmetric-Distributions-Survey-New-Results-and-Applications.pdf>`_
         E. Ollila, D.E. Tyler, V. Koivunen, H.V. Poor. IEEE Transactions on
```

### Comparing `pyriemann-0.4/pyriemann/utils/distance.py` & `pyriemann-0.5/pyriemann/utils/tangentspace.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,386 +1,398 @@
-"""Distances between SPD matrices."""
+"""Tangent space for SPD/HPD matrices."""
 
 import numpy as np
-from scipy.linalg import eigvalsh, solve
 
-from .base import logm, sqrtm, invsqrtm
+from .base import sqrtm, invsqrtm, logm, expm
+from .mean import mean_covariance
 
 
-def _check_inputs(A, B):
-    """Recursive function with two inputs."""
-    if not isinstance(A, np.ndarray) or not isinstance(B, np.ndarray):
-        raise ValueError('Inputs must be ndarrays')
-    if not A.shape == B.shape:
-        raise ValueError('Inputs must have equal dimensions')
-    if A.ndim < 2:
-        raise ValueError('Inputs must be at least a 2D ndarray')
-
-
-def _recursive(fun, A, B, *args, **kwargs):
-    """Recursive function with two inputs."""
-    if A.ndim == 2:
-        return fun(A, B, *args, **kwargs)
-    else:
-        return np.asarray(
-            [_recursive(fun, a, b, *args, **kwargs) for a, b in zip(A, B)]
-        )
-
-
-###############################################################################
-# Distances between matrices
+def _check_dimensions(X, Cref):
+    n_1, n_2 = X.shape[-2:]
+    n_3, n_4 = Cref.shape
+    if not (n_1 == n_2 == n_3 == n_4):
+        raise ValueError("Inputs have incompatible dimensions.")
 
 
-def distance_euclid(A, B):
-    r"""Euclidean distance between SPD matrices.
+def exp_map_euclid(X, Cref):
+    r"""Project matrices back to manifold by Euclidean exponential map.
 
-    The Euclidean distance between two SPD matrices A and B is defined
-    as the Frobenius norm of the difference of the two matrices:
+    The projection of a matrix :math:`\mathbf{X}` from tangent space
+    to manifold with Euclidean exponential map
+    according to a reference matrix :math:`\mathbf{C}_\text{ref}` is:
 
     .. math::
-        d(\mathbf{A},\mathbf{B}) = \Vert \mathbf{A} - \mathbf{B} \Vert_F
+        \mathbf{X}_\text{original} = \mathbf{X} + \mathbf{C}_\text{ref}
 
     Parameters
     ----------
-    A : ndarray, shape (..., n, n)
-        First SPD matrices, at least 2D ndarray.
-    B : ndarray, shape (..., n, n)
-        Second SPD matrices, same dimensions as A.
+    X : ndarray, shape (..., n, m)
+        Matrices in tangent space.
+    Cref : ndarray, shape (n, m)
+        The reference matrix.
 
     Returns
     -------
-    d : ndarray, shape (...,) or float
-        Euclidean distance between A and B.
+    X_original : ndarray, shape (..., n, m)
+        Matrices in manifold.
+
+    Notes
+    -----
+    .. versionadded:: 0.4
     """
-    _check_inputs(A, B)
-    return np.linalg.norm(A - B, ord='fro', axis=(-2, -1))
+    return X + Cref
 
 
-def distance_harmonic(A, B):
-    r"""Harmonic distance between SPD matrices.
+def exp_map_logeuclid(X, Cref):
+    r"""Project matrices back to manifold by Log-Euclidean exponential map.
 
-    The harmonic distance between two SPD matrices A and B is:
+    The projection of a matrix :math:`\mathbf{X}` from tangent space
+    to SPD/HPD manifold with Log-Euclidean exponential map
+    according to a reference SPD/HPD matrix :math:`\mathbf{C}_\text{ref}` is:
 
     .. math::
-        d(\mathbf{A},\mathbf{B}) =
-        \Vert \mathbf{A}^{-1} - \mathbf{B}^{-1} \Vert_F
+        \mathbf{X}_\text{original} =
+        \exp(\mathbf{X} + \log(\mathbf{C}_\text{ref}))
 
     Parameters
     ----------
-    A : ndarray, shape (..., n, n)
-        First SPD matrices, at least 2D ndarray.
-    B : ndarray, shape (..., n, n)
-        Second SPD matrices, same dimensions as A.
+    X : ndarray, shape (..., n, n)
+        Matrices in tangent space.
+    Cref : ndarray, shape (n, n)
+        The reference SPD/HPD matrix.
 
     Returns
     -------
-    d : ndarray, shape (...,) or float
-        Harmonic distance between A and B.
+    X_original : ndarray, shape (..., n, n)
+        Matrices in SPD/HPD manifold.
+
+    Notes
+    -----
+    .. versionadded:: 0.4
     """
-    return distance_euclid(np.linalg.inv(A), np.linalg.inv(B))
+    return expm(X + logm(Cref))
+
 
+def exp_map_riemann(X, Cref, Cm12=False):
+    r"""Project matrices back to manifold by Riemannian exponential map.
 
-def distance_kullback(A, B):
-    r"""Kullback-Leibler divergence between SPD matrices.
+    The projection of a matrix :math:`\mathbf{X}` from tangent space
+    to SPD/HPD manifold with Riemannian exponential map
+    according to a reference SPD/HPD matrix :math:`\mathbf{C}_\text{ref}` is:
+
+    .. math::
+        \mathbf{X}_\text{original} = \mathbf{C}_\text{ref}^{1/2}
+        \exp(\mathbf{X}) \mathbf{C}_\text{ref}^{1/2}
 
-    The left Kullback-Leibler divergence between two SPD matrices A and B is:
+    When Cm12=True, it returns the full Riemannian exponential map:
 
     .. math::
-        d(\mathbf{A},\mathbf{B}) =
-        \frac{1}{2} \left( \text{tr}(\mathbf{B}^{-1}\mathbf{A}) - n
-        + \log(\frac{\det(\mathbf{B})}{\det(\mathbf{A})}) \right)
+        \mathbf{X}_\text{original} = \mathbf{C}_\text{ref}^{1/2}
+        \exp( \mathbf{C}_\text{ref}^{-1/2} \mathbf{X}
+        \mathbf{C}_\text{ref}^{-1/2}) \mathbf{C}_\text{ref}^{1/2}
 
     Parameters
     ----------
-    A : ndarray, shape (..., n, n)
-        First SPD matrices, at least 2D ndarray.
-    B : ndarray, shape (..., n, n)
-        Second SPD matrices, same dimensions as A.
+    X : ndarray, shape (..., n, n)
+        Matrices in tangent space.
+    Cref : ndarray, shape (n, n)
+        The reference SPD/HPD matrix.
+    Cm12 : bool, default=False
+        If True, it returns the full Riemannian exponential map.
 
     Returns
     -------
-    d : ndarray, shape (...,) or float
-        Left Kullback-Leibler divergence between A and B.
-    """
-    _check_inputs(A, B)
-    n = A.shape[-1]
-    tr = np.trace(_recursive(solve, B, A, assume_a='pos'), axis1=-2, axis2=-1)
-    logdet = np.linalg.slogdet(B)[1] - np.linalg.slogdet(A)[1]
-    return 0.5 * (tr - n + logdet)
-
-
-def distance_kullback_right(A, B):
-    """Wrapper for right Kullback-Leibler divergence."""
-    return distance_kullback(B, A)
-
+    X_original : ndarray, shape (..., n, n)
+        Matrices in SPD/HPD manifold.
 
-def distance_kullback_sym(A, B):
-    """Symmetrized Kullback-Leibler divergence between SPD matrices.
-
-    The symmetrized Kullback-Leibler divergence between two SPD matrices A and
-    B is the sum of left and right Kullback-Leibler divergences.
+    Notes
+    -----
+    .. versionadded:: 0.4
     """
-    return distance_kullback(A, B) + distance_kullback_right(A, B)
-
+    if Cm12:
+        Cm12 = invsqrtm(Cref)
+        X = Cm12 @ X @ Cm12
+    C12 = sqrtm(Cref)
+    return C12 @ expm(X) @ C12
 
-def distance_logdet(A, B):
-    r"""Log-det distance between SPD matrices.
 
-    The log-det distance between two SPD matrices A and B is:
+def log_map_euclid(X, Cref):
+    r"""Project matrices in tangent space by Euclidean logarithmic map.
+
+    The projection of a matrix :math:`\mathbf{X}` from manifold
+    to tangent space by Euclidean logarithmic map
+    according to a reference matrix :math:`\mathbf{C}_\text{ref}` is:
 
     .. math::
-        d(\mathbf{A},\mathbf{B}) =
-        \sqrt{\log(\det(\frac{\mathbf{A}+\mathbf{B}}{2}))
-        - \frac{1}{2} \log(\det(\mathbf{A} \mathbf{B}))}
+        \mathbf{X}_\text{new} = \mathbf{X} - \mathbf{C}_\text{ref}
 
     Parameters
     ----------
-    A : ndarray, shape (..., n, n)
-        First SPD matrices, at least 2D ndarray.
-    B : ndarray, shape (..., n, n)
-        Second SPD matrices, same dimensions as A.
+    X : ndarray, shape (..., n, m)
+        Matrices in manidold.
+    Cref : ndarray, shape (n, m)
+        The reference matrix.
 
     Returns
     -------
-    d : ndarray, shape (...,) or float
-        Log-det distance between A and B.
+    X_new : ndarray, shape (..., n, m)
+        Matrices projected in tangent space.
+
+    Notes
+    -----
+    .. versionadded:: 0.4
     """
-    _check_inputs(A, B)
-    logdet_ApB = np.linalg.slogdet((A + B) / 2.0)[1]
-    logdet_AxB = np.linalg.slogdet(A @ B)[1]
-    dist2 = logdet_ApB - 0.5 * logdet_AxB
-    dist2 = np.maximum(0, dist2)
-    return np.sqrt(dist2)
+    return X - Cref
 
 
-def distance_logeuclid(A, B):
-    r"""Log-Euclidean distance between SPD matrices.
+def log_map_logeuclid(X, Cref):
+    r"""Project matrices in tangent space by Log-Euclidean logarithmic map.
 
-    The Log-Euclidean distance between two SPD matrices A and B is:
+    The projection of a matrix :math:`\mathbf{X}` from SPD/HPD manifold
+    to tangent space by Log-Euclidean logarithmic map
+    according to a SPD/HPD reference matrix :math:`\mathbf{C}_\text{ref}` is:
 
     .. math::
-        d(\mathbf{A},\mathbf{B}) =
-        \Vert \log(\mathbf{A}) - \log(\mathbf{B}) \Vert_F
+        \mathbf{X}_\text{new} = \log(\mathbf{X}) - \log(\mathbf{C}_\text{ref})
 
     Parameters
     ----------
-    A : ndarray, shape (..., n, n)
-        First SPD matrices, at least 2D ndarray.
-    B : ndarray, shape (..., n, n)
-        Second SPD matrices, same dimensions as A.
+    X : ndarray, shape (..., n, n)
+        Matrices in SPD/HPD manidold.
+    Cref : ndarray, shape (n, n)
+        The reference SPD matrix.
 
     Returns
     -------
-    d : ndarray, shape (...,) or float
-        Log-Euclidean distance between A and B.
+    X_new : ndarray, shape (..., n, n)
+        Matrices projected in tangent space.
+
+    Notes
+    -----
+    .. versionadded:: 0.4
     """
-    return distance_euclid(logm(A), logm(B))
+    _check_dimensions(X, Cref)
+    return logm(X) - logm(Cref)
 
 
-def distance_riemann(A, B):
-    r"""Affine-invariant Riemannian distance between SPD matrices.
+def log_map_riemann(X, Cref, C12=False):
+    r"""Project matrices in tangent space by Riemannian logarithmic map.
 
-    The affine-invariant Riemannian distance between two SPD matrices A and B
-    is:
+    The projection of a matrix :math:`\mathbf{X}` from SPD/HPD manifold
+    to tangent space by Riemannian logarithmic map
+    according to a SPD/HPD reference matrix :math:`\mathbf{C}_\text{ref}` is:
 
     .. math::
-        d(\mathbf{A},\mathbf{B}) =
-        {\left( \sum_i \log(\lambda_i)^2 \right)}^{1/2}
+        \mathbf{X}_\text{new} = \log ( \mathbf{C}_\text{ref}^{-1/2}
+        \mathbf{X} \mathbf{C}_\text{ref}^{-1/2})
 
-    where :math:`\lambda_i` are the joint eigenvalues of :math:`\mathbf{A}` and
-    :math:`\mathbf{B}`.
+    When C12=True, it returns the full Riemannian logarithmic map:
+
+    .. math::
+        \mathbf{X}_\text{new} = \mathbf{C}_\text{ref}^{1/2}
+        \log( \mathbf{C}_\text{ref}^{-1/2} \mathbf{X}
+        \mathbf{C}_\text{ref}^{-1/2}) \mathbf{C}_\text{ref}^{1/2}
 
     Parameters
     ----------
-    A : ndarray, shape (..., n, n)
-        First SPD matrices, at least 2D ndarray.
-    B : ndarray, shape (..., n, n)
-        Second SPD matrices, same dimensions as A.
+    X : ndarray, shape (..., n, n)
+        Matrices in SPD/HPD manidold.
+    Cref : ndarray, shape (n, n)
+        The reference SPD/HPD matrix.
+    C12 : bool, default=False
+        If True, it returns the full Riemannian logarithmic map.
 
     Returns
     -------
-    d : ndarray, shape (...,) or float
-        Affine-invariant Riemannian distance between A and B.
+    X_new : ndarray, shape (..., n, n)
+        Matrices projected in tangent space.
+
+    Notes
+    -----
+    .. versionadded:: 0.4
     """
-    _check_inputs(A, B)
-    return np.sqrt((np.log(_recursive(eigvalsh, A, B))**2).sum(axis=-1))
+    _check_dimensions(X, Cref)
+    Cm12 = invsqrtm(Cref)
+    X_new = logm(Cm12 @ X @ Cm12)
+    if C12:
+        C12 = sqrtm(Cref)
+        X_new = C12 @ X_new @ C12
+    return X_new
+
+
+def upper(X):
+    r"""Return the weighted upper triangular part of matrices.
+
+    This function computes the minimal representation of a matrix in tangent
+    space [1]_: it keeps the upper triangular part of the symmetric/Hermitian
+    matrix and vectorizes it by applying unity weight for diagonal elements and
+    :math:`\sqrt{2}` weight for out-of-diagonal elements.
+
+    Parameters
+    ----------
+    X : ndarray, shape (..., n, n)
+        Symmetric/Hermitian matrices.
 
+    Returns
+    -------
+    T : ndarray, shape (..., n * (n + 1) / 2)
+        Weighted upper triangular parts of symmetric/Hermitian matrices.
 
-def distance_wasserstein(A, B):
-    r"""Wasserstein distance between SPD matrices.
+    Notes
+    -----
+    .. versionadded:: 0.4
 
-    The Wasserstein distance between two SPD matrices A and B is:
+    References
+    ----------
+    .. [1] `Pedestrian detection via classification on Riemannian manifolds
+        <https://ieeexplore.ieee.org/document/4479482>`_
+        O. Tuzel, F. Porikli, and P. Meer. IEEE Transactions on Pattern
+        Analysis and Machine Intelligence, Volume 30, Issue 10, October 2008.
+    """
+    n = X.shape[-1]
+    if X.shape[-2] != n:
+        raise ValueError("Matrices must be square")
+    idx = np.triu_indices_from(np.empty((n, n)))
+    coeffs = (np.sqrt(2) * np.triu(np.ones((n, n)), 1) + np.eye(n))[idx]
+    T = coeffs * X[..., idx[0], idx[1]]
+    return T
 
-    .. math::
-        d(\mathbf{A},\mathbf{B}) =
-        \sqrt{ \text{tr}(A + B - 2(B^{1/2} A B^{1/2})^{1/2}) }
+
+def unupper(T):
+    """Inverse upper function.
+
+    This function is the inverse of upper function: it reconstructs symmetric/
+    Hermitian matrices from their weighted upper triangular parts.
 
     Parameters
     ----------
-    A : ndarray, shape (..., n, n)
-        First SPD matrices, at least 2D ndarray.
-    B : ndarray, shape (..., n, n)
-        Second SPD matrices, same dimensions as A.
+    T : ndarray, shape (..., n * (n + 1) / 2)
+        Weighted upper triangular parts of symmetric/Hermitian matrices.
 
     Returns
     -------
-    d : ndarray, shape (...,) or float
-        Wasserstein distance between A and B.
-    """
-    _check_inputs(A, B)
-    B12 = sqrtm(B)
-    dist2 = np.trace(A + B - 2 * sqrtm(B12 @ A @ B12), axis1=-2, axis2=-1)
-    dist2 = np.maximum(0, dist2)
-    return np.sqrt(dist2)
+    X : ndarray, shape (..., n, n)
+        Symmetric/Hermitian matrices.
 
+    See Also
+    --------
+    upper
 
-###############################################################################
+    Notes
+    -----
+    .. versionadded:: 0.4
+    """
+    dims = T.shape
+    n = int((np.sqrt(1 + 8 * dims[-1]) - 1) / 2)
+    X = np.empty((*dims[:-1], n, n), dtype=T.dtype)
+    idx = np.triu_indices_from(np.empty((n, n)))
+    X[..., idx[0], idx[1]] = T
+    idx = np.triu_indices_from(np.empty((n, n)), k=1)
+    X[..., idx[0], idx[1]] /= np.sqrt(2)
+    X[..., idx[1], idx[0]] = X[..., idx[0], idx[1]].conj()
+    return X
 
 
-distance_methods = {
-    'euclid': distance_euclid,
-    'harmonic': distance_harmonic,
-    'kullback': distance_kullback,
-    'kullback_right': distance_kullback_right,
-    'kullback_sym': distance_kullback_sym,
-    'logdet': distance_logdet,
-    'logeuclid': distance_logeuclid,
-    'riemann': distance_riemann,
-    'wasserstein': distance_wasserstein,
-}
-
-
-def _check_distance_method(method):
-    """Check distance methods."""
-    if isinstance(method, str):
-        if method not in distance_methods.keys():
-            raise ValueError('Unknown distance method')
-        else:
-            method = distance_methods[method]
-    elif not hasattr(method, '__call__'):
-        raise ValueError('Distance method must be a function or a string.')
-    return method
-
-
-def distance(A, B, metric='riemann'):
-    """Distance between SPD matrices according to a metric.
-
-    Compute the distance between two SPD matrices A and B according to a
-    metric, or between a set of SPD matrices A and a SPD matrix B.
+def tangent_space(X, Cref, *, metric='riemann'):
+    """Transform matrices into tangent vectors.
+
+    Transform matrices into tangent vectors, according to a reference
+    matrix Cref and to a specific logarithmic map.
 
     Parameters
     ----------
-    A : ndarray, shape (n, n) or shape (n_matrices, n, n)
-        First SPD matrix.
-    B : ndarray, shape (n, n)
-        Second SPD matrix.
+    X : ndarray, shape (..., n, n)
+        Matrices in manidold.
+    Cref : ndarray, shape (n, n)
+        The reference matrix.
     metric : string, default='riemann'
-        The metric for distance, can be: 'euclid', 'harmonic', 'kullback',
-        'kullback_right', 'kullback_sym', 'logdet', 'logeuclid', 'riemann',
-        'wasserstein', or a callable function.
+        The metric used for logarithmic map, can be: 'euclid', 'logeuclid',
+        'riemann'.
 
     Returns
     -------
-    d : float or ndarray, shape (n_matrices, 1)
-        The distance(s) between A and B.
-    """
-    if callable(metric):
-        distance_function = metric
-    else:
-        distance_function = distance_methods[metric]
-
-    shape_A = A.shape
-    if len(shape_A) == B.ndim:
-        d = distance_function(A, B)
-    elif len(shape_A) == 3:
-        d = np.empty((shape_A[0], 1))
-        for i in range(shape_A[0]):
-            d[i] = distance_function(A[i], B)
-    else:
-        raise ValueError("Inputs have incompatible dimensions.")
+    T : ndarray, shape (..., n * (n + 1) / 2)
+        Tangent vectors.
+
+    See Also
+    --------
+    log_map_euclid
+    log_map_logeuclid
+    log_map_riemann
+    upper
+    """
+    log_map_functions = {
+        'euclid': log_map_euclid,
+        'logeuclid': log_map_logeuclid,
+        'riemann': log_map_riemann,
+    }
+    X_ = log_map_functions[metric](X, Cref)
+    T = upper(X_)
 
-    return d
+    return T
 
 
-def pairwise_distance(X, Y=None, metric='riemann'):
-    """Pairwise distance matrix.
+def untangent_space(T, Cref, *, metric='riemann'):
+    """Transform tangent vectors back to matrices.
 
-    Compute the matrix of distances between pairs of elements of X and Y.
+    Transform tangent vectors back to matrices, according to a reference
+    matrix Cref and to a specific exponential map.
 
     Parameters
     ----------
-    X : ndarray, shape (n_matrices_X, n, n)
-        First set of SPD matrices.
-    Y : None | ndarray, shape (n_matrices_Y, n, n), default=None
-        Second set of SPD matrices. If None, Y is set to X.
+    T : ndarray, shape (..., n * (n + 1) / 2)
+        Tangent vectors.
+    Cref : ndarray, shape (n, n)
+        The reference matrix.
     metric : string, default='riemann'
-        The metric for distance, can be: 'euclid', 'harmonic', 'kullback',
-        'kullback_right', 'kullback_sym', 'logdet', 'logeuclid', 'riemann',
-        'wasserstein', or a callable function.
+        The metric used for exponential map, can be: 'euclid', 'logeuclid',
+        'riemann'.
 
     Returns
     -------
-    dist : ndarray, shape (n_matrices_X, n_matrices_X) or (n_matrices_X, \
-            n_matrices_Y)
-        The distances between pairs of elements of X if Y is None, or between
-        elements of X and Y.
-    """
-    n_matrices_X, _, _ = X.shape
-
-    if Y is None:
-        dist = np.zeros((n_matrices_X, n_matrices_X))
-        for i in range(n_matrices_X):
-            for j in range(i + 1, n_matrices_X):
-                dist[i, j] = distance(X[i], X[j], metric)
-        dist += dist.T
-    else:
-        n_matrices_Y, _, _ = Y.shape
-        dist = np.empty((n_matrices_X, n_matrices_Y))
-        for i in range(n_matrices_X):
-            for j in range(n_matrices_Y):
-                dist[i, j] = distance(X[i], Y[j], metric)
-    return dist
+    X : ndarray, shape (..., n, n)
+        Matrices in manidold.
 
+    See Also
+    --------
+    unupper
+    exp_map_euclid
+    exp_map_logeuclid
+    exp_map_riemann
+    """
+    X_ = unupper(T)
+    exp_map_functions = {
+        'euclid': exp_map_euclid,
+        'logeuclid': exp_map_logeuclid,
+        'riemann': exp_map_riemann,
+    }
+    X = exp_map_functions[metric](X_, Cref)
 
-###############################################################################
-# Distances between vectors and matrices
+    return X
 
 
-def distance_mahalanobis(X, cov, mean=None):
-    r"""Mahalanobis distance between vectors and a Gaussian distribution.
+###############################################################################
 
-    The Mahalanobis distance between a vector :math:`x` and a Gaussian
-    distribution :math:`\mathcal{N}(\mu, C)`, with mean :math:`\mu` and
-    covariance matrix :math:`C`, is:
 
-    .. math::
-        d(x, \mathcal{N}(\mu, C)) = \sqrt{ (x - \mu)^H C^{-1} (x - \mu) }
+# NOT IN API
+def transport(Covs, Cref, metric='riemann'):
+    """Parallel transport of a set of SPD matrices towards a reference matrix.
 
     Parameters
     ----------
-    X : ndarray, shape (n_channels, n_vectors)
-        Multi-channel vectors.
-    cov : ndarray, shape (n_channels, n_channels)
-        Covariance matrix of the Gaussian distribution.
-    mean : None | ndarray, shape (n_channels, 1), default=None
-        Mean of the Gaussian distribution. If None, distribution is considered
-        as centered.
+    Covs : ndarray, shape (n_matrices, n, n)
+        Set of SPD matrices.
+    Cref : ndarray, shape (n, n)
+        The reference SPD matrix.
+    metric : string, default='riemann'
+        The metric used for mean, can be: 'euclid', 'logeuclid', 'riemann'.
 
     Returns
     -------
-    d : ndarray, shape (n_vectors,)
-        Mahalanobis distances.
-
-    Notes
-    -----
-    .. versionadded:: 0.3.1
-
-    References
-    ----------
-    .. [1] https://docs.scipy.org/doc/scipy/reference/generated/scipy.spatial.distance.mahalanobis.html
-    """  # noqa
-    if mean is not None:
-        X -= mean
-
-    Xw = invsqrtm(cov) @ X
-    dist2 = np.einsum('ij,ji->i', Xw.conj().T, Xw)
-    return np.sqrt(dist2)
+    out : ndarray, shape (n_matrices, n, n)
+        Set of transported SPD matrices.
+    """
+    C = mean_covariance(Covs, metric=metric)
+    iC = invsqrtm(C)
+    E = sqrtm(iC @ Cref @ iC)
+    out = E @ Covs @ E.T
+    return out
```

### Comparing `pyriemann-0.4/pyriemann/utils/docs.py` & `pyriemann-0.5/pyriemann/utils/docs.py`

 * *Files identical despite different names*

### Comparing `pyriemann-0.4/pyriemann/utils/geodesic.py` & `pyriemann-0.5/pyriemann/utils/geodesic.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,127 +1,131 @@
-"""Geodesics for SPD matrices."""
+"""Geodesics for SPD/HPD matrices."""
 
 from .base import sqrtm, invsqrtm, powm, logm, expm
 
 
 def geodesic_euclid(A, B, alpha=0.5):
-    r"""Euclidean geodesic between SPD matrices.
+    r"""Euclidean geodesic between matrices.
 
-    The matrix at the position alpha on the Euclidean geodesic between two SPD
-    matrices A and B is:
+    The matrix at position :math:`\alpha` on the Euclidean geodesic
+    between two matrices :math:`\mathbf{A}` and :math:`\mathbf{B}` is:
 
     .. math::
         \mathbf{C} = (1-\alpha) \mathbf{A} + \alpha \mathbf{B}
 
-    C is equal to A if alpha = 0 and B if alpha = 1.
+    :math:`\mathbf{C}` is equal to :math:`\mathbf{A}` if :math:`\alpha` = 0,
+    and :math:`\mathbf{B}` if :math:`\alpha` = 1.
 
     Parameters
     ----------
-    A : ndarray, shape (..., n, n)
-        First SPD matrices.
-    B : ndarray, shape (..., n, n)
-        Second SPD matrices.
+    A : ndarray, shape (..., n, m)
+        First matrices.
+    B : ndarray, shape (..., n, m)
+        Second matrices.
     alpha : float, default=0.5
         The position on the geodesic.
 
     Returns
     -------
-    C : ndarray, shape (..., n, n)
-        SPD matrices on the Euclidean geodesic.
+    C : ndarray, shape (..., n, m)
+        Matrices on the Euclidean geodesic.
     """
     return (1 - alpha) * A + alpha * B
 
 
 def geodesic_logeuclid(A, B, alpha=0.5):
-    r"""Log-Euclidean geodesic between SPD matrices.
+    r"""Log-Euclidean geodesic between SPD/HPD matrices.
 
-    The matrix at the position alpha on the Log-Euclidean geodesic between two
-    SPD matrices A and B is:
+    The matrix at position :math:`\alpha` on the Log-Euclidean geodesic
+    between two SPD/HPD matrices :math:`\mathbf{A}` and :math:`\mathbf{B}` is:
 
     .. math::
         \mathbf{C} = \exp \left( (1-\alpha) \log(\mathbf{A})
                      + \alpha \log(\mathbf{B}) \right)
 
-    C is equal to A if alpha = 0 and B if alpha = 1.
+    :math:`\mathbf{C}` is equal to :math:`\mathbf{A}` if :math:`\alpha` = 0,
+    and :math:`\mathbf{B}` if :math:`\alpha` = 1.
 
     Parameters
     ----------
     A : ndarray, shape (..., n, n)
-        First SPD matrices.
+        First SPD/HPD matrices.
     B : ndarray, shape (..., n, n)
-        Second SPD matrices.
+        Second SPD/HPD matrices.
     alpha : float, default=0.5
         The position on the geodesic.
 
     Returns
     -------
     C : ndarray, shape (..., n, n)
-        SPD matrices on the Log-Euclidean geodesic.
+        SPD/HPD matrices on the Log-Euclidean geodesic.
     """
     return expm((1 - alpha) * logm(A) + alpha * logm(B))
 
 
 def geodesic_riemann(A, B, alpha=0.5):
-    r"""Affine-invariant Riemannian geodesic between SPD matrices.
+    r"""Affine-invariant Riemannian geodesic between SPD/HPD matrices.
 
-    The matrix at the position alpha on the affine-invariant Riemannian
-    geodesic between two SPD matrices A and B is:
+    The matrix at position :math:`\alpha` on the affine-invariant Riemannian
+    geodesic between two SPD/HPD matrices :math:`\mathbf{A}` and
+    :math:`\mathbf{B}` is:
 
     .. math::
         \mathbf{C} = \mathbf{A}^{1/2} \left( \mathbf{A}^{-1/2} \mathbf{B}
                      \mathbf{A}^{-1/2} \right)^\alpha \mathbf{A}^{1/2}
 
-    C is equal to A if alpha = 0 and B if alpha = 1.
+    :math:`\mathbf{C}` is equal to :math:`\mathbf{A}` if :math:`\alpha` = 0,
+    and :math:`\mathbf{B}` if :math:`\alpha` = 1.
 
     Parameters
     ----------
     A : ndarray, shape (..., n, n)
-        First SPD matrices.
+        First SPD/HPD matrices.
     B : ndarray, shape (..., n, n)
-        Second SPD matrices.
+        Second SPD/HPD matrices.
     alpha : float, default=0.5
         The position on the geodesic.
 
     Returns
     -------
     C : ndarray, shape (..., n, n)
-        SPD matrices on the affine-invariant Riemannian geodesic.
+        SPD/HPD matrices on the affine-invariant Riemannian geodesic.
     """
     sA, isA = sqrtm(A), invsqrtm(A)
     C = isA @ B @ isA
     D = powm(C, alpha)
     E = sA @ D @ sA
     return E
 
 
 ###############################################################################
 
 
 def geodesic(A, B, alpha, metric='riemann'):
-    """Geodesic between SPD matrices according to a metric.
+    """Geodesic between matrices according to a metric.
 
-    Return the matrix at the position alpha on the geodesic between SPD
-    matrices A and B according to a metric.
+    Return the matrix at the position alpha on the geodesic between matrices
+    A and B according to a metric.
 
     Parameters
     ----------
     A : ndarray, shape (..., n, n)
-        First SPD matrices.
+        First matrices.
     B : ndarray, shape (..., n, n)
-        Second SPD matrices.
+        Second matrices.
     alpha : float
         The position on the geodesic.
     metric : string, default='riemann'
         The metric used for geodesic, can be: 'euclid', 'logeuclid', 'riemann'.
 
     Returns
     -------
     C : ndarray, shape (..., n, n)
-        SPD matrices on the geodesic.
+        Matrices on the geodesic.
     """
-    options = {
+    geodesic_functions = {
         'euclid': geodesic_euclid,
         'logeuclid': geodesic_logeuclid,
         'riemann': geodesic_riemann,
     }
-    C = options[metric](A, B, alpha)
+    C = geodesic_functions[metric](A, B, alpha)
     return C
```

### Comparing `pyriemann-0.4/pyriemann/utils/kernel.py` & `pyriemann-0.5/pyriemann/utils/kernel.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,28 +3,29 @@
 import numpy as np
 
 from .base import invsqrtm, logm
 from .mean import mean_riemann
 
 
 def kernel_euclid(X, Y=None, *, reg=1e-10, **kwargs):
-    r"""Euclidean kernel between two sets of SPD matrices.
+    r"""Euclidean kernel between two sets of matrices.
 
-    Calculates the Euclidean kernel matrix K of inner products of two sets
-    X and Y of SPD matrices by calculating pairwise:
+    Calculates the Euclidean kernel matrix :math:`\mathbf{K}` of inner products
+    of two sets :math:`\mathbf{X}` and :math:`\mathbf{Y}` of matrices in
+    :math:`\mathbb{R}^{n \times m}` by calculating pairwise products:
 
     .. math::
-        K_{i,j} = \text{tr}(X_i Y_j)
+        \mathbf{K}_{i,j} = \text{tr}(\mathbf{X}_i^T \mathbf{Y}_j)
 
     Parameters
     ----------
-    X : ndarray, shape (n_matrices_X, n_channels, n_channels)
-        First set of SPD matrices.
-    Y : None | ndarray, shape (n_matrices_Y, n_channels, n_channels), default=None
-        Second set of SPD matrices. If None, Y is set to X.
+    X : ndarray, shape (n_matrices_X, n, m)
+        First set of matrices.
+    Y : None | ndarray, shape (n_matrices_Y, n, m), default=None
+        Second set of matrices. If None, Y is set to X.
     reg : float, default=1e-10
         Regularization parameter to mitigate numerical errors in kernel
         matrix estimation.
 
     Returns
     -------
     K : ndarray, shape (n_matrices_X, n_matrices_Y)
@@ -33,35 +34,37 @@
     Notes
     -----
     .. versionadded:: 0.3
 
     See Also
     --------
     kernel
-    """  # noqa
+    """
     def kernelfct(X, Cref):
         return X
 
     return _apply_matrix_kernel(kernelfct, X, Y, reg=reg)
 
 
 def kernel_logeuclid(X, Y=None, *, reg=1e-10, **kwargs):
     r"""Log-Euclidean kernel between two sets of SPD matrices.
 
-    Calculates the Log-Euclidean kernel matrix K of inner products of two sets
-    X and Y of SPD matrices by calculating pairwise [1]_:
+    Calculates the Log-Euclidean kernel matrix :math:`\mathbf{K}` of inner
+    products of two sets :math:`\mathbf{X}` and :math:`\mathbf{Y}` of SPD
+    matrices in :math:`\mathbb{R}^{n \times n}` by calculating pairwise
+    products [1]_:
 
     .. math::
-        K_{i,j} = \text{tr}(\log(X_i) \log(Y_j))
+        \mathbf{K}_{i,j} = \text{tr}(\log(\mathbf{X}_i) \log(\mathbf{Y}_j))
 
     Parameters
     ----------
-    X : ndarray, shape (n_matrices_X, n_channels, n_channels)
+    X : ndarray, shape (n_matrices_X, n, n)
         First set of SPD matrices.
-    Y : None | ndarray, shape (n_matrices_Y, n_channels, n_channels), default=None
+    Y : None | ndarray, shape (n_matrices_Y, n, n), default=None
         Second set of SPD matrices. If None, Y is set to X.
     reg : float, default=1e-10
         Regularization parameter to mitigate numerical errors in kernel
         matrix estimation.
 
     Returns
     -------
@@ -79,39 +82,42 @@
     References
     ----------
     .. [1] `Classification of covariance matrices using a Riemannian-based
         kernel for BCI applications
         <https://hal.archives-ouvertes.fr/hal-00820475/>`_
         A. Barachant, S. Bonnet, M. Congedo and C. Jutten. Neurocomputing,
         Elsevier, 2013, 112, pp.172-178.
-    """  # noqa
+    """
     def kernelfct(X, Cref):
         return logm(X)
 
     return _apply_matrix_kernel(kernelfct, X, Y, reg=reg)
 
 
 def kernel_riemann(X, Y=None, *, Cref=None, reg=1e-10):
     r"""Affine-invariant Riemannian kernel between two sets of SPD matrices.
 
-    Calculates the affine-invariant Riemannian kernel matrix K of inner
-    products of two sets X and Y of SPD matrices on tangent space of Cref by
-    calculating pairwise [1]_:
+    Calculates the affine-invariant Riemannian kernel matrix :math:`\mathbf{K}`
+    of inner products of two sets :math:`\mathbf{X}` and :math:`\mathbf{Y}` of
+    SPD matrices in :math:`\mathbb{R}^{n \times n}` on tangent space at
+    :math:`\mathbf{C}_\text{ref}` by calculating pairwise products [1]_:
 
     .. math::
-        K_{i,j} = \text{tr}(\log(C_\text{ref}^{-1/2} X_i C_\text{ref}^{-1/2})
-        \log(C_\text{ref}^{-1/2} Y_j C_\text{ref}^{-1/2}) )
+        \mathbf{K}_{i,j} = \text{tr}( \log( \mathbf{C}_\text{ref}^{-1/2}
+        \mathbf{X}_i \mathbf{C}_\text{ref}^{-1/2} )
+        \log( \mathbf{C}_\text{ref}^{-1/2} \mathbf{Y}_j
+        \mathbf{C}_\text{ref}^{-1/2}) )
 
     Parameters
     ----------
-    X : ndarray, shape (n_matrices_X, n_channels, n_channels)
+    X : ndarray, shape (n_matrices_X, n, n)
         First set of SPD matrices.
-    Y : None | ndarray, shape (n_matrices_Y, n_channels, n_channels), default=None
+    Y : None | ndarray, shape (n_matrices_Y, n, n), default=None
         Second set of SPD matrices. If None, Y is set to X.
-    Cref : None | ndarray, shape (n_channels, n_channels), default=None
+    Cref : None | ndarray, shape (n, n), default=None
         Reference point for the tangent space and inner product calculation.
         If None, Cref is calculated as the Riemannian mean of X.
     reg : float, default=1e-10
         Regularization parameter to mitigate numerical errors in kernel
         matrix estimation.
 
     Returns
@@ -130,15 +136,15 @@
     References
     ----------
     .. [1] `Classification of covariance matrices using a Riemannian-based
         kernel for BCI applications
         <https://hal.archives-ouvertes.fr/hal-00820475/>`_
         A. Barachant, S. Bonnet, M. Congedo and C. Jutten. Neurocomputing,
         Elsevier, 2013, 112, pp.172-178.
-    """  # noqa
+    """
     def kernelfct(X, Cref):
         if Cref is None:
             Cref = mean_riemann(X)
 
         C_invsq = invsqrtm(Cref)
         X_ = logm(C_invsq @ X @ C_invsq)
         return X_
@@ -163,53 +169,47 @@
                                           f"Expected {X.shape[1:]}, got " \
                                           f"{Cref.shape}."
 
 
 def _apply_matrix_kernel(kernel_fct, X, Y=None, *, Cref=None, reg=1e-10):
     """Apply a matrix kernel function."""
     _check_dimensions(X, Y, Cref)
-    n_matrices_X, n_channels, n_channels = X.shape
+    n_matrices_X, n, n = X.shape
 
     X_ = kernel_fct(X, Cref)
 
     if isinstance(Y, type(None)) or np.array_equal(X, Y):
         Y_ = X_
-
     else:
         Y_ = kernel_fct(Y, Cref)
 
-    # calculate scalar products
-    # for i in range(n_matrices_X):
-    #     for j in range(n_matrices_Y):
-    #         K[i][j] = np.trace(X_[i] @ Y_[j])
-    # einsum does same as that just a looooooot faster
-
-    K = np.einsum('abc,dbc->ad', X_, Y_, optimize=True)
+    # calculate scalar products: K[i,j] = np.trace(X_[i]^T @ Y_[j])
+    X_T = X_.transpose((0, 2, 1))
+    K = np.einsum('acb,dbc->ad', X_T, Y_, optimize=True)
 
     # regularization due to numerical errors
     if np.array_equal(X_, Y_):
         K.flat[:: n_matrices_X + 1] += reg
 
     return K
 
 
 def kernel(X, Y=None, *, Cref=None, metric='riemann', reg=1e-10):
-    """Kernel matrix between SPD matrices according to a specified metric.
+    """Kernel matrix between matrices according to a specified metric.
 
     Calculates the kernel matrix K of inner products of two sets X and Y of
-    SPD matrices on the tangent space of Cref according to a specified metric.
+    matrices on the tangent space at Cref according to a specified metric.
 
     Parameters
     ----------
-    X : ndarray, shape (n_matrices_X, n_channels, n_channels)
-        First set of SPD matrices.
-    Y : None | ndarray, shape (n_matrices_Y, n_channels, n_channels), \
-            default=None
-        Second set of SPD matrices. If None, Y is set to X.
-    Cref : None | ndarray, shape (n_channels, n_channels), default=None
+    X : ndarray, shape (n_matrices_X, n, n)
+        First set of matrices.
+    Y : None | ndarray, shape (n_matrices_Y, n, n), default=None
+        Second set of matrices. If None, Y is set to X.
+    Cref : None | ndarray, shape (n, n), default=None
         Reference point for the tangent space and inner product
         calculation. Only used if metric='riemann'.
     metric : {'euclid', 'logeuclid', 'riemann'}, default='riemann'
         The type of metric used for tangent space and mean estimation.
     reg : float, default=1e-10
         Regularization parameter to mitigate numerical errors in kernel
         matrix estimation, to provide a positive-definite kernel matrix.
```

### Comparing `pyriemann-0.4/pyriemann/utils/mean.py` & `pyriemann-0.5/pyriemann/utils/mean.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,228 +1,256 @@
-"""Means of SPD matrices."""
+"""Means of SPD/HPD matrices."""
 
-import warnings
 from copy import deepcopy
 import numpy as np
+import warnings
 
 from .ajd import ajd_pham
 from .base import sqrtm, invsqrtm, logm, expm, powm
 from .distance import distance_riemann
 from .geodesic import geodesic_riemann
 from .utils import check_weights
 
 
 def mean_ale(covmats, tol=10e-7, maxiter=50, sample_weight=None):
     """AJD-based log-Euclidean (ALE) mean of SPD matrices.
 
-    Return the mean of a set of SPD matrices using the AJD-based log-Euclidean
-    (ALE) mean [1]_.
+    Return the mean of a set of SPD matrices using the approximate joint
+    diagonalization (AJD) based log-Euclidean (ALE) mean [1]_.
 
     Parameters
     ----------
-    covmats : ndarray, shape (n_matrices, n_channels, n_channels)
+    covmats : ndarray, shape (n_matrices, n, n)
         Set of SPD matrices.
     tol : float, default=10e-7
         The tolerance to stop the gradient descent.
     maxiter : int, default=50
         The maximum number of iterations.
     sample_weight : None | ndarray, shape (n_matrices,), default=None
         Weights for each matrix. If None, it uses equal weights.
 
     Returns
     -------
-    C : ndarray, shape (n_channels, n_channels)
+    C : ndarray, shape (n, n)
         ALE mean.
 
     Notes
     -----
     .. versionadded:: 0.2.4
 
+    See Also
+    --------
+    mean_covariance
+
     References
     ----------
     .. [1] `Approximate Joint Diagonalization and Geometric Mean of Symmetric
         Positive Definite Matrices
         <https://arxiv.org/abs/1505.07343>`_
         M. Congedo, B. Afsari, A. Barachant, M. Moakher. PLOS ONE, 2015
     """
-    n_matrices, n_channels, _ = covmats.shape
+    n_matrices, n, _ = covmats.shape
     sample_weight = check_weights(sample_weight, n_matrices)
 
     # init with AJD
-    B, _ = ajd_pham(covmats)
+    B = ajd_pham(covmats)[0]
 
+    eye_n = np.eye(n)
     crit = np.inf
     for _ in range(maxiter):
-        J = np.einsum('a,abc->bc', sample_weight, logm(B.T @ covmats @ B))
-        update = np.diag(np.diag(expm(J)))
-        B = B @ invsqrtm(update)
+        J = np.einsum(
+            'a,abc->bc',
+            sample_weight,
+            logm(B @ covmats @ B.conj().T)
+        )
+        delta = np.real(np.diag(expm(J)))
+        B = (np.abs(delta) ** -.5)[:, np.newaxis] * B
 
-        crit = distance_riemann(np.eye(n_channels), update)
+        crit = distance_riemann(eye_n, np.diag(delta))
         if crit <= tol:
             break
     else:
-        warnings.warn('Convergence not reached')
+        warnings.warn("Convergence not reached")
 
+    J = np.einsum('a,abc->bc', sample_weight, logm(B @ covmats @ B.conj().T))
     A = np.linalg.inv(B)
-    J = np.einsum('a,abc->bc', sample_weight, logm(B.T @ covmats @ B))
-    C = A.T @ expm(J) @ A
+    C = A @ expm(J) @ A.conj().T
     return C
 
 
 def mean_alm(covmats, tol=1e-14, maxiter=100, sample_weight=None):
-    r"""Ando-Li-Mathias (ALM) mean of SPD matrices.
+    r"""Ando-Li-Mathias (ALM) mean of SPD/HPD matrices.
 
     Return the geometric mean recursively [1]_, generalizing from:
 
     .. math::
-        \mathbf{C} = A^{\frac{1}{2}}(A^{-\frac{1}{2}}B^{\frac{1}{2}}
-                     A^{-\frac{1}{2}})^{\frac{1}{2}}A^{\frac{1}{2}}
+        \mathbf{C} = X_1^{\frac{1}{2}} (X_1^{-\frac{1}{2}}X_2^{\frac{1}{2}}
+                     X_1^{-\frac{1}{2}})^{\frac{1}{2}} X_1^{\frac{1}{2}}
 
     and requiring a high number of iterations.
-
-    This is the adaptation of the Matlab code proposed by Dario Bini and
-    Bruno Iannazzo, http://bezout.dm.unipi.it/software/mmtoolbox/ .
     Extremely slow, due to the recursive formulation.
 
     Parameters
     ----------
-    covmats : ndarray, shape (n_matrices, n_channels, n_channels)
-        Set of SPD matrices.
+    covmats : ndarray, shape (n_matrices, n, n)
+        Set of SPD/HPD matrices.
     tol : float, default=10e-14
         The tolerance to stop the gradient descent.
     maxiter : int, default=100
         The maximum number of iterations.
     sample_weight : None | ndarray, shape (n_matrices,), default=None
         Weights for each matrix. If None, it uses equal weights.
 
     Returns
     -------
-    C : ndarray, shape (n_channels, n_channels)
+    C : ndarray, shape (n, n)
         ALM mean.
 
     Notes
     -----
     .. versionadded:: 0.3
 
+    See Also
+    --------
+    mean_covariance
+
     References
     ----------
     .. [1] `Geometric Means
         <https://www.sciencedirect.com/science/article/pii/S0024379503008693>`_
         T. Ando, C.-K. Li, and R. Mathias. Linear Algebra and its Applications.
         Volume 385, July 2004, Pages 305-334.
     """
     n_matrices, _, _ = covmats.shape
     sample_weight = check_weights(sample_weight, n_matrices)
-    C = covmats
-    C_iter = np.zeros_like(C)
+
     if n_matrices == 2:
         alpha = sample_weight[1] / sample_weight[0] / 2
-        X = geodesic_riemann(covmats[0], covmats[1], alpha=alpha)
-        return X
+        C = geodesic_riemann(covmats[0], covmats[1], alpha=alpha)
+        return C
+
+    C = covmats
+    C_iter = np.zeros_like(C)
+    for _ in range(maxiter):
+        for h in range(n_matrices):
+            s = np.mod(np.arange(h, h + n_matrices - 1) + 1, n_matrices)
+            C_iter[h] = mean_alm(C[s], sample_weight=sample_weight[s])
+
+        norm_iter = np.linalg.norm(C_iter[0] - C[0], 2)
+        norm_c = np.linalg.norm(C[0], 2)
+        if (norm_iter / norm_c) < tol:
+            break
+        C = deepcopy(C_iter)
     else:
-        for _ in range(maxiter):
-            for h in range(n_matrices):
-                s = np.mod(np.arange(h, h + n_matrices - 1) + 1, n_matrices)
-                C_iter[h] = mean_alm(C[s], sample_weight=sample_weight[s])
-
-            norm_iter = np.linalg.norm(C_iter[0] - C[0], 2)
-            norm_c = np.linalg.norm(C[0], 2)
-            if (norm_iter / norm_c) < tol:
-                break
-            C = deepcopy(C_iter)
-        else:
-            warnings.warn('Convergence not reached')
-        return C_iter.mean(axis=0)
+        warnings.warn("Convergence not reached")
+
+    return C_iter.mean(axis=0)
 
 
 def mean_euclid(covmats, sample_weight=None):
     r"""Mean of matrices according to the Euclidean metric.
 
     .. math::
-        \mathbf{C} = \frac{1}{m} \sum_i \mathbf{C}_i
+        \mathbf{C} = \sum_i w_i \ \mathbf{X}_i
 
     This mean is also called arithmetic.
 
     Parameters
     ----------
-    covmats : ndarray, shape (n_matrices, n_channels, n_channels)
+    covmats : ndarray, shape (n_matrices, n, m)
         Set of matrices.
     sample_weight : None | ndarray, shape (n_matrices,), default=None
         Weights for each matrix. If None, it uses equal weights.
 
     Returns
     -------
-    C : ndarray, shape (n_channels, n_channels)
+    C : ndarray, shape (n, m)
         Euclidean mean.
+
+    See Also
+    --------
+    mean_covariance
     """
     return np.average(covmats, axis=0, weights=sample_weight)
 
 
 def mean_harmonic(covmats, sample_weight=None):
-    r"""Harmonic mean of SPD matrices.
+    r"""Harmonic mean of invertible matrices.
 
     .. math::
-        \mathbf{C} = \left(\frac{1}{m} \sum_i {\mathbf{C}_i}^{-1}\right)^{-1}
+        \mathbf{C} = \left( \sum_i wi \ {\mathbf{X}_i}^{-1} \right)^{-1}
 
     Parameters
     ----------
-    covmats : ndarray, shape (n_matrices, n_channels, n_channels)
-        Set of SPD matrices.
+    covmats : ndarray, shape (n_matrices, n, n)
+        Set of invertible matrices.
     sample_weight : None | ndarray, shape (n_matrices,), default=None
         Weights for each matrix. If None, it uses equal weights.
 
     Returns
     -------
-    C : ndarray, shape (n_channels, n_channels)
+    C : ndarray, shape (n, n)
         Harmonic mean.
+
+    See Also
+    --------
+    mean_covariance
     """
     T = mean_euclid(np.linalg.inv(covmats), sample_weight=sample_weight)
     C = np.linalg.inv(T)
     return C
 
 
 def mean_identity(covmats, sample_weight=None):
     r"""Identity matrix corresponding to the matrices dimension.
 
     .. math::
-        \mathbf{C} = \mathbf{I}_c
+        \mathbf{C} = \mathbf{I}_n
 
     Parameters
     ----------
-    covmats : ndarray, shape (n_matrices, n_channels, n_channels)
-        Set of SPD matrices.
+    covmats : ndarray, shape (n_matrices, n, n)
+        Set of square matrices.
     sample_weight : None
         Not used, here for compatibility with other means.
 
     Returns
     -------
-    C : ndarray, shape (n_channels, n_channels)
+    C : ndarray, shape (n, n)
         Identity matrix.
+
+    See Also
+    --------
+    mean_covariance
     """
     C = np.eye(covmats.shape[-1])
     return C
 
 
 def mean_kullback_sym(covmats, sample_weight=None):
-    """Mean of SPD matrices according to Kullback-Leibler divergence.
+    """Mean of SPD/HPD matrices according to Kullback-Leibler divergence.
 
     Symmetrized Kullback-Leibler mean is the geometric mean between the
-    Euclidean and the harmonic means, as shown in [1]_.
+    Euclidean and the harmonic means [1]_.
 
     Parameters
     ----------
-    covmats : ndarray, shape (n_matrices, n_channels, n_channels)
-        Set of SPD matrices.
+    covmats : ndarray, shape (n_matrices, n, n)
+        Set of SPD/HPD matrices.
     sample_weight : None | ndarray, shape (n_matrices,), default=None
         Weights for each matrix. If None, it uses equal weights.
 
     Returns
     -------
-    C : ndarray, shape (n_channels, n_channels)
-        Kullback-Leibler mean.
+    C : ndarray, shape (n, n)
+        Symmetrized Kullback-Leibler mean.
+
+    See Also
+    --------
+    mean_covariance
 
     References
     ----------
     .. [1] `Symmetric positive-definite matrices: From geometry to applications
         and visualization
         <https://link.springer.com/chapter/10.1007/3-540-31272-2_17>`_
         M. Moakher and P. Batchelor. Visualization and Processing of Tensor
@@ -231,40 +259,44 @@
     C_euclid = mean_euclid(covmats, sample_weight=sample_weight)
     C_harmonic = mean_harmonic(covmats, sample_weight=sample_weight)
     C = geodesic_riemann(C_euclid, C_harmonic, 0.5)
     return C
 
 
 def mean_logdet(covmats, tol=10e-5, maxiter=50, init=None, sample_weight=None):
-    r"""Mean of SPD matrices according to the log-det metric.
+    r"""Mean of SPD/HPD matrices according to the log-det metric.
 
     Log-det mean is obtained by an iterative procedure where the update is:
 
     .. math::
-        \mathbf{C} = \left(\sum_i \left( 0.5 \mathbf{C}
-                     + 0.5 \mathbf{C}_i \right)^{-1} \right)^{-1}
+        \mathbf{C} = \left( \sum_i w_i \ \left( 0.5 \mathbf{C}
+                     + 0.5 \mathbf{X}_i \right)^{-1} \right)^{-1}
 
     Parameters
     ----------
-    covmats : ndarray, shape (n_matrices, n_channels, n_channels)
-        Set of SPD matrices.
+    covmats : ndarray, shape (n_matrices, n, n)
+        Set of SPD/HPD matrices.
     tol : float, default=10e-5
         The tolerance to stop the gradient descent.
     maxiter : int, default=50
         The maximum number of iterations.
-    init : None | ndarray, shape (n_channels, n_channels), default=None
-        A SPD matrix used to initialize the gradient descent.
+    init : None | ndarray, shape (n, n), default=None
+        A SPD/HPD matrix used to initialize the gradient descent.
         If None, the weighted Euclidean mean is used.
     sample_weight : None | ndarray, shape (n_matrices,), default=None
         Weights for each matrix. If None, it uses equal weights.
 
     Returns
     -------
-    C : ndarray, shape (n_channels, n_channels)
+    C : ndarray, shape (n, n)
         Log-det mean.
+
+    See Also
+    --------
+    mean_covariance
     """
     n_matrices, _, _ = covmats.shape
     sample_weight = check_weights(sample_weight, n_matrices)
     if init is None:
         C = mean_euclid(covmats, sample_weight=sample_weight)
     else:
         C = init
@@ -276,85 +308,93 @@
         Cnew = np.linalg.inv(J)
 
         crit = np.linalg.norm(Cnew - C, ord='fro')
         C = Cnew
         if crit <= tol:
             break
     else:
-        warnings.warn('Convergence not reached')
+        warnings.warn("Convergence not reached")
 
     return C
 
 
 def mean_logeuclid(covmats, sample_weight=None):
-    r"""Mean of SPD matrices according to the log-Euclidean metric.
+    r"""Mean of SPD/HPD matrices according to the log-Euclidean metric.
 
     Log-Euclidean mean is [1]_:
 
     .. math::
-        \mathbf{C} = \exp{(\frac{1}{m} \sum_i \log{\mathbf{C}_i})}
+        \mathbf{C} = \exp{ \left( \sum_i w_i \ \log{\mathbf{X}_i} \right) }
 
     Parameters
     ----------
-    covmats : ndarray, shape (n_matrices, n_channels, n_channels)
-        Set of SPD matrices.
+    covmats : ndarray, shape (n_matrices, n, n)
+        Set of SPD/HPD matrices.
     sample_weight : None | ndarray, shape (n_matrices,), default=None
         Weights for each matrix. If None, it uses equal weights.
 
     Returns
     -------
-    C : ndarray, shape (n_channels, n_channels)
+    C : ndarray, shape (n, n)
         Log-Euclidean mean.
 
+    See Also
+    --------
+    mean_covariance
+
     References
     ----------
     .. [1] `Geometric means in a novel vector space structure on symmetric
         positive-definite matrices
         <https://epubs.siam.org/doi/abs/10.1137/050637996?journalCode=sjmael>`_
         V. Arsigny, P. Fillard, X. Pennec, and N. Ayache. SIAM Journal on
         Matrix Analysis and Applications. Volume 29, Issue 1 (2007).
     """
     C = expm(mean_euclid(logm(covmats), sample_weight=sample_weight))
     return C
 
 
 def mean_power(covmats, p, *, sample_weight=None, zeta=10e-10, maxiter=100):
-    r"""Power mean of SPD matrices.
+    r"""Power mean of SPD/HPD matrices.
 
-    Power mean is the solution of [1]_ [2]_:
+    Power mean of order p is the solution of [1]_ [2]_:
 
     .. math::
-        \mathbf{C} = \frac{1}{m} \sum_i \mathbf{C} \sharp_p \mathbf{C}_i
+        \mathbf{C} = \sum_i w_i \ \mathbf{C} \sharp_p \mathbf{X}_i
 
     where :math:`\mathbf{A} \sharp_p \mathbf{B}` is the geodesic between
     matrices :math:`\mathbf{A}` and :math:`\mathbf{B}`.
 
     Parameters
     ----------
-    covmats : ndarray, shape (n_matrices, n_channels, n_channels)
-        Set of SPD matrices.
+    covmats : ndarray, shape (n_matrices, n, n)
+        Set of SPD/HPD matrices.
     p : float
         Exponent, in [-1,+1]. For p=0, it returns
         :func:`pyriemann.utils.mean.mean_riemann`.
     sample_weight : None | ndarray, shape (n_matrices,), default=None
         Weights for each matrix. If None, it uses equal weights.
     zeta : float, default=10e-10
         Stopping criterion.
     maxiter : int, default=100
         The maximum number of iterations.
 
     Returns
     -------
-    C : ndarray, shape (n_channels, n_channels)
+    C : ndarray, shape (n, n)
         Power mean.
 
     Notes
     -----
     .. versionadded:: 0.3
 
+    See Also
+    --------
+    mean_covariance
+
     References
     ----------
     .. [1] `Matrix Power means and the Karcher mean
         <https://www.sciencedirect.com/science/article/pii/S0022123611004101>`_
         Y. Lim and M. Palfia. Journal of Functional Analysis, Volume 262,
         Issue 4, 15 February 2012, Pages 1498-1514.
     .. [2] `Fixed Point Algorithms for Estimating Power Means of Positive
@@ -364,87 +404,99 @@
         Processing, Volume 65, Issue 9, pp.2211-2220, May 2017
     """
     if not isinstance(p, (int, float)):
         raise ValueError("Power mean only defined for a scalar exponent")
     if p < -1 or 1 < p:
         raise ValueError("Exponent must be in [-1,+1]")
 
-    if p == 0:
+    if p == 1:
+        return mean_euclid(covmats, sample_weight=sample_weight)
+    elif p == 0:
         return mean_riemann(covmats, sample_weight=sample_weight)
+    elif p == -1:
+        return mean_harmonic(covmats, sample_weight=sample_weight)
 
-    n_matrices, n_channels, _ = covmats.shape
+    n_matrices, n, _ = covmats.shape
     sample_weight = check_weights(sample_weight, n_matrices)
     phi = 0.375 / np.abs(p)
 
     G = np.einsum('a,abc->bc', sample_weight, powm(covmats, p))
     if p > 0:
         X = invsqrtm(G)
     else:
         X = sqrtm(G)
 
-    eye_n, sqrt_n = np.eye(n_channels), np.sqrt(n_channels)
+    eye_n, sqrt_n = np.eye(n), np.sqrt(n)
     crit = 10 * zeta
     for _ in range(maxiter):
         H = np.einsum(
             'a,abc->bc',
             sample_weight,
-            powm(X @ powm(covmats, np.sign(p)) @ X.T, np.abs(p))
+            powm(X @ powm(covmats, np.sign(p)) @ X.conj().T, np.abs(p))
         )
         X = powm(H, -phi) @ X
 
         crit = np.linalg.norm(H - eye_n) / sqrt_n
         if crit <= zeta:
             break
     else:
-        warnings.warn('Convergence not reached')
+        warnings.warn("Convergence not reached")
 
+    C = X.conj().T @ X
     if p > 0:
-        C = np.linalg.inv(X) @ np.linalg.inv(X.T)
-    else:
-        C = X.T @ X
+        C = np.linalg.inv(C)
 
     return C
 
 
 def mean_riemann(covmats, tol=10e-9, maxiter=50, init=None,
                  sample_weight=None):
-    r"""Mean of SPD matrices according to the Riemannian metric.
+    r"""Mean of SPD/HPD matrices according to the Riemannian metric.
 
     The affine-invariant Riemannian mean minimizes the sum of squared
-    affine-invariant Riemannian distances :math:`d_R` to all matrices [1]_:
+    affine-invariant Riemannian distances :math:`d_R` to all SPD/HPD matrices
+    [1]_ [2]_:
 
     .. math::
-         \arg \min_{\mathbf{C}} \sum_i w_i d_R (\mathbf{C}, \mathbf{C}_i)^2
+         \arg \min_{\mathbf{C}} \sum_i w_i \ d_R (\mathbf{C}, \mathbf{X}_i)^2
 
     Parameters
     ----------
-    covmats : ndarray, shape (n_matrices, n_channels, n_channels)
-        Set of SPD matrices.
+    covmats : ndarray, shape (n_matrices, n, n)
+        Set of SPD/HPD matrices.
     tol : float, default=10e-9
         The tolerance to stop the gradient descent.
     maxiter : int, default=50
         The maximum number of iterations.
-    init : None | ndarray, shape (n_channels, n_channels), default=None
-        A SPD matrix used to initialize the gradient descent.
+    init : None | ndarray, shape (n, n), default=None
+        A SPD/HPD matrix used to initialize the gradient descent.
         If None, the weighted Euclidean mean is used.
     sample_weight : None | ndarray, shape (n_matrices,), default=None
         Weights for each matrix. If None, it uses equal weights.
 
     Returns
     -------
-    C : ndarray, shape (n_channels, n_channels)
+    C : ndarray, shape (n, n)
         Affine-invariant Riemannian mean.
 
+    See Also
+    --------
+    mean_covariance
+
     References
     ----------
-    .. [1] `A differential geometric approach to the geometric mean of
+    .. [1] `Principal geodesic analysis for the study of nonlinear statistics
+        of shape
+        <https://ieeexplore.ieee.org/document/1318725>`_
+        P.T. Fletcher, C. Lu, S. M. Pizer, S. Joshi.
+        IEEE Trans Med Imaging, 2004, 23(8), pp. 995-1005
+    .. [2] `A differential geometric approach to the geometric mean of
         symmetric positive-definite matrices
         <https://epubs.siam.org/doi/10.1137/S0895479803436937>`_
-        M. Moakher, SIAM Journal on Matrix Analysis and Applications.
-        Volume 26, Issue 3, 2005
+        M. Moakher. SIAM J Matrix Anal Appl, 2005, 26 (3), pp. 735-747
     """
     n_matrices, _, _ = covmats.shape
     sample_weight = check_weights(sample_weight, n_matrices)
     if init is None:
         C = mean_euclid(covmats, sample_weight=sample_weight)
     else:
         C = init
@@ -463,51 +515,55 @@
             nu = 0.95 * nu
             tau = h
         else:
             nu = 0.5 * nu
         if crit <= tol or nu <= tol:
             break
     else:
-        warnings.warn('Convergence not reached')
+        warnings.warn("Convergence not reached")
 
     return C
 
 
 def mean_wasserstein(covmats, tol=10e-4, maxiter=50, init=None,
                      sample_weight=None):
-    r"""Mean of SPD matrices according to the Wasserstein metric.
+    r"""Mean of SPD/HPD matrices according to the Wasserstein metric.
 
     Wasserstein mean is obtained by an iterative procedure where the update is
     [1]_:
 
     .. math::
-        \mathbf{K} = \left(\sum_i \left( \mathbf{K} \mathbf{C}_i \mathbf{K}
-                     \right)^{1/2} \right)^{1/2}
+        \mathbf{K} = \left( \sum_i w_i \ \left( \mathbf{K} \mathbf{X}_i
+                     \mathbf{K} \right)^{1/2} \right)^{1/2}
 
     with :math:`\mathbf{K} = \mathbf{C}^{1/2}`.
 
     Parameters
     ----------
-    covmats : ndarray, shape (n_matrices, n_channels, n_channels)
-        Set of SPD matrices.
+    covmats : ndarray, shape (n_matrices, n, n)
+        Set of SPD/HPD matrices.
     tol : float, default=10e-4
         The tolerance to stop the gradient descent.
     maxiter : int, default=50
         The maximum number of iterations.
-    init : None | ndarray, shape (n_channels, n_channels), default=None
-        A SPD matrix used to initialize the gradient descent.
+    init : None | ndarray, shape (n, n), default=None
+        A SPD/HPD matrix used to initialize the gradient descent.
         If None the Euclidean mean is used.
     sample_weight : None | ndarray, shape (n_matrices,), default=None
         Weights for each matrix. If None, it uses equal weights.
 
     Returns
     -------
-    C : ndarray, shape (n_channels, n_channels)
+    C : ndarray, shape (n, n)
         Wasserstein mean.
 
+    See Also
+    --------
+    mean_covariance
+
     References
     ----------
     .. [1] `Geometric Radar Processing based on Frechet distance: Information
         geometry versus Optimal Transport Theory
         <https://ieeexplore.ieee.org/document/6042179>`_
         F. Barbaresco. 12th International Radar Symposium (IRS), October 2011
     """
@@ -525,90 +581,103 @@
         Knew = sqrtm(J)
 
         crit = np.linalg.norm(Knew - K, ord='fro')
         K = Knew
         if crit <= tol:
             break
     else:
-        warnings.warn('Convergence not reached')
+        warnings.warn("Convergence not reached")
 
     C = K @ K
     return C
 
 
 ###############################################################################
 
 
-mean_methods = {
+mean_functions = {
     'ale': mean_ale,
     'alm': mean_alm,
     'euclid': mean_euclid,
     'harmonic': mean_harmonic,
     'identity': mean_identity,
     'kullback_sym': mean_kullback_sym,
     'logdet': mean_logdet,
     'logeuclid': mean_logeuclid,
     'riemann': mean_riemann,
     'wasserstein': mean_wasserstein,
 }
 
 
-def _check_mean_method(method):
-    """Check mean methods."""
-    if isinstance(method, str):
-        if method not in mean_methods.keys():
-            raise ValueError('Unknown mean method')
+def _check_mean_function(metric):
+    """Check mean function."""
+    if isinstance(metric, str):
+        if metric not in mean_functions.keys():
+            raise ValueError(f"Unknown mean metric '{metric}'")
         else:
-            method = mean_methods[method]
-    elif not hasattr(method, '__call__'):
-        raise ValueError('Mean method must be a function or a string.')
-    return method
+            metric = mean_functions[metric]
+    elif not hasattr(metric, '__call__'):
+        raise ValueError("Mean metric must be a function or a string "
+                         f"(Got {type(metric)}.")
+    return metric
+
 
+def mean_covariance(covmats, metric='riemann', sample_weight=None, **kwargs):
+    """Mean of matrices according to a metric.
 
-def mean_covariance(covmats, metric='riemann', sample_weight=None, *args):
-    """Mean of SPD matrices according to a metric.
+    Compute the mean of a set of matrices according to a metric [1]_.
 
     Parameters
     ----------
-    covmats : ndarray, shape (n_matrices, n_channels, n_channels)
-        Set of SPD matrices.
+    covmats : ndarray, shape (n_matrices, n, n)
+        Set of matrices.
     metric : string, default='riemann'
         The metric for mean, can be: 'ale', 'alm', 'euclid', 'harmonic',
         'identity', 'kullback_sym', 'logdet', 'logeuclid', 'riemann',
         'wasserstein', or a callable function.
     sample_weight : None | ndarray, shape (n_matrices,), default=None
         Weights for each matrix. If None, it uses equal weights.
-    args : list of params
-        The arguments passed to the sub function.
+    **kwargs : dict
+        The keyword arguments passed to the sub function.
 
     Returns
     -------
-    C : ndarray, shape (n_channels, n_channels)
-        Mean of SPD matrices.
-    """
-    if callable(metric):
-        C = metric(covmats, sample_weight=sample_weight, *args)
-    else:
-        C = mean_methods[metric](covmats, sample_weight=sample_weight, *args)
+    C : ndarray, shape (n, n)
+        Mean of matrices.
+
+    References
+    ----------
+    .. [1] `Review of Riemannian distances and divergences, applied to
+        SSVEP-based BCI
+        <https://hal.archives-ouvertes.fr/LISV/hal-03015762v1>`_
+        S. Chevallier, E. K. Kalunga, Q. Barthélemy, E. Monacelli.
+        Neuroinformatics, Springer, 2021, 19 (1), pp.93-106
+    """
+    mean_function = _check_mean_function(metric)
+    C = mean_function(
+        covmats,
+        sample_weight=sample_weight,
+        **kwargs,
+    )
     return C
 
 
 ###############################################################################
 
 
 def _get_mask_from_nan(covmat):
     nan_col = np.all(np.isnan(covmat), axis=0)
     nan_row = np.all(np.isnan(covmat), axis=1)
     if not np.array_equal(nan_col, nan_row):
-        raise ValueError('NaN values are not symmetric.')
+        raise ValueError("NaN values are not symmetric.")
     nan_inds = np.where(nan_col)
     subcovmat_ = np.delete(covmat, nan_inds, axis=0)
     subcovmat = np.delete(subcovmat_, nan_inds, axis=1)
     if np.any(np.isnan(subcovmat)):
-        raise ValueError('NaN values must fill rows and columns.')
+        raise ValueError("NaN values must fill rows and columns.")
     mask = np.delete(np.eye(covmat.shape[0]), nan_inds, axis=1)
     return mask
 
 
 def _get_masks_from_nan(covmats):
     masks = []
     for i in range(len(covmats)):
@@ -621,69 +690,74 @@
     for i in range(len(covmats)):
         maskedcovmats.append(masks[i].T @ covmats[i] @ masks[i])
     return maskedcovmats
 
 
 def maskedmean_riemann(covmats, masks, tol=10e-9, maxiter=100, init=None,
                        sample_weight=None):
-    """Masked Riemannian mean of SPD matrices.
+    """Masked Riemannian mean of SPD/HPD matrices.
 
     Given masks defined as semi-orthogonal matrices, the masked Riemannian mean
-    of SPD matrices is obtained with a gradient descent minimizing the sum of
-    affine-invariant Riemannian distances between masked SPD matrices and the
-    masked mean [1]_.
+    of SPD/HPD matrices is obtained with a gradient descent minimizing the sum
+    of affine-invariant Riemannian distances between masked SPD/HPD matrices
+    and the masked mean [1]_.
 
     Parameters
     ----------
-    covmats : ndarray, shape (n_matrices, n_channels, n_channels)
-        Set of SPD matrices.
-    masks : list of n_matrices ndarray of shape (n_channels, n_channels_i), \
-            with different n_channels_i, such that n_channels_i <= n_channels
+    covmats : ndarray, shape (n_matrices, n, n)
+        Set of SPD/HPD matrices.
+    masks : list of n_matrices ndarray of shape (n, n_i), \
+            with different n_i, such that n_i <= n
         Masks, defined as semi-orthogonal matrices. See [1]_.
     tol : float, default=10e-9
         The tolerance to stop the gradient descent.
     maxiter : int, default=100
         The maximum number of iteration.
-    init : None | ndarray, shape (n_channels, n_channels), default=None
-        A SPD matrix used to initialize the gradient descent.
+    init : None | ndarray, shape (n, n), default=None
+        A SPD/HPD matrix used to initialize the gradient descent.
         If None, the Identity is used.
     sample_weight : None | ndarray, shape (n_matrices,), default=None
         Weights for each matrix. If None, it uses equal weights.
 
     Returns
     -------
-    C : ndarray, shape (n_channels, n_channels)
+    C : ndarray, shape (n, n)
         Masked Riemannian mean.
 
     Notes
     -----
     .. versionadded:: 0.3
 
+    See Also
+    --------
+    mean_riemann
+    mean_covariance
+
     References
     ----------
     .. [1] `Geodesically-convex optimization for averaging partially observed
         covariance matrices
         <https://hal.archives-ouvertes.fr/hal-02984423>`_
         F. Yger, S. Chevallier, Q. Barthélemy, and S. Sra. Asian Conference on
         Machine Learning (ACML), Nov 2020, Bangkok, Thailand. pp.417 - 432.
     """
-    n_matrices, n_channels, _ = covmats.shape
+    n_matrices, n, _ = covmats.shape
     sample_weight = check_weights(sample_weight, n_matrices)
     maskedcovmats = _apply_masks(covmats, masks)
     if init is None:
-        C = np.eye(n_channels)
+        C = np.eye(n)
     else:
         C = init
 
     nu = 1.0
     tau = np.finfo(np.float64).max
     crit = np.finfo(np.float64).max
     for _ in range(maxiter):
         maskedC = _apply_masks(np.tile(C, (n_matrices, 1, 1)), masks)
-        J = np.zeros((n_channels, n_channels))
+        J = np.zeros((n, n), dtype=covmats.dtype)
         for i in range(n_matrices):
             C12, Cm12 = sqrtm(maskedC[i]), invsqrtm(maskedC[i])
             tmp = C12 @ logm(Cm12 @ maskedcovmats[i] @ Cm12) @ C12
             J += sample_weight[i] * masks[i] @ tmp @ masks[i].T
         C12, Cm12 = sqrtm(C), invsqrtm(C)
         C = C12 @ expm(Cm12 @ (nu * J) @ Cm12) @ C12
 
@@ -693,60 +767,65 @@
             nu = 0.95 * nu
             tau = h
         else:
             nu = 0.5 * nu
         if crit <= tol or nu <= tol:
             break
     else:
-        warnings.warn('Convergence not reached')
+        warnings.warn("Convergence not reached")
 
     return C
 
 
 def nanmean_riemann(covmats, tol=10e-9, maxiter=100, init=None,
                     sample_weight=None):
-    """Riemannian NaN-mean of SPD matrices.
+    """Riemannian NaN-mean of SPD/HPD matrices.
 
-    The Riemannian NaN-mean is the masked Riemannian mean applied to SPD
+    The Riemannian NaN-mean is the masked Riemannian mean applied to SPD/HPD
     matrices potentially corrupted by symmetric NaN values [1]_.
 
     Parameters
     ----------
-    covmats : ndarray, shape (n_matrices, n_channels, n_channels)
-        Set of SPD matrices, corrupted by symmetric NaN values [1]_.
+    covmats : ndarray, shape (n_matrices, n, n)
+        Set of SPD/HPD matrices, corrupted by symmetric NaN values [1]_.
     tol : float, default=10e-9
         The tolerance to stop the gradient descent.
     maxiter : int, default=100
         The maximum number of iteration.
-    init : None | ndarray, shape (n_channels, n_channels), default=None
-        A SPD matrix used to initialize the gradient descent.
+    init : None | ndarray, shape (n, n), default=None
+        A SPD/HPD matrix used to initialize the gradient descent.
         If None, a regularized Euclidean NaN-mean is used.
     sample_weight : None | ndarray, shape (n_matrices,), default=None
         Weights for each matrix. If None, it uses equal weights.
 
     Returns
     -------
-    C : ndarray, shape (n_channels, n_channels)
+    C : ndarray, shape (n, n)
         Riemannian NaN-mean.
 
     Notes
     -----
     .. versionadded:: 0.3
 
+    See Also
+    --------
+    maskedmean_riemann
+    mean_covariance
+
     References
     ----------
     .. [1] `Geodesically-convex optimization for averaging partially observed
         covariance matrices
         <https://hal.archives-ouvertes.fr/hal-02984423>`_
         F. Yger, S. Chevallier, Q. Barthélemy, and S. Sra. Asian Conference on
         Machine Learning (ACML), Nov 2020, Bangkok, Thailand. pp.417 - 432.
     """
-    n_matrices, n_channels, _ = covmats.shape
+    n_matrices, n, _ = covmats.shape
     if init is None:
-        Cinit = np.nanmean(covmats, axis=0) + 1e-6 * np.eye(n_channels)
+        Cinit = np.nanmean(covmats, axis=0) + 1e-6 * np.eye(n)
     else:
         Cinit = init
 
     C = maskedmean_riemann(
         np.nan_to_num(covmats),  # avoid nan contamination in matmul
         _get_masks_from_nan(covmats),
         tol=tol,
```

### Comparing `pyriemann-0.4/pyriemann/utils/median.py` & `pyriemann-0.5/pyriemann/utils/median.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,51 +1,52 @@
-"""Medians of SPD matrices."""
+"""Medians of SPD/HPD matrices."""
 
 import warnings
 import numpy as np
 
 from .base import sqrtm, invsqrtm, logm, expm
-from .distance import pairwise_distance
+from .distance import distance
 from .mean import mean_euclid
 from .utils import check_weights
 
 
 def median_euclid(X, *, tol=10e-6, maxiter=50, init=None, weights=None):
     r"""Euclidean geometric median of matrices.
 
     The Euclidean geometric median minimizes the sum of Euclidean distances
     :math:`d_E` to all matrices [1]_ [2]_:
 
     .. math::
-        \arg \min_{\mathbf{M}} \sum_i w_i d_E (\mathbf{M}, \mathbf{X}_i)
+        \arg \min_{\mathbf{M}} \sum_i w_i \ d_E (\mathbf{M}, \mathbf{X}_i)
 
-    It is different from the marginal median provided by NumPy [3]_.
+    Geometric median is different from the marginal median provided by NumPy
+    [3]_.
 
     Parameters
     ----------
-    X : ndarray, shape (n_matrices, n_channels, n_channels)
+    X : ndarray, shape (n_matrices, n, m)
         Set of matrices.
     tol : float, default=10e-6
         The tolerance to stop the iterative algorithm.
     maxiter : int, default=50
         The maximum number of iterations.
-    init : None | ndarray, shape (n_channels, n_channels), default=None
+    init : None | ndarray, shape (n, m), default=None
         A matrix used to initialize the iterative algorithm.
         If None, the weighted Euclidean mean is used.
     weights : None | ndarray, shape (n_matrices,), default=None
         Weights for each matrix. If None, it uses equal weights.
 
     Returns
     -------
-    M : ndarray, shape (n_channels, n_channels)
+    M : ndarray, shape (n, m)
         Euclidean geometric median.
 
     Notes
     -----
-    .. versionadded:: 0.3.1
+    .. versionadded:: 0.4
 
     References
     ----------
     .. [1] `Sur le point pour lequel la somme des distances de n points donnés
         est minimum
         <https://www.jstage.jst.go.jp/article/tmj1911/43/0/43_0_355/_pdf>`_
         E Weiszfeld. Tohoku Mathematical Journal, 1937, 43, pp. 355-386.
@@ -59,19 +60,15 @@
     weights = check_weights(weights, n_matrices)
     if init is None:
         M = mean_euclid(X, sample_weight=weights)
     else:
         M = init
 
     for _ in range(maxiter):
-        dists = pairwise_distance(
-            X,
-            M[np.newaxis, ...],
-            metric='euclid'
-        )[:, 0]
+        dists = distance(X, M, metric='euclid')[:, 0]
         is_zero = (dists == 0)
 
         w = weights[~is_zero] / dists[~is_zero]
         Mnew = mean_euclid(X[~is_zero], sample_weight=w)  # Eq(2.4) of [2]
 
         n_zeros = np.sum(is_zero)
         if n_zeros > 0:
@@ -81,53 +78,54 @@
             Mnew = max(0, 1 - rinv) * Mnew + min(1, rinv) * M  # Eq(2.6)
 
         crit = np.linalg.norm(Mnew - M, ord='fro')
         M = Mnew
         if crit <= tol:
             break
     else:
-        warnings.warn('Convergence not reached')
+        warnings.warn("Convergence not reached")
 
     return M
 
 
 def median_riemann(X, *, tol=10e-6, maxiter=50, init=None, weights=None,
                    step_size=1):
-    r"""Affine-invariant Riemannian geometric median of SPD matrices.
+    r"""Affine-invariant Riemannian geometric median of SPD/HPD matrices.
 
     The affine-invariant Riemannian geometric median minimizes the sum of
-    affine-invariant Riemannian distances :math:`d_R` to all SPD matrices [1]_:
+    affine-invariant Riemannian distances :math:`d_R` to all SPD/HPD matrices
+    [1]_:
 
     .. math::
-        \arg \min_{\mathbf{M}} \sum_i w_i d_R (\mathbf{M}, \mathbf{X}_i)
+        \arg \min_{\mathbf{M}} \sum_i w_i \ d_R (\mathbf{M}, \mathbf{X}_i)
 
     Parameters
     ----------
-    X : ndarray, shape (n_matrices, n_channels, n_channels)
-        Set of SPD matrices.
+    X : ndarray, shape (n_matrices, n, n)
+        Set of SPD/HPD matrices.
     tol : float, default=10e-6
         The tolerance to stop the gradient descent.
     maxiter : int, default=50
         The maximum number of iterations.
-    init : None | ndarray, shape (n_channels, n_channels), default=None
-        A SPD matrix used to initialize the gradient descent.
+    init : None | ndarray, shape (n, n), default=None
+        A SPD/HPD matrix used to initialize the gradient descent.
         If None, the weighted Euclidean mean is used.
     weights : None | ndarray, shape (n_matrices,), default=None
         Weights for each matrix. If None, it uses equal weights.
     step_size : float, default=1.0
         The step size of the gradient descent, in (0,2].
 
     Returns
     -------
-    M : ndarray, shape (n_channels, n_channels)
+    M : ndarray, shape (n, n)
         Affine-invariant Riemannian geometric median.
 
     Notes
     -----
-    .. versionadded:: 0.3.1
+    .. versionadded:: 0.4
 
     References
     ----------
     .. [1] `The geometric median on Riemannian manifolds with application to
         robust atlas estimation
         <https://www.ncbi.nlm.nih.gov/pmc/articles/PMC2735114/>`_
         PT. Fletcher, S. Venkatasubramanian S and S. Joshi.
@@ -136,37 +134,33 @@
         detection
         <https://ieeexplore.ieee.org/abstract/document/5615027>`_
         L Yang, M Arnaudon and F Barbaresco. 7th European Radar Conference,
         2010, pp. 415-418
     """
     if not 0 < step_size <= 2:
         raise ValueError(
-            'Value step_size must be included in (0, 2] (Got %d)' % step_size)
+            f"Value step_size must be included in (0, 2] (Got {step_size})")
     n_matrices, _, _ = X.shape
     weights = check_weights(weights, n_matrices)
     if init is None:
         M = mean_euclid(X, sample_weight=weights)
     else:
         M = init
 
     for _ in range(maxiter):
-        dists = pairwise_distance(
-            X,
-            M[np.newaxis, ...],
-            metric='riemann'
-        )[:, 0]
+        dists = distance(X, M, metric='riemann')[:, 0]
         is_zero = (dists == 0)
         w = weights[~is_zero] / dists[~is_zero]
 
         # Eq(11) of [1]
         M12, Mm12 = sqrtm(M), invsqrtm(M)
         tangvecs = logm(Mm12 @ X[~is_zero] @ Mm12)
         J = np.einsum('a,abc->bc', w / np.sum(w), tangvecs)
         M = M12 @ expm(step_size * J) @ M12
 
         crit = np.linalg.norm(J, ord='fro')
         if crit <= tol:
             break
     else:
-        warnings.warn('Convergence not reached')
+        warnings.warn("Convergence not reached")
 
     return M
```

### Comparing `pyriemann-0.4/pyriemann/utils/test.py` & `pyriemann-0.5/pyriemann/utils/test.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import numpy as np
 
 
 def _get_eigenvals(X):
-    """ Private function to compute eigen values. """
+    """Private function to compute all eigen values."""
     n = X.shape[-1]
     return np.linalg.eigvals(X.reshape((-1, n, n)))
 
 
 def is_square(X):
-    """ Check if matrices are square.
+    """Check if matrices are square.
 
     Parameters
     ----------
     X : ndarray, shape (..., n, n)
         The set of square matrices, at least 2D ndarray.
 
     Returns
@@ -20,15 +20,15 @@
     ret : boolean
         True if matrices are square.
     """
     return X.ndim >= 2 and X.shape[-2] == X.shape[-1]
 
 
 def is_sym(X):
-    """ Check if all matrices are symmetric.
+    """Check if all matrices are symmetric.
 
     Parameters
     ----------
     X : ndarray, shape (..., n, n)
         The set of square matrices, at least 2D ndarray.
 
     Returns
@@ -52,27 +52,27 @@
     ret : boolean
         True if all matrices are skew-symmetric.
     """
     return is_square(X) and np.allclose(X, -np.swapaxes(X, -2, -1))
 
 
 def is_real(X):
-    """Check if all complex matrices are strictly real.
+    """Check if all matrices are strictly real.
 
     Better management of numerical imprecisions than np.all(np.isreal()).
 
     Parameters
     ----------
-    X : ndarray
+    X : ndarray, shape (..., n, m)
         The set of matrices.
 
     Returns
     -------
     ret : boolean
-        True if all complex matrices are strictly real.
+        True if all matrices are strictly real.
     """
     return np.allclose(X.imag, np.zeros_like(X.imag))
 
 
 def is_hermitian(X):
     """Check if all matrices are Hermitian.
 
@@ -88,99 +88,120 @@
     -------
     ret : boolean
         True if all matrices are Hermitian.
     """
     return is_sym(X.real) and is_skew_sym(X.imag)
 
 
-def is_pos_def(X, fast_mode=False):
-    """ Check if all matrices are positive definite.
+def is_pos_def(X, tol=0.0, fast_mode=False):
+    """Check if all matrices are positive definite (PD).
 
     Check if all matrices are positive definite, fast verification is done
     with Cholesky decomposition, while full check compute all eigenvalues
     to verify that they are positive.
 
     Parameters
     ----------
     X : ndarray, shape (..., n, n)
         The set of square matrices, at least 2D ndarray.
+    tol : float, default 0.0
+        Threshold below which eigen values are considered zero.
     fast_mode : boolean, default=False
         Use Cholesky decomposition to avoid computing all eigenvalues.
 
-
     Returns
     -------
     ret : boolean
         True if all matrices are positive definite.
     """
     if fast_mode:
         try:
             np.linalg.cholesky(X)
             return True
         except np.linalg.LinAlgError:
             return False
     else:
-        return is_square(X) and np.all(_get_eigenvals(X) > 0.0)
+        return is_square(X) and np.all(_get_eigenvals(X) > tol)
 
 
 def is_pos_semi_def(X):
-    """ Check if all matrices are positive semi-definite.
+    """Check if all matrices are positive semi-definite (PSD).
 
     Parameters
     ----------
     X : ndarray, shape (..., n, n)
         The set of square matrices, at least 2D ndarray.
 
     Returns
     -------
     ret : boolean
         True if all matrices are positive semi-definite.
     """
     return is_square(X) and np.all(_get_eigenvals(X) >= 0.0)
 
 
-def is_sym_pos_def(X):
-    """ Check if all matrices are symmetric positive-definite.
+def is_sym_pos_def(X, tol=0.0):
+    """Check if all matrices are symmetric positive-definite (SPD).
 
     Parameters
     ----------
     X : ndarray, shape (..., n, n)
         The set of square matrices, at least 2D ndarray.
+    tol : float, default 0.0
+        Threshold below which eigen values are considered zero.
 
     Returns
     -------
     ret : boolean
         True if all matrices are symmetric positive-definite.
     """
-    return is_sym(X) and is_pos_def(X)
+    return is_sym(X) and is_pos_def(X, tol=tol)
 
 
 def is_sym_pos_semi_def(X):
-    """ Check if all matrices are symmetric positive semi-definite.
+    """Check if all matrices are symmetric positive semi-definite (SPSD).
 
     Parameters
     ----------
     X : ndarray, shape (..., n, n)
         The set of square matrices, at least 2D ndarray.
 
     Returns
     -------
     ret : boolean
         True if all matrices are symmetric positive semi-definite.
     """
     return is_sym(X) and is_pos_semi_def(X)
 
 
-def is_herm_pos_def(X):
-    """ Check if all matrices are Hermitian positive-definite.
+def is_herm_pos_def(X, tol=0.0):
+    """Check if all matrices are Hermitian positive-definite (HPD).
 
     Parameters
     ----------
     X : ndarray, shape (..., n, n)
         The set of square matrices, at least 2D ndarray.
+    tol : float, default 0.0
+        Threshold below which eigen values are considered zero.
 
     Returns
     -------
     ret : boolean
         True if all matrices are Hermitian positive-definite.
     """
-    return is_hermitian(X) and is_pos_def(X)
+    return is_hermitian(X) and is_pos_def(X, tol=tol)
+
+
+def is_herm_pos_semi_def(X):
+    """Check if all matrices are Hermitian positive semi-definite (HPSD).
+
+    Parameters
+    ----------
+    X : ndarray, shape (..., n, n)
+        The set of square matrices, at least 2D ndarray.
+
+    Returns
+    -------
+    ret : boolean
+        True if all matrices are Hermitian positive semi-definite.
+    """
+    return is_hermitian(X) and is_pos_semi_def(X)
```

### Comparing `pyriemann-0.4/pyriemann/utils/utils.py` & `pyriemann-0.5/pyriemann/utils/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     if weights is None:
         weights = np.ones(n_weights)
 
     else:
         weights = np.asarray(weights)
         if weights.shape != (n_weights,):
             raise ValueError(
-                'Weights do not have the good shape. Should be (%d,) but got '
-                '%s.' % (n_weights, weights.shape,)
+                "Weights do not have the good shape. Should be (%d,) but got "
+                "%s." % (n_weights, weights.shape,)
             )
         if check_positivity and any(weights <= 0):
             raise ValueError("Weights must be strictly positive.")
 
     weights /= np.sum(weights)
     return weights
```

### Comparing `pyriemann-0.4/pyriemann/utils/viz.py` & `pyriemann-0.5/pyriemann/utils/viz.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,10 @@
 """Helpers for vizualization."""
-import pandas as pd
 import numpy as np
-from sklearn.metrics import confusion_matrix
 from ..embedding import SpectralEmbedding, LocallyLinearEmbedding
-from . import deprecated
-
-
-@deprecated(
-    "plot_confusion_matrix is deprecated and will be remove in 0.4.0; "
-    "please use sklearn confusion_matrix and ConfusionMatrixDisplay; "
-    "see examples/ERP/plot_classify_EEG_tangentspace.py"
-)
-def plot_confusion_matrix(
-    targets, predictions, target_names, title="Confusion matrix", cmap="Blues"
-):
-    """Plot Confusion Matrix."""
-    try:
-        import seaborn as sns
-    except ImportError:
-        raise ImportError("Install seaborn to plot confusion matrix")
-
-    cm = confusion_matrix(targets, predictions)
-    cm = 100 * cm.astype("float") / cm.sum(axis=1)[:, np.newaxis]
-
-    df = pd.DataFrame(data=cm, columns=target_names, index=target_names)
-    g = sns.heatmap(
-        df, annot=True, fmt=".1f", linewidths=0.5, vmin=0, vmax=100, cmap=cmap
-    )
-    g.set_title(title)
-    g.set_ylabel("True label")
-    g.set_xlabel("Predicted label")
-    return g
 
 
 def plot_embedding(X,
                    y=None,
                    *,
                    metric="riemann",
                    title="Embedding of covariances",
```

### Comparing `pyriemann-0.4/pyriemann.egg-info/PKG-INFO` & `pyriemann-0.5/pyriemann.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyriemann
-Version: 0.4
+Version: 0.5
 Summary: Biosignals classification with Riemannian geometry
 Home-page: https://pyriemann.readthedocs.io
 Author: Alexandre Barachant
 Author-email: alexandre.barachant@gmail.com
 License: BSD (3-clause)
 Project-URL: Documentation, https://pyriemann.readthedocs.io
 Project-URL: Source, https://github.com/pyRiemann/pyRiemann
@@ -52,29 +52,35 @@
 ```
 or using pip+git for the latest version of the code :
 
 ```
 pip install git+https://github.com/pyRiemann/pyRiemann
 ```
 
-Anaconda is not currently supported, if you want to use anaconda, you need to create a virtual environment in anaconda,
-activate it and use the above command to install it.
+#### Using conda
+
+The package is distributed via [conda-forge](https://conda-forge.org).
+You could install it in your working environment, with the following command:
+
+```shell
+conda install -c conda-forge pyriemann
+```
 
 #### From sources
 
-For the latest version, you can install the package from the sources using the setup.py script
+For the latest version, you can install the package from the sources using ``pip``:
 
-```
-python setup.py install
+```shell
+pip install .
 ```
 
-or in developer mode to be able to modify the sources.
+or in editable mode to be able to modify the sources:
 
-```
-python setup.py develop
+```shell
+pip install -e .
 ```
 
 ## How to use it
 
 Most of the functions mimic the scikit-learn API, and therefore can be directly used with sklearn.
 For example, for cross-validation classification of EEG signal using the MDM algorithm described in [[2]](#2), it is easy as:
```

### Comparing `pyriemann-0.4/pyriemann.egg-info/SOURCES.txt` & `pyriemann-0.5/pyriemann.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -37,8 +37,33 @@
 pyriemann/utils/geodesic.py
 pyriemann/utils/kernel.py
 pyriemann/utils/mean.py
 pyriemann/utils/median.py
 pyriemann/utils/tangentspace.py
 pyriemann/utils/test.py
 pyriemann/utils/utils.py
-pyriemann/utils/viz.py
+pyriemann/utils/viz.py
+tests/test_channelselection.py
+tests/test_classification.py
+tests/test_clustering.py
+tests/test_embedding.py
+tests/test_estimation.py
+tests/test_preprocessing.py
+tests/test_regression.py
+tests/test_sampling.py
+tests/test_simulated.py
+tests/test_spatialfilters.py
+tests/test_stats.py
+tests/test_tangentspace.py
+tests/test_transfer.py
+tests/test_utils_ajd.py
+tests/test_utils_base.py
+tests/test_utils_covariance.py
+tests/test_utils_distance.py
+tests/test_utils_geodesic.py
+tests/test_utils_kernel.py
+tests/test_utils_mean.py
+tests/test_utils_median.py
+tests/test_utils_tangent_space.py
+tests/test_utils_test.py
+tests/test_utils_utils.py
+tests/test_utils_viz.py
```

### Comparing `pyriemann-0.4/setup.py` & `pyriemann-0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,21 +38,21 @@
     platforms="any",
     python_requires=">=3.7",
     install_requires=[
         "numpy!=1.24.0",
         "scipy",
         "scikit-learn",
         "joblib",
-        "pandas"
     ],
     extras_require={
         "docs": [
             "sphinx-gallery",
             "sphinx-bootstrap_theme",
             "numpydoc",
             "mne",
             "seaborn",
+            "pandas",
         ],
         "tests": ["pytest", "seaborn", "flake8"],
     },
     zip_safe=False,
 )
```

