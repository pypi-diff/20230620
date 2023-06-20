# Comparing `tmp/vsaa-1.8.1.tar.gz` & `tmp/vsaa-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vsaa-1.8.1.tar", last modified: Tue Jun 20 14:42:07 2023, max compression
+gzip compressed data, was "vsaa-1.8.2.tar", last modified: Tue Jun 20 14:47:01 2023, max compression
```

## Comparing `vsaa-1.8.1.tar` & `vsaa-1.8.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:42:07.029135 vsaa-1.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-20 14:41:41.000000 vsaa-1.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-20 14:42:07.029135 vsaa-1.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-20 14:41:41.000000 vsaa-1.8.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-20 14:42:07.033135 vsaa-1.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-06-20 14:41:41.000000 vsaa-1.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:42:07.029135 vsaa-1.8.1/vsaa/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-20 14:41:41.000000 vsaa-1.8.1/vsaa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-20 14:41:41.000000 vsaa-1.8.1/vsaa/_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    10199 2023-06-20 14:41:41.000000 vsaa-1.8.1/vsaa/abstract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:42:07.029135 vsaa-1.8.1/vsaa/antialiasers/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-20 14:41:41.000000 vsaa-1.8.1/vsaa/antialiasers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-06-20 14:41:41.000000 vsaa-1.8.1/vsaa/antialiasers/eedi2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-06-20 14:41:41.000000 vsaa-1.8.1/vsaa/antialiasers/eedi3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-06-20 14:41:41.000000 vsaa-1.8.1/vsaa/antialiasers/nnedi3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-20 14:41:41.000000 vsaa-1.8.1/vsaa/antialiasers/sangnom.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-20 14:41:41.000000 vsaa-1.8.1/vsaa/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    13832 2023-06-20 14:41:41.000000 vsaa-1.8.1/vsaa/funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-20 14:41:41.000000 vsaa-1.8.1/vsaa/mask.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:41:41.000000 vsaa-1.8.1/vsaa/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:42:07.029135 vsaa-1.8.1/vsaa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-20 14:42:07.000000 vsaa-1.8.1/vsaa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-20 14:42:07.000000 vsaa-1.8.1/vsaa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 14:42:07.000000 vsaa-1.8.1/vsaa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-20 14:42:07.000000 vsaa-1.8.1/vsaa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-20 14:42:07.000000 vsaa-1.8.1/vsaa.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:47:01.029363 vsaa-1.8.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-20 14:46:37.000000 vsaa-1.8.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-20 14:47:01.029363 vsaa-1.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-20 14:46:37.000000 vsaa-1.8.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-20 14:47:01.029363 vsaa-1.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-06-20 14:46:37.000000 vsaa-1.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:47:01.025364 vsaa-1.8.2/vsaa/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-20 14:46:37.000000 vsaa-1.8.2/vsaa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-20 14:46:37.000000 vsaa-1.8.2/vsaa/_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10199 2023-06-20 14:46:37.000000 vsaa-1.8.2/vsaa/abstract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:47:01.029363 vsaa-1.8.2/vsaa/antialiasers/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-20 14:46:37.000000 vsaa-1.8.2/vsaa/antialiasers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-06-20 14:46:37.000000 vsaa-1.8.2/vsaa/antialiasers/eedi2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-06-20 14:46:37.000000 vsaa-1.8.2/vsaa/antialiasers/eedi3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-06-20 14:46:37.000000 vsaa-1.8.2/vsaa/antialiasers/nnedi3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-20 14:46:37.000000 vsaa-1.8.2/vsaa/antialiasers/sangnom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-20 14:46:37.000000 vsaa-1.8.2/vsaa/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13832 2023-06-20 14:46:37.000000 vsaa-1.8.2/vsaa/funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-20 14:46:37.000000 vsaa-1.8.2/vsaa/mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:46:37.000000 vsaa-1.8.2/vsaa/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:47:01.025364 vsaa-1.8.2/vsaa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-20 14:47:01.000000 vsaa-1.8.2/vsaa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-20 14:47:01.000000 vsaa-1.8.2/vsaa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 14:47:01.000000 vsaa-1.8.2/vsaa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-20 14:47:01.000000 vsaa-1.8.2/vsaa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-20 14:47:01.000000 vsaa-1.8.2/vsaa.egg-info/top_level.txt
```

### Comparing `vsaa-1.8.1/LICENSE` & `vsaa-1.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vsaa-1.8.1/PKG-INFO` & `vsaa-1.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsaa
-Version: 1.8.1
+Version: 1.8.2
 Summary: VapourSynth anti aliasing and scaling functions
 Author: Setsugen no ao
 Author-email: setsugen@setsugen.dev
 Maintainer: Setsugen no ao
 Maintainer-email: setsugen@setsugen.dev
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/vs-aa
 Project-URL: Documentation, https://vsaa.encode.moe/en/latest/
```

### Comparing `vsaa-1.8.1/setup.cfg` & `vsaa-1.8.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `vsaa-1.8.1/setup.py` & `vsaa-1.8.2/setup.py`

 * *Files identical despite different names*

### Comparing `vsaa-1.8.1/vsaa/abstract.py` & `vsaa-1.8.2/vsaa/abstract.py`

 * *Files identical despite different names*

### Comparing `vsaa-1.8.1/vsaa/antialiasers/eedi2.py` & `vsaa-1.8.2/vsaa/antialiasers/eedi2.py`

 * *Files identical despite different names*

### Comparing `vsaa-1.8.1/vsaa/antialiasers/eedi3.py` & `vsaa-1.8.2/vsaa/antialiasers/eedi3.py`

 * *Files identical despite different names*

### Comparing `vsaa-1.8.1/vsaa/antialiasers/nnedi3.py` & `vsaa-1.8.2/vsaa/antialiasers/nnedi3.py`

 * *Files identical despite different names*

### Comparing `vsaa-1.8.1/vsaa/antialiasers/sangnom.py` & `vsaa-1.8.2/vsaa/antialiasers/sangnom.py`

 * *Files identical despite different names*

### Comparing `vsaa-1.8.1/vsaa/funcs.py` & `vsaa-1.8.2/vsaa/funcs.py`

 * *Files identical despite different names*

### Comparing `vsaa-1.8.1/vsaa/mask.py` & `vsaa-1.8.2/vsaa/mask.py`

 * *Files identical despite different names*

### Comparing `vsaa-1.8.1/vsaa.egg-info/PKG-INFO` & `vsaa-1.8.2/vsaa.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsaa
-Version: 1.8.1
+Version: 1.8.2
 Summary: VapourSynth anti aliasing and scaling functions
 Author: Setsugen no ao
 Author-email: setsugen@setsugen.dev
 Maintainer: Setsugen no ao
 Maintainer-email: setsugen@setsugen.dev
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/vs-aa
 Project-URL: Documentation, https://vsaa.encode.moe/en/latest/
```

