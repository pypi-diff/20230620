# Comparing `tmp/spacyspellcheck-0.0.5.tar.gz` & `tmp/spacyspellcheck-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spacyspellcheck-0.0.5.tar", last modified: Tue Jun 20 14:38:37 2023, max compression
+gzip compressed data, was "spacyspellcheck-0.0.6.tar", last modified: Tue Jun 20 14:46:05 2023, max compression
```

## Comparing `spacyspellcheck-0.0.5.tar` & `spacyspellcheck-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:38:37.664010 spacyspellcheck-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-20 14:38:26.000000 spacyspellcheck-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-20 14:38:37.664010 spacyspellcheck-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-20 14:38:26.000000 spacyspellcheck-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-20 14:38:37.668010 spacyspellcheck-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-06-20 14:38:26.000000 spacyspellcheck-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:38:37.664010 spacyspellcheck-0.0.5/spacyspellcheck/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 14:38:26.000000 spacyspellcheck-0.0.5/spacyspellcheck/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-06-20 14:38:26.000000 spacyspellcheck-0.0.5/spacyspellcheck/spellcheck.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:38:37.664010 spacyspellcheck-0.0.5/spacyspellcheck.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-20 14:38:37.000000 spacyspellcheck-0.0.5/spacyspellcheck.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-20 14:38:37.000000 spacyspellcheck-0.0.5/spacyspellcheck.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 14:38:37.000000 spacyspellcheck-0.0.5/spacyspellcheck.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 14:38:37.000000 spacyspellcheck-0.0.5/spacyspellcheck.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-20 14:38:37.000000 spacyspellcheck-0.0.5/spacyspellcheck.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-20 14:38:37.000000 spacyspellcheck-0.0.5/spacyspellcheck.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:46:05.840706 spacyspellcheck-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-20 14:45:55.000000 spacyspellcheck-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-20 14:46:05.840706 spacyspellcheck-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-20 14:45:55.000000 spacyspellcheck-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-20 14:46:05.840706 spacyspellcheck-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-06-20 14:45:55.000000 spacyspellcheck-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:46:05.840706 spacyspellcheck-0.0.6/spacyspellcheck/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 14:45:55.000000 spacyspellcheck-0.0.6/spacyspellcheck/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-06-20 14:45:55.000000 spacyspellcheck-0.0.6/spacyspellcheck/spellcheck.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:46:05.840706 spacyspellcheck-0.0.6/spacyspellcheck.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-20 14:46:05.000000 spacyspellcheck-0.0.6/spacyspellcheck.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-20 14:46:05.000000 spacyspellcheck-0.0.6/spacyspellcheck.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 14:46:05.000000 spacyspellcheck-0.0.6/spacyspellcheck.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 14:46:05.000000 spacyspellcheck-0.0.6/spacyspellcheck.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-20 14:46:05.000000 spacyspellcheck-0.0.6/spacyspellcheck.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-20 14:46:05.000000 spacyspellcheck-0.0.6/spacyspellcheck.egg-info/top_level.txt
```

### Comparing `spacyspellcheck-0.0.5/LICENSE` & `spacyspellcheck-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `spacyspellcheck-0.0.5/PKG-INFO` & `spacyspellcheck-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spacyspellcheck
-Version: 0.0.5
+Version: 0.0.6
 Summary: spell check using spacy vocab and in built levenshtein distance
 Home-page: https://github.com/Vishnunkumar/spacyspellcheck
 Author: Vishnu Nandakumar
 Author-email: nkumarvishnu25@gmail.com
 License: MIT license
 Keywords: spacyspellcheck
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `spacyspellcheck-0.0.5/setup.py` & `spacyspellcheck-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 requirements = [            
   'spacy'
 ]
 
 setuptools.setup(
     name="spacyspellcheck",
-    version="0.0.5",
+    version="0.0.6",
     author="Vishnu Nandakumar",
     author_email="nkumarvishnu25@gmail.com",
     description="spell check using spacy vocab and in built levenshtein distance",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url = 'https://github.com/Vishnunkumar/spacyspellcheck',
     packages=[
```

### Comparing `spacyspellcheck-0.0.5/spacyspellcheck/spellcheck.py` & `spacyspellcheck-0.0.6/spacyspellcheck/spellcheck.py`

 * *Files identical despite different names*

### Comparing `spacyspellcheck-0.0.5/spacyspellcheck.egg-info/PKG-INFO` & `spacyspellcheck-0.0.6/spacyspellcheck.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spacyspellcheck
-Version: 0.0.5
+Version: 0.0.6
 Summary: spell check using spacy vocab and in built levenshtein distance
 Home-page: https://github.com/Vishnunkumar/spacyspellcheck
 Author: Vishnu Nandakumar
 Author-email: nkumarvishnu25@gmail.com
 License: MIT license
 Keywords: spacyspellcheck
 Classifier: Development Status :: 3 - Alpha
```

