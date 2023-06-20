# Comparing `tmp/autogluon-0.8.1b20230619.tar.gz` & `tmp/autogluon-0.8.1b20230620.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon-0.8.1b20230619.tar", last modified: Mon Jun 19 09:04:28 2023, max compression
+gzip compressed data, was "autogluon-0.8.1b20230620.tar", last modified: Tue Jun 20 09:04:27 2023, max compression
```

## Comparing `autogluon-0.8.1b20230619.tar` & `autogluon-0.8.1b20230620.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:04:28.633082 autogluon-0.8.1b20230619/
--rw-r--r--   0 runner    (1001) docker     (123)    12508 2023-06-19 09:04:28.633082 autogluon-0.8.1b20230619/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 09:04:28.633082 autogluon-0.8.1b20230619/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-06-19 09:03:45.000000 autogluon-0.8.1b20230619/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:04:28.629082 autogluon-0.8.1b20230619/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:04:28.629082 autogluon-0.8.1b20230619/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:04:28.633082 autogluon-0.8.1b20230619/src/autogluon/_internal_/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 09:03:45.000000 autogluon-0.8.1b20230619/src/autogluon/_internal_/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:04:28.633082 autogluon-0.8.1b20230619/src/autogluon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12508 2023-06-19 09:04:28.000000 autogluon-0.8.1b20230619/src/autogluon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-19 09:04:28.000000 autogluon-0.8.1b20230619/src/autogluon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 09:04:28.000000 autogluon-0.8.1b20230619/src/autogluon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-19 09:04:28.000000 autogluon-0.8.1b20230619/src/autogluon.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-19 09:04:28.000000 autogluon-0.8.1b20230619/src/autogluon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-19 09:04:28.000000 autogluon-0.8.1b20230619/src/autogluon.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 09:04:28.000000 autogluon-0.8.1b20230619/src/autogluon.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:04:27.676495 autogluon-0.8.1b20230620/
+-rw-r--r--   0 runner    (1001) docker     (123)    12508 2023-06-20 09:04:27.676495 autogluon-0.8.1b20230620/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 09:04:27.676495 autogluon-0.8.1b20230620/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-06-20 09:03:44.000000 autogluon-0.8.1b20230620/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:04:27.676495 autogluon-0.8.1b20230620/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:04:27.676495 autogluon-0.8.1b20230620/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:04:27.676495 autogluon-0.8.1b20230620/src/autogluon/_internal_/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 09:03:44.000000 autogluon-0.8.1b20230620/src/autogluon/_internal_/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:04:27.676495 autogluon-0.8.1b20230620/src/autogluon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12508 2023-06-20 09:04:27.000000 autogluon-0.8.1b20230620/src/autogluon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-20 09:04:27.000000 autogluon-0.8.1b20230620/src/autogluon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 09:04:27.000000 autogluon-0.8.1b20230620/src/autogluon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-20 09:04:27.000000 autogluon-0.8.1b20230620/src/autogluon.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-20 09:04:27.000000 autogluon-0.8.1b20230620/src/autogluon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-20 09:04:27.000000 autogluon-0.8.1b20230620/src/autogluon.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 09:04:27.000000 autogluon-0.8.1b20230620/src/autogluon.egg-info/zip-safe
```

### Comparing `autogluon-0.8.1b20230619/PKG-INFO` & `autogluon-0.8.1b20230620/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon
-Version: 0.8.1b20230619
+Version: 0.8.1b20230620
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon-0.8.1b20230619/setup.py` & `autogluon-0.8.1b20230620/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon-0.8.1b20230619/src/autogluon.egg-info/PKG-INFO` & `autogluon-0.8.1b20230620/src/autogluon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon
-Version: 0.8.1b20230619
+Version: 0.8.1b20230620
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

