# Comparing `tmp/soda-core-bigquery-3.0.8.tar.gz` & `tmp/soda-core-bigquery-3.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soda-core-bigquery-3.0.8.tar", last modified: Wed Sep 21 19:41:27 2022, max compression
+gzip compressed data, was "soda-core-bigquery-3.0.9.tar", last modified: Tue Sep 27 20:19:38 2022, max compression
```

## Comparing `soda-core-bigquery-3.0.8.tar` & `soda-core-bigquery-3.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 19:41:27.955378 soda-core-bigquery-3.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-09-21 19:41:27.955378 soda-core-bigquery-3.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-21 19:41:27.955378 soda-core-bigquery-3.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      637 2022-09-21 19:41:14.000000 soda-core-bigquery-3.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 19:41:27.951378 soda-core-bigquery-3.0.8/soda/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 19:41:27.951378 soda-core-bigquery-3.0.8/soda/data_sources/
--rw-r--r--   0 runner    (1001) docker     (121)     9019 2022-09-21 19:41:14.000000 soda-core-bigquery-3.0.8/soda/data_sources/bigquery_data_source.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 19:41:27.951378 soda-core-bigquery-3.0.8/soda_core_bigquery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-09-21 19:41:27.000000 soda-core-bigquery-3.0.8/soda_core_bigquery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      259 2022-09-21 19:41:27.000000 soda-core-bigquery-3.0.8/soda_core_bigquery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-21 19:41:27.000000 soda-core-bigquery-3.0.8/soda_core_bigquery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       52 2022-09-21 19:41:27.000000 soda-core-bigquery-3.0.8/soda_core_bigquery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-09-21 19:41:27.000000 soda-core-bigquery-3.0.8/soda_core_bigquery.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 20:19:38.667763 soda-core-bigquery-3.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)       62 2022-09-27 20:19:38.667763 soda-core-bigquery-3.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-27 20:19:38.667763 soda-core-bigquery-3.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      637 2022-09-27 20:19:27.000000 soda-core-bigquery-3.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 20:19:38.667763 soda-core-bigquery-3.0.9/soda/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 20:19:38.667763 soda-core-bigquery-3.0.9/soda/data_sources/
+-rw-r--r--   0 runner    (1001) docker     (121)     9324 2022-09-27 20:19:27.000000 soda-core-bigquery-3.0.9/soda/data_sources/bigquery_data_source.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 20:19:38.667763 soda-core-bigquery-3.0.9/soda_core_bigquery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)       62 2022-09-27 20:19:38.000000 soda-core-bigquery-3.0.9/soda_core_bigquery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      259 2022-09-27 20:19:38.000000 soda-core-bigquery-3.0.9/soda_core_bigquery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-27 20:19:38.000000 soda-core-bigquery-3.0.9/soda_core_bigquery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       52 2022-09-27 20:19:38.000000 soda-core-bigquery-3.0.9/soda_core_bigquery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        5 2022-09-27 20:19:38.000000 soda-core-bigquery-3.0.9/soda_core_bigquery.egg-info/top_level.txt
```

### Comparing `soda-core-bigquery-3.0.8/setup.py` & `soda-core-bigquery-3.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 if sys.version_info < (3, 7):
     print("Error: Soda SQL requires at least Python 3.7")
     print("Error: Please upgrade your Python version to 3.7 or later")
     sys.exit(1)
 
 package_name = "soda-core-bigquery"
-package_version = "3.0.8"
+package_version = "3.0.9"
 description = "Soda Core Bigquery Package"
 
 requires = [
     f"soda-core=={package_version}",
     "google-cloud-bigquery>=2.25.0, <3.0",
 ]
 # TODO Fix the params
```

### Comparing `soda-core-bigquery-3.0.8/soda/data_sources/bigquery_data_source.py` & `soda-core-bigquery-3.0.9/soda/data_sources/bigquery_data_source.py`

 * *Files 4% similar despite different names*

```diff
@@ -117,21 +117,27 @@
         # Set schema and table prefix to the same value as dataset, we need one attribute to access this value as it's used in building sql statements.
         self.update_schema(self.dataset)
 
         self.location = data_source_properties.get("location")
         self.client_info = data_source_properties.get("client_info")
         self.client_options = data_source_properties.get("client_options")
 
+        # Allow to separate default dataset location from compute (project_id).
+        self.storage_project_id = self.project_id
+        storage_project_id = data_source_properties.get("storage_project_id")
+        if storage_project_id:
+            self.storage_project_id = storage_project_id
+
     def connect(self):
         try:
             self.client = bigquery.Client(
                 project=self.project_id,
                 credentials=self.credentials,
                 default_query_job_config=bigquery.QueryJobConfig(
-                    default_dataset=f"{self.project_id}.{self.dataset}",
+                    default_dataset=f"{self.storage_project_id}.{self.dataset}",
                 ),
                 location=self.location,
                 client_info=self.client_info,
                 client_options=self.client_options,
             )
             self.connection = dbapi.Connection(self.client)
```

