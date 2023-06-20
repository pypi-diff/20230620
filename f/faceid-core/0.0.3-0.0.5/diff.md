# Comparing `tmp/faceid_core-0.0.3.tar.gz` & `tmp/faceid_core-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faceid_core-0.0.3.tar", last modified: Tue Jun 20 12:36:21 2023, max compression
+gzip compressed data, was "faceid_core-0.0.5.tar", last modified: Tue Jun 20 13:00:11 2023, max compression
```

## Comparing `faceid_core-0.0.3.tar` & `faceid_core-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 12:36:21.439496 faceid_core-0.0.3/
--rw-rw-rw-   0        0        0      358 2023-06-20 12:36:21.439496 faceid_core-0.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-20 12:36:21.426685 faceid_core-0.0.3/faceid_core/
--rw-rw-rw-   0        0        0      137 2023-06-20 12:16:38.000000 faceid_core-0.0.3/faceid_core/__init__.py
--rw-rw-rw-   0        0        0      589 2023-06-20 12:11:39.000000 faceid_core-0.0.3/faceid_core/deploy_configuration.py
--rw-rw-rw-   0        0        0     3707 2023-06-20 12:21:29.000000 faceid_core-0.0.3/faceid_core/face_recognition.py
-drwxrwxrwx   0        0        0        0 2023-06-20 12:36:21.439496 faceid_core-0.0.3/faceid_core.egg-info/
--rw-rw-rw-   0        0        0      358 2023-06-20 12:36:21.000000 faceid_core-0.0.3/faceid_core.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      274 2023-06-20 12:36:21.000000 faceid_core-0.0.3/faceid_core.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 12:36:21.000000 faceid_core-0.0.3/faceid_core.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-06-20 12:36:21.000000 faceid_core-0.0.3/faceid_core.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-20 12:36:21.000000 faceid_core-0.0.3/faceid_core.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-20 12:36:21.439496 faceid_core-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      713 2023-06-20 12:36:17.000000 faceid_core-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 13:00:11.642921 faceid_core-0.0.5/
+-rw-rw-rw-   0        0        0      358 2023-06-20 13:00:11.642921 faceid_core-0.0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-20 13:00:11.622716 faceid_core-0.0.5/faceid_core/
+-rw-rw-rw-   0        0        0      137 2023-06-20 12:16:38.000000 faceid_core-0.0.5/faceid_core/__init__.py
+-rw-rw-rw-   0        0        0      589 2023-06-20 12:11:39.000000 faceid_core-0.0.5/faceid_core/deploy_configuration.py
+-rw-rw-rw-   0        0        0     3716 2023-06-20 12:54:07.000000 faceid_core-0.0.5/faceid_core/face_recognition.py
+drwxrwxrwx   0        0        0        0 2023-06-20 13:00:11.642921 faceid_core-0.0.5/faceid_core.egg-info/
+-rw-rw-rw-   0        0        0      358 2023-06-20 13:00:11.000000 faceid_core-0.0.5/faceid_core.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      274 2023-06-20 13:00:11.000000 faceid_core-0.0.5/faceid_core.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 13:00:11.000000 faceid_core-0.0.5/faceid_core.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-06-20 13:00:11.000000 faceid_core-0.0.5/faceid_core.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-20 13:00:11.000000 faceid_core-0.0.5/faceid_core.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-20 13:00:11.642921 faceid_core-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      713 2023-06-20 13:00:00.000000 faceid_core-0.0.5/setup.py
```

### Comparing `faceid_core-0.0.3/faceid_core/deploy_configuration.py` & `faceid_core-0.0.5/faceid_core/deploy_configuration.py`

 * *Files identical despite different names*

### Comparing `faceid_core-0.0.3/faceid_core/face_recognition.py` & `faceid_core-0.0.5/faceid_core/face_recognition.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import cv2
 import insightface
 import numpy as np
 from pathlib import Path
 from sklearn import preprocessing
-import deploy_configuration
+from faceid_core.deploy_configuration import DeployConfig
 
 
 class FaceRecognition:
     def __init__(self, conf_file):
-        self.config = deploy_configuration.DeployConfig(conf_file)
+        self.config = DeployConfig(conf_file)
         self.model = insightface.app.FaceAnalysis()
         self.model.prepare(ctx_id=self.config.gpu_id, det_size=(640, 640))
         self.faces_embedding = list()
         #
         self.load_faces(self.config.face_db)
 
     #
```

### Comparing `faceid_core-0.0.3/setup.py` & `faceid_core-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup_args = dict(
     name='faceid_core',
-    version='0.0.3',
+    version='0.0.5',
     description='Face Recognition',
     long_description_content_type="text/markdown",
     license='MIT',
     packages=find_packages(),
     author='Orhan Salahetdinov',
     author_email='salahetdinovorxan@gmail.com',
     keywords=['FaceId', 'Face Recognition', 'Python 3'],
```

