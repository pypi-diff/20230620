# Comparing `tmp/soda-core-spark-df-3.0.8.tar.gz` & `tmp/soda-core-spark-df-3.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soda-core-spark-df-3.0.8.tar", last modified: Wed Sep 21 19:42:01 2022, max compression
+gzip compressed data, was "soda-core-spark-df-3.0.9.tar", last modified: Tue Sep 27 20:20:11 2022, max compression
```

## Comparing `soda-core-spark-df-3.0.8.tar` & `soda-core-spark-df-3.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 19:42:01.767367 soda-core-spark-df-3.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-09-21 19:42:01.767367 soda-core-spark-df-3.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-21 19:42:01.767367 soda-core-spark-df-3.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      622 2022-09-21 19:41:14.000000 soda-core-spark-df-3.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 19:42:01.763367 soda-core-spark-df-3.0.8/soda/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 19:42:01.767367 soda-core-spark-df-3.0.8/soda/data_sources/
--rw-r--r--   0 runner    (1001) docker     (121)      426 2022-09-21 19:41:14.000000 soda-core-spark-df-3.0.8/soda/data_sources/spark_df_connection.py
--rw-r--r--   0 runner    (1001) docker     (121)     1509 2022-09-21 19:41:14.000000 soda-core-spark-df-3.0.8/soda/data_sources/spark_df_cursor.py
--rw-r--r--   0 runner    (1001) docker     (121)     1751 2022-09-21 19:41:14.000000 soda-core-spark-df-3.0.8/soda/data_sources/spark_df_data_source.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 19:42:01.767367 soda-core-spark-df-3.0.8/soda_core_spark_df.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-09-21 19:42:01.000000 soda-core-spark-df-3.0.8/soda_core_spark_df.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      337 2022-09-21 19:42:01.000000 soda-core-spark-df-3.0.8/soda_core_spark_df.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-21 19:42:01.000000 soda-core-spark-df-3.0.8/soda_core_spark_df.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       31 2022-09-21 19:42:01.000000 soda-core-spark-df-3.0.8/soda_core_spark_df.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-09-21 19:42:01.000000 soda-core-spark-df-3.0.8/soda_core_spark_df.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 20:20:11.836235 soda-core-spark-df-3.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)       62 2022-09-27 20:20:11.836235 soda-core-spark-df-3.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-27 20:20:11.836235 soda-core-spark-df-3.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      622 2022-09-27 20:19:27.000000 soda-core-spark-df-3.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 20:20:11.832235 soda-core-spark-df-3.0.9/soda/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 20:20:11.836235 soda-core-spark-df-3.0.9/soda/data_sources/
+-rw-r--r--   0 runner    (1001) docker     (121)      426 2022-09-27 20:19:27.000000 soda-core-spark-df-3.0.9/soda/data_sources/spark_df_connection.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1509 2022-09-27 20:19:27.000000 soda-core-spark-df-3.0.9/soda/data_sources/spark_df_cursor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1751 2022-09-27 20:19:27.000000 soda-core-spark-df-3.0.9/soda/data_sources/spark_df_data_source.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 20:20:11.836235 soda-core-spark-df-3.0.9/soda_core_spark_df.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)       62 2022-09-27 20:20:11.000000 soda-core-spark-df-3.0.9/soda_core_spark_df.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      337 2022-09-27 20:20:11.000000 soda-core-spark-df-3.0.9/soda_core_spark_df.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-27 20:20:11.000000 soda-core-spark-df-3.0.9/soda_core_spark_df.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       31 2022-09-27 20:20:11.000000 soda-core-spark-df-3.0.9/soda_core_spark_df.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        5 2022-09-27 20:20:11.000000 soda-core-spark-df-3.0.9/soda_core_spark_df.egg-info/top_level.txt
```

### Comparing `soda-core-spark-df-3.0.8/setup.py` & `soda-core-spark-df-3.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 if sys.version_info < (3, 7):
     print("Error: Soda SQL requires at least Python 3.7")
     print("Error: Please upgrade your Python version to 3.7 or later")
     sys.exit(1)
 
 package_name = "soda-core-spark-df"
-package_version = "3.0.8"
+package_version = "3.0.9"
 description = "Soda Core Spark Dataframe Package"
 
 requires = [
     f"soda-core-spark=={package_version}",
     "pyspark",
 ]
 # TODO Fix the params
```

### Comparing `soda-core-spark-df-3.0.8/soda/data_sources/spark_df_cursor.py` & `soda-core-spark-df-3.0.9/soda/data_sources/spark_df_cursor.py`

 * *Files identical despite different names*

### Comparing `soda-core-spark-df-3.0.8/soda/data_sources/spark_df_data_source.py` & `soda-core-spark-df-3.0.9/soda/data_sources/spark_df_data_source.py`

 * *Files identical despite different names*

