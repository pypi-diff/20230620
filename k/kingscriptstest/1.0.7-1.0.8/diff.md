# Comparing `tmp/kingscriptstest-1.0.7.tar.gz` & `tmp/kingscriptstest-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kingscriptstest-1.0.7.tar", last modified: Tue Jun 20 18:10:31 2023, max compression
+gzip compressed data, was "kingscriptstest-1.0.8.tar", last modified: Tue Jun 20 18:15:51 2023, max compression
```

## Comparing `kingscriptstest-1.0.7.tar` & `kingscriptstest-1.0.8.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 18:10:31.343032 kingscriptstest-1.0.7/
--rw-rw-rw-   0        0        0     1513 2023-06-20 18:10:31.341959 kingscriptstest-1.0.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-20 18:10:31.340940 kingscriptstest-1.0.7/kingscriptstest.egg-info/
--rw-rw-rw-   0        0        0     1513 2023-06-20 18:10:31.000000 kingscriptstest-1.0.7/kingscriptstest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2023-06-20 18:10:31.000000 kingscriptstest-1.0.7/kingscriptstest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 18:10:31.000000 kingscriptstest-1.0.7/kingscriptstest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-06-20 18:10:31.000000 kingscriptstest-1.0.7/kingscriptstest.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 18:10:31.000000 kingscriptstest-1.0.7/kingscriptstest.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-20 18:10:31.343032 kingscriptstest-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1406 2023-06-20 18:10:27.000000 kingscriptstest-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 18:15:51.764060 kingscriptstest-1.0.8/
+-rw-rw-rw-   0        0        0     1513 2023-06-20 18:15:51.763053 kingscriptstest-1.0.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-20 18:15:51.760998 kingscriptstest-1.0.8/kingscriptstest.egg-info/
+-rw-rw-rw-   0        0        0     1513 2023-06-20 18:15:51.000000 kingscriptstest-1.0.8/kingscriptstest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2023-06-20 18:15:51.000000 kingscriptstest-1.0.8/kingscriptstest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 18:15:51.000000 kingscriptstest-1.0.8/kingscriptstest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-06-20 18:15:51.000000 kingscriptstest-1.0.8/kingscriptstest.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 18:15:51.000000 kingscriptstest-1.0.8/kingscriptstest.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-20 18:15:51.764060 kingscriptstest-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1406 2023-06-20 18:15:50.000000 kingscriptstest-1.0.8/setup.py
```

### Comparing `kingscriptstest-1.0.7/PKG-INFO` & `kingscriptstest-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kingscriptstest
-Version: 1.0.7
+Version: 1.0.8
 Summary: Test push of the King Scripts
 Home-page: https://github.com/kingoperating/v2
 Author: Michael Tanner
 Author-email: mtanner@kingoperating.com
 License: MIT
 Keywords: maps location address
 Classifier: Development Status :: 4 - Beta
```

### Comparing `kingscriptstest-1.0.7/kingscriptstest.egg-info/PKG-INFO` & `kingscriptstest-1.0.8/kingscriptstest.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kingscriptstest
-Version: 1.0.7
+Version: 1.0.8
 Summary: Test push of the King Scripts
 Home-page: https://github.com/kingoperating/v2
 Author: Michael Tanner
 Author-email: mtanner@kingoperating.com
 License: MIT
 Keywords: maps location address
 Classifier: Development Status :: 4 - Beta
```

### Comparing `kingscriptstest-1.0.7/setup.py` & `kingscriptstest-1.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     'Programming Language :: Python :: 3.3',
     'Programming Language :: Python :: 3.4',
     'Programming Language :: Python :: 3.5',
 ]
 
 # calling the setup function
 setup(name='kingscriptstest',
-      version='1.0.7',
+      version='1.0.8',
       description='Test push of the King Scripts',
       long_description=long_description,
       url='https://github.com/kingoperating/v2',
       author='Michael Tanner',
       author_email='mtanner@kingoperating.com',
       license='MIT',
       packages_dir={'': 'kingscriptstest'},
```

