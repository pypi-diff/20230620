# Comparing `tmp/skmetpy-0.2.7.tar.gz` & `tmp/skmetpy-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skmetpy-0.2.7.tar", last modified: Tue Jun 20 10:20:08 2023, max compression
+gzip compressed data, was "skmetpy-0.2.8.tar", last modified: Tue Jun 20 10:22:18 2023, max compression
```

## Comparing `skmetpy-0.2.7.tar` & `skmetpy-0.2.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 10:20:07.998736 skmetpy-0.2.7/
--rw-rw-rw-   0        0        0      259 2023-06-20 10:20:07.997736 skmetpy-0.2.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-20 10:20:07.992731 skmetpy-0.2.7/nunpy/
--rw-rw-rw-   0        0        0       24 2023-06-17 16:06:02.000000 skmetpy-0.2.7/nunpy/__init__.py
--rw-rw-rw-   0        0        0    30825 2023-06-20 10:20:00.000000 skmetpy-0.2.7/nunpy/rechape.py
--rw-rw-rw-   0        0        0       42 2023-06-20 10:20:07.999738 skmetpy-0.2.7/setup.cfg
--rw-rw-rw-   0        0        0      324 2023-06-20 10:20:05.000000 skmetpy-0.2.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-20 10:20:07.996734 skmetpy-0.2.7/skmetpy.egg-info/
--rw-rw-rw-   0        0        0      259 2023-06-20 10:20:07.000000 skmetpy-0.2.7/skmetpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      167 2023-06-20 10:20:07.000000 skmetpy-0.2.7/skmetpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 10:20:07.000000 skmetpy-0.2.7/skmetpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-20 10:20:07.000000 skmetpy-0.2.7/skmetpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-20 10:22:18.487818 skmetpy-0.2.8/
+-rw-rw-rw-   0        0        0      259 2023-06-20 10:22:18.487818 skmetpy-0.2.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-20 10:22:18.482049 skmetpy-0.2.8/nunpy/
+-rw-rw-rw-   0        0        0       24 2023-06-17 16:06:02.000000 skmetpy-0.2.8/nunpy/__init__.py
+-rw-rw-rw-   0        0        0    30825 2023-06-20 10:20:00.000000 skmetpy-0.2.8/nunpy/rechape.py
+-rw-rw-rw-   0        0        0       42 2023-06-20 10:22:18.487818 skmetpy-0.2.8/setup.cfg
+-rw-rw-rw-   0        0        0      324 2023-06-20 10:22:16.000000 skmetpy-0.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 10:22:18.486815 skmetpy-0.2.8/skmetpy.egg-info/
+-rw-rw-rw-   0        0        0      259 2023-06-20 10:22:18.000000 skmetpy-0.2.8/skmetpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      167 2023-06-20 10:22:18.000000 skmetpy-0.2.8/skmetpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 10:22:18.000000 skmetpy-0.2.8/skmetpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-20 10:22:18.000000 skmetpy-0.2.8/skmetpy.egg-info/top_level.txt
```

### Comparing `skmetpy-0.2.7/nunpy/rechape.py` & `skmetpy-0.2.8/nunpy/rechape.py`

 * *Files identical despite different names*

