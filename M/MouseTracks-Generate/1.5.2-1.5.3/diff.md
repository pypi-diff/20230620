# Comparing `tmp/MouseTracks_Generate-1.5.2.tar.gz` & `tmp/MouseTracks_Generate-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MouseTracks_Generate-1.5.2.tar", last modified: Tue Jun 20 12:59:14 2023, max compression
+gzip compressed data, was "MouseTracks_Generate-1.5.3.tar", last modified: Tue Jun 20 13:05:58 2023, max compression
```

## Comparing `MouseTracks_Generate-1.5.2.tar` & `MouseTracks_Generate-1.5.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 12:59:14.646101 MouseTracks_Generate-1.5.2/
--rw-rw-rw-   0        0        0     1068 2023-06-20 02:28:28.000000 MouseTracks_Generate-1.5.2/LICENCE
--rw-rw-rw-   0        0        0       90 2023-06-20 05:44:42.000000 MouseTracks_Generate-1.5.2/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2023-06-20 12:59:14.622074 MouseTracks_Generate-1.5.2/MouseTracks_Generate/
--rw-rw-rw-   0        0        0      181 2023-06-20 12:58:16.000000 MouseTracks_Generate-1.5.2/MouseTracks_Generate/__init__.py
--rw-rw-rw-   0        0        0     5410 2023-06-20 12:50:50.000000 MouseTracks_Generate-1.5.2/MouseTracks_Generate/generate.py
--rw-rw-rw-   0        0        0    80957 2023-06-08 02:12:28.000000 MouseTracks_Generate-1.5.2/MouseTracks_Generate/length_analysis.csv
--rw-rw-rw-   0        0        0   149928 2023-06-20 02:41:13.000000 MouseTracks_Generate-1.5.2/MouseTracks_Generate/model2.h5
-drwxrwxrwx   0        0        0        0 2023-06-20 12:59:14.646101 MouseTracks_Generate-1.5.2/MouseTracks_Generate.egg-info/
--rw-rw-rw-   0        0        0      275 2023-06-20 12:59:14.000000 MouseTracks_Generate-1.5.2/MouseTracks_Generate.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      385 2023-06-20 12:59:14.000000 MouseTracks_Generate-1.5.2/MouseTracks_Generate.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 12:59:14.000000 MouseTracks_Generate-1.5.2/MouseTracks_Generate.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-06-20 12:59:14.000000 MouseTracks_Generate-1.5.2/MouseTracks_Generate.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-06-20 12:59:14.000000 MouseTracks_Generate-1.5.2/MouseTracks_Generate.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      275 2023-06-20 12:59:14.646101 MouseTracks_Generate-1.5.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-20 12:59:14.646101 MouseTracks_Generate-1.5.2/setup.cfg
--rw-rw-rw-   0        0        0      630 2023-06-20 12:59:01.000000 MouseTracks_Generate-1.5.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 13:05:58.419756 MouseTracks_Generate-1.5.3/
+-rw-rw-rw-   0        0        0     1068 2023-06-20 02:28:28.000000 MouseTracks_Generate-1.5.3/LICENCE
+-rw-rw-rw-   0        0        0       90 2023-06-20 05:44:42.000000 MouseTracks_Generate-1.5.3/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2023-06-20 13:05:58.388512 MouseTracks_Generate-1.5.3/MouseTracks_Generate/
+-rw-rw-rw-   0        0        0      161 2023-06-20 13:05:06.000000 MouseTracks_Generate-1.5.3/MouseTracks_Generate/__init__.py
+-rw-rw-rw-   0        0        0     5418 2023-06-20 13:04:11.000000 MouseTracks_Generate-1.5.3/MouseTracks_Generate/generate.py
+-rw-rw-rw-   0        0        0    80957 2023-06-08 02:12:28.000000 MouseTracks_Generate-1.5.3/MouseTracks_Generate/length_analysis.csv
+-rw-rw-rw-   0        0        0   149928 2023-06-20 02:41:13.000000 MouseTracks_Generate-1.5.3/MouseTracks_Generate/model2.h5
+drwxrwxrwx   0        0        0        0 2023-06-20 13:05:58.419756 MouseTracks_Generate-1.5.3/MouseTracks_Generate.egg-info/
+-rw-rw-rw-   0        0        0      275 2023-06-20 13:05:58.000000 MouseTracks_Generate-1.5.3/MouseTracks_Generate.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      385 2023-06-20 13:05:58.000000 MouseTracks_Generate-1.5.3/MouseTracks_Generate.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 13:05:58.000000 MouseTracks_Generate-1.5.3/MouseTracks_Generate.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-06-20 13:05:58.000000 MouseTracks_Generate-1.5.3/MouseTracks_Generate.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-06-20 13:05:58.000000 MouseTracks_Generate-1.5.3/MouseTracks_Generate.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      275 2023-06-20 13:05:58.419756 MouseTracks_Generate-1.5.3/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-20 13:05:58.419756 MouseTracks_Generate-1.5.3/setup.cfg
+-rw-rw-rw-   0        0        0      630 2023-06-20 13:05:06.000000 MouseTracks_Generate-1.5.3/setup.py
```

### Comparing `MouseTracks_Generate-1.5.2/LICENCE` & `MouseTracks_Generate-1.5.3/LICENCE`

 * *Files identical despite different names*

### Comparing `MouseTracks_Generate-1.5.2/MouseTracks_Generate/generate.py` & `MouseTracks_Generate-1.5.3/MouseTracks_Generate/generate.py`

 * *Files 0% similar despite different names*

```diff
@@ -147,15 +147,15 @@
 
 # OUTPUT_DIR = 'generated_actions'
 MODEL_NAME = 'model2.h5'
 
 point = Tuple[int, int]
 points = List[point]
 # List[Tuple[int, int]]
-def generate_trace(endpoints: points):
+def generate_trace(endpoints: points)-> None :
     # load model
     current_dirr = os.path.dirname(__file__)
     file_path = os.path.join(current_dirr, MODEL_NAME)
     autoencoder = load_model(file_path, compile=False)
     steps = len(endpoints)
     for i in range(steps):
         startx, starty = pyautogui.position()
```

### Comparing `MouseTracks_Generate-1.5.2/MouseTracks_Generate/length_analysis.csv` & `MouseTracks_Generate-1.5.3/MouseTracks_Generate/length_analysis.csv`

 * *Files identical despite different names*

### Comparing `MouseTracks_Generate-1.5.2/MouseTracks_Generate/model2.h5` & `MouseTracks_Generate-1.5.3/MouseTracks_Generate/model2.h5`

 * *Files identical despite different names*

### Comparing `MouseTracks_Generate-1.5.2/setup.py` & `MouseTracks_Generate-1.5.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('readme.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='MouseTracks_Generate',
-    version='1.5.2',
+    version='1.5.3',
     author='momo',
     long_description=long_description,
     include_package_data=True,
     packages=setuptools.find_packages(),
     install_requires=[
         'pandas',
         'numpy',
```
