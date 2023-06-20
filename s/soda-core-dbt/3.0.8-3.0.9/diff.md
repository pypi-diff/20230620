# Comparing `tmp/soda-core-dbt-3.0.8.tar.gz` & `tmp/soda-core-dbt-3.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soda-core-dbt-3.0.8.tar", last modified: Wed Sep 21 19:41:39 2022, max compression
+gzip compressed data, was "soda-core-dbt-3.0.9.tar", last modified: Tue Sep 27 20:19:48 2022, max compression
```

## Comparing `soda-core-dbt-3.0.8.tar` & `soda-core-dbt-3.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 19:41:39.083376 soda-core-dbt-3.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-21 19:41:39.083376 soda-core-dbt-3.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-21 19:41:39.083376 soda-core-dbt-3.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      608 2022-09-21 19:41:14.000000 soda-core-dbt-3.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 19:41:39.079376 soda-core-dbt-3.0.8/soda/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 19:41:39.079376 soda-core-dbt-3.0.8/soda/cloud/
--rw-r--r--   0 runner    (1001) docker     (121)    16926 2022-09-21 19:41:14.000000 soda-core-dbt-3.0.8/soda/cloud/dbt.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 19:41:39.079376 soda-core-dbt-3.0.8/soda/execution/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 19:41:39.079376 soda-core-dbt-3.0.8/soda/execution/check/
--rw-r--r--   0 runner    (1001) docker     (121)     2461 2022-09-21 19:41:14.000000 soda-core-dbt-3.0.8/soda/execution/check/dbt_check.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 19:41:39.079376 soda-core-dbt-3.0.8/soda/sodacl/
--rw-r--r--   0 runner    (1001) docker     (121)      424 2022-09-21 19:41:14.000000 soda-core-dbt-3.0.8/soda/sodacl/dbt_check_cfg.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 19:41:39.083376 soda-core-dbt-3.0.8/soda_core_dbt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-21 19:41:39.000000 soda-core-dbt-3.0.8/soda_core_dbt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      273 2022-09-21 19:41:39.000000 soda-core-dbt-3.0.8/soda_core_dbt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-21 19:41:39.000000 soda-core-dbt-3.0.8/soda_core_dbt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-09-21 19:41:39.000000 soda-core-dbt-3.0.8/soda_core_dbt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-09-21 19:41:39.000000 soda-core-dbt-3.0.8/soda_core_dbt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 20:19:48.591913 soda-core-dbt-3.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-27 20:19:48.591913 soda-core-dbt-3.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-27 20:19:48.591913 soda-core-dbt-3.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      608 2022-09-27 20:19:27.000000 soda-core-dbt-3.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 20:19:48.591913 soda-core-dbt-3.0.9/soda/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 20:19:48.591913 soda-core-dbt-3.0.9/soda/cloud/
+-rw-r--r--   0 runner    (1001) docker     (121)    16926 2022-09-27 20:19:27.000000 soda-core-dbt-3.0.9/soda/cloud/dbt.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 20:19:48.591913 soda-core-dbt-3.0.9/soda/execution/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 20:19:48.591913 soda-core-dbt-3.0.9/soda/execution/check/
+-rw-r--r--   0 runner    (1001) docker     (121)     2461 2022-09-27 20:19:27.000000 soda-core-dbt-3.0.9/soda/execution/check/dbt_check.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 20:19:48.591913 soda-core-dbt-3.0.9/soda/sodacl/
+-rw-r--r--   0 runner    (1001) docker     (121)      424 2022-09-27 20:19:27.000000 soda-core-dbt-3.0.9/soda/sodacl/dbt_check_cfg.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 20:19:48.591913 soda-core-dbt-3.0.9/soda_core_dbt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-27 20:19:48.000000 soda-core-dbt-3.0.9/soda_core_dbt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      273 2022-09-27 20:19:48.000000 soda-core-dbt-3.0.9/soda_core_dbt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-27 20:19:48.000000 soda-core-dbt-3.0.9/soda_core_dbt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       33 2022-09-27 20:19:48.000000 soda-core-dbt-3.0.9/soda_core_dbt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        5 2022-09-27 20:19:48.000000 soda-core-dbt-3.0.9/soda_core_dbt.egg-info/top_level.txt
```

### Comparing `soda-core-dbt-3.0.8/setup.py` & `soda-core-dbt-3.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 if sys.version_info < (3, 7):
     print("Error: Soda Core requires at least Python 3.7")
     print("Error: Please upgrade your Python version to 3.7 or later")
     sys.exit(1)
 
 package_name = "soda-core-dbt"
-package_version = "3.0.8"
+package_version = "3.0.9"
 description = "Soda Core dbt Package"
 
 requires = [
     f"soda-core=={package_version}",
     "dbt-core~=1.2.0",
 ]
 # TODO Fix the params
```

### Comparing `soda-core-dbt-3.0.8/soda/cloud/dbt.py` & `soda-core-dbt-3.0.9/soda/cloud/dbt.py`

 * *Files identical despite different names*

### Comparing `soda-core-dbt-3.0.8/soda/execution/check/dbt_check.py` & `soda-core-dbt-3.0.9/soda/execution/check/dbt_check.py`

 * *Files identical despite different names*

