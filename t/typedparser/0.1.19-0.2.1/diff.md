# Comparing `tmp/typedparser-0.1.19.tar.gz` & `tmp/typedparser-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typedparser-0.1.19.tar", last modified: Thu May 11 09:57:06 2023, max compression
+gzip compressed data, was "typedparser-0.2.1.tar", last modified: Tue Jun 20 09:56:20 2023, max compression
```

## Comparing `typedparser-0.1.19.tar` & `typedparser-0.2.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-05-11 09:57:06.336286 typedparser-0.1.19/
--rw-------   0 gings    (14999) lmb-mit   (1061)    11336 2023-04-24 08:52:38.000000 typedparser-0.1.19/LICENSE
--rw-------   0 gings    (14999) lmb-mit   (1061)     3578 2023-05-11 09:57:06.336286 typedparser-0.1.19/PKG-INFO
--rw-------   0 gings    (14999) lmb-mit   (1061)     2764 2023-05-11 09:56:25.000000 typedparser-0.1.19/README.md
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)     2347 2023-04-24 08:57:37.000000 typedparser-0.1.19/pyproject.toml
--rw-------   0 gings    (14999) lmb-mit   (1061)       10 2023-05-11 09:56:25.000000 typedparser-0.1.19/requirements.txt
--rw-------   0 gings    (14999) lmb-mit   (1061)       38 2023-05-11 09:57:06.336286 typedparser-0.1.19/setup.cfg
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-05-11 09:57:06.284285 typedparser-0.1.19/src/
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-05-11 09:57:06.308285 typedparser-0.1.19/src/typedparser/
--rw-------   0 gings    (14999) lmb-mit   (1061)      246 2023-05-11 09:56:25.000000 typedparser-0.1.19/src/typedparser/__init__.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     3521 2023-05-11 09:56:25.000000 typedparser-0.1.19/src/typedparser/_typedparser.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     2321 2023-05-11 09:56:25.000000 typedparser-0.1.19/src/typedparser/custom_format.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     5406 2023-05-11 09:56:25.000000 typedparser-0.1.19/src/typedparser/funcs.py
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-05-11 09:57:06.332286 typedparser-0.1.19/src/typedparser.egg-info/
--rw-------   0 gings    (14999) lmb-mit   (1061)     3578 2023-05-11 09:57:06.000000 typedparser-0.1.19/src/typedparser.egg-info/PKG-INFO
--rw-------   0 gings    (14999) lmb-mit   (1061)      395 2023-05-11 09:57:06.000000 typedparser-0.1.19/src/typedparser.egg-info/SOURCES.txt
--rw-------   0 gings    (14999) lmb-mit   (1061)        1 2023-05-11 09:57:06.000000 typedparser-0.1.19/src/typedparser.egg-info/dependency_links.txt
--rw-------   0 gings    (14999) lmb-mit   (1061)       10 2023-05-11 09:57:06.000000 typedparser-0.1.19/src/typedparser.egg-info/requires.txt
--rw-------   0 gings    (14999) lmb-mit   (1061)       12 2023-05-11 09:57:06.000000 typedparser-0.1.19/src/typedparser.egg-info/top_level.txt
--rw-------   0 gings    (14999) lmb-mit   (1061)        1 2023-04-24 09:16:04.000000 typedparser-0.1.19/src/typedparser.egg-info/zip-safe
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-06-20 09:56:20.992917 typedparser-0.2.1/
+-rw-------   0 gings    (14999) lmb-mit   (1061)    11336 2023-04-24 08:52:38.000000 typedparser-0.2.1/LICENSE
+-rw-------   0 gings    (14999) lmb-mit   (1061)     3577 2023-06-20 09:56:20.988917 typedparser-0.2.1/PKG-INFO
+-rw-------   0 gings    (14999) lmb-mit   (1061)     2764 2023-06-20 09:54:26.000000 typedparser-0.2.1/README.md
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)     2347 2023-04-24 08:57:37.000000 typedparser-0.2.1/pyproject.toml
+-rw-------   0 gings    (14999) lmb-mit   (1061)       10 2023-06-20 09:54:26.000000 typedparser-0.2.1/requirements.txt
+-rw-------   0 gings    (14999) lmb-mit   (1061)       38 2023-06-20 09:56:20.992917 typedparser-0.2.1/setup.cfg
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-06-20 09:56:20.940916 typedparser-0.2.1/src/
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-06-20 09:56:20.964916 typedparser-0.2.1/src/typedparser/
+-rw-------   0 gings    (14999) lmb-mit   (1061)      245 2023-06-20 09:54:25.000000 typedparser-0.2.1/src/typedparser/__init__.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     3518 2023-06-20 09:54:25.000000 typedparser-0.2.1/src/typedparser/_typedparser.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     2321 2023-06-20 09:54:25.000000 typedparser-0.2.1/src/typedparser/custom_format.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     5406 2023-06-20 09:54:25.000000 typedparser-0.2.1/src/typedparser/funcs.py
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-06-20 09:56:20.984917 typedparser-0.2.1/src/typedparser.egg-info/
+-rw-------   0 gings    (14999) lmb-mit   (1061)     3577 2023-06-20 09:56:20.000000 typedparser-0.2.1/src/typedparser.egg-info/PKG-INFO
+-rw-------   0 gings    (14999) lmb-mit   (1061)      395 2023-06-20 09:56:20.000000 typedparser-0.2.1/src/typedparser.egg-info/SOURCES.txt
+-rw-------   0 gings    (14999) lmb-mit   (1061)        1 2023-06-20 09:56:20.000000 typedparser-0.2.1/src/typedparser.egg-info/dependency_links.txt
+-rw-------   0 gings    (14999) lmb-mit   (1061)       10 2023-06-20 09:56:20.000000 typedparser-0.2.1/src/typedparser.egg-info/requires.txt
+-rw-------   0 gings    (14999) lmb-mit   (1061)       12 2023-06-20 09:56:20.000000 typedparser-0.2.1/src/typedparser.egg-info/top_level.txt
+-rw-------   0 gings    (14999) lmb-mit   (1061)        1 2023-06-20 09:55:33.000000 typedparser-0.2.1/src/typedparser.egg-info/zip-safe
```

### Comparing `typedparser-0.1.19/LICENSE` & `typedparser-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `typedparser-0.1.19/PKG-INFO` & `typedparser-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typedparser
-Version: 0.1.19
+Version: 0.2.1
 Summary: Extension for python argparse with typehints and typechecks.
 Author: gingsi
 License: Apache-2.0
 Project-URL: Project-URL, https://github.com/gingsi/typedparser
 Keywords: attrs,typing,dict,attr
 Platform: any
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `typedparser-0.1.19/README.md` & `typedparser-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `typedparser-0.1.19/pyproject.toml` & `typedparser-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `typedparser-0.1.19/src/typedparser/_typedparser.py` & `typedparser-0.2.1/src/typedparser/_typedparser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import argparse
 from dataclasses import dataclass
 from typing import Optional, Any, Type
 
 from attr import field, define
 
-from typedattr.typeutils import AttrsClass
+from typedattr.typext import AttrsClass
 from .custom_format import CustomArgparseFmt
 from .funcs import parse_typed_args, add_typed_args
 
 
 @dataclass
 class TypedParser:
     parser: argparse.ArgumentParser
```

### Comparing `typedparser-0.1.19/src/typedparser/custom_format.py` & `typedparser-0.2.1/src/typedparser/custom_format.py`

 * *Files identical despite different names*

### Comparing `typedparser-0.1.19/src/typedparser/funcs.py` & `typedparser-0.2.1/src/typedparser/funcs.py`

 * *Files identical despite different names*

### Comparing `typedparser-0.1.19/src/typedparser.egg-info/PKG-INFO` & `typedparser-0.2.1/src/typedparser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typedparser
-Version: 0.1.19
+Version: 0.2.1
 Summary: Extension for python argparse with typehints and typechecks.
 Author: gingsi
 License: Apache-2.0
 Project-URL: Project-URL, https://github.com/gingsi/typedparser
 Keywords: attrs,typing,dict,attr
 Platform: any
 Classifier: Development Status :: 3 - Alpha
```

