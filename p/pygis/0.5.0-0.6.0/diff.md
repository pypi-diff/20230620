# Comparing `tmp/pygis-0.5.0.tar.gz` & `tmp/pygis-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygis-0.5.0.tar", last modified: Tue Nov 29 05:27:51 2022, max compression
+gzip compressed data, was "pygis-0.6.0.tar", last modified: Tue Jun 20 01:56:02 2023, max compression
```

## Comparing `pygis-0.5.0.tar` & `pygis-0.6.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-29 05:27:51.317705 pygis-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1070 2022-11-29 05:27:37.000000 pygis-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      122 2022-11-29 05:27:37.000000 pygis-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1902 2022-11-29 05:27:51.317705 pygis-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1117 2022-11-29 05:27:37.000000 pygis-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-29 05:27:51.313705 pygis-0.5.0/pygis/
--rw-r--r--   0 runner    (1001) docker     (122)      120 2022-11-29 05:27:37.000000 pygis-0.5.0/pygis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       19 2022-11-29 05:27:37.000000 pygis-0.5.0/pygis/pygis.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-29 05:27:51.317705 pygis-0.5.0/pygis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1902 2022-11-29 05:27:51.000000 pygis-0.5.0/pygis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      270 2022-11-29 05:27:51.000000 pygis-0.5.0/pygis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)      481 2022-11-29 05:27:51.000000 pygis-0.5.0/pygis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-29 05:27:51.000000 pygis-0.5.0/pygis.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      189 2022-11-29 05:27:51.000000 pygis-0.5.0/pygis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2022-11-29 05:27:51.000000 pygis-0.5.0/pygis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      480 2022-11-29 05:27:37.000000 pygis-0.5.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)      388 2022-11-29 05:27:51.317705 pygis-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1759 2022-11-29 05:27:37.000000 pygis-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 01:56:02.752286 pygis-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-20 01:55:53.000000 pygis-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-20 01:55:53.000000 pygis-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-06-20 01:56:02.752286 pygis-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-06-20 01:55:53.000000 pygis-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 01:56:02.752286 pygis-0.6.0/pygis/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-20 01:55:53.000000 pygis-0.6.0/pygis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-20 01:55:53.000000 pygis-0.6.0/pygis/pygis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 01:56:02.752286 pygis-0.6.0/pygis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-06-20 01:56:02.000000 pygis-0.6.0/pygis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-20 01:56:02.000000 pygis-0.6.0/pygis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-06-20 01:56:02.000000 pygis-0.6.0/pygis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 01:56:02.000000 pygis-0.6.0/pygis.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-20 01:56:02.000000 pygis-0.6.0/pygis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-20 01:56:02.000000 pygis-0.6.0/pygis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-20 01:55:53.000000 pygis-0.6.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-20 01:56:02.752286 pygis-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-06-20 01:55:53.000000 pygis-0.6.0/setup.py
```

### Comparing `pygis-0.5.0/LICENSE` & `pygis-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pygis-0.5.0/PKG-INFO` & `pygis-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygis
-Version: 0.5.0
+Version: 0.6.0
 Summary: A Python package for installing optional dependencies for geemap and leafmap.
 Home-page: https://github.com/giswqs/pygis
 Author: Qiusheng Wu
 Author-email: giswqs@gmail.com
 License: MIT license
 Keywords: pygis
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `pygis-0.5.0/README.md` & `pygis-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `pygis-0.5.0/pygis.egg-info/PKG-INFO` & `pygis-0.6.0/pygis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygis
-Version: 0.5.0
+Version: 0.6.0
 Summary: A Python package for installing optional dependencies for geemap and leafmap.
 Home-page: https://github.com/giswqs/pygis
 Author: Qiusheng Wu
 Author-email: giswqs@gmail.com
 License: MIT license
 Keywords: pygis
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `pygis-0.5.0/setup.py` & `pygis-0.6.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,10 +49,10 @@
     keywords='pygis',
     name='pygis',
     packages=find_packages(include=['pygis', 'pygis.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/giswqs/pygis',
-    version='0.5.0',
+    version='0.6.0',
     zip_safe=False,
 )
```

