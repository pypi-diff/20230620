# Comparing `tmp/skmetpy-0.2.5.tar.gz` & `tmp/skmetpy-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skmetpy-0.2.5.tar", last modified: Tue Jun 20 10:15:57 2023, max compression
+gzip compressed data, was "skmetpy-0.2.6.tar", last modified: Tue Jun 20 10:17:32 2023, max compression
```

## Comparing `skmetpy-0.2.5.tar` & `skmetpy-0.2.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 10:15:57.550246 skmetpy-0.2.5/
--rw-rw-rw-   0        0        0      259 2023-06-20 10:15:57.550246 skmetpy-0.2.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-20 10:15:57.544222 skmetpy-0.2.5/nunpy/
--rw-rw-rw-   0        0        0       24 2023-06-17 16:06:02.000000 skmetpy-0.2.5/nunpy/__init__.py
--rw-rw-rw-   0        0        0    30825 2023-06-20 10:11:41.000000 skmetpy-0.2.5/nunpy/rechape.py
--rw-rw-rw-   0        0        0       42 2023-06-20 10:15:57.550246 skmetpy-0.2.5/setup.cfg
--rw-rw-rw-   0        0        0      324 2023-06-20 10:15:55.000000 skmetpy-0.2.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-20 10:15:57.549243 skmetpy-0.2.5/skmetpy.egg-info/
--rw-rw-rw-   0        0        0      259 2023-06-20 10:15:57.000000 skmetpy-0.2.5/skmetpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      167 2023-06-20 10:15:57.000000 skmetpy-0.2.5/skmetpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 10:15:57.000000 skmetpy-0.2.5/skmetpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-20 10:15:57.000000 skmetpy-0.2.5/skmetpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-20 10:17:32.863427 skmetpy-0.2.6/
+-rw-rw-rw-   0        0        0      259 2023-06-20 10:17:32.863427 skmetpy-0.2.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-20 10:17:32.857692 skmetpy-0.2.6/nunpy/
+-rw-rw-rw-   0        0        0       24 2023-06-17 16:06:02.000000 skmetpy-0.2.6/nunpy/__init__.py
+-rw-rw-rw-   0        0        0    30825 2023-06-20 10:11:41.000000 skmetpy-0.2.6/nunpy/rechape.py
+-rw-rw-rw-   0        0        0       42 2023-06-20 10:17:32.864429 skmetpy-0.2.6/setup.cfg
+-rw-rw-rw-   0        0        0      324 2023-06-20 10:17:31.000000 skmetpy-0.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 10:17:32.862424 skmetpy-0.2.6/skmetpy.egg-info/
+-rw-rw-rw-   0        0        0      259 2023-06-20 10:17:32.000000 skmetpy-0.2.6/skmetpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      167 2023-06-20 10:17:32.000000 skmetpy-0.2.6/skmetpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 10:17:32.000000 skmetpy-0.2.6/skmetpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-20 10:17:32.000000 skmetpy-0.2.6/skmetpy.egg-info/top_level.txt
```

### Comparing `skmetpy-0.2.5/nunpy/rechape.py` & `skmetpy-0.2.6/nunpy/rechape.py`

 * *Files identical despite different names*

