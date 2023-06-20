# Comparing `tmp/soda-core-pandas-dask-3.0.40.tar.gz` & `tmp/soda-core-pandas-dask-3.0.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soda-core-pandas-dask-3.0.40.tar", last modified: Fri Jun 16 08:29:07 2023, max compression
+gzip compressed data, was "soda-core-pandas-dask-3.0.41.tar", last modified: Tue Jun 20 12:55:11 2023, max compression
```

## Comparing `soda-core-pandas-dask-3.0.40.tar` & `soda-core-pandas-dask-3.0.41.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 08:29:07.754683 soda-core-pandas-dask-3.0.40/
--rw-r--r--   0 runner    (1001) docker     (122)       66 2023-06-16 08:29:07.754683 soda-core-pandas-dask-3.0.40/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-16 08:29:07.754683 soda-core-pandas-dask-3.0.40/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      619 2023-06-16 08:28:48.000000 soda-core-pandas-dask-3.0.40/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 08:29:07.750682 soda-core-pandas-dask-3.0.40/soda/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 08:29:07.754683 soda-core-pandas-dask-3.0.40/soda/data_sources/
--rw-r--r--   0 runner    (1001) docker     (122)      386 2023-06-16 08:28:48.000000 soda-core-pandas-dask-3.0.40/soda/data_sources/dask_connection.py
--rw-r--r--   0 runner    (1001) docker     (122)     2732 2023-06-16 08:28:48.000000 soda-core-pandas-dask-3.0.40/soda/data_sources/dask_cursor.py
--rw-r--r--   0 runner    (1001) docker     (122)    13934 2023-06-16 08:28:48.000000 soda-core-pandas-dask-3.0.40/soda/data_sources/dask_data_source.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 08:29:07.754683 soda-core-pandas-dask-3.0.40/soda_core_pandas_dask.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)       66 2023-06-16 08:29:07.000000 soda-core-pandas-dask-3.0.40/soda_core_pandas_dask.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      359 2023-06-16 08:29:07.000000 soda-core-pandas-dask-3.0.40/soda_core_pandas_dask.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-16 08:29:07.000000 soda-core-pandas-dask-3.0.40/soda_core_pandas_dask.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       64 2023-06-16 08:29:07.000000 soda-core-pandas-dask-3.0.40/soda_core_pandas_dask.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-16 08:29:07.000000 soda-core-pandas-dask-3.0.40/soda_core_pandas_dask.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 08:29:07.754683 soda-core-pandas-dask-3.0.40/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      139 2023-06-16 08:28:48.000000 soda-core-pandas-dask-3.0.40/tests/test_dask.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 12:55:11.126637 soda-core-pandas-dask-3.0.41/
+-rw-r--r--   0 runner    (1001) docker     (122)       66 2023-06-20 12:55:11.126637 soda-core-pandas-dask-3.0.41/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-20 12:55:11.126637 soda-core-pandas-dask-3.0.41/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      619 2023-06-20 12:54:46.000000 soda-core-pandas-dask-3.0.41/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 12:55:11.126637 soda-core-pandas-dask-3.0.41/soda/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 12:55:11.126637 soda-core-pandas-dask-3.0.41/soda/data_sources/
+-rw-r--r--   0 runner    (1001) docker     (122)      386 2023-06-20 12:54:46.000000 soda-core-pandas-dask-3.0.41/soda/data_sources/dask_connection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2732 2023-06-20 12:54:46.000000 soda-core-pandas-dask-3.0.41/soda/data_sources/dask_cursor.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13934 2023-06-20 12:54:46.000000 soda-core-pandas-dask-3.0.41/soda/data_sources/dask_data_source.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 12:55:11.126637 soda-core-pandas-dask-3.0.41/soda_core_pandas_dask.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)       66 2023-06-20 12:55:11.000000 soda-core-pandas-dask-3.0.41/soda_core_pandas_dask.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      359 2023-06-20 12:55:11.000000 soda-core-pandas-dask-3.0.41/soda_core_pandas_dask.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-20 12:55:11.000000 soda-core-pandas-dask-3.0.41/soda_core_pandas_dask.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       64 2023-06-20 12:55:11.000000 soda-core-pandas-dask-3.0.41/soda_core_pandas_dask.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-20 12:55:11.000000 soda-core-pandas-dask-3.0.41/soda_core_pandas_dask.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 12:55:11.126637 soda-core-pandas-dask-3.0.41/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      139 2023-06-20 12:54:46.000000 soda-core-pandas-dask-3.0.41/tests/test_dask.py
```

### Comparing `soda-core-pandas-dask-3.0.40/setup.py` & `soda-core-pandas-dask-3.0.41/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 if sys.version_info < (3, 7):
     print("Error: Soda Core requires at least Python 3.7")
     print("Error: Please upgrade your Python version to 3.7 or later")
     sys.exit(1)
 
 package_name = "soda-core-pandas-dask"
-package_version = "3.0.40"
+package_version = "3.0.41"
 description = "Soda Core Dask Package"
 
 requires = [f"soda-core=={package_version}", "dask>=2022.10.0", "dask-sql>=2022.12.0,<2023.6.0"]
 
 setup(
     name=package_name,
     version=package_version,
```

### Comparing `soda-core-pandas-dask-3.0.40/soda/data_sources/dask_cursor.py` & `soda-core-pandas-dask-3.0.41/soda/data_sources/dask_cursor.py`

 * *Files identical despite different names*

### Comparing `soda-core-pandas-dask-3.0.40/soda/data_sources/dask_data_source.py` & `soda-core-pandas-dask-3.0.41/soda/data_sources/dask_data_source.py`

 * *Files identical despite different names*

