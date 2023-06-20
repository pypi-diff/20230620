# Comparing `tmp/neuroshape-0.0.4.4.tar.gz` & `tmp/neuroshape-0.0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuroshape-0.0.4.4.tar", last modified: Fri Jun 16 04:11:28 2023, max compression
+gzip compressed data, was "neuroshape-0.0.4.5.tar", last modified: Mon Jun 19 07:43:38 2023, max compression
```

## Comparing `neuroshape-0.0.4.4.tar` & `neuroshape-0.0.4.5.tar`

### file list

```diff
@@ -1,63 +1,56 @@
-drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-16 04:11:28.338609 neuroshape-0.0.4.4/
--rw-r--r--   0 nik        (502) admin       (80)     1501 2023-06-07 02:08:37.000000 neuroshape-0.0.4.4/LICENSE
--rw-r--r--   0 nik        (502) admin       (80)      468 2023-06-16 04:11:28.338269 neuroshape-0.0.4.4/PKG-INFO
--rw-r--r--   0 nik        (502) admin       (80)     4445 2023-06-08 03:48:59.000000 neuroshape-0.0.4.4/README.rst
-drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-16 04:11:28.227810 neuroshape-0.0.4.4/neuroshape/
--rw-r--r--   0 nik        (502) admin       (80)        0 2023-06-04 23:43:38.000000 neuroshape-0.0.4.4/neuroshape/__init__.py
--rw-r--r--   0 nik        (502) admin       (80)    22407 2023-06-15 03:59:02.000000 neuroshape-0.0.4.4/neuroshape/connectopic_laplacian.py
--rw-r--r--   0 nik        (502) admin       (80)    22975 2023-06-16 04:08:55.000000 neuroshape-0.0.4.4/neuroshape/eigenmodes.py
-drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-16 04:11:28.229283 neuroshape-0.0.4.4/neuroshape/nipype/
--rw-r--r--   0 nik        (502) admin       (80)        0 2023-06-04 23:43:38.000000 neuroshape-0.0.4.4/neuroshape/nipype/__init__.py
-drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-16 04:11:28.229505 neuroshape-0.0.4.4/neuroshape/nipype/interfaces/
--rw-r--r--   0 nik        (502) admin       (80)        0 2023-06-04 23:43:38.000000 neuroshape-0.0.4.4/neuroshape/nipype/interfaces/__init__.py
-drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-16 04:11:28.230006 neuroshape-0.0.4.4/neuroshape/nipype/interfaces/workbench/
--rw-r--r--   0 nik        (502) admin       (80)      269 2023-06-04 23:43:38.000000 neuroshape-0.0.4.4/neuroshape/nipype/interfaces/workbench/__init__.py
--rw-r--r--   0 nik        (502) admin       (80)    13219 2023-06-04 23:43:38.000000 neuroshape-0.0.4.4/neuroshape/nipype/interfaces/workbench/metric.py
-drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-16 04:11:28.248498 neuroshape-0.0.4.4/neuroshape/nulls/
--rw-r--r--   0 nik        (502) admin       (80)       44 2023-06-08 03:48:59.000000 neuroshape-0.0.4.4/neuroshape/nulls/__init__.py
--rw-r--r--   0 nik        (502) admin       (80)     5351 2023-06-04 23:43:38.000000 neuroshape-0.0.4.4/neuroshape/nulls/burt.py
--rw-r--r--   0 nik        (502) admin       (80)    20808 2023-06-13 01:26:03.000000 neuroshape-0.0.4.4/neuroshape/nulls/eigenshuff.py
--rw-r--r--   0 nik        (502) admin       (80)    11949 2023-06-15 23:21:48.000000 neuroshape-0.0.4.4/neuroshape/nulls/eigensphere.py
--rw-r--r--   0 nik        (502) admin       (80)    25239 2023-06-04 23:43:38.000000 neuroshape-0.0.4.4/neuroshape/nulls/nulls.py
--rw-r--r--   0 nik        (502) admin       (80)    27669 2023-06-04 23:43:38.000000 neuroshape-0.0.4.4/neuroshape/nulls/spins.py
-drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-16 04:11:28.284392 neuroshape-0.0.4.4/neuroshape/nulls/tests/
--rw-r--r--   0 nik        (502) admin       (80)        0 2023-06-04 23:43:38.000000 neuroshape-0.0.4.4/neuroshape/nulls/tests/__init__.py
--rw-r--r--   0 nik        (502) admin       (80)     4890 2023-06-13 05:36:45.000000 neuroshape-0.0.4.4/neuroshape/nulls/tests/eigenmode_replication.py
--rw-r--r--   0 nik        (502) admin       (80)      530 2023-06-04 23:43:38.000000 neuroshape-0.0.4.4/neuroshape/nulls/tests/test_burt.py
--rw-r--r--   0 nik        (502) admin       (80)     4119 2023-06-15 23:21:48.000000 neuroshape-0.0.4.4/neuroshape/nulls/tests/test_eigenresamp.py
--rw-r--r--   0 nik        (502) admin       (80)      695 2023-06-04 23:43:38.000000 neuroshape-0.0.4.4/neuroshape/nulls/tests/test_nulls.py
--rw-r--r--   0 nik        (502) admin       (80)      814 2023-06-04 23:43:38.000000 neuroshape-0.0.4.4/neuroshape/nulls/tests/test_spins.py
--rw-r--r--   0 nik        (502) admin       (80)    12845 2023-06-04 23:43:38.000000 neuroshape-0.0.4.4/neuroshape/nulls/waveshuff.py
--rw-r--r--   0 nik        (502) admin       (80)     4078 2023-06-04 23:43:38.000000 neuroshape-0.0.4.4/neuroshape/permutation.py
--rw-r--r--   0 nik        (502) admin       (80)    13885 2023-06-14 05:13:56.000000 neuroshape-0.0.4.4/neuroshape/recon.py
--rw-r--r--   0 nik        (502) admin       (80)     5400 2023-06-04 23:43:38.000000 neuroshape-0.0.4.4/neuroshape/stats.py
-drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-16 04:11:28.289305 neuroshape-0.0.4.4/neuroshape/utils/
--rw-r--r--   0 nik        (502) admin       (80)       25 2023-06-07 00:31:38.000000 neuroshape-0.0.4.4/neuroshape/utils/__init__.py
--rw-r--r--   0 nik        (502) admin       (80)     1345 2023-06-04 23:43:38.000000 neuroshape-0.0.4.4/neuroshape/utils/check_fs_subjid.py
--rw-r--r--   0 nik        (502) admin       (80)      616 2023-06-04 23:43:38.000000 neuroshape-0.0.4.4/neuroshape/utils/check_map.py
--rw-r--r--   0 nik        (502) admin       (80)     6553 2023-06-04 23:43:38.000000 neuroshape-0.0.4.4/neuroshape/utils/checks.py
--rw-r--r--   0 nik        (502) admin       (80)      917 2023-06-04 23:43:38.000000 neuroshape-0.0.4.4/neuroshape/utils/compare_parallel.py
--rw-r--r--   0 nik        (502) admin       (80)     3501 2023-06-04 23:43:38.000000 neuroshape-0.0.4.4/neuroshape/utils/compute_geodesic_distance.py
--rw-r--r--   0 nik        (502) admin       (80)     6248 2023-06-04 23:43:38.000000 neuroshape-0.0.4.4/neuroshape/utils/concavehull.py
--rw-r--r--   0 nik        (502) admin       (80)    12044 2023-06-15 23:21:48.000000 neuroshape-0.0.4.4/neuroshape/utils/eigen.py
--rw-r--r--   0 nik        (502) admin       (80)      763 2023-06-13 01:26:03.000000 neuroshape-0.0.4.4/neuroshape/utils/fetch_atlas.py
--rw-r--r--   0 nik        (502) admin       (80)    25397 2023-06-04 23:43:38.000000 neuroshape-0.0.4.4/neuroshape/utils/fs_shapeDNA.py
--rw-r--r--   0 nik        (502) admin       (80)    30218 2023-06-16 03:21:06.000000 neuroshape-0.0.4.4/neuroshape/utils/geometry.py
--rw-r--r--   0 nik        (502) admin       (80)      348 2023-06-04 23:43:38.000000 neuroshape-0.0.4.4/neuroshape/utils/load_mesh_vertices.py
--rw-r--r--   0 nik        (502) admin       (80)     2639 2023-06-04 23:43:38.000000 neuroshape-0.0.4.4/neuroshape/utils/meshtransforms.py
--rw-r--r--   0 nik        (502) admin       (80)      222 2023-06-13 01:26:03.000000 neuroshape-0.0.4.4/neuroshape/utils/normalize_data.py
--rw-r--r--   0 nik        (502) admin       (80)      201 2023-06-04 23:43:38.000000 neuroshape-0.0.4.4/neuroshape/utils/swap_single_row.py
--rw-r--r--   0 nik        (502) admin       (80)      540 2023-06-04 23:43:38.000000 neuroshape-0.0.4.4/neuroshape/utils/tmpname.py
--rw-r--r--   0 nik        (502) admin       (80)      193 2023-06-04 23:43:38.000000 neuroshape-0.0.4.4/neuroshape/utils/zscore_avg_method.py
-drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-16 04:11:28.228984 neuroshape-0.0.4.4/neuroshape.egg-info/
--rw-r--r--   0 nik        (502) admin       (80)      468 2023-06-16 04:11:28.000000 neuroshape-0.0.4.4/neuroshape.egg-info/PKG-INFO
--rw-r--r--   0 nik        (502) admin       (80)     1554 2023-06-16 04:11:28.000000 neuroshape-0.0.4.4/neuroshape.egg-info/SOURCES.txt
--rw-r--r--   0 nik        (502) admin       (80)        1 2023-06-16 04:11:28.000000 neuroshape-0.0.4.4/neuroshape.egg-info/dependency_links.txt
--rw-r--r--   0 nik        (502) admin       (80)       11 2023-06-16 04:11:28.000000 neuroshape-0.0.4.4/neuroshape.egg-info/top_level.txt
--rw-r--r--   0 nik        (502) admin       (80)      618 2023-06-16 04:11:22.000000 neuroshape-0.0.4.4/pyproject.toml
--rw-r--r--   0 nik        (502) admin       (80)       38 2023-06-16 04:11:28.338698 neuroshape-0.0.4.4/setup.cfg
--rw-r--r--   0 nik        (502) admin       (80)     1046 2023-06-16 04:11:08.000000 neuroshape-0.0.4.4/setup.py
-drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-16 04:11:28.317860 neuroshape-0.0.4.4/src/
--rw-r--r--   0 nik        (502) admin       (80)     5389 2023-06-09 06:16:05.000000 neuroshape-0.0.4.4/src/eta_squared.c
--rw-r--r--   0 nik        (502) admin       (80)     2545 2023-06-06 05:49:54.000000 neuroshape-0.0.4.4/src/euler_threshold.c
--rw-r--r--   0 nik        (502) admin       (80)     5946 2023-06-06 05:46:53.000000 neuroshape-0.0.4.4/src/glmfit.c
+drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-19 07:43:38.703756 neuroshape-0.0.4.5/
+-rw-r--r--   0 nik        (502) admin       (80)     1501 2023-06-07 02:08:37.000000 neuroshape-0.0.4.5/LICENSE
+-rw-r--r--   0 nik        (502) admin       (80)      468 2023-06-19 07:43:38.703365 neuroshape-0.0.4.5/PKG-INFO
+-rw-r--r--   0 nik        (502) admin       (80)     4445 2023-06-08 03:48:59.000000 neuroshape-0.0.4.5/README.rst
+drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-19 07:43:38.504448 neuroshape-0.0.4.5/neuroshape/
+-rw-r--r--   0 nik        (502) admin       (80)        0 2023-06-04 23:43:38.000000 neuroshape-0.0.4.5/neuroshape/__init__.py
+-rw-r--r--   0 nik        (502) admin       (80)    22407 2023-06-15 03:59:02.000000 neuroshape-0.0.4.5/neuroshape/connectopic_laplacian.py
+-rw-r--r--   0 nik        (502) admin       (80)    22913 2023-06-18 23:49:14.000000 neuroshape-0.0.4.5/neuroshape/eigenmodes.py
+drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-19 07:43:38.531090 neuroshape-0.0.4.5/neuroshape/nulls/
+-rw-r--r--   0 nik        (502) admin       (80)       44 2023-06-08 03:48:59.000000 neuroshape-0.0.4.5/neuroshape/nulls/__init__.py
+-rw-r--r--   0 nik        (502) admin       (80)     5351 2023-06-04 23:43:38.000000 neuroshape-0.0.4.5/neuroshape/nulls/burt.py
+-rw-r--r--   0 nik        (502) admin       (80)    20808 2023-06-13 01:26:03.000000 neuroshape-0.0.4.5/neuroshape/nulls/eigenshuff.py
+-rw-r--r--   0 nik        (502) admin       (80)    11838 2023-06-19 05:24:56.000000 neuroshape-0.0.4.5/neuroshape/nulls/eigensphere.py
+-rw-r--r--   0 nik        (502) admin       (80)    25239 2023-06-04 23:43:38.000000 neuroshape-0.0.4.5/neuroshape/nulls/nulls.py
+-rw-r--r--   0 nik        (502) admin       (80)    27669 2023-06-04 23:43:38.000000 neuroshape-0.0.4.5/neuroshape/nulls/spins.py
+drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-19 07:43:38.534463 neuroshape-0.0.4.5/neuroshape/nulls/tests/
+-rw-r--r--   0 nik        (502) admin       (80)        0 2023-06-04 23:43:38.000000 neuroshape-0.0.4.5/neuroshape/nulls/tests/__init__.py
+-rw-r--r--   0 nik        (502) admin       (80)     5042 2023-06-19 01:29:34.000000 neuroshape-0.0.4.5/neuroshape/nulls/tests/eigenmode_replication.py
+-rw-r--r--   0 nik        (502) admin       (80)      530 2023-06-04 23:43:38.000000 neuroshape-0.0.4.5/neuroshape/nulls/tests/test_burt.py
+-rw-r--r--   0 nik        (502) admin       (80)     4137 2023-06-17 23:29:12.000000 neuroshape-0.0.4.5/neuroshape/nulls/tests/test_eigenresamp.py
+-rw-r--r--   0 nik        (502) admin       (80)      695 2023-06-04 23:43:38.000000 neuroshape-0.0.4.5/neuroshape/nulls/tests/test_nulls.py
+-rw-r--r--   0 nik        (502) admin       (80)      814 2023-06-04 23:43:38.000000 neuroshape-0.0.4.5/neuroshape/nulls/tests/test_spins.py
+-rw-r--r--   0 nik        (502) admin       (80)    12845 2023-06-04 23:43:38.000000 neuroshape-0.0.4.5/neuroshape/nulls/waveshuff.py
+-rw-r--r--   0 nik        (502) admin       (80)     4078 2023-06-04 23:43:38.000000 neuroshape-0.0.4.5/neuroshape/permutation.py
+-rw-r--r--   0 nik        (502) admin       (80)    13180 2023-06-18 23:49:14.000000 neuroshape-0.0.4.5/neuroshape/recon.py
+-rw-r--r--   0 nik        (502) admin       (80)     5400 2023-06-04 23:43:38.000000 neuroshape-0.0.4.5/neuroshape/stats.py
+drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-19 07:43:38.598903 neuroshape-0.0.4.5/neuroshape/utils/
+-rw-r--r--   0 nik        (502) admin       (80)       25 2023-06-07 00:31:38.000000 neuroshape-0.0.4.5/neuroshape/utils/__init__.py
+-rw-r--r--   0 nik        (502) admin       (80)     1345 2023-06-04 23:43:38.000000 neuroshape-0.0.4.5/neuroshape/utils/check_fs_subjid.py
+-rw-r--r--   0 nik        (502) admin       (80)      616 2023-06-04 23:43:38.000000 neuroshape-0.0.4.5/neuroshape/utils/check_map.py
+-rw-r--r--   0 nik        (502) admin       (80)     6553 2023-06-04 23:43:38.000000 neuroshape-0.0.4.5/neuroshape/utils/checks.py
+-rw-r--r--   0 nik        (502) admin       (80)      917 2023-06-04 23:43:38.000000 neuroshape-0.0.4.5/neuroshape/utils/compare_parallel.py
+-rw-r--r--   0 nik        (502) admin       (80)     3501 2023-06-04 23:43:38.000000 neuroshape-0.0.4.5/neuroshape/utils/compute_geodesic_distance.py
+-rw-r--r--   0 nik        (502) admin       (80)     6248 2023-06-04 23:43:38.000000 neuroshape-0.0.4.5/neuroshape/utils/concavehull.py
+-rw-r--r--   0 nik        (502) admin       (80)    11452 2023-06-19 05:08:45.000000 neuroshape-0.0.4.5/neuroshape/utils/eigen.py
+-rw-r--r--   0 nik        (502) admin       (80)      763 2023-06-13 01:26:03.000000 neuroshape-0.0.4.5/neuroshape/utils/fetch_atlas.py
+-rw-r--r--   0 nik        (502) admin       (80)    25397 2023-06-04 23:43:38.000000 neuroshape-0.0.4.5/neuroshape/utils/fs_shapeDNA.py
+-rw-r--r--   0 nik        (502) admin       (80)    31133 2023-06-18 23:49:14.000000 neuroshape-0.0.4.5/neuroshape/utils/geometry.py
+-rw-r--r--   0 nik        (502) admin       (80)      348 2023-06-04 23:43:38.000000 neuroshape-0.0.4.5/neuroshape/utils/load_mesh_vertices.py
+-rw-r--r--   0 nik        (502) admin       (80)     2639 2023-06-04 23:43:38.000000 neuroshape-0.0.4.5/neuroshape/utils/meshtransforms.py
+-rw-r--r--   0 nik        (502) admin       (80)      222 2023-06-13 01:26:03.000000 neuroshape-0.0.4.5/neuroshape/utils/normalize_data.py
+-rw-r--r--   0 nik        (502) admin       (80)      201 2023-06-04 23:43:38.000000 neuroshape-0.0.4.5/neuroshape/utils/swap_single_row.py
+-rw-r--r--   0 nik        (502) admin       (80)      540 2023-06-04 23:43:38.000000 neuroshape-0.0.4.5/neuroshape/utils/tmpname.py
+-rw-r--r--   0 nik        (502) admin       (80)      193 2023-06-04 23:43:38.000000 neuroshape-0.0.4.5/neuroshape/utils/zscore_avg_method.py
+drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-19 07:43:38.506972 neuroshape-0.0.4.5/neuroshape.egg-info/
+-rw-r--r--   0 nik        (502) admin       (80)      468 2023-06-19 07:43:38.000000 neuroshape-0.0.4.5/neuroshape.egg-info/PKG-INFO
+-rw-r--r--   0 nik        (502) admin       (80)     1383 2023-06-19 07:43:38.000000 neuroshape-0.0.4.5/neuroshape.egg-info/SOURCES.txt
+-rw-r--r--   0 nik        (502) admin       (80)        1 2023-06-19 07:43:38.000000 neuroshape-0.0.4.5/neuroshape.egg-info/dependency_links.txt
+-rw-r--r--   0 nik        (502) admin       (80)       11 2023-06-19 07:43:38.000000 neuroshape-0.0.4.5/neuroshape.egg-info/top_level.txt
+-rw-r--r--   0 nik        (502) admin       (80)      839 2023-06-19 00:20:26.000000 neuroshape-0.0.4.5/pyproject.toml
+-rw-r--r--   0 nik        (502) admin       (80)       38 2023-06-19 07:43:38.703868 neuroshape-0.0.4.5/setup.cfg
+-rw-r--r--   0 nik        (502) admin       (80)     1046 2023-06-19 00:19:59.000000 neuroshape-0.0.4.5/setup.py
+drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-19 07:43:38.664586 neuroshape-0.0.4.5/src/
+-rw-r--r--   0 nik        (502) admin       (80)     5389 2023-06-09 06:16:05.000000 neuroshape-0.0.4.5/src/eta_squared.c
+-rw-r--r--   0 nik        (502) admin       (80)     2545 2023-06-06 05:49:54.000000 neuroshape-0.0.4.5/src/euler_threshold.c
+-rw-r--r--   0 nik        (502) admin       (80)     5946 2023-06-06 05:46:53.000000 neuroshape-0.0.4.5/src/glmfit.c
```

### Comparing `neuroshape-0.0.4.4/LICENSE` & `neuroshape-0.0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.4/README.rst` & `neuroshape-0.0.4.5/README.rst`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.4/neuroshape/connectopic_laplacian.py` & `neuroshape-0.0.4.5/neuroshape/connectopic_laplacian.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.4/neuroshape/eigenmodes.py` & `neuroshape-0.0.4.5/neuroshape/eigenmodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,41 +100,39 @@
                   surface from the <sid>/surfs directory.
 
 
 OPTIONAL ARGUMENTS
 
 --sdir <name>     Subjects directory (or set via environment $SUBJECTS_DIR)
 
---outdir <name>   Output directory (default: <sdir>/<sid>/brainprint/ )
+--outdir <name>   Output directory (default: <sdir>/<sid>/neuroshape/ )
 
 --outsurf <name>  Name for surface output (with --asegid)
                   (default: aseg.<asegid>.surf )
 
 --outevec <name>    Name for eigenmodes output
                   (default: <(out)surf>.<shapedna_parameters>.txt )
                   
 --savegii <name>  Name for gifti output if input is surface
 
 --label <name>    Label to create surface patch if input is surface
 
 --savenii <name>  Name for nifti output (modes are projected to new volume in freesurfer space)
 
-ShapeDNA parameters (see shapeDNA --help for details):
+ShapeDNA parameters (see shapeDNA [1] for details):
 
 --num <int>       Number of eigenvalues/vectors to compute (default: 50)
 
 --degree <int>    FEM degree (default 1)
 
 --bcond <int>     Boundary condition (0=Dirichlet, 1=Neumann default)
 
 --evec            Additionally compute eigenvectors
 
 --ignorelq        Ignore low quality in input mesh
-
---sparam "<str>"  Additional parameters for shapeDNA-tria
 """
 
 def split_callback(option, opt, value, parser):
   setattr(parser.values, option.dest, value.split(','))
   
 def options_parse():
     """
```

### Comparing `neuroshape-0.0.4.4/neuroshape/nulls/burt.py` & `neuroshape-0.0.4.5/neuroshape/nulls/burt.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.4/neuroshape/nulls/eigenshuff.py` & `neuroshape-0.0.4.5/neuroshape/nulls/eigenshuff.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.4/neuroshape/nulls/eigensphere.py` & `neuroshape-0.0.4.5/neuroshape/nulls/eigensphere.py`

 * *Files 2% similar despite different names*

```diff
@@ -173,21 +173,22 @@
     #     else:
     #         raise ValueError("Normalization type must be 'constant', 'number', 'volume', 'area'")
     if decomp_method is not None:
         if decomp_method in methods:
             method = decomp_method
         else:
             raise ValueError("Eigenmode decomposition method must be 'matrix' or 'regression'")
-    # if not given angles
-    if angles is None:
-        angles = np.random.random_sample(size=emodes.shape[1] - 1) * np.pi
-    
+            
     # find eigengroups
     groups = _get_eigengroups(emodes)
     
+    # if not given angles
+    if angles is None:
+        angles = np.random.random_sample(size=len(groups) - 1) * 2 * np.pi
+    
     # initialize the new modes
     new_modes = np.zeros_like(emodes)
     
     # resample the hypersphere (except for groups 1 and 2)
     for group in groups:
         group_modes = emodes[:, group]
         group_evals = evals[group]
@@ -195,38 +196,34 @@
         
         if len(group) == 1:
             # resample along the line of real numbers (0, 1)
             group_modes *= np.random.random()
             # ensure orthonormal
             new_modes[:, group] = group_modes / np.linalg.norm(group_modes)
         
-        if len(group) == 2:
-            r_i = 1
+        if len(group) == 3:
             # do simple rotation
             # initialize the points
-            p = r_i * group_modes
-            for i in range(1, group_modes.shape[1]):
-                for j in range(i):
-                    r_i *= np.sin(angles[j])
-                    if i < group_modes.shape[0] - 1:
-                        r_i *= np.cos(angles[j-1])
-            
+            p = group_modes
+            for i in range(0, group_modes.shape[1]):
+                r_i = 1 * np.sin(angles[0])
                 p += r_i * group_modes[i]
             
             # ensure orthonormal
             group_new_modes = p
-            new_modes[:, group] = np.linalg.qr(group_new_modes, mode='reduced')[0]
-            
+             # get the index for the angles
+            #new_modes[:, group] = np.linalg.qr(group_new_modes, mode='reduced')[0]
+        m = 1   
         # else, transform to spheroid and index the angles properly
         group_modes = transform_to_spheroid(group_evals, group_modes)
-        group_new_modes = resample_spheroid(group_modes, angles[group])
+        group_new_modes = resample_spheroid(group_modes, angles[m])
         
         # transform back to ellipsoid
         new_modes[:, group] = transform_to_ellipsoid(group_evals, group_new_modes)
-    
+        m += 1
     # reconstruct the new surface
     # if normalize == 'constant':
     #     if norm_factor > 0.:
     #         new_surface = reconstruct_surface(surface, new_modes, normalize=normalize, norm_factor=norm_factor, method=method)
     #     else:
     #         raise ValueError("Normalization factor must be greater than zero")
     # else:
```

### Comparing `neuroshape-0.0.4.4/neuroshape/nulls/nulls.py` & `neuroshape-0.0.4.5/neuroshape/nulls/nulls.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.4/neuroshape/nulls/spins.py` & `neuroshape-0.0.4.5/neuroshape/nulls/spins.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.4/neuroshape/nulls/tests/eigenmode_replication.py` & `neuroshape-0.0.4.5/neuroshape/nulls/tests/eigenmode_replication.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 """
+- Load in the functional data of HCP subject 100206 
+- calculate the functional connectivity of a particular time step
+- Do the LBO on the same surface
 - Split the eigenvectors of an eigengroup into half the brain and the other half
 - See if the eigenvector activity of one half predicts the other half
 - Do all, but expected to be medium frequency (20/30/40/50)
 - Coefficients of eigenmodes to reconstruct the original data
 - Are the coefficents correlated/similar at the front and back
 - False positives concerns:
     - Too low frequency of the eigenmodes
```

### Comparing `neuroshape-0.0.4.4/neuroshape/nulls/tests/test_burt.py` & `neuroshape-0.0.4.5/neuroshape/nulls/tests/test_burt.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.4/neuroshape/nulls/tests/test_eigenresamp.py` & `neuroshape-0.0.4.5/neuroshape/nulls/tests/test_eigenresamp.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     coords, faces = surface.darrays
     
     coords = coords.data
     faces = faces.data
     
     # compute LBO
     tria = TriaMesh(coords, faces)
-    ev = compute_shapedna(tria, k=n)
+    ev = compute_shapedna(tria, k=n, use_cholmod=True)
     
     # exclude the zeroth mode
     emodes = ev['Eigenvectors'][:,1:]
     emodes = emodes/np.linalg.norm(emodes, axis=0)
     evals = ev['Eigenvalues'][1:]
     
     # initialize the surrogate array - compute only the vertices, the faces are the same
```

### Comparing `neuroshape-0.0.4.4/neuroshape/nulls/tests/test_nulls.py` & `neuroshape-0.0.4.5/neuroshape/nulls/tests/test_nulls.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.4/neuroshape/nulls/tests/test_spins.py` & `neuroshape-0.0.4.5/neuroshape/nulls/tests/test_spins.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.4/neuroshape/nulls/waveshuff.py` & `neuroshape-0.0.4.5/neuroshape/nulls/waveshuff.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.4/neuroshape/permutation.py` & `neuroshape-0.0.4.5/neuroshape/permutation.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.4/neuroshape/stats.py` & `neuroshape-0.0.4.5/neuroshape/stats.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.4/neuroshape/utils/check_fs_subjid.py` & `neuroshape-0.0.4.5/neuroshape/utils/check_fs_subjid.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.4/neuroshape/utils/check_map.py` & `neuroshape-0.0.4.5/neuroshape/utils/check_map.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.4/neuroshape/utils/checks.py` & `neuroshape-0.0.4.5/neuroshape/utils/checks.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.4/neuroshape/utils/compare_parallel.py` & `neuroshape-0.0.4.5/neuroshape/utils/compare_parallel.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.4/neuroshape/utils/compute_geodesic_distance.py` & `neuroshape-0.0.4.5/neuroshape/utils/compute_geodesic_distance.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.4/neuroshape/utils/concavehull.py` & `neuroshape-0.0.4.5/neuroshape/utils/concavehull.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.4/neuroshape/utils/eigen.py` & `neuroshape-0.0.4.5/neuroshape/utils/eigen.py`

 * *Files 8% similar despite different names*

```diff
@@ -103,35 +103,41 @@
             return eigs_.T
     except:
         return eigs_.T
     eigs_ = eigs_swapped
     previous_corr = next_corr
     
 
-def reconstruct_data(coeffs, eigenmodes, n=100):
+def reconstruct_data(coeffs, eigenmodes, pv=100.0):
     """
     Reconstruct a dataset of `n_vertices` given a set of eigenmodes and coeffs
     conditioned on data using ordinary least squares (OLS)
 
     Parameters
     ----------
     coeffs : np.ndarray of shape (M,)
         Coefficients output from fitting OLS
     eigenmodes : np.ndarray of shape (n_vertices, M)
         Eigenmodes of `n_vertices` by number of eigenvalues M
-    n : int (default 100)
-        Number of eigenmodes to use for reconstruction
+    pv : float (default 100), rounds up to nearest index
+        Percentage of `eigenmodes` to use for reconstruction (default 100%)
 
     Returns
     -------
     new_data : np.ndarray of (n_vertices,)
         Reconstructed data
 
     """
     
+    if pv == 0.0:
+        raise ValueError("Percentage of modes to use for reconstruction must be greater than 1")
+        
+    _, M = eigenmodes.shape
+    n = int(np.ceil(M * pv / 100))
+    
     eigenmodes = eigenmodes[:,:n]
     coeffs = coeffs[:n].reshape(-1, 1)
     
     new_data = np.matmul(eigenmodes, coeffs)
     
     return new_data.squeeze()
     
@@ -290,59 +296,39 @@
     ellipsoid_axes = compute_axes_ellipsoid(eigenvalues)
     
     ellipsoid_eigenmodes = eigenmodes * ellipsoid_axes
     
     return ellipsoid_eigenmodes
 
 
-def resample_spheroid(spheroid_eigenmodes, angles=None):
+def resample_spheroid(spheroid_eigenmodes, angle):
     """
     Resample the N-D hypersphere generated by the N orthogonal unit modes
 
     """
     # radius = 1 on the unit hypersphere
     r = 1
     # ensure the eigenmodes are normalized on the unit hypersphere
     spheroid_eigenmodes = spheroid_eigenmodes / np.linalg.norm(spheroid_eigenmodes, axis=0)
     
     # initialize the new points p
     p = r * spheroid_eigenmodes
     
-    # check if angles are input or not
-    if angles is not None:
-        if angles.shape[0] != spheroid_eigenmodes.shape[1]:
-            raise ValueError("The number of angles should be the same as the number of basis modes")
-        angles = angles
-    else:
-        angles = np.random.random_sample(size=spheroid_eigenmodes.shape[1] - 1) * 2 * np.pi
-        
     # Compute the coordinates for new points p
     print("Computing the coordinates for each dimension")
     for i in range(1, spheroid_eigenmodes.shape[1]):
-        r_i = r
-        for j in range(i):
-            if np.mod(i, 2) == 1: #ODD
-                if angles[j] > np.pi:
-                    angles[j] = (angles[j] % np.pi)*np.pi
-                r_i *= np.sin(angles[j])
-            else: #EVEN
-                if angles[j] > 2*np.pi: 
-                    angles[j] = (angles[j] % 2*np.pi)*2*np.pi
-                r_i *= np.cos(angles[j])
-        if i < spheroid_eigenmodes.shape[0] - 1:
-            r_i *= np.cos(angles[j-1])
-        
+        p = r * spheroid_eigenmodes
+        r_i = np.sin(angle)
         p += r_i * spheroid_eigenmodes[i]
         
     # find the unit modes that describe the points p
     new_modes = p / np.linalg.norm(p)
     
     # ensure that the unit modes are orthonormal (QR decomposition)
-    print("Ensuring the new modes are orthonormal")
-    new_modes = np.linalg.qr(new_modes, mode='reduced')[0]
+    #new_modes = np.linalg.qr(new_modes, mode='reduced')[0]
     
     return new_modes
 
 def _cartesian_to_spherical(x, y, z):
     """
     Convert Cartesian coordinates to spherical coordinates.
```

### Comparing `neuroshape-0.0.4.4/neuroshape/utils/fetch_atlas.py` & `neuroshape-0.0.4.5/neuroshape/utils/fetch_atlas.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.4/neuroshape/utils/fs_shapeDNA.py` & `neuroshape-0.0.4.5/neuroshape/utils/fs_shapeDNA.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.4/neuroshape/utils/geometry.py` & `neuroshape-0.0.4.5/neuroshape/utils/geometry.py`

 * *Files 2% similar despite different names*

```diff
@@ -902,8 +902,37 @@
     
     with open(filepath, 'w') as fobj:
         fobj.write(start_line)
         fobj.write(f'{magic_number}\n')
         
         #now write vertex and label array
         label_array = np.vstack((np.array(range(vnum)), vertices.T, vector.T)).T.astype('>f4')
-        np.savetxt(fobj, label_array, fmt=['%i','%f','%f','%f','%f'])
+        np.savetxt(fobj, label_array, fmt=['%i','%f','%f','%f','%f'])
+        
+def read_morph_data(filepath):
+    """Read a Freesurfer morphometry data file.
+
+    This function reads in what Freesurfer internally calls "curv" file types,
+    (e.g. ?h. curv, ?h.thickness), but as that has the potential to cause
+    confusion where "curv" also refers to the surface curvature values,
+    we refer to these files as "morphometry" files with PySurfer.
+
+    Parameters
+    ----------
+    filepath : str
+        Path to morphometry file
+
+    Returns
+    -------
+    curv : numpy array
+        Vector representation of surface morpometry values
+    """
+    with open(filepath, "rb") as fobj:
+        magic = _fread3(fobj)
+        if magic == 16777215:
+            vnum = np.fromfile(fobj, ">i4", 3)[0]
+            curv = np.fromfile(fobj, ">f4", vnum)
+        else:
+            vnum = magic
+            _fread3(fobj)
+            curv = np.fromfile(fobj, ">i2", vnum) / 100
+    return curv
```

### Comparing `neuroshape-0.0.4.4/neuroshape/utils/meshtransforms.py` & `neuroshape-0.0.4.5/neuroshape/utils/meshtransforms.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.4/neuroshape/utils/tmpname.py` & `neuroshape-0.0.4.5/neuroshape/utils/tmpname.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.4/neuroshape.egg-info/SOURCES.txt` & `neuroshape-0.0.4.5/neuroshape.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -8,18 +8,14 @@
 neuroshape/permutation.py
 neuroshape/recon.py
 neuroshape/stats.py
 neuroshape.egg-info/PKG-INFO
 neuroshape.egg-info/SOURCES.txt
 neuroshape.egg-info/dependency_links.txt
 neuroshape.egg-info/top_level.txt
-neuroshape/nipype/__init__.py
-neuroshape/nipype/interfaces/__init__.py
-neuroshape/nipype/interfaces/workbench/__init__.py
-neuroshape/nipype/interfaces/workbench/metric.py
 neuroshape/nulls/__init__.py
 neuroshape/nulls/burt.py
 neuroshape/nulls/eigenshuff.py
 neuroshape/nulls/eigensphere.py
 neuroshape/nulls/nulls.py
 neuroshape/nulls/spins.py
 neuroshape/nulls/waveshuff.py
```

### Comparing `neuroshape-0.0.4.4/pyproject.toml` & `neuroshape-0.0.4.5/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,26 @@
 [build-system]
 requires = ["setuptools>=42", "wheel", "numpy"]
 build-backend = "setuptools.build_meta"
+requires = [
+    "python >= '3.8'",
+    "lapy >= '0.6', < '0.7'",
+    "neuromaps >= 0.0.4",
+    "scikit-sparse >= 0.4.8",
+    "nibabel >= 3.0",
+    "nilearn >= 0.7",
+    "scipy",
+    "numpy >= 1.14",
+    "brainsmash",
+]
+
 
 [project]
 name = "neuroshape"
-version = "0.0.4.4"
+version = "0.0.4.5"
 description = "For computing connectopic and geometric Laplacian eigenmodes and performing null hypothesis testing. As implementation is ongoing, this description is subject to rapid change."
 readme = "README.rst"
 authors = [
     {name = "Nikitas C. Koussis", email = "nikitas.koussis@gmail.com"},
 ]
 license = { file = "LICENSE" }
```

### Comparing `neuroshape-0.0.4.4/setup.py` & `neuroshape-0.0.4.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,14 +13,14 @@
 #                   include_dirs=[numpy.get_include()])
 
 #euler = Extension('neuroshape.euler', sources=['src/euler_threshold.c'],
 #                  include_dirs=[numpy.get_include()])
 
 # run the setup
 setup(name='neuroshape',
-      version='0.0.4.4',
+      version='0.0.4.5',
       description="For computing connectopic and geometric Laplacian eigenmodes and performing null hypothesis testing. As implementation is ongoing, this description is subject to rapid change.",
       author='Nikitas C. Koussis, Systems Neuroscience Group Newcastle',
       author_email='nikitas.koussis@gmail.com',
       url='https://github.com/nikitas-k/neuroshape-dev',
       packages=find_packages())
       #ext_modules=[eta, glmfit, euler])
```

### Comparing `neuroshape-0.0.4.4/src/eta_squared.c` & `neuroshape-0.0.4.5/src/eta_squared.c`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.4/src/euler_threshold.c` & `neuroshape-0.0.4.5/src/euler_threshold.c`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.4/src/glmfit.c` & `neuroshape-0.0.4.5/src/glmfit.c`

 * *Files identical despite different names*

