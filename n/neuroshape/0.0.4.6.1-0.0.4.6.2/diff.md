# Comparing `tmp/neuroshape-0.0.4.6.1.tar.gz` & `tmp/neuroshape-0.0.4.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuroshape-0.0.4.6.1.tar", last modified: Tue Jun 20 06:22:11 2023, max compression
+gzip compressed data, was "neuroshape-0.0.4.6.2.tar", last modified: Tue Jun 20 06:23:25 2023, max compression
```

## Comparing `neuroshape-0.0.4.6.1.tar` & `neuroshape-0.0.4.6.2.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-20 06:22:11.496789 neuroshape-0.0.4.6.1/
--rw-r--r--   0 nik        (502) admin       (80)     1501 2023-06-07 02:08:37.000000 neuroshape-0.0.4.6.1/LICENSE
--rw-r--r--   0 nik        (502) admin       (80)      470 2023-06-20 06:22:11.495020 neuroshape-0.0.4.6.1/PKG-INFO
--rw-r--r--   0 nik        (502) admin       (80)     4445 2023-06-08 03:48:59.000000 neuroshape-0.0.4.6.1/README.rst
-drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-20 06:22:11.470775 neuroshape-0.0.4.6.1/neuroshape/
--rw-r--r--   0 nik        (502) admin       (80)        0 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.1/neuroshape/__init__.py
--rw-r--r--   0 nik        (502) admin       (80)    22407 2023-06-15 03:59:02.000000 neuroshape-0.0.4.6.1/neuroshape/connectopic_laplacian.py
--rw-r--r--   0 nik        (502) admin       (80)    22913 2023-06-18 23:49:14.000000 neuroshape-0.0.4.6.1/neuroshape/eigenmodes.py
-drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-20 06:22:11.478399 neuroshape-0.0.4.6.1/neuroshape/nulls/
--rw-r--r--   0 nik        (502) admin       (80)       44 2023-06-08 03:48:59.000000 neuroshape-0.0.4.6.1/neuroshape/nulls/__init__.py
--rw-r--r--   0 nik        (502) admin       (80)     5351 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.1/neuroshape/nulls/burt.py
--rw-r--r--   0 nik        (502) admin       (80)    20808 2023-06-13 01:26:03.000000 neuroshape-0.0.4.6.1/neuroshape/nulls/eigenshuff.py
--rw-r--r--   0 nik        (502) admin       (80)    11987 2023-06-20 06:06:13.000000 neuroshape-0.0.4.6.1/neuroshape/nulls/eigensphere.py
--rw-r--r--   0 nik        (502) admin       (80)    25239 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.1/neuroshape/nulls/nulls.py
--rw-r--r--   0 nik        (502) admin       (80)    27669 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.1/neuroshape/nulls/spins.py
-drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-20 06:22:11.481608 neuroshape-0.0.4.6.1/neuroshape/nulls/tests/
--rw-r--r--   0 nik        (502) admin       (80)        0 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.1/neuroshape/nulls/tests/__init__.py
--rw-r--r--   0 nik        (502) admin       (80)     5042 2023-06-19 01:29:34.000000 neuroshape-0.0.4.6.1/neuroshape/nulls/tests/eigenmode_replication.py
--rw-r--r--   0 nik        (502) admin       (80)      530 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.1/neuroshape/nulls/tests/test_burt.py
--rw-r--r--   0 nik        (502) admin       (80)     4137 2023-06-17 23:29:12.000000 neuroshape-0.0.4.6.1/neuroshape/nulls/tests/test_eigenresamp.py
--rw-r--r--   0 nik        (502) admin       (80)      695 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.1/neuroshape/nulls/tests/test_nulls.py
--rw-r--r--   0 nik        (502) admin       (80)      814 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.1/neuroshape/nulls/tests/test_spins.py
--rw-r--r--   0 nik        (502) admin       (80)    12845 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.1/neuroshape/nulls/waveshuff.py
--rw-r--r--   0 nik        (502) admin       (80)     4078 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.1/neuroshape/permutation.py
--rw-r--r--   0 nik        (502) admin       (80)    13180 2023-06-18 23:49:14.000000 neuroshape-0.0.4.6.1/neuroshape/recon.py
--rw-r--r--   0 nik        (502) admin       (80)     5400 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.1/neuroshape/stats.py
-drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-20 06:22:11.492250 neuroshape-0.0.4.6.1/neuroshape/utils/
--rw-r--r--   0 nik        (502) admin       (80)       25 2023-06-07 00:31:38.000000 neuroshape-0.0.4.6.1/neuroshape/utils/__init__.py
--rw-r--r--   0 nik        (502) admin       (80)     1345 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.1/neuroshape/utils/check_fs_subjid.py
--rw-r--r--   0 nik        (502) admin       (80)      616 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.1/neuroshape/utils/check_map.py
--rw-r--r--   0 nik        (502) admin       (80)     6553 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.1/neuroshape/utils/checks.py
--rw-r--r--   0 nik        (502) admin       (80)      917 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.1/neuroshape/utils/compare_parallel.py
--rw-r--r--   0 nik        (502) admin       (80)     3501 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.1/neuroshape/utils/compute_geodesic_distance.py
--rw-r--r--   0 nik        (502) admin       (80)     6248 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.1/neuroshape/utils/concavehull.py
--rw-r--r--   0 nik        (502) admin       (80)    11844 2023-06-20 04:35:08.000000 neuroshape-0.0.4.6.1/neuroshape/utils/eigen.py
--rw-r--r--   0 nik        (502) admin       (80)      763 2023-06-13 01:26:03.000000 neuroshape-0.0.4.6.1/neuroshape/utils/fetch_atlas.py
--rw-r--r--   0 nik        (502) admin       (80)    25397 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.1/neuroshape/utils/fs_shapeDNA.py
--rw-r--r--   0 nik        (502) admin       (80)    31133 2023-06-18 23:49:14.000000 neuroshape-0.0.4.6.1/neuroshape/utils/geometry.py
--rw-r--r--   0 nik        (502) admin       (80)      348 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.1/neuroshape/utils/load_mesh_vertices.py
--rw-r--r--   0 nik        (502) admin       (80)     2639 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.1/neuroshape/utils/meshtransforms.py
--rw-r--r--   0 nik        (502) admin       (80)      222 2023-06-13 01:26:03.000000 neuroshape-0.0.4.6.1/neuroshape/utils/normalize_data.py
--rw-r--r--   0 nik        (502) admin       (80)      201 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.1/neuroshape/utils/swap_single_row.py
--rw-r--r--   0 nik        (502) admin       (80)      540 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.1/neuroshape/utils/tmpname.py
--rw-r--r--   0 nik        (502) admin       (80)      193 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.1/neuroshape/utils/zscore_avg_method.py
-drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-20 06:22:11.473639 neuroshape-0.0.4.6.1/neuroshape.egg-info/
--rw-r--r--   0 nik        (502) admin       (80)      470 2023-06-20 06:22:11.000000 neuroshape-0.0.4.6.1/neuroshape.egg-info/PKG-INFO
--rw-r--r--   0 nik        (502) admin       (80)     1383 2023-06-20 06:22:11.000000 neuroshape-0.0.4.6.1/neuroshape.egg-info/SOURCES.txt
--rw-r--r--   0 nik        (502) admin       (80)        1 2023-06-20 06:22:11.000000 neuroshape-0.0.4.6.1/neuroshape.egg-info/dependency_links.txt
--rw-r--r--   0 nik        (502) admin       (80)       11 2023-06-20 06:22:11.000000 neuroshape-0.0.4.6.1/neuroshape.egg-info/top_level.txt
--rw-r--r--   0 nik        (502) admin       (80)      828 2023-06-20 06:21:38.000000 neuroshape-0.0.4.6.1/pyproject.toml
--rw-r--r--   0 nik        (502) admin       (80)       38 2023-06-20 06:22:11.497341 neuroshape-0.0.4.6.1/setup.cfg
--rw-r--r--   0 nik        (502) admin       (80)     1048 2023-06-20 06:22:07.000000 neuroshape-0.0.4.6.1/setup.py
-drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-20 06:22:11.493909 neuroshape-0.0.4.6.1/src/
--rw-r--r--   0 nik        (502) admin       (80)     5389 2023-06-09 06:16:05.000000 neuroshape-0.0.4.6.1/src/eta_squared.c
--rw-r--r--   0 nik        (502) admin       (80)     2545 2023-06-06 05:49:54.000000 neuroshape-0.0.4.6.1/src/euler_threshold.c
--rw-r--r--   0 nik        (502) admin       (80)     5946 2023-06-06 05:46:53.000000 neuroshape-0.0.4.6.1/src/glmfit.c
+drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-20 06:23:25.400699 neuroshape-0.0.4.6.2/
+-rw-r--r--   0 nik        (502) admin       (80)     1501 2023-06-07 02:08:37.000000 neuroshape-0.0.4.6.2/LICENSE
+-rw-r--r--   0 nik        (502) admin       (80)      470 2023-06-20 06:23:25.399880 neuroshape-0.0.4.6.2/PKG-INFO
+-rw-r--r--   0 nik        (502) admin       (80)     4445 2023-06-08 03:48:59.000000 neuroshape-0.0.4.6.2/README.rst
+drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-20 06:23:25.352449 neuroshape-0.0.4.6.2/neuroshape/
+-rw-r--r--   0 nik        (502) admin       (80)        0 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.2/neuroshape/__init__.py
+-rw-r--r--   0 nik        (502) admin       (80)    22407 2023-06-15 03:59:02.000000 neuroshape-0.0.4.6.2/neuroshape/connectopic_laplacian.py
+-rw-r--r--   0 nik        (502) admin       (80)    22913 2023-06-18 23:49:14.000000 neuroshape-0.0.4.6.2/neuroshape/eigenmodes.py
+drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-20 06:23:25.366507 neuroshape-0.0.4.6.2/neuroshape/nulls/
+-rw-r--r--   0 nik        (502) admin       (80)       44 2023-06-08 03:48:59.000000 neuroshape-0.0.4.6.2/neuroshape/nulls/__init__.py
+-rw-r--r--   0 nik        (502) admin       (80)     5351 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.2/neuroshape/nulls/burt.py
+-rw-r--r--   0 nik        (502) admin       (80)    20808 2023-06-13 01:26:03.000000 neuroshape-0.0.4.6.2/neuroshape/nulls/eigenshuff.py
+-rw-r--r--   0 nik        (502) admin       (80)    11987 2023-06-20 06:06:13.000000 neuroshape-0.0.4.6.2/neuroshape/nulls/eigensphere.py
+-rw-r--r--   0 nik        (502) admin       (80)    25239 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.2/neuroshape/nulls/nulls.py
+-rw-r--r--   0 nik        (502) admin       (80)    27669 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.2/neuroshape/nulls/spins.py
+drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-20 06:23:25.375340 neuroshape-0.0.4.6.2/neuroshape/nulls/tests/
+-rw-r--r--   0 nik        (502) admin       (80)        0 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.2/neuroshape/nulls/tests/__init__.py
+-rw-r--r--   0 nik        (502) admin       (80)     5042 2023-06-19 01:29:34.000000 neuroshape-0.0.4.6.2/neuroshape/nulls/tests/eigenmode_replication.py
+-rw-r--r--   0 nik        (502) admin       (80)      530 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.2/neuroshape/nulls/tests/test_burt.py
+-rw-r--r--   0 nik        (502) admin       (80)     4137 2023-06-17 23:29:12.000000 neuroshape-0.0.4.6.2/neuroshape/nulls/tests/test_eigenresamp.py
+-rw-r--r--   0 nik        (502) admin       (80)      695 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.2/neuroshape/nulls/tests/test_nulls.py
+-rw-r--r--   0 nik        (502) admin       (80)      814 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.2/neuroshape/nulls/tests/test_spins.py
+-rw-r--r--   0 nik        (502) admin       (80)    12845 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.2/neuroshape/nulls/waveshuff.py
+-rw-r--r--   0 nik        (502) admin       (80)     4078 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.2/neuroshape/permutation.py
+-rw-r--r--   0 nik        (502) admin       (80)    13180 2023-06-18 23:49:14.000000 neuroshape-0.0.4.6.2/neuroshape/recon.py
+-rw-r--r--   0 nik        (502) admin       (80)     5400 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.2/neuroshape/stats.py
+drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-20 06:23:25.396773 neuroshape-0.0.4.6.2/neuroshape/utils/
+-rw-r--r--   0 nik        (502) admin       (80)       25 2023-06-07 00:31:38.000000 neuroshape-0.0.4.6.2/neuroshape/utils/__init__.py
+-rw-r--r--   0 nik        (502) admin       (80)     1345 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.2/neuroshape/utils/check_fs_subjid.py
+-rw-r--r--   0 nik        (502) admin       (80)      616 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.2/neuroshape/utils/check_map.py
+-rw-r--r--   0 nik        (502) admin       (80)     6553 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.2/neuroshape/utils/checks.py
+-rw-r--r--   0 nik        (502) admin       (80)      917 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.2/neuroshape/utils/compare_parallel.py
+-rw-r--r--   0 nik        (502) admin       (80)     3501 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.2/neuroshape/utils/compute_geodesic_distance.py
+-rw-r--r--   0 nik        (502) admin       (80)     6248 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.2/neuroshape/utils/concavehull.py
+-rw-r--r--   0 nik        (502) admin       (80)    11844 2023-06-20 04:35:08.000000 neuroshape-0.0.4.6.2/neuroshape/utils/eigen.py
+-rw-r--r--   0 nik        (502) admin       (80)      763 2023-06-13 01:26:03.000000 neuroshape-0.0.4.6.2/neuroshape/utils/fetch_atlas.py
+-rw-r--r--   0 nik        (502) admin       (80)    25397 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.2/neuroshape/utils/fs_shapeDNA.py
+-rw-r--r--   0 nik        (502) admin       (80)    31133 2023-06-18 23:49:14.000000 neuroshape-0.0.4.6.2/neuroshape/utils/geometry.py
+-rw-r--r--   0 nik        (502) admin       (80)      348 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.2/neuroshape/utils/load_mesh_vertices.py
+-rw-r--r--   0 nik        (502) admin       (80)     2639 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.2/neuroshape/utils/meshtransforms.py
+-rw-r--r--   0 nik        (502) admin       (80)      222 2023-06-13 01:26:03.000000 neuroshape-0.0.4.6.2/neuroshape/utils/normalize_data.py
+-rw-r--r--   0 nik        (502) admin       (80)      201 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.2/neuroshape/utils/swap_single_row.py
+-rw-r--r--   0 nik        (502) admin       (80)      540 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.2/neuroshape/utils/tmpname.py
+-rw-r--r--   0 nik        (502) admin       (80)      193 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.2/neuroshape/utils/zscore_avg_method.py
+drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-20 06:23:25.355097 neuroshape-0.0.4.6.2/neuroshape.egg-info/
+-rw-r--r--   0 nik        (502) admin       (80)      470 2023-06-20 06:23:25.000000 neuroshape-0.0.4.6.2/neuroshape.egg-info/PKG-INFO
+-rw-r--r--   0 nik        (502) admin       (80)     1383 2023-06-20 06:23:25.000000 neuroshape-0.0.4.6.2/neuroshape.egg-info/SOURCES.txt
+-rw-r--r--   0 nik        (502) admin       (80)        1 2023-06-20 06:23:25.000000 neuroshape-0.0.4.6.2/neuroshape.egg-info/dependency_links.txt
+-rw-r--r--   0 nik        (502) admin       (80)       11 2023-06-20 06:23:25.000000 neuroshape-0.0.4.6.2/neuroshape.egg-info/top_level.txt
+-rw-r--r--   0 nik        (502) admin       (80)      822 2023-06-20 06:23:16.000000 neuroshape-0.0.4.6.2/pyproject.toml
+-rw-r--r--   0 nik        (502) admin       (80)       38 2023-06-20 06:23:25.400980 neuroshape-0.0.4.6.2/setup.cfg
+-rw-r--r--   0 nik        (502) admin       (80)     1048 2023-06-20 06:23:19.000000 neuroshape-0.0.4.6.2/setup.py
+drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-20 06:23:25.398989 neuroshape-0.0.4.6.2/src/
+-rw-r--r--   0 nik        (502) admin       (80)     5389 2023-06-09 06:16:05.000000 neuroshape-0.0.4.6.2/src/eta_squared.c
+-rw-r--r--   0 nik        (502) admin       (80)     2545 2023-06-06 05:49:54.000000 neuroshape-0.0.4.6.2/src/euler_threshold.c
+-rw-r--r--   0 nik        (502) admin       (80)     5946 2023-06-06 05:46:53.000000 neuroshape-0.0.4.6.2/src/glmfit.c
```

### Comparing `neuroshape-0.0.4.6.1/LICENSE` & `neuroshape-0.0.4.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.1/README.rst` & `neuroshape-0.0.4.6.2/README.rst`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.1/neuroshape/connectopic_laplacian.py` & `neuroshape-0.0.4.6.2/neuroshape/connectopic_laplacian.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.1/neuroshape/eigenmodes.py` & `neuroshape-0.0.4.6.2/neuroshape/eigenmodes.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.1/neuroshape/nulls/burt.py` & `neuroshape-0.0.4.6.2/neuroshape/nulls/burt.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.1/neuroshape/nulls/eigenshuff.py` & `neuroshape-0.0.4.6.2/neuroshape/nulls/eigenshuff.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.1/neuroshape/nulls/eigensphere.py` & `neuroshape-0.0.4.6.2/neuroshape/nulls/eigensphere.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.1/neuroshape/nulls/nulls.py` & `neuroshape-0.0.4.6.2/neuroshape/nulls/nulls.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.1/neuroshape/nulls/spins.py` & `neuroshape-0.0.4.6.2/neuroshape/nulls/spins.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.1/neuroshape/nulls/tests/eigenmode_replication.py` & `neuroshape-0.0.4.6.2/neuroshape/nulls/tests/eigenmode_replication.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.1/neuroshape/nulls/tests/test_burt.py` & `neuroshape-0.0.4.6.2/neuroshape/nulls/tests/test_burt.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.1/neuroshape/nulls/tests/test_eigenresamp.py` & `neuroshape-0.0.4.6.2/neuroshape/nulls/tests/test_eigenresamp.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.1/neuroshape/nulls/tests/test_nulls.py` & `neuroshape-0.0.4.6.2/neuroshape/nulls/tests/test_nulls.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.1/neuroshape/nulls/tests/test_spins.py` & `neuroshape-0.0.4.6.2/neuroshape/nulls/tests/test_spins.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.1/neuroshape/nulls/waveshuff.py` & `neuroshape-0.0.4.6.2/neuroshape/nulls/waveshuff.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.1/neuroshape/permutation.py` & `neuroshape-0.0.4.6.2/neuroshape/permutation.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.1/neuroshape/recon.py` & `neuroshape-0.0.4.6.2/neuroshape/recon.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.1/neuroshape/stats.py` & `neuroshape-0.0.4.6.2/neuroshape/stats.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.1/neuroshape/utils/check_fs_subjid.py` & `neuroshape-0.0.4.6.2/neuroshape/utils/check_fs_subjid.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.1/neuroshape/utils/check_map.py` & `neuroshape-0.0.4.6.2/neuroshape/utils/check_map.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.1/neuroshape/utils/checks.py` & `neuroshape-0.0.4.6.2/neuroshape/utils/checks.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.1/neuroshape/utils/compare_parallel.py` & `neuroshape-0.0.4.6.2/neuroshape/utils/compare_parallel.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.1/neuroshape/utils/compute_geodesic_distance.py` & `neuroshape-0.0.4.6.2/neuroshape/utils/compute_geodesic_distance.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.1/neuroshape/utils/concavehull.py` & `neuroshape-0.0.4.6.2/neuroshape/utils/concavehull.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.1/neuroshape/utils/eigen.py` & `neuroshape-0.0.4.6.2/neuroshape/utils/eigen.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.1/neuroshape/utils/fetch_atlas.py` & `neuroshape-0.0.4.6.2/neuroshape/utils/fetch_atlas.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.1/neuroshape/utils/fs_shapeDNA.py` & `neuroshape-0.0.4.6.2/neuroshape/utils/fs_shapeDNA.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.1/neuroshape/utils/geometry.py` & `neuroshape-0.0.4.6.2/neuroshape/utils/geometry.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.1/neuroshape/utils/meshtransforms.py` & `neuroshape-0.0.4.6.2/neuroshape/utils/meshtransforms.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.1/neuroshape/utils/tmpname.py` & `neuroshape-0.0.4.6.2/neuroshape/utils/tmpname.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.1/neuroshape.egg-info/SOURCES.txt` & `neuroshape-0.0.4.6.2/neuroshape.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.1/pyproject.toml` & `neuroshape-0.0.4.6.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = [
-    "python >= '3.8'",
-    "lapy >= '0.6', < '0.7'",
+    "python >= 3.8",
+    "lapy >= 0.6, < 0.7",
     "neuromaps >= 0.0.4",
     "scikit-sparse >= 0.4.8",
     "nibabel >= 3.0",
     "nilearn >= 0.7",
     "scipy",
     "numpy >= 1.14",
     "brainsmash",
     "setuptools>=42",
     "wheel",
 ]
 
 
 [project]
 name = "neuroshape"
-version = "0.0.4.6.1"
+version = "0.0.4.6.2"
 description = "For computing connectopic and geometric Laplacian eigenmodes and performing null hypothesis testing. As implementation is ongoing, this description is subject to rapid change."
 readme = "README.rst"
 authors = [
     {name = "Nikitas C. Koussis", email = "nikitas.koussis@gmail.com"},
 ]
 license = { file = "LICENSE" }
```

### Comparing `neuroshape-0.0.4.6.1/setup.py` & `neuroshape-0.0.4.6.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,14 +13,14 @@
 #                   include_dirs=[numpy.get_include()])
 
 #euler = Extension('neuroshape.euler', sources=['src/euler_threshold.c'],
 #                  include_dirs=[numpy.get_include()])
 
 # run the setup
 setup(name='neuroshape',
-      version='0.0.4.6.1',
+      version='0.0.4.6.2',
       description="For computing connectopic and geometric Laplacian eigenmodes and performing null hypothesis testing. As implementation is ongoing, this description is subject to rapid change.",
       author='Nikitas C. Koussis, Systems Neuroscience Group Newcastle',
       author_email='nikitas.koussis@gmail.com',
       url='https://github.com/nikitas-k/neuroshape-dev',
       packages=find_packages())
       #ext_modules=[eta, glmfit, euler])
```

### Comparing `neuroshape-0.0.4.6.1/src/eta_squared.c` & `neuroshape-0.0.4.6.2/src/eta_squared.c`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.1/src/euler_threshold.c` & `neuroshape-0.0.4.6.2/src/euler_threshold.c`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.1/src/glmfit.c` & `neuroshape-0.0.4.6.2/src/glmfit.c`

 * *Files identical despite different names*

