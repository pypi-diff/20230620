# Comparing `tmp/theamazingtestfirstofitskind-0.0.1.tar.gz` & `tmp/theamazingtestfirstofitskind-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "theamazingtestfirstofitskind-0.0.1.tar", last modified: Mon Jun 19 16:48:51 2023, max compression
+gzip compressed data, was "theamazingtestfirstofitskind-0.0.3.tar", last modified: Tue Jun 20 13:00:38 2023, max compression
```

## Comparing `theamazingtestfirstofitskind-0.0.1.tar` & `theamazingtestfirstofitskind-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:48:51.538473 theamazingtestfirstofitskind-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-19 16:48:51.538473 theamazingtestfirstofitskind-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 16:48:51.538473 theamazingtestfirstofitskind-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-19 16:48:41.000000 theamazingtestfirstofitskind-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:48:51.538473 theamazingtestfirstofitskind-0.0.1/testops/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-19 16:48:41.000000 theamazingtestfirstofitskind-0.0.1/testops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-19 16:48:41.000000 theamazingtestfirstofitskind-0.0.1/testops/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:48:51.538473 theamazingtestfirstofitskind-0.0.1/theamazingtestfirstofitskind.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-19 16:48:51.000000 theamazingtestfirstofitskind-0.0.1/theamazingtestfirstofitskind.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-19 16:48:51.000000 theamazingtestfirstofitskind-0.0.1/theamazingtestfirstofitskind.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 16:48:51.000000 theamazingtestfirstofitskind-0.0.1/theamazingtestfirstofitskind.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-19 16:48:51.000000 theamazingtestfirstofitskind-0.0.1/theamazingtestfirstofitskind.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:00:38.779417 theamazingtestfirstofitskind-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-06-20 13:00:38.779417 theamazingtestfirstofitskind-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 13:00:38.779417 theamazingtestfirstofitskind-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-20 13:00:26.000000 theamazingtestfirstofitskind-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:00:38.779417 theamazingtestfirstofitskind-0.0.3/testops/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-20 13:00:26.000000 theamazingtestfirstofitskind-0.0.3/testops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-20 13:00:26.000000 theamazingtestfirstofitskind-0.0.3/testops/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:00:38.779417 theamazingtestfirstofitskind-0.0.3/theamazingtestfirstofitskind.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-06-20 13:00:38.000000 theamazingtestfirstofitskind-0.0.3/theamazingtestfirstofitskind.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-20 13:00:38.000000 theamazingtestfirstofitskind-0.0.3/theamazingtestfirstofitskind.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 13:00:38.000000 theamazingtestfirstofitskind-0.0.3/theamazingtestfirstofitskind.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-20 13:00:38.000000 theamazingtestfirstofitskind-0.0.3/theamazingtestfirstofitskind.egg-info/top_level.txt
```

### Comparing `theamazingtestfirstofitskind-0.0.1/setup.py` & `theamazingtestfirstofitskind-0.0.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup, find_packages
 
 
-VERSION = '0.0.1'
-DESCRIPTION = 'basic test'
-LONG_DESCRIPTION = 'first dev test'
+VERSION = '0.0.3'
+DESCRIPTION = 'basic test2'
+LONG_DESCRIPTION = 'second dev test'
 
 # Setting up
 setup(
     name="theamazingtestfirstofitskind",
-    version="0.0.1",
+    version=VERSION,
     author="lotan hakli shel ashkelon",
-    author_email="<ilotanagar@gmail.com>",
+    author_email="<lotanagar@gmail.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
     install_requires=[],
     keywords=['python',  'sockets'],
     classifiers=[
```

