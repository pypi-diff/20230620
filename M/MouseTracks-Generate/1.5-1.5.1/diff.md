# Comparing `tmp/MouseTracks_Generate-1.5.tar.gz` & `tmp/MouseTracks_Generate-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MouseTracks_Generate-1.5.tar", last modified: Tue Jun 20 12:10:57 2023, max compression
+gzip compressed data, was "MouseTracks_Generate-1.5.1.tar", last modified: Tue Jun 20 12:54:35 2023, max compression
```

## Comparing `MouseTracks_Generate-1.5.tar` & `MouseTracks_Generate-1.5.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 12:10:57.630334 MouseTracks_Generate-1.5/
--rw-rw-rw-   0        0        0     1068 2023-06-20 02:28:28.000000 MouseTracks_Generate-1.5/LICENCE
--rw-rw-rw-   0        0        0       90 2023-06-20 05:44:42.000000 MouseTracks_Generate-1.5/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2023-06-20 12:10:57.603982 MouseTracks_Generate-1.5/MouseTracks_Generate/
--rw-rw-rw-   0        0        0      181 2023-06-20 12:08:10.000000 MouseTracks_Generate-1.5/MouseTracks_Generate/__init__.py
--rw-rw-rw-   0        0        0     5346 2023-06-20 12:00:14.000000 MouseTracks_Generate-1.5/MouseTracks_Generate/generate.py
--rw-rw-rw-   0        0        0    80957 2023-06-08 02:12:28.000000 MouseTracks_Generate-1.5/MouseTracks_Generate/length_analysis.csv
--rw-rw-rw-   0        0        0   149928 2023-06-20 02:41:13.000000 MouseTracks_Generate-1.5/MouseTracks_Generate/model2.h5
-drwxrwxrwx   0        0        0        0 2023-06-20 12:10:57.622328 MouseTracks_Generate-1.5/MouseTracks_Generate.egg-info/
--rw-rw-rw-   0        0        0      273 2023-06-20 12:10:57.000000 MouseTracks_Generate-1.5/MouseTracks_Generate.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      385 2023-06-20 12:10:57.000000 MouseTracks_Generate-1.5/MouseTracks_Generate.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 12:10:57.000000 MouseTracks_Generate-1.5/MouseTracks_Generate.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-06-20 12:10:57.000000 MouseTracks_Generate-1.5/MouseTracks_Generate.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-06-20 12:10:57.000000 MouseTracks_Generate-1.5/MouseTracks_Generate.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      273 2023-06-20 12:10:57.630334 MouseTracks_Generate-1.5/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-20 12:10:57.630334 MouseTracks_Generate-1.5/setup.cfg
--rw-rw-rw-   0        0        0      628 2023-06-20 12:10:41.000000 MouseTracks_Generate-1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 12:54:35.347504 MouseTracks_Generate-1.5.1/
+-rw-rw-rw-   0        0        0     1068 2023-06-20 02:28:28.000000 MouseTracks_Generate-1.5.1/LICENCE
+-rw-rw-rw-   0        0        0       90 2023-06-20 05:44:42.000000 MouseTracks_Generate-1.5.1/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2023-06-20 12:54:35.301154 MouseTracks_Generate-1.5.1/MouseTracks_Generate/
+-rw-rw-rw-   0        0        0      177 2023-06-20 12:48:44.000000 MouseTracks_Generate-1.5.1/MouseTracks_Generate/__init__.py
+-rw-rw-rw-   0        0        0     5410 2023-06-20 12:50:50.000000 MouseTracks_Generate-1.5.1/MouseTracks_Generate/generate.py
+-rw-rw-rw-   0        0        0    80957 2023-06-08 02:12:28.000000 MouseTracks_Generate-1.5.1/MouseTracks_Generate/length_analysis.csv
+-rw-rw-rw-   0        0        0   149928 2023-06-20 02:41:13.000000 MouseTracks_Generate-1.5.1/MouseTracks_Generate/model2.h5
+drwxrwxrwx   0        0        0        0 2023-06-20 12:54:35.332407 MouseTracks_Generate-1.5.1/MouseTracks_Generate.egg-info/
+-rw-rw-rw-   0        0        0      275 2023-06-20 12:54:34.000000 MouseTracks_Generate-1.5.1/MouseTracks_Generate.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      385 2023-06-20 12:54:35.000000 MouseTracks_Generate-1.5.1/MouseTracks_Generate.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 12:54:34.000000 MouseTracks_Generate-1.5.1/MouseTracks_Generate.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-06-20 12:54:34.000000 MouseTracks_Generate-1.5.1/MouseTracks_Generate.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-06-20 12:54:34.000000 MouseTracks_Generate-1.5.1/MouseTracks_Generate.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      275 2023-06-20 12:54:35.347504 MouseTracks_Generate-1.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-20 12:54:35.347504 MouseTracks_Generate-1.5.1/setup.cfg
+-rw-rw-rw-   0        0        0      630 2023-06-20 12:54:12.000000 MouseTracks_Generate-1.5.1/setup.py
```

### Comparing `MouseTracks_Generate-1.5/LICENCE` & `MouseTracks_Generate-1.5.1/LICENCE`

 * *Files identical despite different names*

### Comparing `MouseTracks_Generate-1.5/MouseTracks_Generate/generate.py` & `MouseTracks_Generate-1.5.1/MouseTracks_Generate/generate.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pandas as pd
 import os
 import time
 from keras.models import load_model
 import numpy as np
-from typing import List
+from typing import List, Tuple
 import pyautogui
 import os
 import random
 import math
 os.environ["KMP_DUPLICATE_LIB_OK"] = "TRUE"
 os.environ['TF_CPP_MIN_LOG_LEVEL'] = '2'
 
@@ -144,15 +144,18 @@
     for spot in spots:
         pyautogui.moveTo(spot)
     pyautogui.click()
 
 # OUTPUT_DIR = 'generated_actions'
 MODEL_NAME = 'model2.h5'
 
-def generate_trace(endpoints: List[tuple[int, int]]):
+point = Tuple[int, int]
+points = List[point]
+# List[Tuple[int, int]]
+def generate_trace(endpoints: points):
     # load model
     current_dirr = os.path.dirname(__file__)
     file_path = os.path.join(current_dirr, MODEL_NAME)
     autoencoder = load_model(file_path, compile=False)
     steps = len(endpoints)
     for i in range(steps):
         startx, starty = pyautogui.position()
```

### Comparing `MouseTracks_Generate-1.5/MouseTracks_Generate/length_analysis.csv` & `MouseTracks_Generate-1.5.1/MouseTracks_Generate/length_analysis.csv`

 * *Files identical despite different names*

### Comparing `MouseTracks_Generate-1.5/MouseTracks_Generate/model2.h5` & `MouseTracks_Generate-1.5.1/MouseTracks_Generate/model2.h5`

 * *Files identical despite different names*

### Comparing `MouseTracks_Generate-1.5/setup.py` & `MouseTracks_Generate-1.5.1/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('readme.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='MouseTracks_Generate',
-    version='1.5',
+    version='1.5.1',
     author='momo',
     long_description=long_description,
     include_package_data=True,
     packages=setuptools.find_packages(),
     install_requires=[
         'pandas',
         'numpy',
```

