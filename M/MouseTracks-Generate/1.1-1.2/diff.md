# Comparing `tmp/MouseTracks_Generate-1.1.tar.gz` & `tmp/MouseTracks_Generate-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MouseTracks_Generate-1.1.tar", last modified: Tue Jun 20 03:48:07 2023, max compression
+gzip compressed data, was "MouseTracks_Generate-1.2.tar", last modified: Tue Jun 20 03:54:07 2023, max compression
```

## Comparing `MouseTracks_Generate-1.1.tar` & `MouseTracks_Generate-1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 03:48:07.843648 MouseTracks_Generate-1.1/
--rw-rw-rw-   0        0        0     1068 2023-06-20 02:28:28.000000 MouseTracks_Generate-1.1/LICENCE
-drwxrwxrwx   0        0        0        0 2023-06-20 03:48:07.826629 MouseTracks_Generate-1.1/MouseTracks_Generate/
--rw-rw-rw-   0        0        0      176 2023-06-20 03:41:49.000000 MouseTracks_Generate-1.1/MouseTracks_Generate/__init__.py
--rw-rw-rw-   0        0        0      541 2023-06-20 03:02:27.000000 MouseTracks_Generate-1.1/MouseTracks_Generate/analysis.py
--rw-rw-rw-   0        0        0     4693 2023-06-20 03:47:41.000000 MouseTracks_Generate-1.1/MouseTracks_Generate/generate.py
-drwxrwxrwx   0        0        0        0 2023-06-20 03:48:07.839640 MouseTracks_Generate-1.1/MouseTracks_Generate.egg-info/
--rw-rw-rw-   0        0        0      273 2023-06-20 03:48:07.000000 MouseTracks_Generate-1.1/MouseTracks_Generate.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      334 2023-06-20 03:48:07.000000 MouseTracks_Generate-1.1/MouseTracks_Generate.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 03:48:07.000000 MouseTracks_Generate-1.1/MouseTracks_Generate.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-06-20 03:48:07.000000 MouseTracks_Generate-1.1/MouseTracks_Generate.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-06-20 03:48:07.000000 MouseTracks_Generate-1.1/MouseTracks_Generate.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      273 2023-06-20 03:48:07.842653 MouseTracks_Generate-1.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-20 03:48:07.843648 MouseTracks_Generate-1.1/setup.cfg
--rw-rw-rw-   0        0        0      551 2023-06-20 03:47:55.000000 MouseTracks_Generate-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 03:54:07.653276 MouseTracks_Generate-1.2/
+-rw-rw-rw-   0        0        0     1068 2023-06-20 02:28:28.000000 MouseTracks_Generate-1.2/LICENCE
+drwxrwxrwx   0        0        0        0 2023-06-20 03:54:07.637648 MouseTracks_Generate-1.2/MouseTracks_Generate/
+-rw-rw-rw-   0        0        0      176 2023-06-20 03:41:49.000000 MouseTracks_Generate-1.2/MouseTracks_Generate/__init__.py
+-rw-rw-rw-   0        0        0      541 2023-06-20 03:02:27.000000 MouseTracks_Generate-1.2/MouseTracks_Generate/analysis.py
+-rw-rw-rw-   0        0        0     4693 2023-06-20 03:47:41.000000 MouseTracks_Generate-1.2/MouseTracks_Generate/generate.py
+drwxrwxrwx   0        0        0        0 2023-06-20 03:54:07.653276 MouseTracks_Generate-1.2/MouseTracks_Generate.egg-info/
+-rw-rw-rw-   0        0        0      273 2023-06-20 03:54:07.000000 MouseTracks_Generate-1.2/MouseTracks_Generate.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      334 2023-06-20 03:54:07.000000 MouseTracks_Generate-1.2/MouseTracks_Generate.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 03:54:07.000000 MouseTracks_Generate-1.2/MouseTracks_Generate.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-06-20 03:54:07.000000 MouseTracks_Generate-1.2/MouseTracks_Generate.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-06-20 03:54:07.000000 MouseTracks_Generate-1.2/MouseTracks_Generate.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      273 2023-06-20 03:54:07.653276 MouseTracks_Generate-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-20 03:54:07.653276 MouseTracks_Generate-1.2/setup.cfg
+-rw-rw-rw-   0        0        0      551 2023-06-20 03:53:49.000000 MouseTracks_Generate-1.2/setup.py
```

### Comparing `MouseTracks_Generate-1.1/LICENCE` & `MouseTracks_Generate-1.2/LICENCE`

 * *Files identical despite different names*

### Comparing `MouseTracks_Generate-1.1/MouseTracks_Generate/analysis.py` & `MouseTracks_Generate-1.2/MouseTracks_Generate/analysis.py`

 * *Files identical despite different names*

### Comparing `MouseTracks_Generate-1.1/MouseTracks_Generate/generate.py` & `MouseTracks_Generate-1.2/MouseTracks_Generate/generate.py`

 * *Files identical despite different names*

### Comparing `MouseTracks_Generate-1.1/setup.py` & `MouseTracks_Generate-1.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
-with open('README.md', 'r', encoding='utf-8') as fh:
+with open('readme.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='MouseTracks_Generate',
-    version='1.1',
+    version='1.2',
     author='momo',
     long_description=long_description,
     packages=setuptools.find_packages(),
     install_requires=[
         'pandas',
         'numpy',
         'keras',
```

