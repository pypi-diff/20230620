# Comparing `tmp/rendersrt-0.0.6.tar.gz` & `tmp/rendersrt-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rendersrt-0.0.6.tar", last modified: Thu Jun  8 00:50:45 2023, max compression
+gzip compressed data, was "rendersrt-0.0.7.tar", last modified: Tue Jun 20 08:56:41 2023, max compression
```

## Comparing `rendersrt-0.0.6.tar` & `rendersrt-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 00:50:45.879198 rendersrt-0.0.6/
--rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 rendersrt-0.0.6/LICENSE
--rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 rendersrt-0.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0     1563 2023-06-08 00:50:45.879198 rendersrt-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     3055 2023-05-25 12:05:46.000000 rendersrt-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-08 00:50:45.784274 rendersrt-0.0.6/rendersrt/
--rw-rw-rw-   0        0        0    58891 2023-06-08 00:48:12.000000 rendersrt-0.0.6/rendersrt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-08 00:50:45.876202 rendersrt-0.0.6/rendersrt.egg-info/
--rw-rw-rw-   0        0        0     1563 2023-06-08 00:50:45.000000 rendersrt-0.0.6/rendersrt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2023-06-08 00:50:45.000000 rendersrt-0.0.6/rendersrt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 00:50:45.000000 rendersrt-0.0.6/rendersrt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-06-08 00:50:45.000000 rendersrt-0.0.6/rendersrt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       34 2023-06-08 00:50:45.000000 rendersrt-0.0.6/rendersrt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-08 00:50:45.000000 rendersrt-0.0.6/rendersrt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      147 2023-06-08 00:50:45.883696 rendersrt-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1362 2023-06-07 15:11:16.000000 rendersrt-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 08:56:41.286883 rendersrt-0.0.7/
+-rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 rendersrt-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 rendersrt-0.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     1563 2023-06-20 08:56:41.286883 rendersrt-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3055 2023-05-25 12:05:46.000000 rendersrt-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-20 08:56:41.250174 rendersrt-0.0.7/rendersrt/
+-rw-rw-rw-   0        0        0    67807 2023-06-20 08:46:24.000000 rendersrt-0.0.7/rendersrt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 08:56:41.284639 rendersrt-0.0.7/rendersrt.egg-info/
+-rw-rw-rw-   0        0        0     1563 2023-06-20 08:56:40.000000 rendersrt-0.0.7/rendersrt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2023-06-20 08:56:41.000000 rendersrt-0.0.7/rendersrt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 08:56:40.000000 rendersrt-0.0.7/rendersrt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-06-20 08:56:40.000000 rendersrt-0.0.7/rendersrt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       34 2023-06-20 08:56:40.000000 rendersrt-0.0.7/rendersrt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-20 08:56:40.000000 rendersrt-0.0.7/rendersrt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      147 2023-06-20 08:56:41.289880 rendersrt-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1362 2023-06-07 15:11:16.000000 rendersrt-0.0.7/setup.py
```

### Comparing `rendersrt-0.0.6/LICENSE` & `rendersrt-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `rendersrt-0.0.6/PKG-INFO` & `rendersrt-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rendersrt
-Version: 0.0.6
+Version: 0.0.7
 Summary: a utility for rendering subtitle file into video file
 Home-page: https://github.com/botbahlul/rendersrt
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 botbahlul
```

### Comparing `rendersrt-0.0.6/README.md` & `rendersrt-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `rendersrt-0.0.6/rendersrt.egg-info/PKG-INFO` & `rendersrt-0.0.7/rendersrt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rendersrt
-Version: 0.0.6
+Version: 0.0.7
 Summary: a utility for rendering subtitle file into video file
 Home-page: https://github.com/botbahlul/rendersrt
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 botbahlul
```

### Comparing `rendersrt-0.0.6/setup.py` & `rendersrt-0.0.7/setup.py`

 * *Files identical despite different names*

