# Comparing `tmp/skmetpy-0.2.9.tar.gz` & `tmp/skmetpy-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skmetpy-0.2.9.tar", last modified: Tue Jun 20 10:25:13 2023, max compression
+gzip compressed data, was "skmetpy-0.3.0.tar", last modified: Tue Jun 20 10:26:29 2023, max compression
```

## Comparing `skmetpy-0.2.9.tar` & `skmetpy-0.3.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 10:25:13.664793 skmetpy-0.2.9/
--rw-rw-rw-   0        0        0      259 2023-06-20 10:25:13.663792 skmetpy-0.2.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-20 10:25:13.658787 skmetpy-0.2.9/nunpy/
--rw-rw-rw-   0        0        0       24 2023-06-17 16:06:02.000000 skmetpy-0.2.9/nunpy/__init__.py
--rw-rw-rw-   0        0        0    30825 2023-06-20 10:20:00.000000 skmetpy-0.2.9/nunpy/rechape.py
--rw-rw-rw-   0        0        0       42 2023-06-20 10:25:13.664793 skmetpy-0.2.9/setup.cfg
--rw-rw-rw-   0        0        0      324 2023-06-20 10:25:05.000000 skmetpy-0.2.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-20 10:25:13.662792 skmetpy-0.2.9/skmetpy.egg-info/
--rw-rw-rw-   0        0        0      259 2023-06-20 10:25:13.000000 skmetpy-0.2.9/skmetpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      167 2023-06-20 10:25:13.000000 skmetpy-0.2.9/skmetpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 10:25:13.000000 skmetpy-0.2.9/skmetpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-20 10:25:13.000000 skmetpy-0.2.9/skmetpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-20 10:26:29.605604 skmetpy-0.3.0/
+-rw-rw-rw-   0        0        0      259 2023-06-20 10:26:29.604604 skmetpy-0.3.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-20 10:26:29.598598 skmetpy-0.3.0/nunpy/
+-rw-rw-rw-   0        0        0       24 2023-06-17 16:06:02.000000 skmetpy-0.3.0/nunpy/__init__.py
+-rw-rw-rw-   0        0        0    30825 2023-06-20 10:20:00.000000 skmetpy-0.3.0/nunpy/rechape.py
+-rw-rw-rw-   0        0        0       42 2023-06-20 10:26:29.605604 skmetpy-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      324 2023-06-20 10:26:27.000000 skmetpy-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 10:26:29.603603 skmetpy-0.3.0/skmetpy.egg-info/
+-rw-rw-rw-   0        0        0      259 2023-06-20 10:26:29.000000 skmetpy-0.3.0/skmetpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      167 2023-06-20 10:26:29.000000 skmetpy-0.3.0/skmetpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 10:26:29.000000 skmetpy-0.3.0/skmetpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-20 10:26:29.000000 skmetpy-0.3.0/skmetpy.egg-info/top_level.txt
```

### Comparing `skmetpy-0.2.9/nunpy/rechape.py` & `skmetpy-0.3.0/nunpy/rechape.py`

 * *Files identical despite different names*

