# Comparing `tmp/MouseTracks_Generate-1.2.tar.gz` & `tmp/MouseTracks_Generate-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MouseTracks_Generate-1.2.tar", last modified: Tue Jun 20 03:54:07 2023, max compression
+gzip compressed data, was "MouseTracks_Generate-1.3.tar", last modified: Tue Jun 20 05:46:22 2023, max compression
```

## Comparing `MouseTracks_Generate-1.2.tar` & `MouseTracks_Generate-1.3.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 03:54:07.653276 MouseTracks_Generate-1.2/
--rw-rw-rw-   0        0        0     1068 2023-06-20 02:28:28.000000 MouseTracks_Generate-1.2/LICENCE
-drwxrwxrwx   0        0        0        0 2023-06-20 03:54:07.637648 MouseTracks_Generate-1.2/MouseTracks_Generate/
--rw-rw-rw-   0        0        0      176 2023-06-20 03:41:49.000000 MouseTracks_Generate-1.2/MouseTracks_Generate/__init__.py
--rw-rw-rw-   0        0        0      541 2023-06-20 03:02:27.000000 MouseTracks_Generate-1.2/MouseTracks_Generate/analysis.py
--rw-rw-rw-   0        0        0     4693 2023-06-20 03:47:41.000000 MouseTracks_Generate-1.2/MouseTracks_Generate/generate.py
-drwxrwxrwx   0        0        0        0 2023-06-20 03:54:07.653276 MouseTracks_Generate-1.2/MouseTracks_Generate.egg-info/
--rw-rw-rw-   0        0        0      273 2023-06-20 03:54:07.000000 MouseTracks_Generate-1.2/MouseTracks_Generate.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      334 2023-06-20 03:54:07.000000 MouseTracks_Generate-1.2/MouseTracks_Generate.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 03:54:07.000000 MouseTracks_Generate-1.2/MouseTracks_Generate.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-06-20 03:54:07.000000 MouseTracks_Generate-1.2/MouseTracks_Generate.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-06-20 03:54:07.000000 MouseTracks_Generate-1.2/MouseTracks_Generate.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      273 2023-06-20 03:54:07.653276 MouseTracks_Generate-1.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-20 03:54:07.653276 MouseTracks_Generate-1.2/setup.cfg
--rw-rw-rw-   0        0        0      551 2023-06-20 03:53:49.000000 MouseTracks_Generate-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 05:46:22.063526 MouseTracks_Generate-1.3/
+-rw-rw-rw-   0        0        0     1068 2023-06-20 02:28:28.000000 MouseTracks_Generate-1.3/LICENCE
+-rw-rw-rw-   0        0        0       90 2023-06-20 05:44:42.000000 MouseTracks_Generate-1.3/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2023-06-20 05:46:22.046541 MouseTracks_Generate-1.3/MouseTracks_Generate/
+-rw-rw-rw-   0        0        0      176 2023-06-20 03:41:49.000000 MouseTracks_Generate-1.3/MouseTracks_Generate/__init__.py
+-rw-rw-rw-   0        0        0     5323 2023-06-20 05:41:38.000000 MouseTracks_Generate-1.3/MouseTracks_Generate/generate.py
+-rw-rw-rw-   0        0        0    80957 2023-06-08 02:12:28.000000 MouseTracks_Generate-1.3/MouseTracks_Generate/length_analysis.csv
+-rw-rw-rw-   0        0        0   149928 2023-06-20 02:41:13.000000 MouseTracks_Generate-1.3/MouseTracks_Generate/model2.h5
+drwxrwxrwx   0        0        0        0 2023-06-20 05:46:22.059526 MouseTracks_Generate-1.3/MouseTracks_Generate.egg-info/
+-rw-rw-rw-   0        0        0      273 2023-06-20 05:46:21.000000 MouseTracks_Generate-1.3/MouseTracks_Generate.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      385 2023-06-20 05:46:21.000000 MouseTracks_Generate-1.3/MouseTracks_Generate.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 05:46:21.000000 MouseTracks_Generate-1.3/MouseTracks_Generate.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-06-20 05:46:21.000000 MouseTracks_Generate-1.3/MouseTracks_Generate.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-06-20 05:46:21.000000 MouseTracks_Generate-1.3/MouseTracks_Generate.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      273 2023-06-20 05:46:22.062564 MouseTracks_Generate-1.3/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-20 05:46:22.063526 MouseTracks_Generate-1.3/setup.cfg
+-rw-rw-rw-   0        0        0      583 2023-06-20 05:46:09.000000 MouseTracks_Generate-1.3/setup.py
```

### Comparing `MouseTracks_Generate-1.2/LICENCE` & `MouseTracks_Generate-1.3/LICENCE`

 * *Files identical despite different names*

### Comparing `MouseTracks_Generate-1.2/MouseTracks_Generate/generate.py` & `MouseTracks_Generate-1.3/MouseTracks_Generate/generate.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,39 @@
 import pandas as pd
 import os
 import time
 from keras.models import load_model
 import numpy as np
 from typing import List
-from analysis import get_length
 import pyautogui
 import os
+import random
+import math
 os.environ["KMP_DUPLICATE_LIB_OK"] = "TRUE"
 os.environ['TF_CPP_MIN_LOG_LEVEL'] = '2'
 
+current_dir = os.path.dirname(__file__)
+file_path = os.path.join(current_dir, 'length_analysis.csv')
+ana = pd.read_csv(file_path)
+ana = ana.sort_values(by='distance')
+y = ana['length'].values
+x = ana['distance'].values
+p = np.polyfit(x, y, 6)
+fx = np.poly1d(p)
+
+
+def get_length(startx ,starty, stopx, stopy):
+    dx = abs(stopx - startx)
+    dy = abs(stopy - starty)
+    distance = int(math.sqrt(dx**2 + dy**2))
+    length = int(fx(distance))
+    length = random.randint(length-10, length+10)
+    return length
+
+
 def create_actions(startx, starty, stopx, stopy):
     length = get_length(startx, starty, stopx, stopy)
 
     x1 = startx
     x2 = stopx
     y1 = starty
     y2 = stopy
@@ -121,20 +141,22 @@
             zero_position = i
             break
     spots = cord[0:zero_position]
     for spot in spots:
         pyautogui.moveTo(spot)
     pyautogui.click()
 
-OUTPUT_DIR = 'generated_actions'
+# OUTPUT_DIR = 'generated_actions'
 MODEL_NAME = 'model2.h5'
 
 def generate_trace(endpoints):
     # load model
-    autoencoder = load_model(MODEL_NAME, compile=False)
+    current_dirr = os.path.dirname(__file__)
+    file_path = os.path.join(current_dirr, MODEL_NAME)
+    autoencoder = load_model(file_path, compile=False)
     steps = len(endpoints)
     for i in range(steps):
         startx, starty = pyautogui.position()
         stopx = endpoints[i][0]
         stopy = endpoints[i][1]
         array, length = create_actions(startx, starty, stopx, stopy)
         nsamples, nfeatures = array.shape  # 行数，列数
```

### Comparing `MouseTracks_Generate-1.2/setup.py` & `MouseTracks_Generate-1.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import setuptools
 
 with open('readme.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='MouseTracks_Generate',
-    version='1.2',
+    version='1.3',
     author='momo',
     long_description=long_description,
+    include_package_data=True,
     packages=setuptools.find_packages(),
     install_requires=[
         'pandas',
         'numpy',
         'keras',
     ],
     classifiers=[
```

