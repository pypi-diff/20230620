# Comparing `tmp/soda-core-postgres-3.0.8.tar.gz` & `tmp/soda-core-postgres-3.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soda-core-postgres-3.0.8.tar", last modified: Wed Sep 21 19:41:45 2022, max compression
+gzip compressed data, was "soda-core-postgres-3.0.9.tar", last modified: Tue Sep 27 20:19:54 2022, max compression
```

## Comparing `soda-core-postgres-3.0.8.tar` & `soda-core-postgres-3.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 19:41:45.603369 soda-core-postgres-3.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-09-21 19:41:45.603369 soda-core-postgres-3.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-21 19:41:45.603369 soda-core-postgres-3.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      649 2022-09-21 19:41:14.000000 soda-core-postgres-3.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 19:41:45.599369 soda-core-postgres-3.0.8/soda/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 19:41:45.603369 soda-core-postgres-3.0.8/soda/data_sources/
--rw-r--r--   0 runner    (1001) docker     (121)    15469 2022-09-21 19:41:14.000000 soda-core-postgres-3.0.8/soda/data_sources/postgres_data_source.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 19:41:45.603369 soda-core-postgres-3.0.8/soda_core_postgres.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-09-21 19:41:45.000000 soda-core-postgres-3.0.8/soda_core_postgres.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      259 2022-09-21 19:41:45.000000 soda-core-postgres-3.0.8/soda_core_postgres.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-21 19:41:45.000000 soda-core-postgres-3.0.8/soda_core_postgres.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-09-21 19:41:45.000000 soda-core-postgres-3.0.8/soda_core_postgres.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-09-21 19:41:45.000000 soda-core-postgres-3.0.8/soda_core_postgres.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 20:19:54.955979 soda-core-postgres-3.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)       62 2022-09-27 20:19:54.955979 soda-core-postgres-3.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-27 20:19:54.955979 soda-core-postgres-3.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      649 2022-09-27 20:19:27.000000 soda-core-postgres-3.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 20:19:54.955979 soda-core-postgres-3.0.9/soda/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 20:19:54.955979 soda-core-postgres-3.0.9/soda/data_sources/
+-rw-r--r--   0 runner    (1001) docker     (121)    15469 2022-09-27 20:19:27.000000 soda-core-postgres-3.0.9/soda/data_sources/postgres_data_source.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 20:19:54.955979 soda-core-postgres-3.0.9/soda_core_postgres.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)       62 2022-09-27 20:19:54.000000 soda-core-postgres-3.0.9/soda_core_postgres.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      259 2022-09-27 20:19:54.000000 soda-core-postgres-3.0.9/soda_core_postgres.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-27 20:19:54.000000 soda-core-postgres-3.0.9/soda_core_postgres.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       45 2022-09-27 20:19:54.000000 soda-core-postgres-3.0.9/soda_core_postgres.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        5 2022-09-27 20:19:54.000000 soda-core-postgres-3.0.9/soda_core_postgres.egg-info/top_level.txt
```

### Comparing `soda-core-postgres-3.0.8/setup.py` & `soda-core-postgres-3.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 if sys.version_info < (3, 7):
     print("Error: Soda SQL requires at least Python 3.7")
     print("Error: Please upgrade your Python version to 3.7 or later")
     sys.exit(1)
 
 package_name = "soda-core-postgres"
-package_version = "3.0.8"
+package_version = "3.0.9"
 # TODO Add proper description
 description = "Soda Core Postgres Package"
 
 requires = [f"soda-core=={package_version}", "psycopg2-binary>=2.8.5, <3.0"]
 # TODO Fix the params
 setup(
     name=package_name,
```

### Comparing `soda-core-postgres-3.0.8/soda/data_sources/postgres_data_source.py` & `soda-core-postgres-3.0.9/soda/data_sources/postgres_data_source.py`

 * *Files identical despite different names*

