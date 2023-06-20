# Comparing `tmp/soda-core-mysql-3.0.8.tar.gz` & `tmp/soda-core-mysql-3.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soda-core-mysql-3.0.8.tar", last modified: Wed Sep 21 19:41:42 2022, max compression
+gzip compressed data, was "soda-core-mysql-3.0.9.tar", last modified: Tue Sep 27 20:19:51 2022, max compression
```

## Comparing `soda-core-mysql-3.0.8.tar` & `soda-core-mysql-3.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 19:41:42.315369 soda-core-mysql-3.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)       59 2022-09-21 19:41:42.315369 soda-core-mysql-3.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-21 19:41:42.315369 soda-core-mysql-3.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      626 2022-09-21 19:41:14.000000 soda-core-mysql-3.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 19:41:42.311370 soda-core-mysql-3.0.8/soda/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 19:41:42.311370 soda-core-mysql-3.0.8/soda/data_sources/
--rw-r--r--   0 runner    (1001) docker     (121)     4128 2022-09-21 19:41:14.000000 soda-core-mysql-3.0.8/soda/data_sources/mysql_data_source.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 19:41:42.315369 soda-core-mysql-3.0.8/soda_core_mysql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)       59 2022-09-21 19:41:42.000000 soda-core-mysql-3.0.8/soda_core_mysql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      241 2022-09-21 19:41:42.000000 soda-core-mysql-3.0.8/soda_core_mysql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-21 19:41:42.000000 soda-core-mysql-3.0.8/soda_core_mysql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-09-21 19:41:42.000000 soda-core-mysql-3.0.8/soda_core_mysql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-09-21 19:41:42.000000 soda-core-mysql-3.0.8/soda_core_mysql.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 20:19:51.475956 soda-core-mysql-3.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)       59 2022-09-27 20:19:51.475956 soda-core-mysql-3.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-27 20:19:51.475956 soda-core-mysql-3.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      626 2022-09-27 20:19:27.000000 soda-core-mysql-3.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 20:19:51.471955 soda-core-mysql-3.0.9/soda/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 20:19:51.471955 soda-core-mysql-3.0.9/soda/data_sources/
+-rw-r--r--   0 runner    (1001) docker     (121)     4128 2022-09-27 20:19:27.000000 soda-core-mysql-3.0.9/soda/data_sources/mysql_data_source.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 20:19:51.475956 soda-core-mysql-3.0.9/soda_core_mysql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)       59 2022-09-27 20:19:51.000000 soda-core-mysql-3.0.9/soda_core_mysql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      241 2022-09-27 20:19:51.000000 soda-core-mysql-3.0.9/soda_core_mysql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-27 20:19:51.000000 soda-core-mysql-3.0.9/soda_core_mysql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       48 2022-09-27 20:19:51.000000 soda-core-mysql-3.0.9/soda_core_mysql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        5 2022-09-27 20:19:51.000000 soda-core-mysql-3.0.9/soda_core_mysql.egg-info/top_level.txt
```

### Comparing `soda-core-mysql-3.0.8/setup.py` & `soda-core-mysql-3.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 if sys.version_info < (3, 7):
     print("Error: Soda SQL requires at least Python 3.7")
     print("Error: Please upgrade your Python version to 3.7 or later")
     sys.exit(1)
 
 package_name = "soda-core-mysql"
-package_version = "3.0.8"
+package_version = "3.0.9"
 description = "Soda Core MySQL Package"
 
 requires = [
     f"soda-core=={package_version}",
     "mysql-connector-python==8.0.30",
 ]
 # TODO Fix the params
```

### Comparing `soda-core-mysql-3.0.8/soda/data_sources/mysql_data_source.py` & `soda-core-mysql-3.0.9/soda/data_sources/mysql_data_source.py`

 * *Files identical despite different names*

