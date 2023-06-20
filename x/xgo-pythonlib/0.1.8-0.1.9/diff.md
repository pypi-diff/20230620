# Comparing `tmp/xgo-pythonlib-0.1.8.tar.gz` & `tmp/xgo-pythonlib-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xgo-pythonlib-0.1.8.tar", last modified: Mon Jun 19 03:03:48 2023, max compression
+gzip compressed data, was "xgo-pythonlib-0.1.9.tar", last modified: Tue Jun 20 08:23:58 2023, max compression
```

## Comparing `xgo-pythonlib-0.1.8.tar` & `xgo-pythonlib-0.1.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 03:03:48.503513 xgo-pythonlib-0.1.8/
--rw-rw-rw-   0        0        0     2111 2023-06-19 03:03:48.503513 xgo-pythonlib-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     1484 2023-06-14 22:43:47.000000 xgo-pythonlib-0.1.8/README.md
--rw-rw-rw-   0        0        0       42 2023-06-19 03:03:48.503513 xgo-pythonlib-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     3744 2023-06-19 02:58:00.000000 xgo-pythonlib-0.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-19 03:03:48.491381 xgo-pythonlib-0.1.8/xgo_pythonlib.egg-info/
--rw-rw-rw-   0        0        0     2111 2023-06-19 03:03:48.000000 xgo-pythonlib-0.1.8/xgo_pythonlib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      272 2023-06-19 03:03:48.000000 xgo-pythonlib-0.1.8/xgo_pythonlib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 03:03:48.000000 xgo-pythonlib-0.1.8/xgo_pythonlib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-06-19 03:03:48.000000 xgo-pythonlib-0.1.8/xgo_pythonlib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-19 03:03:48.493380 xgo-pythonlib-0.1.8/xgoedu/
--rw-rw-rw-   0        0        0    37464 2023-06-19 03:01:26.000000 xgo-pythonlib-0.1.8/xgoedu/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 03:03:48.495453 xgo-pythonlib-0.1.8/xgolib/
--rw-rw-rw-   0        0        0    26390 2023-06-19 03:02:36.000000 xgo-pythonlib-0.1.8/xgolib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 03:03:48.501506 xgo-pythonlib-0.1.8/xgoscreen/
--rw-rw-rw-   0        0        0     5339 2023-06-07 11:44:32.000000 xgo-pythonlib-0.1.8/xgoscreen/LCD_2inch.py
--rw-rw-rw-   0        0        0        0 2023-06-06 11:56:39.000000 xgo-pythonlib-0.1.8/xgoscreen/__init__.py
--rw-rw-rw-   0        0        0     2214 2023-06-06 01:30:25.000000 xgo-pythonlib-0.1.8/xgoscreen/lcdconfig.py
+drwxrwxrwx   0        0        0        0 2023-06-20 08:23:58.012508 xgo-pythonlib-0.1.9/
+-rw-rw-rw-   0        0        0     2276 2023-06-20 08:23:58.012508 xgo-pythonlib-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1649 2023-06-20 08:21:49.000000 xgo-pythonlib-0.1.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-20 08:23:58.012508 xgo-pythonlib-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     3744 2023-06-20 08:17:37.000000 xgo-pythonlib-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 08:23:58.002011 xgo-pythonlib-0.1.9/xgo_pythonlib.egg-info/
+-rw-rw-rw-   0        0        0     2276 2023-06-20 08:23:57.000000 xgo-pythonlib-0.1.9/xgo_pythonlib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      272 2023-06-20 08:23:57.000000 xgo-pythonlib-0.1.9/xgo_pythonlib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 08:23:57.000000 xgo-pythonlib-0.1.9/xgo_pythonlib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-06-20 08:23:57.000000 xgo-pythonlib-0.1.9/xgo_pythonlib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-20 08:23:58.004020 xgo-pythonlib-0.1.9/xgoedu/
+-rw-rw-rw-   0        0        0    37464 2023-06-20 08:17:19.000000 xgo-pythonlib-0.1.9/xgoedu/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 08:23:58.006017 xgo-pythonlib-0.1.9/xgolib/
+-rw-rw-rw-   0        0        0    26390 2023-06-19 03:02:36.000000 xgo-pythonlib-0.1.9/xgolib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 08:23:58.011018 xgo-pythonlib-0.1.9/xgoscreen/
+-rw-rw-rw-   0        0        0     5339 2023-06-07 11:44:32.000000 xgo-pythonlib-0.1.9/xgoscreen/LCD_2inch.py
+-rw-rw-rw-   0        0        0        0 2023-06-06 11:56:39.000000 xgo-pythonlib-0.1.9/xgoscreen/__init__.py
+-rw-rw-rw-   0        0        0     2214 2023-06-06 01:30:25.000000 xgo-pythonlib-0.1.9/xgoscreen/lcdconfig.py
```

### Comparing `xgo-pythonlib-0.1.8/PKG-INFO` & `xgo-pythonlib-0.1.9/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xgo-pythonlib
-Version: 0.1.8
+Version: 0.1.9
 Summary: PythonLib for XGO2-DOG
 Home-page: https://github.com/Xgorobot/XGO-PythonLib
 Author: luwudynamics
 Author-email: hello@xgorobot.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -56,15 +56,23 @@
 ```
 xgolib library example
 ```python
 from xgolib import XGO
 dog = XGO('xgomini')
 dog.action(1)
 ```
-### Lastest Verion:0.1.7
+### Lastest Verion:0.1.9
 
-### xgolib_version=1.3.1
+### xgolib_version=1.3.3
 
-### xgoedu_version=1.2.3
+### xgoedu_version=1.2.5
+
+## Change Log
+
+## [0.1.9] - 2023-06-20
+
+### Fixed
+
+- Fixed the issue with the xgoTakePhoto method that was causing abnormal RGB colors in the saved photos.
```

### Comparing `xgo-pythonlib-0.1.8/README.md` & `xgo-pythonlib-0.1.9/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -38,15 +38,23 @@
 ```
 xgolib library example
 ```python
 from xgolib import XGO
 dog = XGO('xgomini')
 dog.action(1)
 ```
-### Lastest Verion:0.1.7
+### Lastest Verion:0.1.9
 
-### xgolib_version=1.3.1
+### xgolib_version=1.3.3
 
-### xgoedu_version=1.2.3
+### xgoedu_version=1.2.5
+
+## Change Log
+
+## [0.1.9] - 2023-06-20
+
+### Fixed
+
+- Fixed the issue with the xgoTakePhoto method that was causing abnormal RGB colors in the saved photos.
```

### Comparing `xgo-pythonlib-0.1.8/setup.py` & `xgo-pythonlib-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 NAME = 'xgo-pythonlib'
 DESCRIPTION = 'PythonLib for XGO2-DOG'
 URL = 'https://github.com/Xgorobot/XGO-PythonLib'
 EMAIL = 'hello@xgorobot.com'
 AUTHOR = 'luwudynamics'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.1.8'
+VERSION = '0.1.9'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
 ]
 
 # What packages are optional?
```

### Comparing `xgo-pythonlib-0.1.8/xgo_pythonlib.egg-info/PKG-INFO` & `xgo-pythonlib-0.1.9/xgo_pythonlib.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xgo-pythonlib
-Version: 0.1.8
+Version: 0.1.9
 Summary: PythonLib for XGO2-DOG
 Home-page: https://github.com/Xgorobot/XGO-PythonLib
 Author: luwudynamics
 Author-email: hello@xgorobot.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -56,15 +56,23 @@
 ```
 xgolib library example
 ```python
 from xgolib import XGO
 dog = XGO('xgomini')
 dog.action(1)
 ```
-### Lastest Verion:0.1.7
+### Lastest Verion:0.1.9
 
-### xgolib_version=1.3.1
+### xgolib_version=1.3.3
 
-### xgoedu_version=1.2.3
+### xgoedu_version=1.2.5
+
+## Change Log
+
+## [0.1.9] - 2023-06-20
+
+### Fixed
+
+- Fixed the issue with the xgoTakePhoto method that was causing abnormal RGB colors in the saved photos.
```

### Comparing `xgo-pythonlib-0.1.8/xgoedu/__init__.py` & `xgo-pythonlib-0.1.9/xgoedu/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 import json
 import threading
 # from xgolib import XGO
 # from keras.preprocessing import image
 # import _thread  使用_thread会报错，坑！
 
 
-__versinon__ = '1.2.4'
-__last_modified__ = '2023/6/19'
+__versinon__ = '1.2.5'
+__last_modified__ = '2023/6/20'
 
 GPIO.setwarnings(False)
 GPIO.setmode(GPIO.BCM)
 
 camera_still=False
 
 
@@ -309,22 +309,22 @@
 
     def xgoTakePhoto(self,filename="photo"):
         path="/home/pi/xgoPictures/"
         self.camera_still=False
         time.sleep(0.6)
         self.open_camera()
         success,image = self.cap.read()
+        cv2.imwrite(path+filename+'.jpg',image)
         if not success:
             print("Ignoring empty camera frame")
         b,g,r = cv2.split(image)
         image = cv2.merge((r,g,b))
         image = cv2.flip(image,1)
         imgok = Image.fromarray(image)
         self.display.ShowImage(imgok)
-        cv2.imwrite(path+filename+'.jpg',image)
         print('photo writed!')
         time.sleep(0.7)
         self.xgoCamera(True)
 
 
     '''
     开启摄像头  A键拍照 B键录像 C键退出
```

### Comparing `xgo-pythonlib-0.1.8/xgolib/__init__.py` & `xgo-pythonlib-0.1.9/xgolib/__init__.py`

 * *Files identical despite different names*

### Comparing `xgo-pythonlib-0.1.8/xgoscreen/LCD_2inch.py` & `xgo-pythonlib-0.1.9/xgoscreen/LCD_2inch.py`

 * *Files identical despite different names*

### Comparing `xgo-pythonlib-0.1.8/xgoscreen/lcdconfig.py` & `xgo-pythonlib-0.1.9/xgoscreen/lcdconfig.py`

 * *Files identical despite different names*

