# Comparing `tmp/cp-version-testing-1.0.2.tar.gz` & `tmp/cp-version-testing-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cp-version-testing-1.0.2.tar", last modified: Tue Jun 20 05:46:35 2023, max compression
+gzip compressed data, was "cp-version-testing-1.0.3.tar", last modified: Tue Jun 20 05:51:20 2023, max compression
```

## Comparing `cp-version-testing-1.0.2.tar` & `cp-version-testing-1.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 05:46:35.928818 cp-version-testing-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-20 05:46:35.928818 cp-version-testing-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-20 05:46:27.000000 cp-version-testing-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 05:46:35.924818 cp-version-testing-1.0.2/cp-version-testing/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-20 05:46:27.000000 cp-version-testing-1.0.2/cp-version-testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-20 05:46:27.000000 cp-version-testing-1.0.2/cp-version-testing/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 05:46:35.928818 cp-version-testing-1.0.2/cp_version_testing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-20 05:46:35.000000 cp-version-testing-1.0.2/cp_version_testing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-20 05:46:35.000000 cp-version-testing-1.0.2/cp_version_testing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 05:46:35.000000 cp-version-testing-1.0.2/cp_version_testing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-20 05:46:35.000000 cp-version-testing-1.0.2/cp_version_testing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 05:46:35.928818 cp-version-testing-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-20 05:46:27.000000 cp-version-testing-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 05:51:20.665668 cp-version-testing-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-20 05:51:20.665668 cp-version-testing-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-20 05:51:07.000000 cp-version-testing-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 05:51:20.665668 cp-version-testing-1.0.3/cp-version-testing/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-20 05:51:07.000000 cp-version-testing-1.0.3/cp-version-testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-20 05:51:07.000000 cp-version-testing-1.0.3/cp-version-testing/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 05:51:20.665668 cp-version-testing-1.0.3/cp_version_testing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-20 05:51:20.000000 cp-version-testing-1.0.3/cp_version_testing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-20 05:51:20.000000 cp-version-testing-1.0.3/cp_version_testing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 05:51:20.000000 cp-version-testing-1.0.3/cp_version_testing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-20 05:51:20.000000 cp-version-testing-1.0.3/cp_version_testing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 05:51:20.665668 cp-version-testing-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-20 05:51:07.000000 cp-version-testing-1.0.3/setup.py
```

### Comparing `cp-version-testing-1.0.2/setup.py` & `cp-version-testing-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="cp-version-testing",
-    version="1.0.2",
+    version="1.0.3",
     author_email="roniz@checkpoint.com",
     author="Check Point",
     license='Apache 2.0',
     description="Check Point",
     long_description="Check Point",
     long_description_content_type="text/plain",
     url="https://github.com/CheckPointSW/",
```

