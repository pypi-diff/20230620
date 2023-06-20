# Comparing `tmp/soda-core-spark-3.0.8.tar.gz` & `tmp/soda-core-spark-3.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soda-core-spark-3.0.8.tar", last modified: Wed Sep 21 19:41:58 2022, max compression
+gzip compressed data, was "soda-core-spark-3.0.9.tar", last modified: Tue Sep 27 20:20:09 2022, max compression
```

## Comparing `soda-core-spark-3.0.8.tar` & `soda-core-spark-3.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 19:41:58.703367 soda-core-spark-3.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)      128 2022-09-21 19:41:58.703367 soda-core-spark-3.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-21 19:41:58.703367 soda-core-spark-3.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      754 2022-09-21 19:41:14.000000 soda-core-spark-3.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 19:41:58.699367 soda-core-spark-3.0.8/soda/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 19:41:58.699367 soda-core-spark-3.0.8/soda/data_sources/
--rw-r--r--   0 runner    (1001) docker     (121)    12166 2022-09-21 19:41:14.000000 soda-core-spark-3.0.8/soda/data_sources/spark_data_source.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 19:41:58.703367 soda-core-spark-3.0.8/soda_core_spark.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      128 2022-09-21 19:41:58.000000 soda-core-spark-3.0.8/soda_core_spark.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      241 2022-09-21 19:41:58.000000 soda-core-spark-3.0.8/soda_core_spark.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-21 19:41:58.000000 soda-core-spark-3.0.8/soda_core_spark.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       92 2022-09-21 19:41:58.000000 soda-core-spark-3.0.8/soda_core_spark.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-09-21 19:41:58.000000 soda-core-spark-3.0.8/soda_core_spark.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 20:20:09.092201 soda-core-spark-3.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)      128 2022-09-27 20:20:09.092201 soda-core-spark-3.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-27 20:20:09.092201 soda-core-spark-3.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      754 2022-09-27 20:19:27.000000 soda-core-spark-3.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 20:20:09.088201 soda-core-spark-3.0.9/soda/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 20:20:09.088201 soda-core-spark-3.0.9/soda/data_sources/
+-rw-r--r--   0 runner    (1001) docker     (121)    12166 2022-09-27 20:19:27.000000 soda-core-spark-3.0.9/soda/data_sources/spark_data_source.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 20:20:09.092201 soda-core-spark-3.0.9/soda_core_spark.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      128 2022-09-27 20:20:09.000000 soda-core-spark-3.0.9/soda_core_spark.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      241 2022-09-27 20:20:09.000000 soda-core-spark-3.0.9/soda_core_spark.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-27 20:20:09.000000 soda-core-spark-3.0.9/soda_core_spark.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       92 2022-09-27 20:20:09.000000 soda-core-spark-3.0.9/soda_core_spark.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        5 2022-09-27 20:20:09.000000 soda-core-spark-3.0.9/soda_core_spark.egg-info/top_level.txt
```

### Comparing `soda-core-spark-3.0.8/setup.py` & `soda-core-spark-3.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 if sys.version_info < (3, 7):
     print("Error: Soda SQL requires at least Python 3.7")
     print("Error: Please upgrade your Python version to 3.7 or later")
     sys.exit(1)
 
 package_name = "soda-core-spark"
-package_version = "3.0.8"
+package_version = "3.0.9"
 description = "Soda Core Spark Package"
 
 requires = [f"soda-core=={package_version}"]
 
 extras = {
     "hive": [
         "PyHive[hive]",
```

### Comparing `soda-core-spark-3.0.8/soda/data_sources/spark_data_source.py` & `soda-core-spark-3.0.9/soda/data_sources/spark_data_source.py`

 * *Files identical despite different names*

