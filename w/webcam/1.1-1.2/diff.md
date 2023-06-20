# Comparing `tmp/webcam-1.1.tar.gz` & `tmp/webcam-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webcam-1.1.tar", last modified: Tue May  9 10:13:09 2023, max compression
+gzip compressed data, was "webcam-1.2.tar", last modified: Tue Jun 20 14:08:41 2023, max compression
```

## Comparing `webcam-1.1.tar` & `webcam-1.2.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 10:13:09.215116 webcam-1.1/
--rw-rw-rw-   0        0        0     1089 2023-05-04 16:30:34.000000 webcam-1.1/LICENSE
--rw-rw-rw-   0        0        0     4224 2023-05-09 10:13:09.214123 webcam-1.1/PKG-INFO
--rw-rw-rw-   0        0        0     3145 2023-05-09 10:11:35.000000 webcam-1.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-09 10:13:09.215116 webcam-1.1/setup.cfg
--rw-rw-rw-   0        0        0     1321 2023-05-09 10:11:54.000000 webcam-1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-09 10:13:09.191289 webcam-1.1/webcam/
--rw-rw-rw-   0        0        0       42 2023-05-08 10:15:20.000000 webcam-1.1/webcam/__init__.py
--rw-rw-rw-   0        0        0     2687 2023-05-05 12:14:40.000000 webcam-1.1/webcam/_video_webcam.py
--rw-rw-rw-   0        0        0     1812 2023-05-05 10:19:36.000000 webcam-1.1/webcam/_webcam_background.py
--rw-rw-rw-   0        0        0    13307 2023-05-08 13:07:07.000000 webcam-1.1/webcam/webcam.py
-drwxrwxrwx   0        0        0        0 2023-05-09 10:13:09.210958 webcam-1.1/webcam.egg-info/
--rw-rw-rw-   0        0        0     4224 2023-05-09 10:13:09.000000 webcam-1.1/webcam.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      264 2023-05-09 10:13:09.000000 webcam-1.1/webcam.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 10:13:09.000000 webcam-1.1/webcam.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-05-09 10:13:09.000000 webcam-1.1/webcam.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-09 10:13:09.000000 webcam-1.1/webcam.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-20 14:08:41.755682 webcam-1.2/
+-rw-rw-rw-   0        0        0     1089 2023-05-04 16:30:34.000000 webcam-1.2/LICENSE
+-rw-rw-rw-   0        0        0     4224 2023-06-20 14:08:41.754251 webcam-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3145 2023-05-09 10:11:35.000000 webcam-1.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-20 14:08:41.756696 webcam-1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1321 2023-06-20 14:08:30.000000 webcam-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:08:41.690523 webcam-1.2/webcam/
+-rw-rw-rw-   0        0        0       42 2023-05-08 10:15:20.000000 webcam-1.2/webcam/__init__.py
+-rw-rw-rw-   0        0        0     7465 2023-06-20 13:39:41.000000 webcam-1.2/webcam/_perspective_manager.py
+-rw-rw-rw-   0        0        0     2687 2023-05-05 12:14:40.000000 webcam-1.2/webcam/_video_webcam.py
+-rw-rw-rw-   0        0        0     1812 2023-05-05 10:19:36.000000 webcam-1.2/webcam/_webcam_background.py
+-rw-rw-rw-   0        0        0    15396 2023-06-20 14:05:46.000000 webcam-1.2/webcam/webcam.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:08:41.747957 webcam-1.2/webcam.egg-info/
+-rw-rw-rw-   0        0        0     4224 2023-06-20 14:08:41.000000 webcam-1.2/webcam.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      295 2023-06-20 14:08:41.000000 webcam-1.2/webcam.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 14:08:41.000000 webcam-1.2/webcam.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-06-20 14:08:41.000000 webcam-1.2/webcam.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-20 14:08:41.000000 webcam-1.2/webcam.egg-info/top_level.txt
```

### Comparing `webcam-1.1/LICENSE` & `webcam-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `webcam-1.1/PKG-INFO` & `webcam-1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webcam
-Version: 1.1
+Version: 1.2
 Summary: A simple and convenient library to interact with webcams in Python without having to address Hardware Limitations
 Home-page: https://github.com/Eric-Canas/webcam
 Author: Eric-Canas
 Author-email: eric@ericcanas.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `webcam-1.1/README.md` & `webcam-1.2/README.md`

 * *Files identical despite different names*

### Comparing `webcam-1.1/setup.py` & `webcam-1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='webcam',
-    version='1.1',
+    version='1.2',
     author='Eric-Canas',
     author_email='eric@ericcanas.com',
     url='https://github.com/Eric-Canas/webcam',
     description='A simple and convenient library to interact with webcams in Python without having to address Hardware Limitations',
 
     long_description=open('README.md', 'r').read(),
     long_description_content_type='text/markdown',
```

### Comparing `webcam-1.1/webcam/_video_webcam.py` & `webcam-1.2/webcam/_video_webcam.py`

 * *Files identical despite different names*

### Comparing `webcam-1.1/webcam/_webcam_background.py` & `webcam-1.2/webcam/_webcam_background.py`

 * *Files identical despite different names*

### Comparing `webcam-1.1/webcam/webcam.py` & `webcam-1.2/webcam/webcam.py`

 * *Files 24% similar despite different names*

```diff
@@ -16,68 +16,95 @@
 import time
 from typing import Tuple
 
 import os
 
 from webcam._video_webcam import _VideoWebcam
 from webcam._webcam_background import _WebcamBackground
+from webcam._perspective_manager import _PerspectiveManager, _DummyPerspectiveManager
 
 CROP, RESIZE = 'crop', 'resize'
 
 class Webcam:
     def __init__(
         self,
         src: int | str = 0,
         h: int | None = None,
         w: int | None = None,
         as_bgr: bool = False,
         batch_size: int | None = None,
         run_in_background: bool = False,
         max_frame_rate: int | None = None,
         on_aspect_ratio_lost: str = CROP,
+        homography_matrix: np.ndarray | list[list[float], ...] | None = None,
+        crop_on_warping: bool = True
     ):
         """
         Initialize the WebcamReader.
 
         :param src: int or str. The index of the webcam or its path.
         :param h: int or None. Desired height of the frames. If None and `_w` is provided, the aspect ratio will be preserved.
         :param w: int or None. Desired width of the frames. If None and `_h` is provided, the aspect ratio will be preserved.
         :param as_bgr: bool. If True, the frames will be returned in BGR format, otherwise in RGB format.
         :param batch_size: int or None. If not None, the iterator will yield batches of frames (B, H, W, C). If None, the iterator will yield single frames (H, W, C).
         :param run_in_background: bool. If True, the frames will be read in a background thread (speeding up the reading).
         :param max_frame_rate: int or None. The maximum frame rate to read the frames at. If None, there will be no limitations on frame rating.
+        :param on_aspect_ratio_lost: str. What to do if the aspect ratio of the frames is different from the desired aspect ratio. Valid values are: 'crop' and 'resize'.
+        :param homography_matrix: np.ndarray or list[list[float], ...] or None. The homography matrix to warp the frames with.
+        If passed, frames will be warped before any other processing.
+        :param crop_on_warping: bool. Only applied when homography_matrix is given. Determines if there will be visible
+        black perspective boundaries, or if the image will be cropped to hide them. Default: True
         """
         assert on_aspect_ratio_lost in (CROP, RESIZE), f"Invalid value for `on_aspect_ratio_lost`: {on_aspect_ratio_lost}." \
                                                        f" Valid values are: {CROP}, {RESIZE}"
         self._background = run_in_background
         self.on_aspect_ratio_lost = on_aspect_ratio_lost
         # Initialize it for videos if the source is a string and a file exists at the path
         if isinstance(src, str) and os.path.isfile(src):
             self.cap = _VideoWebcam(video_path=src)
         # Otherwise assume it is a webcam (both webcam or RTSP stream)
         else:
             self.cap = cv2.VideoCapture(src) if not run_in_background else _WebcamBackground(src=src).start()
         self.as_bgr = as_bgr
 
+        if homography_matrix is None:
+            self.perspective_manager = None
+        else:
+            self.perspective_manager = _PerspectiveManager(homography_matrix=homography_matrix,
+                                                          default_h=int(self.cap.get(cv2.CAP_PROP_FRAME_HEIGHT)),
+                                                          default_w=int(self.cap.get(cv2.CAP_PROP_FRAME_WIDTH)),
+                                                          crop_boundaries=crop_on_warping)
+
         # Calculate and set output frame size
         self.frame_size_hw = self._calculate_and_set_desired_resolution(h, w)
 
         # Set batch size and frame rate attributes
         self.batch_size = batch_size
         self.start_timestamp = time.time()
         self.max_frame_rate = max_frame_rate
         self.last_frame_timestamp = self.start_timestamp
 
     @property
     def _h(self) -> int:
-        return int(self.cap.get(cv2.CAP_PROP_FRAME_HEIGHT))
+        h = int(self.cap.get(cv2.CAP_PROP_FRAME_HEIGHT))
+        if self.perspective_manager is None:
+            return h
+        w = int(self.cap.get(cv2.CAP_PROP_FRAME_WIDTH))
+        corrected_w, corrected_h = self.perspective_manager.after_warp_image_shape(w=w, h=h)
+        return corrected_h
 
     @property
     def _w(self) -> int:
-        return int(self.cap.get(cv2.CAP_PROP_FRAME_WIDTH))
+        w = int(self.cap.get(cv2.CAP_PROP_FRAME_WIDTH))
+        if self.perspective_manager is None:
+            return w
+        h = int(self.cap.get(cv2.CAP_PROP_FRAME_HEIGHT))
+        corrected_w, corrected_h = self.perspective_manager.after_warp_image_shape(w=w, h=h)
+        return corrected_w
+
 
     @property
     def h(self) -> int:
         return self.frame_size_hw[0]
 
     @property
     def w(self) -> int:
@@ -210,19 +237,21 @@
         :param h: int. The desired height of the output frame.
         :param w: int. The desired width of the output frame.
         :return: np.ndarray. The resized and center-cropped frame.
         """
         current_h, current_w = frame.shape[:2]
         aspect_ratio = current_w / current_h
 
-        # Calculate the new dimensions such that the aspect ratio is preserved
-        if float(h) / w > aspect_ratio:
-            new_h, new_w = h, int(h * aspect_ratio)
+        # Calculate the new dimensions such that the smaller dimension matches the desired size
+        if current_h < current_w:
+            new_h = h
+            new_w = int(np.ceil(new_h * aspect_ratio))
         else:
-            new_w, new_h = w, int(w / aspect_ratio)
+            new_w = w
+            new_h = int(np.ceil(new_w / aspect_ratio))
 
         # Resize the frame to the new dimensions
         frame = cv2.resize(src=frame, dsize=(new_w, new_h))
 
         # Calculate the position of the center crop
         y1, x1 = (new_h - h) // 2, (new_w - w) // 2
         y2, x2 = y1 + h, x1 + w
@@ -237,17 +266,19 @@
         If the webcam's returned frame size is different from the user-set size, the frame is automatically resized.
 
         :return: tuple. A boolean indicating whether the frame was read successfully, and the frame itself.
         """
         ret, frame = self.cap.read()
 
         if ret:
-            # Extract the height and width of the frame
+            # Adjust the perspective (if needed). If homography matrix is not defined it will do nothing
+            if self.perspective_manager is not None:
+                frame = self.perspective_manager.warp(image=frame)
+            # Get the height and width of the frame
             h, w = frame.shape[:2]
-
             # Resize the frame if the webcam's returned frame size is different from the user-set size
             if (h, w) != (self.h, self.w):
                 frame = self._adjust_image_shape(frame=frame, h=self.h, w=self.w)
 
             # Convert the frame from BGR to RGB format if necessary
             if not self.as_bgr:
                 cv2.cvtColor(src=frame, code=cv2.COLOR_BGR2RGB, dst=frame)
```

### Comparing `webcam-1.1/webcam.egg-info/PKG-INFO` & `webcam-1.2/webcam.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webcam
-Version: 1.1
+Version: 1.2
 Summary: A simple and convenient library to interact with webcams in Python without having to address Hardware Limitations
 Home-page: https://github.com/Eric-Canas/webcam
 Author: Eric-Canas
 Author-email: eric@ericcanas.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

