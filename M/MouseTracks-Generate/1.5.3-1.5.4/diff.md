# Comparing `tmp/MouseTracks_Generate-1.5.3.tar.gz` & `tmp/MouseTracks_Generate-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MouseTracks_Generate-1.5.3.tar", last modified: Tue Jun 20 13:05:58 2023, max compression
+gzip compressed data, was "MouseTracks_Generate-1.5.4.tar", last modified: Tue Jun 20 13:30:18 2023, max compression
```

## Comparing `MouseTracks_Generate-1.5.3.tar` & `MouseTracks_Generate-1.5.4.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 13:05:58.419756 MouseTracks_Generate-1.5.3/
--rw-rw-rw-   0        0        0     1068 2023-06-20 02:28:28.000000 MouseTracks_Generate-1.5.3/LICENCE
--rw-rw-rw-   0        0        0       90 2023-06-20 05:44:42.000000 MouseTracks_Generate-1.5.3/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2023-06-20 13:05:58.388512 MouseTracks_Generate-1.5.3/MouseTracks_Generate/
--rw-rw-rw-   0        0        0      161 2023-06-20 13:05:06.000000 MouseTracks_Generate-1.5.3/MouseTracks_Generate/__init__.py
--rw-rw-rw-   0        0        0     5418 2023-06-20 13:04:11.000000 MouseTracks_Generate-1.5.3/MouseTracks_Generate/generate.py
--rw-rw-rw-   0        0        0    80957 2023-06-08 02:12:28.000000 MouseTracks_Generate-1.5.3/MouseTracks_Generate/length_analysis.csv
--rw-rw-rw-   0        0        0   149928 2023-06-20 02:41:13.000000 MouseTracks_Generate-1.5.3/MouseTracks_Generate/model2.h5
-drwxrwxrwx   0        0        0        0 2023-06-20 13:05:58.419756 MouseTracks_Generate-1.5.3/MouseTracks_Generate.egg-info/
--rw-rw-rw-   0        0        0      275 2023-06-20 13:05:58.000000 MouseTracks_Generate-1.5.3/MouseTracks_Generate.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      385 2023-06-20 13:05:58.000000 MouseTracks_Generate-1.5.3/MouseTracks_Generate.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 13:05:58.000000 MouseTracks_Generate-1.5.3/MouseTracks_Generate.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-06-20 13:05:58.000000 MouseTracks_Generate-1.5.3/MouseTracks_Generate.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-06-20 13:05:58.000000 MouseTracks_Generate-1.5.3/MouseTracks_Generate.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      275 2023-06-20 13:05:58.419756 MouseTracks_Generate-1.5.3/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-20 13:05:58.419756 MouseTracks_Generate-1.5.3/setup.cfg
--rw-rw-rw-   0        0        0      630 2023-06-20 13:05:06.000000 MouseTracks_Generate-1.5.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 13:30:18.595472 MouseTracks_Generate-1.5.4/
+-rw-rw-rw-   0        0        0     1068 2023-06-20 02:28:28.000000 MouseTracks_Generate-1.5.4/LICENCE
+-rw-rw-rw-   0        0        0       90 2023-06-20 05:44:42.000000 MouseTracks_Generate-1.5.4/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2023-06-20 13:30:18.566365 MouseTracks_Generate-1.5.4/MouseTracks_Generate/
+-rw-rw-rw-   0        0        0      161 2023-06-20 13:05:06.000000 MouseTracks_Generate-1.5.4/MouseTracks_Generate/__init__.py
+-rw-rw-rw-   0        0        0     5522 2023-06-20 13:29:42.000000 MouseTracks_Generate-1.5.4/MouseTracks_Generate/generate.py
+-rw-rw-rw-   0        0        0    80957 2023-06-08 02:12:28.000000 MouseTracks_Generate-1.5.4/MouseTracks_Generate/length_analysis.csv
+-rw-rw-rw-   0        0        0   149928 2023-06-20 02:41:13.000000 MouseTracks_Generate-1.5.4/MouseTracks_Generate/model2.h5
+-rw-rw-rw-   0        0        0      112 2023-06-20 13:23:29.000000 MouseTracks_Generate-1.5.4/MouseTracks_Generate/test.py
+drwxrwxrwx   0        0        0        0 2023-06-20 13:30:18.579819 MouseTracks_Generate-1.5.4/MouseTracks_Generate.egg-info/
+-rw-rw-rw-   0        0        0      275 2023-06-20 13:30:18.000000 MouseTracks_Generate-1.5.4/MouseTracks_Generate.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      414 2023-06-20 13:30:18.000000 MouseTracks_Generate-1.5.4/MouseTracks_Generate.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 13:30:18.000000 MouseTracks_Generate-1.5.4/MouseTracks_Generate.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-06-20 13:30:18.000000 MouseTracks_Generate-1.5.4/MouseTracks_Generate.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-06-20 13:30:18.000000 MouseTracks_Generate-1.5.4/MouseTracks_Generate.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      275 2023-06-20 13:30:18.595472 MouseTracks_Generate-1.5.4/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-20 13:30:18.595472 MouseTracks_Generate-1.5.4/setup.cfg
+-rw-rw-rw-   0        0        0      630 2023-06-20 13:29:58.000000 MouseTracks_Generate-1.5.4/setup.py
```

### Comparing `MouseTracks_Generate-1.5.3/LICENCE` & `MouseTracks_Generate-1.5.4/LICENCE`

 * *Files identical despite different names*

### Comparing `MouseTracks_Generate-1.5.3/MouseTracks_Generate/generate.py` & `MouseTracks_Generate-1.5.4/MouseTracks_Generate/generate.py`

 * *Files 2% similar despite different names*

```diff
@@ -155,14 +155,17 @@
     # load model
     current_dirr = os.path.dirname(__file__)
     file_path = os.path.join(current_dirr, MODEL_NAME)
     autoencoder = load_model(file_path, compile=False)
     steps = len(endpoints)
     for i in range(steps):
         startx, starty = pyautogui.position()
+        if len(endpoints[i]) != 2:
+            print('please input right points!')
+            break
         stopx = endpoints[i][0]
         stopy = endpoints[i][1]
         array, length = create_actions(startx, starty, stopx, stopy)
         nsamples, nfeatures = array.shape  # 行数，列数
         # nfeatures = nfeatures - 1
         X = array[:, 0:nfeatures]
         X = X.reshape(-1, 128, 2)
```

### Comparing `MouseTracks_Generate-1.5.3/MouseTracks_Generate/length_analysis.csv` & `MouseTracks_Generate-1.5.4/MouseTracks_Generate/length_analysis.csv`

 * *Files identical despite different names*

### Comparing `MouseTracks_Generate-1.5.3/MouseTracks_Generate/model2.h5` & `MouseTracks_Generate-1.5.4/MouseTracks_Generate/model2.h5`

 * *Files identical despite different names*

### Comparing `MouseTracks_Generate-1.5.3/setup.py` & `MouseTracks_Generate-1.5.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('readme.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='MouseTracks_Generate',
-    version='1.5.3',
+    version='1.5.4',
     author='momo',
     long_description=long_description,
     include_package_data=True,
     packages=setuptools.find_packages(),
     install_requires=[
         'pandas',
         'numpy',
```

