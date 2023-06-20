# Comparing `tmp/abi_ds_utils-1.0.2.tar.gz` & `tmp/abi_ds_utils-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abi_ds_utils-1.0.2.tar", max compression
+gzip compressed data, was "abi_ds_utils-1.1.0.tar", max compression
```

## Comparing `abi_ds_utils-1.0.2.tar` & `abi_ds_utils-1.1.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      255 2023-06-19 10:34:08.513948 abi_ds_utils-1.0.2/abi_ds_utils/__init__.py
--rw-r--r--   0        0        0      823 2023-06-19 10:34:08.514948 abi_ds_utils-1.0.2/abi_ds_utils/airflow.py
--rw-r--r--   0        0        0     1737 2023-06-19 10:34:08.514948 abi_ds_utils-1.0.2/abi_ds_utils/aws.py
--rw-r--r--   0        0        0     1356 2023-06-19 10:34:08.514948 abi_ds_utils-1.0.2/abi_ds_utils/spark.py
--rw-r--r--   0        0        0      433 2023-06-19 10:34:08.514948 abi_ds_utils-1.0.2/pyproject.toml
--rw-r--r--   0        0        0      688 2023-06-19 10:34:57.921640 abi_ds_utils-1.0.2/setup.py
--rw-r--r--   0        0        0      561 2023-06-19 10:34:57.921887 abi_ds_utils-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0      255 2023-06-20 09:44:47.141021 abi_ds_utils-1.1.0/abi_ds_utils/__init__.py
+-rw-r--r--   0        0        0      823 2023-06-20 09:44:47.141021 abi_ds_utils-1.1.0/abi_ds_utils/airflow.py
+-rw-r--r--   0        0        0     1737 2023-06-20 09:44:47.141021 abi_ds_utils-1.1.0/abi_ds_utils/aws.py
+-rw-r--r--   0        0        0     1356 2023-06-20 09:44:47.141021 abi_ds_utils-1.1.0/abi_ds_utils/spark.py
+-rw-r--r--   0        0        0      433 2023-06-20 09:44:47.142021 abi_ds_utils-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      688 2023-06-20 09:45:42.098485 abi_ds_utils-1.1.0/setup.py
+-rw-r--r--   0        0        0      561 2023-06-20 09:45:42.098746 abi_ds_utils-1.1.0/PKG-INFO
```

### Comparing `abi_ds_utils-1.0.2/abi_ds_utils/airflow.py` & `abi_ds_utils-1.1.0/abi_ds_utils/airflow.py`

 * *Files identical despite different names*

### Comparing `abi_ds_utils-1.0.2/abi_ds_utils/aws.py` & `abi_ds_utils-1.1.0/abi_ds_utils/aws.py`

 * *Files identical despite different names*

### Comparing `abi_ds_utils-1.0.2/abi_ds_utils/spark.py` & `abi_ds_utils-1.1.0/abi_ds_utils/spark.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         .config("spark.driver.memory", driver_memory)
         .config("spark.dynamicAllocation.enabled", "true")
 
         # PyArrow for dtypes conversions
         .config("spark.sql.execution.arrow.pyspark.enabled", "true")
 
         # Jars compatible with the base-notebook image (Python 3.8, PySpark 3.3.2)
-        .config('spark.jars.packages', 'org.apache.hadoop:hadoop-aws:3.3.2,io.delta:delta-core_2.13:2.2.0')
+        .config('spark.jars.packages', 'org.apache.hadoop:hadoop-aws:3.3.2,io.delta:delta-core_2.12:2.2.0')
 
         # Delta Lake setup
         .config("spark.hadoop.fs.s3a.connection.maximum", 128)
         .config("spark.sql.extensions", "io.delta.sql.DeltaSparkSessionExtension")
         .config("spark.sql.catalog.spark_catalog", "org.apache.spark.sql.delta.catalog.DeltaCatalog")
         .config("spark.delta.logStore.class", "org.apache.spark.sql.delta.storage.S3SingleDriverLogStore")
     )
```

### Comparing `abi_ds_utils-1.0.2/setup.py` & `abi_ds_utils-1.1.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['boto3>=1.21.14,<2.0.0', 'pyarrow>=7.0.0,<8.0.0', 'pyspark==3.3.2']
 
 setup_kwargs = {
     'name': 'abi-ds-utils',
-    'version': '1.0.2',
+    'version': '1.1.0',
     'description': 'Utility modules for working with spark, containers, aws and more.',
     'long_description': None,
     'author': 'Martin Matousek',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `abi_ds_utils-1.0.2/PKG-INFO` & `abi_ds_utils-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abi-ds-utils
-Version: 1.0.2
+Version: 1.1.0
 Summary: Utility modules for working with spark, containers, aws and more.
 License: Private
 Author: Martin Matousek
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

