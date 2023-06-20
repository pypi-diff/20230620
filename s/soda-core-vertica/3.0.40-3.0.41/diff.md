# Comparing `tmp/soda-core-vertica-3.0.40.tar.gz` & `tmp/soda-core-vertica-3.0.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soda-core-vertica-3.0.40.tar", last modified: Fri Jun 16 08:29:54 2023, max compression
+gzip compressed data, was "soda-core-vertica-3.0.41.tar", last modified: Tue Jun 20 12:56:31 2023, max compression
```

## Comparing `soda-core-vertica-3.0.40.tar` & `soda-core-vertica-3.0.41.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 08:29:54.314921 soda-core-vertica-3.0.40/
--rw-r--r--   0 runner    (1001) docker     (122)       62 2023-06-16 08:29:54.314921 soda-core-vertica-3.0.40/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-16 08:29:54.314921 soda-core-vertica-3.0.40/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      597 2023-06-16 08:28:48.000000 soda-core-vertica-3.0.40/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 08:29:54.310921 soda-core-vertica-3.0.40/soda/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 08:29:54.310921 soda-core-vertica-3.0.40/soda/data_sources/
--rw-r--r--   0 runner    (1001) docker     (122)     7672 2023-06-16 08:28:48.000000 soda-core-vertica-3.0.40/soda/data_sources/vertica_data_source.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 08:29:54.310921 soda-core-vertica-3.0.40/soda_core_vertica.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)       62 2023-06-16 08:29:54.000000 soda-core-vertica-3.0.40/soda_core_vertica.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-06-16 08:29:54.000000 soda-core-vertica-3.0.40/soda_core_vertica.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-16 08:29:54.000000 soda-core-vertica-3.0.40/soda_core_vertica.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       45 2023-06-16 08:29:54.000000 soda-core-vertica-3.0.40/soda_core_vertica.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-16 08:29:54.000000 soda-core-vertica-3.0.40/soda_core_vertica.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 08:29:54.310921 soda-core-vertica-3.0.40/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       29 2023-06-16 08:28:48.000000 soda-core-vertica-3.0.40/tests/test_vertica.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 12:56:31.479890 soda-core-vertica-3.0.41/
+-rw-r--r--   0 runner    (1001) docker     (122)       62 2023-06-20 12:56:31.479890 soda-core-vertica-3.0.41/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-20 12:56:31.479890 soda-core-vertica-3.0.41/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      597 2023-06-20 12:54:46.000000 soda-core-vertica-3.0.41/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 12:56:31.475890 soda-core-vertica-3.0.41/soda/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 12:56:31.475890 soda-core-vertica-3.0.41/soda/data_sources/
+-rw-r--r--   0 runner    (1001) docker     (122)     7672 2023-06-20 12:54:46.000000 soda-core-vertica-3.0.41/soda/data_sources/vertica_data_source.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 12:56:31.479890 soda-core-vertica-3.0.41/soda_core_vertica.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)       62 2023-06-20 12:56:31.000000 soda-core-vertica-3.0.41/soda_core_vertica.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-06-20 12:56:31.000000 soda-core-vertica-3.0.41/soda_core_vertica.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-20 12:56:31.000000 soda-core-vertica-3.0.41/soda_core_vertica.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       45 2023-06-20 12:56:31.000000 soda-core-vertica-3.0.41/soda_core_vertica.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-20 12:56:31.000000 soda-core-vertica-3.0.41/soda_core_vertica.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 12:56:31.479890 soda-core-vertica-3.0.41/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       29 2023-06-20 12:54:46.000000 soda-core-vertica-3.0.41/tests/test_vertica.py
```

### Comparing `soda-core-vertica-3.0.40/setup.py` & `soda-core-vertica-3.0.41/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 if sys.version_info < (3, 7):
     print("Error: Soda Core requires at least Python 3.7")
     print("Error: Please upgrade your Python version to 3.7 or later")
     sys.exit(1)
 
 package_name = "soda-core-vertica"
-package_version = "3.0.40"
+package_version = "3.0.41"
 description = "Soda Core Vertica Package"
 
 requires = [f"soda-core=={package_version}", "vertica-python>=1.0.3, <2.0"]
 
 setup(
     name=package_name,
     version=package_version,
```

### Comparing `soda-core-vertica-3.0.40/soda/data_sources/vertica_data_source.py` & `soda-core-vertica-3.0.41/soda/data_sources/vertica_data_source.py`

 * *Files identical despite different names*

