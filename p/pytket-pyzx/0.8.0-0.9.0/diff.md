# Comparing `tmp/pytket-pyzx-0.8.0.tar.gz` & `tmp/pytket-pyzx-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytket-pyzx-0.8.0.tar", last modified: Thu Apr  1 10:57:57 2021, max compression
+gzip compressed data, was "pytket-pyzx-0.9.0.tar", last modified: Wed Apr 28 13:30:13 2021, max compression
```

## Comparing `pytket-pyzx-0.8.0.tar` & `pytket-pyzx-0.9.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-01 10:57:57.044271 pytket-pyzx-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (121)       21 2021-04-01 10:54:45.000000 pytket-pyzx-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1630 2021-04-01 10:57:57.044271 pytket-pyzx-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      583 2021-04-01 10:54:45.000000 pytket-pyzx-0.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       67 2021-04-01 10:54:45.000000 pytket-pyzx-0.8.0/_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-01 10:57:57.040271 pytket-pyzx-0.8.0/pytket/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-01 10:57:57.040271 pytket-pyzx-0.8.0/pytket/extensions/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-01 10:57:57.044271 pytket-pyzx-0.8.0/pytket/extensions/pyzx/
--rw-r--r--   0 runner    (1001) docker     (121)      848 2021-04-01 10:54:45.000000 pytket-pyzx-0.8.0/pytket/extensions/pyzx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       67 2021-04-01 10:57:56.000000 pytket-pyzx-0.8.0/pytket/extensions/pyzx/_metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)     4735 2021-04-01 10:54:45.000000 pytket-pyzx-0.8.0/pytket/extensions/pyzx/pyzx_convert.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-01 10:57:57.044271 pytket-pyzx-0.8.0/pytket_pyzx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1630 2021-04-01 10:57:57.000000 pytket-pyzx-0.8.0/pytket_pyzx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      361 2021-04-01 10:57:57.000000 pytket-pyzx-0.8.0/pytket_pyzx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-01 10:57:57.000000 pytket-pyzx-0.8.0/pytket_pyzx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-01 10:57:57.000000 pytket-pyzx-0.8.0/pytket_pyzx.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       26 2021-04-01 10:57:57.000000 pytket-pyzx-0.8.0/pytket_pyzx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2021-04-01 10:57:57.000000 pytket-pyzx-0.8.0/pytket_pyzx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-04-01 10:57:57.044271 pytket-pyzx-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2073 2021-04-01 10:54:45.000000 pytket-pyzx-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-28 13:30:13.517770 pytket-pyzx-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)       21 2021-04-28 13:26:53.000000 pytket-pyzx-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1630 2021-04-28 13:30:13.517770 pytket-pyzx-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      583 2021-04-28 13:26:53.000000 pytket-pyzx-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       67 2021-04-28 13:26:53.000000 pytket-pyzx-0.9.0/_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-28 13:30:13.513770 pytket-pyzx-0.9.0/pytket/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-28 13:30:13.513770 pytket-pyzx-0.9.0/pytket/extensions/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-28 13:30:13.517770 pytket-pyzx-0.9.0/pytket/extensions/pyzx/
+-rw-r--r--   0 runner    (1001) docker     (121)      848 2021-04-28 13:26:53.000000 pytket-pyzx-0.9.0/pytket/extensions/pyzx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       67 2021-04-28 13:30:13.000000 pytket-pyzx-0.9.0/pytket/extensions/pyzx/_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4735 2021-04-28 13:26:53.000000 pytket-pyzx-0.9.0/pytket/extensions/pyzx/pyzx_convert.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-28 13:30:13.517770 pytket-pyzx-0.9.0/pytket_pyzx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1630 2021-04-28 13:30:13.000000 pytket-pyzx-0.9.0/pytket_pyzx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      361 2021-04-28 13:30:13.000000 pytket-pyzx-0.9.0/pytket_pyzx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-28 13:30:13.000000 pytket-pyzx-0.9.0/pytket_pyzx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-28 13:30:13.000000 pytket-pyzx-0.9.0/pytket_pyzx.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       27 2021-04-28 13:30:13.000000 pytket-pyzx-0.9.0/pytket_pyzx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2021-04-28 13:30:13.000000 pytket-pyzx-0.9.0/pytket_pyzx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-04-28 13:30:13.517770 pytket-pyzx-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2074 2021-04-28 13:26:53.000000 pytket-pyzx-0.9.0/setup.py
```

### Comparing `pytket-pyzx-0.8.0/PKG-INFO` & `pytket-pyzx-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytket-pyzx
-Version: 0.8.0
+Version: 0.9.0
 Summary: Extension for pytket, providing translation to and from the PyZX framework
 Home-page: https://github.com/CQCL/pytket-extensions
 Author: Alexander Cowtan
 Author-email: alexander.cowtan@cambridgequantum.com
 License: Apache 2
 Description: # pytket-pyzx
```

### Comparing `pytket-pyzx-0.8.0/README.md` & `pytket-pyzx-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `pytket-pyzx-0.8.0/pytket/extensions/pyzx/__init__.py` & `pytket-pyzx-0.9.0/pytket/extensions/pyzx/__init__.py`

 * *Files identical despite different names*

### Comparing `pytket-pyzx-0.8.0/pytket/extensions/pyzx/pyzx_convert.py` & `pytket-pyzx-0.9.0/pytket/extensions/pyzx/pyzx_convert.py`

 * *Files identical despite different names*

### Comparing `pytket-pyzx-0.8.0/pytket_pyzx.egg-info/PKG-INFO` & `pytket-pyzx-0.9.0/pytket_pyzx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytket-pyzx
-Version: 0.8.0
+Version: 0.9.0
 Summary: Extension for pytket, providing translation to and from the PyZX framework
 Home-page: https://github.com/CQCL/pytket-extensions
 Author: Alexander Cowtan
 Author-email: alexander.cowtan@cambridgequantum.com
 License: Apache 2
 Description: # pytket-pyzx
```

### Comparing `pytket-pyzx-0.8.0/setup.py` & `pytket-pyzx-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     description="Extension for pytket, providing translation to and from the PyZX "
     "framework",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     license="Apache 2",
     packages=find_namespace_packages(include=["pytket.*"]),
     include_package_data=True,
-    install_requires=["pytket ~= 0.9.0", "pyzx ~= 0.6.3"],
+    install_requires=["pytket ~= 0.10.0", "pyzx ~= 0.6.3"],
     classifiers=[
         "Environment :: Console",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "License :: Other/Proprietary License",
         "Operating System :: MacOS :: MacOS X",
```

