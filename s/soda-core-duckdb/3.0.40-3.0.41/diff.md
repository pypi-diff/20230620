# Comparing `tmp/soda-core-duckdb-3.0.40.tar.gz` & `tmp/soda-core-duckdb-3.0.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soda-core-duckdb-3.0.40.tar", last modified: Fri Jun 16 08:29:22 2023, max compression
+gzip compressed data, was "soda-core-duckdb-3.0.41.tar", last modified: Tue Jun 20 12:55:25 2023, max compression
```

## Comparing `soda-core-duckdb-3.0.40.tar` & `soda-core-duckdb-3.0.41.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 08:29:22.230732 soda-core-duckdb-3.0.40/
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-06-16 08:29:22.230732 soda-core-duckdb-3.0.40/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-16 08:29:22.230732 soda-core-duckdb-3.0.40/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      579 2023-06-16 08:28:48.000000 soda-core-duckdb-3.0.40/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 08:29:22.230732 soda-core-duckdb-3.0.40/soda/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 08:29:22.230732 soda-core-duckdb-3.0.40/soda/data_sources/
--rw-r--r--   0 runner    (1001) docker     (122)     5504 2023-06-16 08:28:48.000000 soda-core-duckdb-3.0.40/soda/data_sources/duckdb_data_source.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 08:29:22.230732 soda-core-duckdb-3.0.40/soda_core_duckdb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-06-16 08:29:22.000000 soda-core-duckdb-3.0.40/soda_core_duckdb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      268 2023-06-16 08:29:22.000000 soda-core-duckdb-3.0.40/soda_core_duckdb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-16 08:29:22.000000 soda-core-duckdb-3.0.40/soda_core_duckdb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-06-16 08:29:22.000000 soda-core-duckdb-3.0.40/soda_core_duckdb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-16 08:29:22.000000 soda-core-duckdb-3.0.40/soda_core_duckdb.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 08:29:22.230732 soda-core-duckdb-3.0.40/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      690 2023-06-16 08:28:48.000000 soda-core-duckdb-3.0.40/tests/test_duckdb.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 12:55:25.786903 soda-core-duckdb-3.0.41/
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-06-20 12:55:25.786903 soda-core-duckdb-3.0.41/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-20 12:55:25.786903 soda-core-duckdb-3.0.41/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      579 2023-06-20 12:54:46.000000 soda-core-duckdb-3.0.41/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 12:55:25.786903 soda-core-duckdb-3.0.41/soda/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 12:55:25.786903 soda-core-duckdb-3.0.41/soda/data_sources/
+-rw-r--r--   0 runner    (1001) docker     (122)     5504 2023-06-20 12:54:46.000000 soda-core-duckdb-3.0.41/soda/data_sources/duckdb_data_source.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 12:55:25.786903 soda-core-duckdb-3.0.41/soda_core_duckdb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-06-20 12:55:25.000000 soda-core-duckdb-3.0.41/soda_core_duckdb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      268 2023-06-20 12:55:25.000000 soda-core-duckdb-3.0.41/soda_core_duckdb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-20 12:55:25.000000 soda-core-duckdb-3.0.41/soda_core_duckdb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-06-20 12:55:25.000000 soda-core-duckdb-3.0.41/soda_core_duckdb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-20 12:55:25.000000 soda-core-duckdb-3.0.41/soda_core_duckdb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 12:55:25.786903 soda-core-duckdb-3.0.41/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      690 2023-06-20 12:54:46.000000 soda-core-duckdb-3.0.41/tests/test_duckdb.py
```

### Comparing `soda-core-duckdb-3.0.40/setup.py` & `soda-core-duckdb-3.0.41/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 if sys.version_info < (3, 7):
     print("Error: Soda Core requires at least Python 3.7")
     print("Error: Please upgrade your Python version to 3.7 or later")
     sys.exit(1)
 
 package_name = "soda-core-duckdb"
-package_version = "3.0.40"
+package_version = "3.0.41"
 description = "Soda Core Duckdb Package"
 
 requires = [f"soda-core=={package_version}", "duckdb<=0.8"]
 
 setup(
     name=package_name,
     version=package_version,
```

### Comparing `soda-core-duckdb-3.0.40/soda/data_sources/duckdb_data_source.py` & `soda-core-duckdb-3.0.41/soda/data_sources/duckdb_data_source.py`

 * *Files identical despite different names*

### Comparing `soda-core-duckdb-3.0.40/tests/test_duckdb.py` & `soda-core-duckdb-3.0.41/tests/test_duckdb.py`

 * *Files identical despite different names*

