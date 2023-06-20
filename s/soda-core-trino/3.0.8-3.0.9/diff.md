# Comparing `tmp/soda-core-trino-3.0.8.tar.gz` & `tmp/soda-core-trino-3.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soda-core-trino-3.0.8.tar", last modified: Wed Sep 21 19:42:08 2022, max compression
+gzip compressed data, was "soda-core-trino-3.0.9.tar", last modified: Tue Sep 27 20:20:17 2022, max compression
```

## Comparing `soda-core-trino-3.0.8.tar` & `soda-core-trino-3.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 19:42:08.451365 soda-core-trino-3.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)       59 2022-09-21 19:42:08.451365 soda-core-trino-3.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-21 19:42:08.451365 soda-core-trino-3.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      579 2022-09-21 19:41:14.000000 soda-core-trino-3.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 19:42:08.447365 soda-core-trino-3.0.8/soda/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 19:42:08.447365 soda-core-trino-3.0.8/soda/data_sources/
--rw-r--r--   0 runner    (1001) docker     (121)     4154 2022-09-21 19:41:14.000000 soda-core-trino-3.0.8/soda/data_sources/trino_data_source.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 19:42:08.451365 soda-core-trino-3.0.8/soda_core_trino.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)       59 2022-09-21 19:42:08.000000 soda-core-trino-3.0.8/soda_core_trino.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      241 2022-09-21 19:42:08.000000 soda-core-trino-3.0.8/soda_core_trino.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-21 19:42:08.000000 soda-core-trino-3.0.8/soda_core_trino.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-09-21 19:42:08.000000 soda-core-trino-3.0.8/soda_core_trino.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-09-21 19:42:08.000000 soda-core-trino-3.0.8/soda_core_trino.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 20:20:17.460311 soda-core-trino-3.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)       59 2022-09-27 20:20:17.456311 soda-core-trino-3.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-27 20:20:17.460311 soda-core-trino-3.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      579 2022-09-27 20:19:27.000000 soda-core-trino-3.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 20:20:17.456311 soda-core-trino-3.0.9/soda/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 20:20:17.456311 soda-core-trino-3.0.9/soda/data_sources/
+-rw-r--r--   0 runner    (1001) docker     (121)     4154 2022-09-27 20:19:27.000000 soda-core-trino-3.0.9/soda/data_sources/trino_data_source.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 20:20:17.456311 soda-core-trino-3.0.9/soda_core_trino.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)       59 2022-09-27 20:20:17.000000 soda-core-trino-3.0.9/soda_core_trino.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      241 2022-09-27 20:20:17.000000 soda-core-trino-3.0.9/soda_core_trino.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-27 20:20:17.000000 soda-core-trino-3.0.9/soda_core_trino.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       32 2022-09-27 20:20:17.000000 soda-core-trino-3.0.9/soda_core_trino.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        5 2022-09-27 20:20:17.000000 soda-core-trino-3.0.9/soda_core_trino.egg-info/top_level.txt
```

### Comparing `soda-core-trino-3.0.8/setup.py` & `soda-core-trino-3.0.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 if sys.version_info < (3, 7):
     print("Error: Soda Core requires at least Python 3.7")
     print("Error: Please upgrade your Python version to 3.7 or later")
     sys.exit(1)
 
 package_name = "soda-core-trino"
-package_version = "3.0.8"
+package_version = "3.0.9"
 description = "Soda Core Trino Package"
 
 requires = [f"soda-core=={package_version}", "trino>=0.315.0"]
 
 setup(
     name=package_name,
     version=package_version,
```

### Comparing `soda-core-trino-3.0.8/soda/data_sources/trino_data_source.py` & `soda-core-trino-3.0.9/soda/data_sources/trino_data_source.py`

 * *Files identical despite different names*

