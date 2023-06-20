# Comparing `tmp/mlpype-spark-0.4.0.tar.gz` & `tmp/mlpype-spark-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlpype-spark-0.4.0.tar", last modified: Fri May  5 10:37:53 2023, max compression
+gzip compressed data, was "mlpype-spark-0.4.1.tar", last modified: Tue Jun 20 16:47:32 2023, max compression
```

## Comparing `mlpype-spark-0.4.0.tar` & `mlpype-spark-0.4.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 vandejer (1865779777) 296108113        0 2023-05-05 10:37:53.344511 mlpype-spark-0.4.0/
--rw-r--r--   0 vandejer (1865779777) 296108113      120 2023-05-05 10:37:53.344225 mlpype-spark-0.4.0/PKG-INFO
-drwxr-xr-x   0 vandejer (1865779777) 296108113        0 2023-05-05 10:37:53.343803 mlpype-spark-0.4.0/mlpype_spark.egg-info/
--rw-r--r--   0 vandejer (1865779777) 296108113      120 2023-05-05 10:37:53.000000 mlpype-spark-0.4.0/mlpype_spark.egg-info/PKG-INFO
--rw-r--r--   0 vandejer (1865779777) 296108113      187 2023-05-05 10:37:53.000000 mlpype-spark-0.4.0/mlpype_spark.egg-info/SOURCES.txt
--rw-r--r--   0 vandejer (1865779777) 296108113        1 2023-05-05 10:37:53.000000 mlpype-spark-0.4.0/mlpype_spark.egg-info/dependency_links.txt
--rw-r--r--   0 vandejer (1865779777) 296108113      175 2023-05-05 10:37:53.000000 mlpype-spark-0.4.0/mlpype_spark.egg-info/requires.txt
--rw-r--r--   0 vandejer (1865779777) 296108113        1 2023-05-05 10:37:53.000000 mlpype-spark-0.4.0/mlpype_spark.egg-info/top_level.txt
--rw-r--r--   0 vandejer (1865779777) 296108113       38 2023-05-05 10:37:53.344580 mlpype-spark-0.4.0/setup.cfg
--rw-r--r--   0 vandejer (1865779777) 296108113      715 2023-05-05 10:18:55.000000 mlpype-spark-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:47:32.652465 mlpype-spark-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-20 16:47:32.648465 mlpype-spark-0.4.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:47:32.648465 mlpype-spark-0.4.1/mlpype_spark.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-20 16:47:32.000000 mlpype-spark-0.4.1/mlpype_spark.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-20 16:47:32.000000 mlpype-spark-0.4.1/mlpype_spark.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 16:47:32.000000 mlpype-spark-0.4.1/mlpype_spark.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-20 16:47:32.000000 mlpype-spark-0.4.1/mlpype_spark.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 16:47:32.000000 mlpype-spark-0.4.1/mlpype_spark.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 16:47:32.652465 mlpype-spark-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-20 16:43:35.000000 mlpype-spark-0.4.1/setup.py
```

### Comparing `mlpype-spark-0.4.0/setup.py` & `mlpype-spark-0.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import find_namespace_packages, setup
 
 if __name__ == "__main__":
-    version = "0.4.0"
+    version = "0.4.1"
 
     deps = [
         f"mlpype-base=={version}",
         # We will provide absolute no guarantees that our integration will work with
         # EVERY version of pyspark. This has been developed under pyspark==3.2.1.
         "pyspark>=3.2.1",
     ]
```

