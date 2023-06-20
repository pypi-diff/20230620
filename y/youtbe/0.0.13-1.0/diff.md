# Comparing `tmp/youtbe-0.0.13.tar.gz` & `tmp/youtbe-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "youtbe-0.0.13.tar", last modified: Mon Jun 19 20:01:35 2023, max compression
+gzip compressed data, was "youtbe-1.0.tar", last modified: Tue Jun 20 16:50:52 2023, max compression
```

## Comparing `youtbe-0.0.13.tar` & `youtbe-1.0.tar`

### file list

```diff
@@ -1,15 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 20:01:35.463133 youtbe-0.0.13/
--rw-rw-rw-   0        0        0     1312 2023-06-19 20:01:35.462135 youtbe-0.0.13/PKG-INFO
--rw-rw-rw-   0        0        0      779 2023-06-19 19:57:04.000000 youtbe-0.0.13/README.md
--rw-rw-rw-   0        0        0       42 2023-06-19 20:01:35.463133 youtbe-0.0.13/setup.cfg
--rw-rw-rw-   0        0        0     1089 2023-06-19 19:58:24.000000 youtbe-0.0.13/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-19 20:01:35.432739 youtbe-0.0.13/youtbe/
--rw-rw-rw-   0        0        0       29 2023-06-19 19:57:58.000000 youtbe-0.0.13/youtbe/__init__.py
--rw-rw-rw-   0        0        0     1315 2023-06-19 19:52:05.000000 youtbe-0.0.13/youtbe/youtbe.py
--rw-rw-rw-   0        0        0       94 2023-06-19 19:28:11.000000 youtbe-0.0.13/youtbe/zeus.py
-drwxrwxrwx   0        0        0        0 2023-06-19 20:01:35.460120 youtbe-0.0.13/youtbe.egg-info/
--rw-rw-rw-   0        0        0     1312 2023-06-19 20:01:35.000000 youtbe-0.0.13/youtbe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      218 2023-06-19 20:01:35.000000 youtbe-0.0.13/youtbe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 20:01:35.000000 youtbe-0.0.13/youtbe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-06-19 20:01:35.000000 youtbe-0.0.13/youtbe.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-19 20:01:35.000000 youtbe-0.0.13/youtbe.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-20 16:50:52.778383 youtbe-1.0/
+-rw-rw-rw-   0        0        0     1309 2023-06-20 16:50:52.777391 youtbe-1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      779 2023-06-19 19:57:04.000000 youtbe-1.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-20 16:50:52.778383 youtbe-1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1086 2023-06-20 16:49:32.000000 youtbe-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 16:50:52.775385 youtbe-1.0/youtbe.egg-info/
+-rw-rw-rw-   0        0        0     1309 2023-06-20 16:50:52.000000 youtbe-1.0/youtbe.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      167 2023-06-20 16:50:52.000000 youtbe-1.0/youtbe.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 16:50:52.000000 youtbe-1.0/youtbe.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-06-20 16:50:52.000000 youtbe-1.0/youtbe.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 16:50:52.000000 youtbe-1.0/youtbe.egg-info/top_level.txt
```

### Comparing `youtbe-0.0.13/PKG-INFO` & `youtbe-1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: youtbe
-Version: 0.0.13
+Version: 1.0
 Summary: Scrap Any Youtube Stats
 Author: vardxg
 Author-email: <dev@vardxg.com>
 Keywords: python,video,stats,video stats
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `youtbe-0.0.13/README.md` & `youtbe-1.0/README.md`

 * *Files identical despite different names*

### Comparing `youtbe-0.0.13/setup.py` & `youtbe-1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.13'
+VERSION = '1.0'
 DESCRIPTION = 'Scrap Any Youtube Stats'
 LONG_DESCRIPTION = 'Simple Package to Scrap Basic Stats from any Youtube Video.'
 
 # Setting up
 setup(
     name="youtbe",
     version=VERSION,
```

### Comparing `youtbe-0.0.13/youtbe.egg-info/PKG-INFO` & `youtbe-1.0/youtbe.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: youtbe
-Version: 0.0.13
+Version: 1.0
 Summary: Scrap Any Youtube Stats
 Author: vardxg
 Author-email: <dev@vardxg.com>
 Keywords: python,video,stats,video stats
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

