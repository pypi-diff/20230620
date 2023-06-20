# Comparing `tmp/soda-core-snowflake-3.0.8.tar.gz` & `tmp/soda-core-snowflake-3.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soda-core-snowflake-3.0.8.tar", last modified: Wed Sep 21 19:41:55 2022, max compression
+gzip compressed data, was "soda-core-snowflake-3.0.9.tar", last modified: Tue Sep 27 20:20:06 2022, max compression
```

## Comparing `soda-core-snowflake-3.0.8.tar` & `soda-core-snowflake-3.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 19:41:55.667367 soda-core-snowflake-3.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-09-21 19:41:55.667367 soda-core-snowflake-3.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-21 19:41:55.667367 soda-core-snowflake-3.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      743 2022-09-21 19:41:14.000000 soda-core-snowflake-3.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 19:41:55.667367 soda-core-snowflake-3.0.8/soda/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 19:41:55.667367 soda-core-snowflake-3.0.8/soda/data_sources/
--rw-r--r--   0 runner    (1001) docker     (121)     7998 2022-09-21 19:41:14.000000 soda-core-snowflake-3.0.8/soda/data_sources/snowflake_data_source.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 19:41:55.667367 soda-core-snowflake-3.0.8/soda_core_snowflake.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-09-21 19:41:55.000000 soda-core-snowflake-3.0.8/soda_core_snowflake.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      265 2022-09-21 19:41:55.000000 soda-core-snowflake-3.0.8/soda_core_snowflake.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-21 19:41:55.000000 soda-core-snowflake-3.0.8/soda_core_snowflake.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-09-21 19:41:55.000000 soda-core-snowflake-3.0.8/soda_core_snowflake.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-09-21 19:41:55.000000 soda-core-snowflake-3.0.8/soda_core_snowflake.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 20:20:06.020156 soda-core-snowflake-3.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)       63 2022-09-27 20:20:06.020156 soda-core-snowflake-3.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-27 20:20:06.020156 soda-core-snowflake-3.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      743 2022-09-27 20:19:27.000000 soda-core-snowflake-3.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 20:20:06.020156 soda-core-snowflake-3.0.9/soda/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 20:20:06.020156 soda-core-snowflake-3.0.9/soda/data_sources/
+-rw-r--r--   0 runner    (1001) docker     (121)     7998 2022-09-27 20:19:27.000000 soda-core-snowflake-3.0.9/soda/data_sources/snowflake_data_source.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 20:20:06.020156 soda-core-snowflake-3.0.9/soda_core_snowflake.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)       63 2022-09-27 20:20:05.000000 soda-core-snowflake-3.0.9/soda_core_snowflake.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      265 2022-09-27 20:20:05.000000 soda-core-snowflake-3.0.9/soda_core_snowflake.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-27 20:20:05.000000 soda-core-snowflake-3.0.9/soda_core_snowflake.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       74 2022-09-27 20:20:05.000000 soda-core-snowflake-3.0.9/soda_core_snowflake.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        5 2022-09-27 20:20:05.000000 soda-core-snowflake-3.0.9/soda_core_snowflake.egg-info/top_level.txt
```

### Comparing `soda-core-snowflake-3.0.8/setup.py` & `soda-core-snowflake-3.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 if sys.version_info < (3, 7):
     print("Error: Soda SQL requires at least Python 3.7")
     print("Error: Please upgrade your Python version to 3.7 or later")
     sys.exit(1)
 
 package_name = "soda-core-snowflake"
-package_version = "3.0.8"
+package_version = "3.0.9"
 description = "Soda Core Snowflake Package"
 
 requires = [
     f"soda-core=={package_version}",
     "snowflake-connector-python~=2.7",
     # https://github.com/snowflakedb/snowflake-connector-python/issues/1206
     "typing-extensions>=4.3.0",
```

### Comparing `soda-core-snowflake-3.0.8/soda/data_sources/snowflake_data_source.py` & `soda-core-snowflake-3.0.9/soda/data_sources/snowflake_data_source.py`

 * *Files identical despite different names*

