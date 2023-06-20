# Comparing `tmp/spacyspellcheck-0.0.2.tar.gz` & `tmp/spacyspellcheck-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spacyspellcheck-0.0.2.tar", last modified: Tue Jun 20 13:12:18 2023, max compression
+gzip compressed data, was "spacyspellcheck-0.0.3.tar", last modified: Tue Jun 20 13:15:36 2023, max compression
```

## Comparing `spacyspellcheck-0.0.2.tar` & `spacyspellcheck-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:12:18.156005 spacyspellcheck-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-20 13:12:09.000000 spacyspellcheck-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-20 13:12:18.156005 spacyspellcheck-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-20 13:12:18.156005 spacyspellcheck-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-06-20 13:12:09.000000 spacyspellcheck-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:12:18.156005 spacyspellcheck-0.0.2/spacyspellcheck/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 13:12:09.000000 spacyspellcheck-0.0.2/spacyspellcheck/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-06-20 13:12:09.000000 spacyspellcheck-0.0.2/spacyspellcheck/spellcheck.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:12:18.156005 spacyspellcheck-0.0.2/spacyspellcheck.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-20 13:12:18.000000 spacyspellcheck-0.0.2/spacyspellcheck.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-20 13:12:18.000000 spacyspellcheck-0.0.2/spacyspellcheck.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 13:12:18.000000 spacyspellcheck-0.0.2/spacyspellcheck.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 13:12:18.000000 spacyspellcheck-0.0.2/spacyspellcheck.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-20 13:12:18.000000 spacyspellcheck-0.0.2/spacyspellcheck.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-20 13:12:18.000000 spacyspellcheck-0.0.2/spacyspellcheck.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:15:36.473672 spacyspellcheck-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-20 13:15:18.000000 spacyspellcheck-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-20 13:15:36.473672 spacyspellcheck-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-20 13:15:18.000000 spacyspellcheck-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-20 13:15:36.473672 spacyspellcheck-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-06-20 13:15:18.000000 spacyspellcheck-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:15:36.469672 spacyspellcheck-0.0.3/spacyspellcheck/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 13:15:18.000000 spacyspellcheck-0.0.3/spacyspellcheck/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-06-20 13:15:18.000000 spacyspellcheck-0.0.3/spacyspellcheck/spellcheck.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:15:36.473672 spacyspellcheck-0.0.3/spacyspellcheck.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-20 13:15:36.000000 spacyspellcheck-0.0.3/spacyspellcheck.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-20 13:15:36.000000 spacyspellcheck-0.0.3/spacyspellcheck.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 13:15:36.000000 spacyspellcheck-0.0.3/spacyspellcheck.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 13:15:36.000000 spacyspellcheck-0.0.3/spacyspellcheck.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-20 13:15:36.000000 spacyspellcheck-0.0.3/spacyspellcheck.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-20 13:15:36.000000 spacyspellcheck-0.0.3/spacyspellcheck.egg-info/top_level.txt
```

### Comparing `spacyspellcheck-0.0.2/LICENSE` & `spacyspellcheck-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `spacyspellcheck-0.0.2/PKG-INFO` & `spacyspellcheck-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spacyspellcheck
-Version: 0.0.2
+Version: 0.0.3
 Summary: spell check using spacy vocab and in built levenshtein distance
 Home-page: https://github.com/Vishnunkumar/spacyspellcheck
 Author: Vishnu Nandakumar
 Author-email: nkumarvishnu25@gmail.com
 License: MIT license
 Keywords: spacyspellcheck
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `spacyspellcheck-0.0.2/setup.py` & `spacyspellcheck-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import setuptools
 
-with open("README.MD", "r") as fh:
+with open("README.md", "r") as fh:
     long_description = fh.read()
 
 requirements = [            
   'spacy'
 ]
 
 setuptools.setup(
     name="spacyspellcheck",
-    version="0.0.2",
+    version="0.0.3",
     author="Vishnu Nandakumar",
     author_email="nkumarvishnu25@gmail.com",
     description="spell check using spacy vocab and in built levenshtein distance",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url = 'https://github.com/Vishnunkumar/spacyspellcheck',
     packages=[
```

### Comparing `spacyspellcheck-0.0.2/spacyspellcheck/spellcheck.py` & `spacyspellcheck-0.0.3/spacyspellcheck/spellcheck.py`

 * *Files identical despite different names*

### Comparing `spacyspellcheck-0.0.2/spacyspellcheck.egg-info/PKG-INFO` & `spacyspellcheck-0.0.3/spacyspellcheck.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spacyspellcheck
-Version: 0.0.2
+Version: 0.0.3
 Summary: spell check using spacy vocab and in built levenshtein distance
 Home-page: https://github.com/Vishnunkumar/spacyspellcheck
 Author: Vishnu Nandakumar
 Author-email: nkumarvishnu25@gmail.com
 License: MIT license
 Keywords: spacyspellcheck
 Classifier: Development Status :: 3 - Alpha
```

