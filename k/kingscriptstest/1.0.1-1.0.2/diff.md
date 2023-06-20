# Comparing `tmp/kingscriptstest-1.0.1.tar.gz` & `tmp/kingscriptstest-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kingscriptstest-1.0.1.tar", last modified: Tue Jun 20 14:46:20 2023, max compression
+gzip compressed data, was "kingscriptstest-1.0.2.tar", last modified: Tue Jun 20 15:01:31 2023, max compression
```

## Comparing `kingscriptstest-1.0.1.tar` & `kingscriptstest-1.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 14:46:20.796834 kingscriptstest-1.0.1/
--rw-rw-rw-   0        0        0     1513 2023-06-20 14:46:20.795789 kingscriptstest-1.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-20 14:46:20.786271 kingscriptstest-1.0.1/kingscriptstest/
--rw-rw-rw-   0        0        0        0 2023-06-20 12:54:44.000000 kingscriptstest-1.0.1/kingscriptstest/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:46:20.794792 kingscriptstest-1.0.1/kingscriptstest.egg-info/
--rw-rw-rw-   0        0        0     1513 2023-06-20 14:46:20.000000 kingscriptstest-1.0.1/kingscriptstest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      230 2023-06-20 14:46:20.000000 kingscriptstest-1.0.1/kingscriptstest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 14:46:20.000000 kingscriptstest-1.0.1/kingscriptstest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-06-20 14:46:20.000000 kingscriptstest-1.0.1/kingscriptstest.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-20 14:46:20.000000 kingscriptstest-1.0.1/kingscriptstest.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-20 14:46:20.796834 kingscriptstest-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1418 2023-06-20 14:27:25.000000 kingscriptstest-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 15:01:31.243327 kingscriptstest-1.0.2/
+-rw-rw-rw-   0        0        0     1513 2023-06-20 15:01:31.242279 kingscriptstest-1.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-20 15:01:31.233284 kingscriptstest-1.0.2/kingscriptstest/
+-rw-rw-rw-   0        0        0       45 2023-06-20 15:00:35.000000 kingscriptstest-1.0.2/kingscriptstest/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 15:01:31.241284 kingscriptstest-1.0.2/kingscriptstest.egg-info/
+-rw-rw-rw-   0        0        0     1513 2023-06-20 15:01:31.000000 kingscriptstest-1.0.2/kingscriptstest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      230 2023-06-20 15:01:31.000000 kingscriptstest-1.0.2/kingscriptstest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 15:01:31.000000 kingscriptstest-1.0.2/kingscriptstest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-06-20 15:01:31.000000 kingscriptstest-1.0.2/kingscriptstest.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-20 15:01:31.000000 kingscriptstest-1.0.2/kingscriptstest.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-20 15:01:31.243327 kingscriptstest-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1418 2023-06-20 15:01:04.000000 kingscriptstest-1.0.2/setup.py
```

### Comparing `kingscriptstest-1.0.1/PKG-INFO` & `kingscriptstest-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kingscriptstest
-Version: 1.0.1
+Version: 1.0.2
 Summary: Test push of the King Scripts
 Home-page: https://github.com/kingoperating/v2
 Author: Michael Tanner
 Author-email: mtanner@kingoperating.com
 License: MIT
 Keywords: maps location address
 Classifier: Development Status :: 4 - Beta
```

### Comparing `kingscriptstest-1.0.1/kingscriptstest.egg-info/PKG-INFO` & `kingscriptstest-1.0.2/kingscriptstest.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kingscriptstest
-Version: 1.0.1
+Version: 1.0.2
 Summary: Test push of the King Scripts
 Home-page: https://github.com/kingoperating/v2
 Author: Michael Tanner
 Author-email: mtanner@kingoperating.com
 License: MIT
 Keywords: maps location address
 Classifier: Development Status :: 4 - Beta
```

### Comparing `kingscriptstest-1.0.1/setup.py` & `kingscriptstest-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     'Programming Language :: Python :: 3.3',
     'Programming Language :: Python :: 3.4',
     'Programming Language :: Python :: 3.5',
 ]
 
 # calling the setup function
 setup(name='kingscriptstest',
-      version='1.0.1',
+      version='1.0.2',
       description='Test push of the King Scripts',
       long_description=long_description,
       url='https://github.com/kingoperating/v2',
       author='Michael Tanner',
       author_email='mtanner@kingoperating.com',
       license='MIT',
       packages_dir={'': 'kingscriptstest'},
```

