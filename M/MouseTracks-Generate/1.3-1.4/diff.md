# Comparing `tmp/MouseTracks_Generate-1.3.tar.gz` & `tmp/MouseTracks_Generate-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MouseTracks_Generate-1.3.tar", last modified: Tue Jun 20 05:46:22 2023, max compression
+gzip compressed data, was "MouseTracks_Generate-1.4.tar", last modified: Tue Jun 20 05:53:04 2023, max compression
```

## Comparing `MouseTracks_Generate-1.3.tar` & `MouseTracks_Generate-1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 05:46:22.063526 MouseTracks_Generate-1.3/
--rw-rw-rw-   0        0        0     1068 2023-06-20 02:28:28.000000 MouseTracks_Generate-1.3/LICENCE
--rw-rw-rw-   0        0        0       90 2023-06-20 05:44:42.000000 MouseTracks_Generate-1.3/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2023-06-20 05:46:22.046541 MouseTracks_Generate-1.3/MouseTracks_Generate/
--rw-rw-rw-   0        0        0      176 2023-06-20 03:41:49.000000 MouseTracks_Generate-1.3/MouseTracks_Generate/__init__.py
--rw-rw-rw-   0        0        0     5323 2023-06-20 05:41:38.000000 MouseTracks_Generate-1.3/MouseTracks_Generate/generate.py
--rw-rw-rw-   0        0        0    80957 2023-06-08 02:12:28.000000 MouseTracks_Generate-1.3/MouseTracks_Generate/length_analysis.csv
--rw-rw-rw-   0        0        0   149928 2023-06-20 02:41:13.000000 MouseTracks_Generate-1.3/MouseTracks_Generate/model2.h5
-drwxrwxrwx   0        0        0        0 2023-06-20 05:46:22.059526 MouseTracks_Generate-1.3/MouseTracks_Generate.egg-info/
--rw-rw-rw-   0        0        0      273 2023-06-20 05:46:21.000000 MouseTracks_Generate-1.3/MouseTracks_Generate.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      385 2023-06-20 05:46:21.000000 MouseTracks_Generate-1.3/MouseTracks_Generate.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 05:46:21.000000 MouseTracks_Generate-1.3/MouseTracks_Generate.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-06-20 05:46:21.000000 MouseTracks_Generate-1.3/MouseTracks_Generate.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-06-20 05:46:21.000000 MouseTracks_Generate-1.3/MouseTracks_Generate.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      273 2023-06-20 05:46:22.062564 MouseTracks_Generate-1.3/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-20 05:46:22.063526 MouseTracks_Generate-1.3/setup.cfg
--rw-rw-rw-   0        0        0      583 2023-06-20 05:46:09.000000 MouseTracks_Generate-1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 05:53:04.459232 MouseTracks_Generate-1.4/
+-rw-rw-rw-   0        0        0     1068 2023-06-20 02:28:28.000000 MouseTracks_Generate-1.4/LICENCE
+-rw-rw-rw-   0        0        0       90 2023-06-20 05:44:42.000000 MouseTracks_Generate-1.4/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2023-06-20 05:53:04.441247 MouseTracks_Generate-1.4/MouseTracks_Generate/
+-rw-rw-rw-   0        0        0      180 2023-06-20 05:52:37.000000 MouseTracks_Generate-1.4/MouseTracks_Generate/__init__.py
+-rw-rw-rw-   0        0        0     5323 2023-06-20 05:41:38.000000 MouseTracks_Generate-1.4/MouseTracks_Generate/generate.py
+-rw-rw-rw-   0        0        0    80957 2023-06-08 02:12:28.000000 MouseTracks_Generate-1.4/MouseTracks_Generate/length_analysis.csv
+-rw-rw-rw-   0        0        0   149928 2023-06-20 02:41:13.000000 MouseTracks_Generate-1.4/MouseTracks_Generate/model2.h5
+drwxrwxrwx   0        0        0        0 2023-06-20 05:53:04.455231 MouseTracks_Generate-1.4/MouseTracks_Generate.egg-info/
+-rw-rw-rw-   0        0        0      273 2023-06-20 05:53:04.000000 MouseTracks_Generate-1.4/MouseTracks_Generate.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      385 2023-06-20 05:53:04.000000 MouseTracks_Generate-1.4/MouseTracks_Generate.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 05:53:04.000000 MouseTracks_Generate-1.4/MouseTracks_Generate.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-06-20 05:53:04.000000 MouseTracks_Generate-1.4/MouseTracks_Generate.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-06-20 05:53:04.000000 MouseTracks_Generate-1.4/MouseTracks_Generate.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      273 2023-06-20 05:53:04.458234 MouseTracks_Generate-1.4/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-20 05:53:04.459232 MouseTracks_Generate-1.4/setup.cfg
+-rw-rw-rw-   0        0        0      583 2023-06-20 05:52:37.000000 MouseTracks_Generate-1.4/setup.py
```

### Comparing `MouseTracks_Generate-1.3/LICENCE` & `MouseTracks_Generate-1.4/LICENCE`

 * *Files identical despite different names*

### Comparing `MouseTracks_Generate-1.3/MouseTracks_Generate/generate.py` & `MouseTracks_Generate-1.4/MouseTracks_Generate/generate.py`

 * *Files identical despite different names*

### Comparing `MouseTracks_Generate-1.3/MouseTracks_Generate/length_analysis.csv` & `MouseTracks_Generate-1.4/MouseTracks_Generate/length_analysis.csv`

 * *Files identical despite different names*

### Comparing `MouseTracks_Generate-1.3/MouseTracks_Generate/model2.h5` & `MouseTracks_Generate-1.4/MouseTracks_Generate/model2.h5`

 * *Files identical despite different names*

### Comparing `MouseTracks_Generate-1.3/setup.py` & `MouseTracks_Generate-1.4/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('readme.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='MouseTracks_Generate',
-    version='1.3',
+    version='1.4',
     author='momo',
     long_description=long_description,
     include_package_data=True,
     packages=setuptools.find_packages(),
     install_requires=[
         'pandas',
         'numpy',
```

