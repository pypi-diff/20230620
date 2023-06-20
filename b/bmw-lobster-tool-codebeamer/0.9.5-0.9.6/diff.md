# Comparing `tmp/bmw-lobster-tool-codebeamer-0.9.5.tar.gz` & `tmp/bmw-lobster-tool-codebeamer-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmw-lobster-tool-codebeamer-0.9.5.tar", last modified: Wed Jun 14 14:03:19 2023, max compression
+gzip compressed data, was "bmw-lobster-tool-codebeamer-0.9.6.tar", last modified: Tue Jun 20 07:30:13 2023, max compression
```

## Comparing `bmw-lobster-tool-codebeamer-0.9.5.tar` & `bmw-lobster-tool-codebeamer-0.9.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-14 14:03:19.757645 bmw-lobster-tool-codebeamer-0.9.5/
--rw-r--r--   0 florian   (1000) florian   (1000)     2181 2023-06-14 14:03:19.757645 bmw-lobster-tool-codebeamer-0.9.5/PKG-INFO
--rw-r--r--   0 florian   (1000) florian   (1000)     1241 2023-06-14 14:03:10.000000 bmw-lobster-tool-codebeamer-0.9.5/README.md
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-14 14:03:19.757645 bmw-lobster-tool-codebeamer-0.9.5/bmw_lobster_tool_codebeamer.egg-info/
--rw-r--r--   0 florian   (1000) florian   (1000)     2181 2023-06-14 14:03:19.000000 bmw-lobster-tool-codebeamer-0.9.5/bmw_lobster_tool_codebeamer.egg-info/PKG-INFO
--rw-r--r--   0 florian   (1000) florian   (1000)      402 2023-06-14 14:03:19.000000 bmw-lobster-tool-codebeamer-0.9.5/bmw_lobster_tool_codebeamer.egg-info/SOURCES.txt
--rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-06-14 14:03:19.000000 bmw-lobster-tool-codebeamer-0.9.5/bmw_lobster_tool_codebeamer.egg-info/dependency_links.txt
--rw-r--r--   0 florian   (1000) florian   (1000)       80 2023-06-14 14:03:19.000000 bmw-lobster-tool-codebeamer-0.9.5/bmw_lobster_tool_codebeamer.egg-info/entry_points.txt
--rw-r--r--   0 florian   (1000) florian   (1000)       39 2023-06-14 14:03:19.000000 bmw-lobster-tool-codebeamer-0.9.5/bmw_lobster_tool_codebeamer.egg-info/requires.txt
--rw-r--r--   0 florian   (1000) florian   (1000)        8 2023-06-14 14:03:19.000000 bmw-lobster-tool-codebeamer-0.9.5/bmw_lobster_tool_codebeamer.egg-info/top_level.txt
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-14 14:03:19.757645 bmw-lobster-tool-codebeamer-0.9.5/lobster/
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-14 14:03:19.757645 bmw-lobster-tool-codebeamer-0.9.5/lobster/tools/
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-14 14:03:19.757645 bmw-lobster-tool-codebeamer-0.9.5/lobster/tools/codebeamer/
--rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-06-14 14:03:19.000000 bmw-lobster-tool-codebeamer-0.9.5/lobster/tools/codebeamer/__init__.py
--rwxr-xr-x   0 florian   (1000) florian   (1000)     9763 2023-06-14 14:03:19.000000 bmw-lobster-tool-codebeamer-0.9.5/lobster/tools/codebeamer/codebeamer.py
--rw-r--r--   0 florian   (1000) florian   (1000)       38 2023-06-14 14:03:19.757645 bmw-lobster-tool-codebeamer-0.9.5/setup.cfg
--rw-r--r--   0 florian   (1000) florian   (1000)     2296 2023-05-08 15:03:18.000000 bmw-lobster-tool-codebeamer-0.9.5/setup.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-20 07:30:13.836885 bmw-lobster-tool-codebeamer-0.9.6/
+-rw-r--r--   0 florian   (1000) florian   (1000)     2181 2023-06-20 07:30:13.836885 bmw-lobster-tool-codebeamer-0.9.6/PKG-INFO
+-rw-r--r--   0 florian   (1000) florian   (1000)     1241 2023-06-14 14:03:10.000000 bmw-lobster-tool-codebeamer-0.9.6/README.md
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-20 07:30:13.836885 bmw-lobster-tool-codebeamer-0.9.6/bmw_lobster_tool_codebeamer.egg-info/
+-rw-r--r--   0 florian   (1000) florian   (1000)     2181 2023-06-20 07:30:13.000000 bmw-lobster-tool-codebeamer-0.9.6/bmw_lobster_tool_codebeamer.egg-info/PKG-INFO
+-rw-r--r--   0 florian   (1000) florian   (1000)      402 2023-06-20 07:30:13.000000 bmw-lobster-tool-codebeamer-0.9.6/bmw_lobster_tool_codebeamer.egg-info/SOURCES.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-06-20 07:30:13.000000 bmw-lobster-tool-codebeamer-0.9.6/bmw_lobster_tool_codebeamer.egg-info/dependency_links.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)       80 2023-06-20 07:30:13.000000 bmw-lobster-tool-codebeamer-0.9.6/bmw_lobster_tool_codebeamer.egg-info/entry_points.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)       39 2023-06-20 07:30:13.000000 bmw-lobster-tool-codebeamer-0.9.6/bmw_lobster_tool_codebeamer.egg-info/requires.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)        8 2023-06-20 07:30:13.000000 bmw-lobster-tool-codebeamer-0.9.6/bmw_lobster_tool_codebeamer.egg-info/top_level.txt
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-20 07:30:13.836885 bmw-lobster-tool-codebeamer-0.9.6/lobster/
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-20 07:30:13.836885 bmw-lobster-tool-codebeamer-0.9.6/lobster/tools/
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-20 07:30:13.836885 bmw-lobster-tool-codebeamer-0.9.6/lobster/tools/codebeamer/
+-rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-06-20 07:30:13.000000 bmw-lobster-tool-codebeamer-0.9.6/lobster/tools/codebeamer/__init__.py
+-rwxr-xr-x   0 florian   (1000) florian   (1000)     9763 2023-06-20 07:30:13.000000 bmw-lobster-tool-codebeamer-0.9.6/lobster/tools/codebeamer/codebeamer.py
+-rw-r--r--   0 florian   (1000) florian   (1000)       38 2023-06-20 07:30:13.836885 bmw-lobster-tool-codebeamer-0.9.6/setup.cfg
+-rw-r--r--   0 florian   (1000) florian   (1000)     2296 2023-05-08 15:03:18.000000 bmw-lobster-tool-codebeamer-0.9.6/setup.py
```

### Comparing `bmw-lobster-tool-codebeamer-0.9.5/PKG-INFO` & `bmw-lobster-tool-codebeamer-0.9.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmw-lobster-tool-codebeamer
-Version: 0.9.5
+Version: 0.9.6
 Summary: LOBSTER Tool for Codebeamer
 Home-page: https://github.com/bmw-software-engineering/lobster
 Author: Bayerische Motoren Werke Aktiengesellschaft (BMW AG)
 Author-email: florian.schanda@bmw.de
 License: GNU Affero General Public License v3
 Project-URL: Bug Tracker, https://github.com/bmw-software-engineering/lobster/issues
 Project-URL: Documentation, https://github.com/pages/bmw-software-engineering/lobster/
```

### Comparing `bmw-lobster-tool-codebeamer-0.9.5/README.md` & `bmw-lobster-tool-codebeamer-0.9.6/README.md`

 * *Files identical despite different names*

### Comparing `bmw-lobster-tool-codebeamer-0.9.5/bmw_lobster_tool_codebeamer.egg-info/PKG-INFO` & `bmw-lobster-tool-codebeamer-0.9.6/bmw_lobster_tool_codebeamer.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmw-lobster-tool-codebeamer
-Version: 0.9.5
+Version: 0.9.6
 Summary: LOBSTER Tool for Codebeamer
 Home-page: https://github.com/bmw-software-engineering/lobster
 Author: Bayerische Motoren Werke Aktiengesellschaft (BMW AG)
 Author-email: florian.schanda@bmw.de
 License: GNU Affero General Public License v3
 Project-URL: Bug Tracker, https://github.com/bmw-software-engineering/lobster/issues
 Project-URL: Documentation, https://github.com/pages/bmw-software-engineering/lobster/
```

### Comparing `bmw-lobster-tool-codebeamer-0.9.5/lobster/tools/codebeamer/codebeamer.py` & `bmw-lobster-tool-codebeamer-0.9.6/lobster/tools/codebeamer/codebeamer.py`

 * *Files identical despite different names*

### Comparing `bmw-lobster-tool-codebeamer-0.9.5/setup.py` & `bmw-lobster-tool-codebeamer-0.9.6/setup.py`

 * *Files identical despite different names*

