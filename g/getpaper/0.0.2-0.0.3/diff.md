# Comparing `tmp/getpaper-0.0.2.tar.gz` & `tmp/getpaper-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getpaper-0.0.2.tar", last modified: Tue Jun 20 21:34:53 2023, max compression
+gzip compressed data, was "getpaper-0.0.3.tar", last modified: Tue Jun 20 21:41:15 2023, max compression
```

## Comparing `getpaper-0.0.2.tar` & `getpaper-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-20 21:34:53.838741 getpaper-0.0.2/
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     1072 2023-06-20 19:48:29.000000 getpaper-0.0.2/LICENSE
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      642 2023-06-20 21:34:53.838741 getpaper-0.0.2/PKG-INFO
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)       28 2023-06-20 19:48:29.000000 getpaper-0.0.2/README.md
-drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-20 21:34:53.838741 getpaper-0.0.2/getpaper/
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-20 20:08:46.000000 getpaper-0.0.2/getpaper/__init__.py
--rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)     3543 2023-06-20 21:23:26.000000 getpaper-0.0.2/getpaper/download.py
-drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-20 21:34:53.838741 getpaper-0.0.2/getpaper.egg-info/
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      642 2023-06-20 21:34:53.000000 getpaper-0.0.2/getpaper.egg-info/PKG-INFO
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      262 2023-06-20 21:34:53.000000 getpaper-0.0.2/getpaper.egg-info/SOURCES.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        1 2023-06-20 21:34:53.000000 getpaper-0.0.2/getpaper.egg-info/dependency_links.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      116 2023-06-20 21:34:53.000000 getpaper-0.0.2/getpaper.egg-info/entry_points.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      132 2023-06-20 21:34:53.000000 getpaper-0.0.2/getpaper.egg-info/requires.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        9 2023-06-20 21:34:53.000000 getpaper-0.0.2/getpaper.egg-info/top_level.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)       38 2023-06-20 21:34:53.838741 getpaper-0.0.2/setup.cfg
--rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)     1453 2023-06-20 21:34:46.000000 getpaper-0.0.2/setup.py
+drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-20 21:41:15.589508 getpaper-0.0.3/
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     1072 2023-06-20 19:48:29.000000 getpaper-0.0.3/LICENSE
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      642 2023-06-20 21:41:15.589508 getpaper-0.0.3/PKG-INFO
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)       28 2023-06-20 19:48:29.000000 getpaper-0.0.3/README.md
+drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-20 21:41:15.589508 getpaper-0.0.3/getpaper/
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-20 20:08:46.000000 getpaper-0.0.3/getpaper/__init__.py
+-rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)     3543 2023-06-20 21:23:26.000000 getpaper-0.0.3/getpaper/download.py
+drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-20 21:41:15.589508 getpaper-0.0.3/getpaper.egg-info/
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      642 2023-06-20 21:41:15.000000 getpaper-0.0.3/getpaper.egg-info/PKG-INFO
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      262 2023-06-20 21:41:15.000000 getpaper-0.0.3/getpaper.egg-info/SOURCES.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        1 2023-06-20 21:41:15.000000 getpaper-0.0.3/getpaper.egg-info/dependency_links.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)       51 2023-06-20 21:41:15.000000 getpaper-0.0.3/getpaper.egg-info/entry_points.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      132 2023-06-20 21:41:15.000000 getpaper-0.0.3/getpaper.egg-info/requires.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        9 2023-06-20 21:41:15.000000 getpaper-0.0.3/getpaper.egg-info/top_level.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)       38 2023-06-20 21:41:15.589508 getpaper-0.0.3/setup.cfg
+-rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)     1378 2023-06-20 21:41:14.000000 getpaper-0.0.3/setup.py
```

### Comparing `getpaper-0.0.2/LICENSE` & `getpaper-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `getpaper-0.0.2/PKG-INFO` & `getpaper-0.0.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getpaper
-Version: 0.0.2
+Version: 0.0.3
 Summary: getpaper - papers download made easy!
 Author: antonkulaga (Anton Kulaga)
 Author-email: <antonkulaga@gmail.com>
 Keywords: python,utils,files,papers,download
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `getpaper-0.0.2/getpaper/download.py` & `getpaper-0.0.3/getpaper/download.py`

 * *Files identical despite different names*

### Comparing `getpaper-0.0.2/getpaper.egg-info/PKG-INFO` & `getpaper-0.0.3/getpaper.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getpaper
-Version: 0.0.2
+Version: 0.0.3
 Summary: getpaper - papers download made easy!
 Author: antonkulaga (Anton Kulaga)
 Author-email: <antonkulaga@gmail.com>
 Keywords: python,utils,files,papers,download
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `getpaper-0.0.2/setup.py` & `getpaper-0.0.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'getpaper - papers download made easy!'
 LONG_DESCRIPTION = 'A package with python functions for downloading papers'
 
 # Setting up
 setup(
     name="getpaper",
     version=VERSION,
@@ -30,12 +30,11 @@
         'Programming Language :: Python :: 3.11',
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
     ],
     entry_points={
      "console_scripts": [
-         "download_doi=getpaper.download:download_doi",
-         "download_pubmed=getpaper.download:download_pubmed"
+         "download=getpaper.download:app"
      ]
     }
 )
```

