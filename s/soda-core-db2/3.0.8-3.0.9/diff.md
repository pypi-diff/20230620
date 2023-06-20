# Comparing `tmp/soda-core-db2-3.0.8.tar.gz` & `tmp/soda-core-db2-3.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soda-core-db2-3.0.8.tar", last modified: Wed Sep 21 19:41:35 2022, max compression
+gzip compressed data, was "soda-core-db2-3.0.9.tar", last modified: Tue Sep 27 20:19:45 2022, max compression
```

## Comparing `soda-core-db2-3.0.8.tar` & `soda-core-db2-3.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 19:41:35.699379 soda-core-db2-3.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-21 19:41:35.699379 soda-core-db2-3.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-21 19:41:35.699379 soda-core-db2-3.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      628 2022-09-21 19:41:14.000000 soda-core-db2-3.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 19:41:35.699379 soda-core-db2-3.0.8/soda/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 19:41:35.699379 soda-core-db2-3.0.8/soda/data_sources/
--rw-r--r--   0 runner    (1001) docker     (121)     5999 2022-09-21 19:41:14.000000 soda-core-db2-3.0.8/soda/data_sources/db2_data_source.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 19:41:35.699379 soda-core-db2-3.0.8/soda_core_db2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-21 19:41:35.000000 soda-core-db2-3.0.8/soda_core_db2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      229 2022-09-21 19:41:35.000000 soda-core-db2-3.0.8/soda_core_db2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-21 19:41:35.000000 soda-core-db2-3.0.8/soda_core_db2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       31 2022-09-21 19:41:35.000000 soda-core-db2-3.0.8/soda_core_db2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-09-21 19:41:35.000000 soda-core-db2-3.0.8/soda_core_db2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 20:19:45.547872 soda-core-db2-3.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-27 20:19:45.547872 soda-core-db2-3.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-27 20:19:45.547872 soda-core-db2-3.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      628 2022-09-27 20:19:27.000000 soda-core-db2-3.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 20:19:45.547872 soda-core-db2-3.0.9/soda/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 20:19:45.547872 soda-core-db2-3.0.9/soda/data_sources/
+-rw-r--r--   0 runner    (1001) docker     (121)     5999 2022-09-27 20:19:27.000000 soda-core-db2-3.0.9/soda/data_sources/db2_data_source.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 20:19:45.547872 soda-core-db2-3.0.9/soda_core_db2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-27 20:19:45.000000 soda-core-db2-3.0.9/soda_core_db2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      229 2022-09-27 20:19:45.000000 soda-core-db2-3.0.9/soda_core_db2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-27 20:19:45.000000 soda-core-db2-3.0.9/soda_core_db2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       31 2022-09-27 20:19:45.000000 soda-core-db2-3.0.9/soda_core_db2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        5 2022-09-27 20:19:45.000000 soda-core-db2-3.0.9/soda_core_db2.egg-info/top_level.txt
```

### Comparing `soda-core-db2-3.0.8/setup.py` & `soda-core-db2-3.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 if sys.version_info < (3, 7):
     print("Error: Soda SQL requires at least Python 3.7")
     print("Error: Please upgrade your Python version to 3.7 or later")
     sys.exit(1)
 
 package_name = "soda-core-db2"
-package_version = "3.0.8"
+package_version = "3.0.9"
 # TODO Add proper description
 description = "Soda Core IBM DB2 Package"
 
 requires = [f"soda-core=={package_version}", "ibm-db==3.1.2"]
 # TODO Fix the params
 setup(
     name=package_name,
```

### Comparing `soda-core-db2-3.0.8/soda/data_sources/db2_data_source.py` & `soda-core-db2-3.0.9/soda/data_sources/db2_data_source.py`

 * *Files identical despite different names*

