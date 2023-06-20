# Comparing `tmp/MouseTracks_Generate-1.0.tar.gz` & `tmp/MouseTracks_Generate-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MouseTracks_Generate-1.0.tar", last modified: Tue Jun 20 03:42:05 2023, max compression
+gzip compressed data, was "MouseTracks_Generate-1.1.tar", last modified: Tue Jun 20 03:48:07 2023, max compression
```

## Comparing `MouseTracks_Generate-1.0.tar` & `MouseTracks_Generate-1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 03:42:05.096040 MouseTracks_Generate-1.0/
--rw-rw-rw-   0        0        0     1068 2023-06-20 02:28:28.000000 MouseTracks_Generate-1.0/LICENCE
-drwxrwxrwx   0        0        0        0 2023-06-20 03:42:05.078051 MouseTracks_Generate-1.0/MouseTracks_Generate/
--rw-rw-rw-   0        0        0      176 2023-06-20 03:41:49.000000 MouseTracks_Generate-1.0/MouseTracks_Generate/__init__.py
--rw-rw-rw-   0        0        0      541 2023-06-20 03:02:27.000000 MouseTracks_Generate-1.0/MouseTracks_Generate/analysis.py
--rw-rw-rw-   0        0        0     4713 2023-06-20 03:26:17.000000 MouseTracks_Generate-1.0/MouseTracks_Generate/generate.py
-drwxrwxrwx   0        0        0        0 2023-06-20 03:42:05.092049 MouseTracks_Generate-1.0/MouseTracks_Generate.egg-info/
--rw-rw-rw-   0        0        0      273 2023-06-20 03:42:04.000000 MouseTracks_Generate-1.0/MouseTracks_Generate.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      334 2023-06-20 03:42:04.000000 MouseTracks_Generate-1.0/MouseTracks_Generate.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 03:42:04.000000 MouseTracks_Generate-1.0/MouseTracks_Generate.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-06-20 03:42:04.000000 MouseTracks_Generate-1.0/MouseTracks_Generate.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-06-20 03:42:04.000000 MouseTracks_Generate-1.0/MouseTracks_Generate.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      273 2023-06-20 03:42:05.094055 MouseTracks_Generate-1.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-20 03:42:05.096040 MouseTracks_Generate-1.0/setup.cfg
--rw-rw-rw-   0        0        0      551 2023-06-20 03:41:49.000000 MouseTracks_Generate-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 03:48:07.843648 MouseTracks_Generate-1.1/
+-rw-rw-rw-   0        0        0     1068 2023-06-20 02:28:28.000000 MouseTracks_Generate-1.1/LICENCE
+drwxrwxrwx   0        0        0        0 2023-06-20 03:48:07.826629 MouseTracks_Generate-1.1/MouseTracks_Generate/
+-rw-rw-rw-   0        0        0      176 2023-06-20 03:41:49.000000 MouseTracks_Generate-1.1/MouseTracks_Generate/__init__.py
+-rw-rw-rw-   0        0        0      541 2023-06-20 03:02:27.000000 MouseTracks_Generate-1.1/MouseTracks_Generate/analysis.py
+-rw-rw-rw-   0        0        0     4693 2023-06-20 03:47:41.000000 MouseTracks_Generate-1.1/MouseTracks_Generate/generate.py
+drwxrwxrwx   0        0        0        0 2023-06-20 03:48:07.839640 MouseTracks_Generate-1.1/MouseTracks_Generate.egg-info/
+-rw-rw-rw-   0        0        0      273 2023-06-20 03:48:07.000000 MouseTracks_Generate-1.1/MouseTracks_Generate.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      334 2023-06-20 03:48:07.000000 MouseTracks_Generate-1.1/MouseTracks_Generate.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 03:48:07.000000 MouseTracks_Generate-1.1/MouseTracks_Generate.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-06-20 03:48:07.000000 MouseTracks_Generate-1.1/MouseTracks_Generate.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-06-20 03:48:07.000000 MouseTracks_Generate-1.1/MouseTracks_Generate.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      273 2023-06-20 03:48:07.842653 MouseTracks_Generate-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-20 03:48:07.843648 MouseTracks_Generate-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      551 2023-06-20 03:47:55.000000 MouseTracks_Generate-1.1/setup.py
```

### Comparing `MouseTracks_Generate-1.0/LICENCE` & `MouseTracks_Generate-1.1/LICENCE`

 * *Files identical despite different names*

### Comparing `MouseTracks_Generate-1.0/MouseTracks_Generate/analysis.py` & `MouseTracks_Generate-1.1/MouseTracks_Generate/analysis.py`

 * *Files identical despite different names*

### Comparing `MouseTracks_Generate-1.0/MouseTracks_Generate/generate.py` & `MouseTracks_Generate-1.1/MouseTracks_Generate/generate.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,15 +126,15 @@
     pyautogui.click()
 
 OUTPUT_DIR = 'generated_actions'
 MODEL_NAME = 'model2.h5'
 
 def generate_trace(endpoints):
     # load model
-    autoencoder = load_model('TRAINED_MODELS/' + MODEL_NAME, compile=False)
+    autoencoder = load_model(MODEL_NAME, compile=False)
     steps = len(endpoints)
     for i in range(steps):
         startx, starty = pyautogui.position()
         stopx = endpoints[i][0]
         stopy = endpoints[i][1]
         array, length = create_actions(startx, starty, stopx, stopy)
         nsamples, nfeatures = array.shape  # 行数，列数
```

### Comparing `MouseTracks_Generate-1.0/setup.py` & `MouseTracks_Generate-1.1/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='MouseTracks_Generate',
-    version='1.0',
+    version='1.1',
     author='momo',
     long_description=long_description,
     packages=setuptools.find_packages(),
     install_requires=[
         'pandas',
         'numpy',
         'keras',
```

