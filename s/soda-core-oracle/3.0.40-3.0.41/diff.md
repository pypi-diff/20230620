# Comparing `tmp/soda-core-oracle-3.0.40.tar.gz` & `tmp/soda-core-oracle-3.0.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soda-core-oracle-3.0.40.tar", last modified: Fri Jun 16 08:29:27 2023, max compression
+gzip compressed data, was "soda-core-oracle-3.0.41.tar", last modified: Tue Jun 20 12:55:31 2023, max compression
```

## Comparing `soda-core-oracle-3.0.40.tar` & `soda-core-oracle-3.0.41.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 08:29:27.866747 soda-core-oracle-3.0.40/
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-06-16 08:29:27.866747 soda-core-oracle-3.0.40/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-16 08:29:27.866747 soda-core-oracle-3.0.40/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      634 2023-06-16 08:28:48.000000 soda-core-oracle-3.0.40/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 08:29:27.862747 soda-core-oracle-3.0.40/soda/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 08:29:27.862747 soda-core-oracle-3.0.40/soda/data_sources/
--rw-r--r--   0 runner    (1001) docker     (122)     9209 2023-06-16 08:28:48.000000 soda-core-oracle-3.0.40/soda/data_sources/oracle_data_source.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 08:29:27.866747 soda-core-oracle-3.0.40/soda_core_oracle.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-06-16 08:29:27.000000 soda-core-oracle-3.0.40/soda_core_oracle.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      247 2023-06-16 08:29:27.000000 soda-core-oracle-3.0.40/soda_core_oracle.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-16 08:29:27.000000 soda-core-oracle-3.0.40/soda_core_oracle.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       34 2023-06-16 08:29:27.000000 soda-core-oracle-3.0.40/soda_core_oracle.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-16 08:29:27.000000 soda-core-oracle-3.0.40/soda_core_oracle.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 12:55:31.583011 soda-core-oracle-3.0.41/
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-06-20 12:55:31.579011 soda-core-oracle-3.0.41/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-20 12:55:31.583011 soda-core-oracle-3.0.41/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      634 2023-06-20 12:54:46.000000 soda-core-oracle-3.0.41/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 12:55:31.579011 soda-core-oracle-3.0.41/soda/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 12:55:31.579011 soda-core-oracle-3.0.41/soda/data_sources/
+-rw-r--r--   0 runner    (1001) docker     (122)     9209 2023-06-20 12:54:46.000000 soda-core-oracle-3.0.41/soda/data_sources/oracle_data_source.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 12:55:31.579011 soda-core-oracle-3.0.41/soda_core_oracle.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-06-20 12:55:31.000000 soda-core-oracle-3.0.41/soda_core_oracle.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-06-20 12:55:31.000000 soda-core-oracle-3.0.41/soda_core_oracle.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-20 12:55:31.000000 soda-core-oracle-3.0.41/soda_core_oracle.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       34 2023-06-20 12:55:31.000000 soda-core-oracle-3.0.41/soda_core_oracle.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-20 12:55:31.000000 soda-core-oracle-3.0.41/soda_core_oracle.egg-info/top_level.txt
```

### Comparing `soda-core-oracle-3.0.40/setup.py` & `soda-core-oracle-3.0.41/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 if sys.version_info < (3, 7):
     print("Error: Soda Core requires at least Python 3.7")
     print("Error: Please upgrade your Python version to 3.7 or later")
     sys.exit(1)
 
 package_name = "soda-core-oracle"
-package_version = "3.0.40"
+package_version = "3.0.41"
 # TODO Add proper description
 description = "Soda Core Oracle Package"
 
 requires = [f"soda-core=={package_version}", "oracledb==1.1.1"]
 # TODO Fix the params
 setup(
     name=package_name,
```

### Comparing `soda-core-oracle-3.0.40/soda/data_sources/oracle_data_source.py` & `soda-core-oracle-3.0.41/soda/data_sources/oracle_data_source.py`

 * *Files identical despite different names*

