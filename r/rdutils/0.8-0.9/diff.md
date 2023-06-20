# Comparing `tmp/rdutils-0.8.tar.gz` & `tmp/rdutils-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rdutils-0.8.tar", last modified: Fri Feb 14 14:48:57 2020, max compression
+gzip compressed data, was "dist/rdutils-0.9.tar", last modified: Fri Feb 14 15:57:38 2020, max compression
```

## Comparing `rdutils-0.8.tar` & `rdutils-0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 robdupre   (501) staff       (20)        0 2020-02-14 14:48:57.000000 rdutils-0.8/
--rw-r--r--   0 robdupre   (501) staff       (20)      520 2020-02-14 14:48:57.000000 rdutils-0.8/PKG-INFO
--rw-r--r--   0 robdupre   (501) staff       (20)       80 2020-01-15 15:54:32.000000 rdutils-0.8/README.md
-drwxr-xr-x   0 robdupre   (501) staff       (20)        0 2020-02-14 14:48:57.000000 rdutils-0.8/rdutils/
--rw-r--r--   0 robdupre   (501) staff       (20)      295 2020-02-14 14:48:41.000000 rdutils-0.8/rdutils/__init__.py
--rwxr-xr-x   0 robdupre   (501) staff       (20)     1523 2020-01-15 15:54:32.000000 rdutils-0.8/rdutils/get_incrementer.py
--rwxr-xr-x   0 robdupre   (501) staff       (20)     5530 2020-02-14 14:41:19.000000 rdutils-0.8/rdutils/image_sequence_streamer.py
--rwxr-xr-x   0 robdupre   (501) staff       (20)     1963 2020-01-15 15:54:32.000000 rdutils-0.8/rdutils/rtsp_recorder.py
--rwxr-xr-x   0 robdupre   (501) staff       (20)     4354 2020-02-14 14:40:23.000000 rdutils-0.8/rdutils/video_streamer.py
--rwxr-xr-x   0 robdupre   (501) staff       (20)     2717 2020-01-15 15:54:32.000000 rdutils-0.8/rdutils/video_to_images.py
-drwxr-xr-x   0 robdupre   (501) staff       (20)        0 2020-02-14 14:48:57.000000 rdutils-0.8/rdutils.egg-info/
--rw-r--r--   0 robdupre   (501) staff       (20)      520 2020-02-14 14:48:57.000000 rdutils-0.8/rdutils.egg-info/PKG-INFO
--rw-r--r--   0 robdupre   (501) staff       (20)      302 2020-02-14 14:48:57.000000 rdutils-0.8/rdutils.egg-info/SOURCES.txt
--rw-r--r--   0 robdupre   (501) staff       (20)        1 2020-02-14 14:48:57.000000 rdutils-0.8/rdutils.egg-info/dependency_links.txt
--rw-r--r--   0 robdupre   (501) staff       (20)        8 2020-02-14 14:48:57.000000 rdutils-0.8/rdutils.egg-info/top_level.txt
--rw-r--r--   0 robdupre   (501) staff       (20)       38 2020-02-14 14:48:57.000000 rdutils-0.8/setup.cfg
--rw-r--r--   0 robdupre   (501) staff       (20)      714 2020-02-14 14:48:49.000000 rdutils-0.8/setup.py
+drwxr-xr-x   0 robdupre   (501) staff       (20)        0 2020-02-14 15:57:38.000000 rdutils-0.9/
+-rw-r--r--   0 robdupre   (501) staff       (20)      520 2020-02-14 15:57:38.000000 rdutils-0.9/PKG-INFO
+-rw-r--r--   0 robdupre   (501) staff       (20)       80 2020-01-15 15:54:32.000000 rdutils-0.9/README.md
+drwxr-xr-x   0 robdupre   (501) staff       (20)        0 2020-02-14 15:57:38.000000 rdutils-0.9/rdutils/
+-rw-r--r--   0 robdupre   (501) staff       (20)      295 2020-02-14 14:48:41.000000 rdutils-0.9/rdutils/__init__.py
+-rwxr-xr-x   0 robdupre   (501) staff       (20)     1523 2020-01-15 15:54:32.000000 rdutils-0.9/rdutils/get_incrementer.py
+-rwxr-xr-x   0 robdupre   (501) staff       (20)     5530 2020-02-14 14:41:19.000000 rdutils-0.9/rdutils/image_sequence_streamer.py
+-rwxr-xr-x   0 robdupre   (501) staff       (20)     1963 2020-01-15 15:54:32.000000 rdutils-0.9/rdutils/rtsp_recorder.py
+-rwxr-xr-x   0 robdupre   (501) staff       (20)     4350 2020-02-14 15:57:31.000000 rdutils-0.9/rdutils/video_streamer.py
+-rwxr-xr-x   0 robdupre   (501) staff       (20)     2717 2020-01-15 15:54:32.000000 rdutils-0.9/rdutils/video_to_images.py
+drwxr-xr-x   0 robdupre   (501) staff       (20)        0 2020-02-14 15:57:38.000000 rdutils-0.9/rdutils.egg-info/
+-rw-r--r--   0 robdupre   (501) staff       (20)      520 2020-02-14 15:57:37.000000 rdutils-0.9/rdutils.egg-info/PKG-INFO
+-rw-r--r--   0 robdupre   (501) staff       (20)      302 2020-02-14 15:57:37.000000 rdutils-0.9/rdutils.egg-info/SOURCES.txt
+-rw-r--r--   0 robdupre   (501) staff       (20)        1 2020-02-14 15:57:37.000000 rdutils-0.9/rdutils.egg-info/dependency_links.txt
+-rw-r--r--   0 robdupre   (501) staff       (20)        8 2020-02-14 15:57:37.000000 rdutils-0.9/rdutils.egg-info/top_level.txt
+-rw-r--r--   0 robdupre   (501) staff       (20)       38 2020-02-14 15:57:38.000000 rdutils-0.9/setup.cfg
+-rw-r--r--   0 robdupre   (501) staff       (20)      714 2020-02-14 15:57:31.000000 rdutils-0.9/setup.py
```

### Comparing `rdutils-0.8/PKG-INFO` & `rdutils-0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdutils
-Version: 0.8
+Version: 0.9
 Summary: A set of python helper utilities
 Home-page: https://gitlab.com/robdupre/rdutils
 Author: Rob Dupre
 Author-email: robdupre@gmail.com
 License: UNKNOWN
 Description: # rdutils
```

### Comparing `rdutils-0.8/rdutils/get_incrementer.py` & `rdutils-0.9/rdutils/get_incrementer.py`

 * *Files identical despite different names*

### Comparing `rdutils-0.8/rdutils/image_sequence_streamer.py` & `rdutils-0.9/rdutils/image_sequence_streamer.py`

 * *Files identical despite different names*

### Comparing `rdutils-0.8/rdutils/rtsp_recorder.py` & `rdutils-0.9/rdutils/rtsp_recorder.py`

 * *Files identical despite different names*

### Comparing `rdutils-0.8/rdutils/video_streamer.py` & `rdutils-0.9/rdutils/video_streamer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # video_streamer.py
 """Implementation of an RTSP or Video stream reader utilising OpenCV"""
 import cv2
-from rdutils.get_incrementer import get_incrementer
+import time
 import numpy as np
 from threading import Thread
+from rdutils.get_incrementer import get_incrementer
 
-__version__ = '0.4'
+__version__ = '0.5'
 __author__ = 'Rob Dupre (KU)'
 
 
 class VideoStreamer:
     def __init__(self, cam_file_path, frame_size=(None, None), identifier=1, threaded=True):
         """Opens a video file
         :param cam_file_path: string of the video file location or RTSP Stream address (with authentication)
@@ -98,15 +99,14 @@
         :param filename: string filename to save the image
         """
         print('Screenshot Saved')
         cv2.imwrite(get_incrementer(self.counter, 6) + '.png', self.current_frame)
 
 
 if __name__ == '__main__':
-    import time
     cap = VideoStreamer('rtsp://admin:admin@192.168.0.35:8554/channels/1', threaded=False)
     # cap = VideoStreamer('test_data/carpark_timelapse.mp4', threaded=True)
     # cap = VideoStreamer('rtsp://admin:admin@192.168.0.35:8554/channels/1', threaded=True)
     cap.start()
     while cap.open():
         # WILL DO NOTHING IF THREADED
         cap.read()
```

### Comparing `rdutils-0.8/rdutils/video_to_images.py` & `rdutils-0.9/rdutils/video_to_images.py`

 * *Files identical despite different names*

### Comparing `rdutils-0.8/rdutils.egg-info/PKG-INFO` & `rdutils-0.9/rdutils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdutils
-Version: 0.8
+Version: 0.9
 Summary: A set of python helper utilities
 Home-page: https://gitlab.com/robdupre/rdutils
 Author: Rob Dupre
 Author-email: robdupre@gmail.com
 License: UNKNOWN
 Description: # rdutils
```

### Comparing `rdutils-0.8/setup.py` & `rdutils-0.9/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 __author__ = 'Rob Dupre (VCA Technology)'
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='rdutils',
-    version='0.8',
+    version='0.9',
     author="Rob Dupre",
     author_email="robdupre@gmail.com",
     description="A set of python helper utilities",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/robdupre/rdutils",
     packages=setuptools.find_packages(),
```

