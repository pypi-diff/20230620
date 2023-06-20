# Comparing `tmp/kingscriptstest-1.0.3.tar.gz` & `tmp/kingscriptstest-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kingscriptstest-1.0.3.tar", last modified: Tue Jun 20 15:06:07 2023, max compression
+gzip compressed data, was "kingscriptstest-1.0.5.tar", last modified: Tue Jun 20 17:58:21 2023, max compression
```

## Comparing `kingscriptstest-1.0.3.tar` & `kingscriptstest-1.0.5.tar`

### file list

```diff
@@ -1,12 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 15:06:07.683249 kingscriptstest-1.0.3/
--rw-rw-rw-   0        0        0     1513 2023-06-20 15:06:07.682250 kingscriptstest-1.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-20 15:06:07.674711 kingscriptstest-1.0.3/kingscriptstest/
--rw-rw-rw-   0        0        0       37 2023-06-20 15:05:40.000000 kingscriptstest-1.0.3/kingscriptstest/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 15:06:07.681253 kingscriptstest-1.0.3/kingscriptstest.egg-info/
--rw-rw-rw-   0        0        0     1513 2023-06-20 15:06:07.000000 kingscriptstest-1.0.3/kingscriptstest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      230 2023-06-20 15:06:07.000000 kingscriptstest-1.0.3/kingscriptstest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 15:06:07.000000 kingscriptstest-1.0.3/kingscriptstest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-06-20 15:06:07.000000 kingscriptstest-1.0.3/kingscriptstest.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-20 15:06:07.000000 kingscriptstest-1.0.3/kingscriptstest.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-20 15:06:07.683249 kingscriptstest-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1418 2023-06-20 15:06:05.000000 kingscriptstest-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 17:58:21.703629 kingscriptstest-1.0.5/
+-rw-rw-rw-   0        0        0     1513 2023-06-20 17:58:21.702624 kingscriptstest-1.0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-20 17:58:21.701624 kingscriptstest-1.0.5/kingscriptstest.egg-info/
+-rw-rw-rw-   0        0        0     1513 2023-06-20 17:58:21.000000 kingscriptstest-1.0.5/kingscriptstest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2023-06-20 17:58:21.000000 kingscriptstest-1.0.5/kingscriptstest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 17:58:21.000000 kingscriptstest-1.0.5/kingscriptstest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-06-20 17:58:21.000000 kingscriptstest-1.0.5/kingscriptstest.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 17:58:21.000000 kingscriptstest-1.0.5/kingscriptstest.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-20 17:58:21.705204 kingscriptstest-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1406 2023-06-20 17:58:20.000000 kingscriptstest-1.0.5/setup.py
```

### Comparing `kingscriptstest-1.0.3/PKG-INFO` & `kingscriptstest-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kingscriptstest
-Version: 1.0.3
+Version: 1.0.5
 Summary: Test push of the King Scripts
 Home-page: https://github.com/kingoperating/v2
 Author: Michael Tanner
 Author-email: mtanner@kingoperating.com
 License: MIT
 Keywords: maps location address
 Classifier: Development Status :: 4 - Beta
```

### Comparing `kingscriptstest-1.0.3/kingscriptstest.egg-info/PKG-INFO` & `kingscriptstest-1.0.5/kingscriptstest.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kingscriptstest
-Version: 1.0.3
+Version: 1.0.5
 Summary: Test push of the King Scripts
 Home-page: https://github.com/kingoperating/v2
 Author: Michael Tanner
 Author-email: mtanner@kingoperating.com
 License: MIT
 Keywords: maps location address
 Classifier: Development Status :: 4 - Beta
```

### Comparing `kingscriptstest-1.0.3/setup.py` & `kingscriptstest-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 # reading long description from file
-with open('kingscriptstest/Readme.md', 'r') as file:
+with open('app/Readme.md', 'r') as file:
     long_description = file.read()
 
 
 # specify requirements of your package here
 REQUIREMENTS = ['requests', 'pandas']
 
 # some more details
@@ -22,15 +22,15 @@
     'Programming Language :: Python :: 3.3',
     'Programming Language :: Python :: 3.4',
     'Programming Language :: Python :: 3.5',
 ]
 
 # calling the setup function
 setup(name='kingscriptstest',
-      version='1.0.3',
+      version='1.0.5',
       description='Test push of the King Scripts',
       long_description=long_description,
       url='https://github.com/kingoperating/v2',
       author='Michael Tanner',
       author_email='mtanner@kingoperating.com',
       license='MIT',
       packages_dir={'': 'kingscriptstest'},
```

