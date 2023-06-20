# Comparing `tmp/namlab_analysis-0.1.0.tar.gz` & `tmp/namlab_analysis-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "namlab_analysis-0.1.0.tar", last modified: Tue Jun 20 00:33:45 2023, max compression
+gzip compressed data, was "namlab_analysis-0.1.1.tar", last modified: Tue Jun 20 00:49:17 2023, max compression
```

## Comparing `namlab_analysis-0.1.0.tar` & `namlab_analysis-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 00:33:45.883605 namlab_analysis-0.1.0/
--rw-rw-rw-   0        0        0      248 2023-06-20 00:33:45.881611 namlab_analysis-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-20 00:33:45.829822 namlab_analysis-0.1.0/namlab_analysis/
--rw-rw-rw-   0        0        0       21 2023-06-19 23:31:01.000000 namlab_analysis-0.1.0/namlab_analysis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 00:33:45.878619 namlab_analysis-0.1.0/namlab_analysis/functions/
--rw-rw-rw-   0        0        0        0 2023-06-20 00:08:19.000000 namlab_analysis-0.1.0/namlab_analysis/functions/__init__.py
--rw-rw-rw-   0        0        0    10594 2023-06-19 23:31:01.000000 namlab_analysis-0.1.0/namlab_analysis/functions/analysis.py
--rw-rw-rw-   0        0        0    12291 2023-06-20 00:26:08.000000 namlab_analysis-0.1.0/namlab_analysis/functions/behavior.py
--rw-rw-rw-   0        0        0    18184 2023-06-20 00:26:08.000000 namlab_analysis-0.1.0/namlab_analysis/functions/data_io.py
--rw-rw-rw-   0        0        0     2600 2023-06-20 00:26:08.000000 namlab_analysis-0.1.0/namlab_analysis/functions/general.py
--rw-rw-rw-   0        0        0    31791 2023-06-19 23:31:01.000000 namlab_analysis-0.1.0/namlab_analysis/functions/nwb.py
--rw-rw-rw-   0        0        0     5504 2023-04-30 22:03:05.000000 namlab_analysis-0.1.0/namlab_analysis/functions/photometry.py
--rw-rw-rw-   0        0        0    31040 2023-06-19 23:31:01.000000 namlab_analysis-0.1.0/namlab_analysis/functions/plot.py
-drwxrwxrwx   0        0        0        0 2023-06-20 00:33:45.858886 namlab_analysis-0.1.0/namlab_analysis.egg-info/
--rw-rw-rw-   0        0        0      248 2023-06-20 00:33:45.000000 namlab_analysis-0.1.0/namlab_analysis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      525 2023-06-20 00:33:45.000000 namlab_analysis-0.1.0/namlab_analysis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 00:33:45.000000 namlab_analysis-0.1.0/namlab_analysis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-19 23:40:39.000000 namlab_analysis-0.1.0/namlab_analysis.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       16 2023-06-20 00:33:45.000000 namlab_analysis-0.1.0/namlab_analysis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-20 00:33:45.883605 namlab_analysis-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      420 2023-06-20 00:33:40.000000 namlab_analysis-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 00:49:17.014282 namlab_analysis-0.1.1/
+-rw-rw-rw-   0        0        0      248 2023-06-20 00:49:17.013284 namlab_analysis-0.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-20 00:49:16.971396 namlab_analysis-0.1.1/namlab_analysis/
+-rw-rw-rw-   0        0        0       21 2023-06-19 23:31:01.000000 namlab_analysis-0.1.1/namlab_analysis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 00:49:17.010325 namlab_analysis-0.1.1/namlab_analysis/functions/
+-rw-rw-rw-   0        0        0        0 2023-06-20 00:08:19.000000 namlab_analysis-0.1.1/namlab_analysis/functions/__init__.py
+-rw-rw-rw-   0        0        0    10594 2023-06-19 23:31:01.000000 namlab_analysis-0.1.1/namlab_analysis/functions/analysis.py
+-rw-rw-rw-   0        0        0    12291 2023-06-20 00:26:08.000000 namlab_analysis-0.1.1/namlab_analysis/functions/behavior.py
+-rw-rw-rw-   0        0        0    18184 2023-06-20 00:26:08.000000 namlab_analysis-0.1.1/namlab_analysis/functions/data_io.py
+-rw-rw-rw-   0        0        0     2600 2023-06-20 00:26:08.000000 namlab_analysis-0.1.1/namlab_analysis/functions/general.py
+-rw-rw-rw-   0        0        0    31791 2023-06-19 23:31:01.000000 namlab_analysis-0.1.1/namlab_analysis/functions/nwb.py
+-rw-rw-rw-   0        0        0     5504 2023-04-30 22:03:05.000000 namlab_analysis-0.1.1/namlab_analysis/functions/photometry.py
+-rw-rw-rw-   0        0        0    31040 2023-06-19 23:31:01.000000 namlab_analysis-0.1.1/namlab_analysis/functions/plot.py
+drwxrwxrwx   0        0        0        0 2023-06-20 00:49:16.986524 namlab_analysis-0.1.1/namlab_analysis.egg-info/
+-rw-rw-rw-   0        0        0      248 2023-06-20 00:49:16.000000 namlab_analysis-0.1.1/namlab_analysis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      525 2023-06-20 00:49:16.000000 namlab_analysis-0.1.1/namlab_analysis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 00:49:16.000000 namlab_analysis-0.1.1/namlab_analysis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-20 00:48:44.000000 namlab_analysis-0.1.1/namlab_analysis.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       16 2023-06-20 00:49:16.000000 namlab_analysis-0.1.1/namlab_analysis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-20 00:49:17.014822 namlab_analysis-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      420 2023-06-20 00:49:04.000000 namlab_analysis-0.1.1/setup.py
```

### Comparing `namlab_analysis-0.1.0/namlab_analysis/functions/analysis.py` & `namlab_analysis-0.1.1/namlab_analysis/functions/analysis.py`

 * *Files identical despite different names*

### Comparing `namlab_analysis-0.1.0/namlab_analysis/functions/behavior.py` & `namlab_analysis-0.1.1/namlab_analysis/functions/behavior.py`

 * *Files identical despite different names*

### Comparing `namlab_analysis-0.1.0/namlab_analysis/functions/data_io.py` & `namlab_analysis-0.1.1/namlab_analysis/functions/data_io.py`

 * *Files identical despite different names*

### Comparing `namlab_analysis-0.1.0/namlab_analysis/functions/general.py` & `namlab_analysis-0.1.1/namlab_analysis/functions/general.py`

 * *Files identical despite different names*

### Comparing `namlab_analysis-0.1.0/namlab_analysis/functions/nwb.py` & `namlab_analysis-0.1.1/namlab_analysis/functions/nwb.py`

 * *Files identical despite different names*

### Comparing `namlab_analysis-0.1.0/namlab_analysis/functions/photometry.py` & `namlab_analysis-0.1.1/namlab_analysis/functions/photometry.py`

 * *Files identical despite different names*

### Comparing `namlab_analysis-0.1.0/namlab_analysis/functions/plot.py` & `namlab_analysis-0.1.1/namlab_analysis/functions/plot.py`

 * *Files identical despite different names*

### Comparing `namlab_analysis-0.1.0/namlab_analysis.egg-info/SOURCES.txt` & `namlab_analysis-0.1.1/namlab_analysis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

