# Comparing `tmp/typedattr-0.2.4.tar.gz` & `tmp/typedattr-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typedattr-0.2.4.tar", last modified: Tue Jun 20 10:17:40 2023, max compression
+gzip compressed data, was "typedattr-0.2.5.tar", last modified: Tue Jun 20 10:24:26 2023, max compression
```

## Comparing `typedattr-0.2.4.tar` & `typedattr-0.2.5.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-06-20 10:17:40.275267 typedattr-0.2.4/
--rw-------   0 gings    (14999) lmb-mit   (1061)    11336 2023-03-30 08:00:06.000000 typedattr-0.2.4/LICENSE
--rw-------   0 gings    (14999) lmb-mit   (1061)     5007 2023-06-20 10:17:40.275267 typedattr-0.2.4/PKG-INFO
--rw-------   0 gings    (14999) lmb-mit   (1061)     4207 2023-06-20 10:15:52.000000 typedattr-0.2.4/README.md
--rw-------   0 gings    (14999) lmb-mit   (1061)     2330 2023-03-30 10:16:34.000000 typedattr-0.2.4/pyproject.toml
--rw-------   0 gings    (14999) lmb-mit   (1061)       46 2023-06-20 10:15:52.000000 typedattr-0.2.4/requirements.txt
--rw-------   0 gings    (14999) lmb-mit   (1061)       38 2023-06-20 10:17:40.279267 typedattr-0.2.4/setup.cfg
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-06-20 10:17:40.199266 typedattr-0.2.4/src/
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-06-20 10:17:40.223266 typedattr-0.2.4/src/typedattr/
--rw-------   0 gings    (14999) lmb-mit   (1061)      209 2023-06-20 10:15:52.000000 typedattr-0.2.4/src/typedattr/__init__.py
--rw-------   0 gings    (14999) lmb-mit   (1061)    12187 2023-06-20 10:15:52.000000 typedattr-0.2.4/src/typedattr/_typedattr.py
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)     5520 2023-06-20 10:15:52.000000 typedattr-0.2.4/src/typedattr/const.py
--rw-------   0 gings    (14999) lmb-mit   (1061)      715 2023-06-20 10:15:52.000000 typedattr-0.2.4/src/typedattr/typext.py
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-06-20 10:17:40.271267 typedattr-0.2.4/src/typedattr/utils/
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)       40 2023-06-20 10:15:52.000000 typedattr-0.2.4/src/typedattr/utils/__init__.py
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)     3090 2023-06-20 10:15:52.000000 typedattr-0.2.4/src/typedattr/utils/caching.py
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)      394 2023-06-20 10:15:52.000000 typedattr-0.2.4/src/typedattr/utils/debugging.py
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)      470 2023-06-20 10:15:52.000000 typedattr-0.2.4/src/typedattr/utils/dtime.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     7262 2023-06-20 10:15:52.000000 typedattr-0.2.4/src/typedattr/utils/import_from_source.py
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)     4229 2023-06-20 10:15:52.000000 typedattr-0.2.4/src/typedattr/utils/log.py
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)     9298 2023-06-20 10:15:52.000000 typedattr-0.2.4/src/typedattr/utils/objects.py
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)     1988 2023-06-20 10:15:52.000000 typedattr-0.2.4/src/typedattr/utils/system.py
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-06-20 10:17:40.247267 typedattr-0.2.4/src/typedattr.egg-info/
--rw-------   0 gings    (14999) lmb-mit   (1061)     5007 2023-06-20 10:17:40.000000 typedattr-0.2.4/src/typedattr.egg-info/PKG-INFO
--rw-------   0 gings    (14999) lmb-mit   (1061)      621 2023-06-20 10:17:40.000000 typedattr-0.2.4/src/typedattr.egg-info/SOURCES.txt
--rw-------   0 gings    (14999) lmb-mit   (1061)        1 2023-06-20 10:17:40.000000 typedattr-0.2.4/src/typedattr.egg-info/dependency_links.txt
--rw-------   0 gings    (14999) lmb-mit   (1061)       46 2023-06-20 10:17:40.000000 typedattr-0.2.4/src/typedattr.egg-info/requires.txt
--rw-------   0 gings    (14999) lmb-mit   (1061)       10 2023-06-20 10:17:40.000000 typedattr-0.2.4/src/typedattr.egg-info/top_level.txt
--rw-------   0 gings    (14999) lmb-mit   (1061)        1 2023-06-20 09:35:51.000000 typedattr-0.2.4/src/typedattr.egg-info/zip-safe
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-06-20 10:24:26.283702 typedattr-0.2.5/
+-rw-------   0 gings    (14999) lmb-mit   (1061)    11336 2023-03-30 08:00:06.000000 typedattr-0.2.5/LICENSE
+-rw-------   0 gings    (14999) lmb-mit   (1061)     5007 2023-06-20 10:24:26.283702 typedattr-0.2.5/PKG-INFO
+-rw-------   0 gings    (14999) lmb-mit   (1061)     4207 2023-06-20 10:23:53.000000 typedattr-0.2.5/README.md
+-rw-------   0 gings    (14999) lmb-mit   (1061)     2330 2023-03-30 10:16:34.000000 typedattr-0.2.5/pyproject.toml
+-rw-------   0 gings    (14999) lmb-mit   (1061)       46 2023-06-20 10:23:53.000000 typedattr-0.2.5/requirements.txt
+-rw-------   0 gings    (14999) lmb-mit   (1061)       38 2023-06-20 10:24:26.287702 typedattr-0.2.5/setup.cfg
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-06-20 10:24:26.187700 typedattr-0.2.5/src/
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-06-20 10:24:26.215701 typedattr-0.2.5/src/typedattr/
+-rw-------   0 gings    (14999) lmb-mit   (1061)      209 2023-06-20 10:23:53.000000 typedattr-0.2.5/src/typedattr/__init__.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)    12187 2023-06-20 10:23:53.000000 typedattr-0.2.5/src/typedattr/_typedattr.py
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)     5520 2023-06-20 10:23:53.000000 typedattr-0.2.5/src/typedattr/const.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)      715 2023-06-20 10:23:53.000000 typedattr-0.2.5/src/typedattr/typext.py
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-06-20 10:24:26.279702 typedattr-0.2.5/src/typedattr/utils/
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)       40 2023-06-20 10:23:53.000000 typedattr-0.2.5/src/typedattr/utils/__init__.py
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)     3090 2023-06-20 10:23:53.000000 typedattr-0.2.5/src/typedattr/utils/caching.py
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)      394 2023-06-20 10:23:53.000000 typedattr-0.2.5/src/typedattr/utils/debugging.py
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)      470 2023-06-20 10:23:53.000000 typedattr-0.2.5/src/typedattr/utils/dtime.py
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)      297 2023-06-20 10:23:53.000000 typedattr-0.2.5/src/typedattr/utils/files.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     7262 2023-06-20 10:23:53.000000 typedattr-0.2.5/src/typedattr/utils/import_from_source.py
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)     4229 2023-06-20 10:23:53.000000 typedattr-0.2.5/src/typedattr/utils/log.py
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)     9298 2023-06-20 10:23:53.000000 typedattr-0.2.5/src/typedattr/utils/objects.py
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)     1988 2023-06-20 10:23:53.000000 typedattr-0.2.5/src/typedattr/utils/system.py
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2023-06-20 10:24:26.243701 typedattr-0.2.5/src/typedattr.egg-info/
+-rw-------   0 gings    (14999) lmb-mit   (1061)     5007 2023-06-20 10:24:26.000000 typedattr-0.2.5/src/typedattr.egg-info/PKG-INFO
+-rw-------   0 gings    (14999) lmb-mit   (1061)      650 2023-06-20 10:24:26.000000 typedattr-0.2.5/src/typedattr.egg-info/SOURCES.txt
+-rw-------   0 gings    (14999) lmb-mit   (1061)        1 2023-06-20 10:24:26.000000 typedattr-0.2.5/src/typedattr.egg-info/dependency_links.txt
+-rw-------   0 gings    (14999) lmb-mit   (1061)       46 2023-06-20 10:24:26.000000 typedattr-0.2.5/src/typedattr.egg-info/requires.txt
+-rw-------   0 gings    (14999) lmb-mit   (1061)       10 2023-06-20 10:24:26.000000 typedattr-0.2.5/src/typedattr.egg-info/top_level.txt
+-rw-------   0 gings    (14999) lmb-mit   (1061)        1 2023-06-20 09:35:51.000000 typedattr-0.2.5/src/typedattr.egg-info/zip-safe
```

### Comparing `typedattr-0.2.4/LICENSE` & `typedattr-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `typedattr-0.2.4/PKG-INFO` & `typedattr-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typedattr
-Version: 0.2.4
+Version: 0.2.5
 Summary: Typed conversion of dictionaries to attrs instances
 Author: gingsi
 License: Apache-2.0
 Project-URL: Project-URL, https://github.com/gingsi/typedattr
 Keywords: attrs,typing,dict,attr
 Platform: any
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `typedattr-0.2.4/README.md` & `typedattr-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `typedattr-0.2.4/pyproject.toml` & `typedattr-0.2.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `typedattr-0.2.4/src/typedattr/_typedattr.py` & `typedattr-0.2.5/src/typedattr/_typedattr.py`

 * *Files identical despite different names*

### Comparing `typedattr-0.2.4/src/typedattr/const.py` & `typedattr-0.2.5/src/typedattr/const.py`

 * *Files identical despite different names*

### Comparing `typedattr-0.2.4/src/typedattr/typext.py` & `typedattr-0.2.5/src/typedattr/typext.py`

 * *Files identical despite different names*

### Comparing `typedattr-0.2.4/src/typedattr/utils/caching.py` & `typedattr-0.2.5/src/typedattr/utils/caching.py`

 * *Files identical despite different names*

### Comparing `typedattr-0.2.4/src/typedattr/utils/import_from_source.py` & `typedattr-0.2.5/src/typedattr/utils/import_from_source.py`

 * *Files identical despite different names*

### Comparing `typedattr-0.2.4/src/typedattr/utils/log.py` & `typedattr-0.2.5/src/typedattr/utils/log.py`

 * *Files identical despite different names*

### Comparing `typedattr-0.2.4/src/typedattr/utils/objects.py` & `typedattr-0.2.5/src/typedattr/utils/objects.py`

 * *Files identical despite different names*

### Comparing `typedattr-0.2.4/src/typedattr/utils/system.py` & `typedattr-0.2.5/src/typedattr/utils/system.py`

 * *Files identical despite different names*

### Comparing `typedattr-0.2.4/src/typedattr.egg-info/PKG-INFO` & `typedattr-0.2.5/src/typedattr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typedattr
-Version: 0.2.4
+Version: 0.2.5
 Summary: Typed conversion of dictionaries to attrs instances
 Author: gingsi
 License: Apache-2.0
 Project-URL: Project-URL, https://github.com/gingsi/typedattr
 Keywords: attrs,typing,dict,attr
 Platform: any
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `typedattr-0.2.4/src/typedattr.egg-info/SOURCES.txt` & `typedattr-0.2.5/src/typedattr.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -12,11 +12,12 @@
 src/typedattr.egg-info/requires.txt
 src/typedattr.egg-info/top_level.txt
 src/typedattr.egg-info/zip-safe
 src/typedattr/utils/__init__.py
 src/typedattr/utils/caching.py
 src/typedattr/utils/debugging.py
 src/typedattr/utils/dtime.py
+src/typedattr/utils/files.py
 src/typedattr/utils/import_from_source.py
 src/typedattr/utils/log.py
 src/typedattr/utils/objects.py
 src/typedattr/utils/system.py
```

