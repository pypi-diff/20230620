# Comparing `tmp/cashooo-1.1.2.tar.gz` & `tmp/cashooo-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cashooo-1.1.2.tar", last modified: Tue Jun 20 05:40:45 2023, max compression
+gzip compressed data, was "cashooo-1.1.3.tar", last modified: Tue Jun 20 06:03:39 2023, max compression
```

## Comparing `cashooo-1.1.2.tar` & `cashooo-1.1.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 05:40:45.207818 cashooo-1.1.2/
--rw-rw-rw-   0        0        0      332 2023-06-20 05:40:45.204369 cashooo-1.1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-20 05:40:45.082512 cashooo-1.1.2/casho/
--rw-rw-rw-   0        0        0       92 2023-06-18 09:23:40.000000 cashooo-1.1.2/casho/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 05:40:45.092345 cashooo-1.1.2/casho/mylibrary/
--rw-rw-rw-   0        0        0       71 2023-06-20 05:31:34.000000 cashooo-1.1.2/casho/mylibrary/__init__.py
--rw-rw-rw-   0        0        0      165 2023-06-18 09:23:40.000000 cashooo-1.1.2/casho/mylibrary/apps.py
-drwxrwxrwx   0        0        0        0 2023-06-20 05:40:45.107443 cashooo-1.1.2/casho/mylibrary/errors/
--rw-rw-rw-   0        0        0      114 2023-06-18 09:23:40.000000 cashooo-1.1.2/casho/mylibrary/errors/__init__.py
--rw-rw-rw-   0        0        0      619 2023-06-18 09:23:40.000000 cashooo-1.1.2/casho/mylibrary/errors/custom_error.py
--rw-rw-rw-   0        0        0      392 2023-06-18 09:23:40.000000 cashooo-1.1.2/casho/mylibrary/errors/database_connection_error.py
-drwxrwxrwx   0        0        0        0 2023-06-20 05:40:45.119814 cashooo-1.1.2/casho/mylibrary/middlewares/
--rw-rw-rw-   0        0        0       97 2023-06-18 09:23:41.000000 cashooo-1.1.2/casho/mylibrary/middlewares/__init__.py
--rw-rw-rw-   0        0        0      626 2023-06-18 09:23:41.000000 cashooo-1.1.2/casho/mylibrary/middlewares/errorhandler.py
--rw-rw-rw-   0        0        0     1713 2023-06-18 09:23:41.000000 cashooo-1.1.2/casho/mylibrary/middlewares/healthcheck.py
-drwxrwxrwx   0        0        0        0 2023-06-20 05:40:45.199098 cashooo-1.1.2/cashooo.egg-info/
--rw-rw-rw-   0        0        0      332 2023-06-20 05:40:44.000000 cashooo-1.1.2/cashooo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      485 2023-06-20 05:40:44.000000 cashooo-1.1.2/cashooo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 05:40:44.000000 cashooo-1.1.2/cashooo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-06-20 05:40:44.000000 cashooo-1.1.2/cashooo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-20 05:40:44.000000 cashooo-1.1.2/cashooo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-20 05:40:45.210359 cashooo-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0      538 2023-06-20 05:27:25.000000 cashooo-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 06:03:39.321633 cashooo-1.1.3/
+-rw-rw-rw-   0        0        0      332 2023-06-20 06:03:39.320465 cashooo-1.1.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-20 06:03:39.287169 cashooo-1.1.3/casho/
+-rw-rw-rw-   0        0        0       92 2023-06-18 09:23:40.000000 cashooo-1.1.3/casho/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 06:03:39.294406 cashooo-1.1.3/casho/mylibrary/
+-rw-rw-rw-   0        0        0      157 2023-06-20 06:03:02.000000 cashooo-1.1.3/casho/mylibrary/__init__.py
+-rw-rw-rw-   0        0        0      165 2023-06-18 09:23:40.000000 cashooo-1.1.3/casho/mylibrary/apps.py
+drwxrwxrwx   0        0        0        0 2023-06-20 06:03:39.298687 cashooo-1.1.3/casho/mylibrary/errors/
+-rw-rw-rw-   0        0        0      114 2023-06-18 09:23:40.000000 cashooo-1.1.3/casho/mylibrary/errors/__init__.py
+-rw-rw-rw-   0        0        0      619 2023-06-18 09:23:40.000000 cashooo-1.1.3/casho/mylibrary/errors/custom_error.py
+-rw-rw-rw-   0        0        0      392 2023-06-18 09:23:40.000000 cashooo-1.1.3/casho/mylibrary/errors/database_connection_error.py
+drwxrwxrwx   0        0        0        0 2023-06-20 06:03:39.303104 cashooo-1.1.3/casho/mylibrary/middlewares/
+-rw-rw-rw-   0        0        0       97 2023-06-18 09:23:41.000000 cashooo-1.1.3/casho/mylibrary/middlewares/__init__.py
+-rw-rw-rw-   0        0        0      626 2023-06-18 09:23:41.000000 cashooo-1.1.3/casho/mylibrary/middlewares/errorhandler.py
+-rw-rw-rw-   0        0        0     1713 2023-06-18 09:23:41.000000 cashooo-1.1.3/casho/mylibrary/middlewares/healthcheck.py
+drwxrwxrwx   0        0        0        0 2023-06-20 06:03:39.319400 cashooo-1.1.3/cashooo.egg-info/
+-rw-rw-rw-   0        0        0      332 2023-06-20 06:03:39.000000 cashooo-1.1.3/cashooo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      485 2023-06-20 06:03:39.000000 cashooo-1.1.3/cashooo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 06:03:39.000000 cashooo-1.1.3/cashooo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-06-20 06:03:39.000000 cashooo-1.1.3/cashooo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-20 06:03:39.000000 cashooo-1.1.3/cashooo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-20 06:03:39.321633 cashooo-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      538 2023-06-20 06:03:34.000000 cashooo-1.1.3/setup.py
```

### Comparing `cashooo-1.1.2/casho/mylibrary/errors/custom_error.py` & `cashooo-1.1.3/casho/mylibrary/errors/custom_error.py`

 * *Files identical despite different names*

### Comparing `cashooo-1.1.2/casho/mylibrary/middlewares/errorhandler.py` & `cashooo-1.1.3/casho/mylibrary/middlewares/errorhandler.py`

 * *Files identical despite different names*

### Comparing `cashooo-1.1.2/casho/mylibrary/middlewares/healthcheck.py` & `cashooo-1.1.3/casho/mylibrary/middlewares/healthcheck.py`

 * *Files identical despite different names*

### Comparing `cashooo-1.1.2/setup.py` & `cashooo-1.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='cashooo',
-    version='1.1.2',
+    version='1.1.3',
     description='Custom errors and middlewares',
     author='yash ',
     author_email='yash.m@royalecheese.com',
     packages=find_packages(),
     install_requires=[
         'Django>=3.2',
         'confluent-kafka'
```

