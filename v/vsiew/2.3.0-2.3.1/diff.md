# Comparing `tmp/vsiew-2.3.0.tar.gz` & `tmp/vsiew-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vsiew-2.3.0.tar", last modified: Tue Jun 20 15:30:12 2023, max compression
+gzip compressed data, was "vsiew-2.3.1.tar", last modified: Tue Jun 20 15:37:15 2023, max compression
```

## Comparing `vsiew-2.3.0.tar` & `vsiew-2.3.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:30:12.515048 vsiew-2.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-20 15:29:44.000000 vsiew-2.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-20 15:30:12.515048 vsiew-2.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-20 15:29:44.000000 vsiew-2.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 15:30:12.515048 vsiew-2.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-20 15:29:44.000000 vsiew-2.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:30:12.511048 vsiew-2.3.0/vsiew/
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-06-20 15:29:44.000000 vsiew-2.3.0/vsiew/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-20 15:29:44.000000 vsiew-2.3.0/vsiew/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-20 15:29:44.000000 vsiew-2.3.0/vsiew/_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-06-20 15:29:44.000000 vsiew-2.3.0/vsiew/init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:30:12.515048 vsiew-2.3.0/vsiew.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-20 15:30:12.000000 vsiew-2.3.0/vsiew.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-20 15:30:12.000000 vsiew-2.3.0/vsiew.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 15:30:12.000000 vsiew-2.3.0/vsiew.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-20 15:30:12.000000 vsiew-2.3.0/vsiew.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-20 15:30:12.000000 vsiew-2.3.0/vsiew.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-20 15:30:12.000000 vsiew-2.3.0/vsiew.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:37:15.152172 vsiew-2.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-20 15:36:48.000000 vsiew-2.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-20 15:37:15.148172 vsiew-2.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-20 15:36:48.000000 vsiew-2.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 15:37:15.152172 vsiew-2.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-20 15:36:48.000000 vsiew-2.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:37:15.148172 vsiew-2.3.1/vsiew/
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-06-20 15:36:48.000000 vsiew-2.3.1/vsiew/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-20 15:36:48.000000 vsiew-2.3.1/vsiew/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-20 15:36:48.000000 vsiew-2.3.1/vsiew/_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-06-20 15:36:48.000000 vsiew-2.3.1/vsiew/init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:37:15.148172 vsiew-2.3.1/vsiew.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-20 15:37:15.000000 vsiew-2.3.1/vsiew.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-20 15:37:15.000000 vsiew-2.3.1/vsiew.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 15:37:15.000000 vsiew-2.3.1/vsiew.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-20 15:37:15.000000 vsiew-2.3.1/vsiew.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-20 15:37:15.000000 vsiew-2.3.1/vsiew.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-20 15:37:15.000000 vsiew-2.3.1/vsiew.egg-info/top_level.txt
```

### Comparing `vsiew-2.3.0/LICENSE` & `vsiew-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vsiew-2.3.0/PKG-INFO` & `vsiew-2.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsiew
-Version: 2.3.0
+Version: 2.3.1
 Summary: VapourSynth packages from Irrational Encoding Wizardry
 Author: Irrational Encoding Wizardry
 Author-email: wizards@encode.moe
 Maintainer: Setsugen no ao
 Maintainer-email: setsugen@setsugen.dev
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry
 Project-URL: Contact, https://discord.gg/qxTxVJGtst
```

### Comparing `vsiew-2.3.0/setup.py` & `vsiew-2.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `vsiew-2.3.0/vsiew/__init__.py` & `vsiew-2.3.1/vsiew/__init__.py`

 * *Files identical despite different names*

### Comparing `vsiew-2.3.0/vsiew/init.py` & `vsiew-2.3.1/vsiew/init.py`

 * *Files identical despite different names*

### Comparing `vsiew-2.3.0/vsiew.egg-info/PKG-INFO` & `vsiew-2.3.1/vsiew.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsiew
-Version: 2.3.0
+Version: 2.3.1
 Summary: VapourSynth packages from Irrational Encoding Wizardry
 Author: Irrational Encoding Wizardry
 Author-email: wizards@encode.moe
 Maintainer: Setsugen no ao
 Maintainer-email: setsugen@setsugen.dev
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry
 Project-URL: Contact, https://discord.gg/qxTxVJGtst
```

