# Comparing `tmp/skmetpy-0.1.9.tar.gz` & `tmp/skmetpy-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skmetpy-0.1.9.tar", last modified: Mon Jun 19 22:43:52 2023, max compression
+gzip compressed data, was "skmetpy-0.2.0.tar", last modified: Mon Jun 19 22:45:49 2023, max compression
```

## Comparing `skmetpy-0.1.9.tar` & `skmetpy-0.2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 22:43:52.173130 skmetpy-0.1.9/
--rw-rw-rw-   0        0        0      259 2023-06-19 22:43:52.171760 skmetpy-0.1.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-19 22:43:52.166757 skmetpy-0.1.9/nunpy/
--rw-rw-rw-   0        0        0       24 2023-06-17 16:06:02.000000 skmetpy-0.1.9/nunpy/__init__.py
--rw-rw-rw-   0        0        0    26428 2023-06-19 22:43:38.000000 skmetpy-0.1.9/nunpy/rechape.py
--rw-rw-rw-   0        0        0       42 2023-06-19 22:43:52.173130 skmetpy-0.1.9/setup.cfg
--rw-rw-rw-   0        0        0      324 2023-06-19 22:43:49.000000 skmetpy-0.1.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-19 22:43:52.170759 skmetpy-0.1.9/skmetpy.egg-info/
--rw-rw-rw-   0        0        0      259 2023-06-19 22:43:52.000000 skmetpy-0.1.9/skmetpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      167 2023-06-19 22:43:52.000000 skmetpy-0.1.9/skmetpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 22:43:52.000000 skmetpy-0.1.9/skmetpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-19 22:43:52.000000 skmetpy-0.1.9/skmetpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-19 22:45:49.272636 skmetpy-0.2.0/
+-rw-rw-rw-   0        0        0      259 2023-06-19 22:45:49.271991 skmetpy-0.2.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-19 22:45:49.265981 skmetpy-0.2.0/nunpy/
+-rw-rw-rw-   0        0        0       24 2023-06-17 16:06:02.000000 skmetpy-0.2.0/nunpy/__init__.py
+-rw-rw-rw-   0        0        0    26428 2023-06-19 22:43:38.000000 skmetpy-0.2.0/nunpy/rechape.py
+-rw-rw-rw-   0        0        0       42 2023-06-19 22:45:49.272636 skmetpy-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      324 2023-06-19 22:45:47.000000 skmetpy-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 22:45:49.270989 skmetpy-0.2.0/skmetpy.egg-info/
+-rw-rw-rw-   0        0        0      259 2023-06-19 22:45:49.000000 skmetpy-0.2.0/skmetpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      167 2023-06-19 22:45:49.000000 skmetpy-0.2.0/skmetpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 22:45:49.000000 skmetpy-0.2.0/skmetpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-19 22:45:49.000000 skmetpy-0.2.0/skmetpy.egg-info/top_level.txt
```

### Comparing `skmetpy-0.1.9/nunpy/rechape.py` & `skmetpy-0.2.0/nunpy/rechape.py`

 * *Files identical despite different names*

