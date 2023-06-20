# Comparing `tmp/pyappauto-1.0.1.tar.gz` & `tmp/pyappauto-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyappauto-1.0.1.tar", last modified: Mon Jun 19 03:40:55 2023, max compression
+gzip compressed data, was "pyappauto-1.0.2.tar", last modified: Tue Jun 20 01:02:27 2023, max compression
```

## Comparing `pyappauto-1.0.1.tar` & `pyappauto-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 03:40:55.051329 pyappauto-1.0.1/
--rw-rw-rw-   0        0        0     1088 2023-06-19 03:18:35.000000 pyappauto-1.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0     1532 2023-06-19 03:40:55.051329 pyappauto-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      857 2023-06-19 03:25:08.000000 pyappauto-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-19 03:40:55.044281 pyappauto-1.0.1/pyappauto/
--rw-rw-rw-   0        0        0    15265 2023-06-19 03:39:04.000000 pyappauto-1.0.1/pyappauto/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 03:40:55.049317 pyappauto-1.0.1/pyappauto/utils/
--rw-rw-rw-   0        0        0      229 2023-06-19 01:57:47.000000 pyappauto-1.0.1/pyappauto/utils/errors.py
--rw-rw-rw-   0        0        0     3736 2023-06-19 02:11:18.000000 pyappauto-1.0.1/pyappauto/utils/keys.py
-drwxrwxrwx   0        0        0        0 2023-06-19 03:40:55.048812 pyappauto-1.0.1/pyappauto.egg-info/
--rw-rw-rw-   0        0        0     1532 2023-06-19 03:40:55.000000 pyappauto-1.0.1/pyappauto.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2023-06-19 03:40:55.000000 pyappauto-1.0.1/pyappauto.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 03:40:55.000000 pyappauto-1.0.1/pyappauto.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2023-06-19 03:40:55.000000 pyappauto-1.0.1/pyappauto.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-19 03:40:55.000000 pyappauto-1.0.1/pyappauto.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-19 03:40:55.051329 pyappauto-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1031 2023-06-19 03:38:34.000000 pyappauto-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 01:02:27.780997 pyappauto-1.0.2/
+-rw-rw-rw-   0        0        0     1088 2023-06-19 03:18:35.000000 pyappauto-1.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     1601 2023-06-20 01:02:27.779999 pyappauto-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      922 2023-06-20 01:00:37.000000 pyappauto-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-20 01:02:27.768936 pyappauto-1.0.2/pyappauto/
+-rw-rw-rw-   0        0        0    15477 2023-06-20 01:02:06.000000 pyappauto-1.0.2/pyappauto/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 01:02:27.778998 pyappauto-1.0.2/pyappauto/utils/
+-rw-rw-rw-   0        0        0      229 2023-06-19 01:57:47.000000 pyappauto-1.0.2/pyappauto/utils/errors.py
+-rw-rw-rw-   0        0        0     3736 2023-06-19 02:11:18.000000 pyappauto-1.0.2/pyappauto/utils/keys.py
+drwxrwxrwx   0        0        0        0 2023-06-20 01:02:27.776481 pyappauto-1.0.2/pyappauto.egg-info/
+-rw-rw-rw-   0        0        0     1601 2023-06-20 01:02:27.000000 pyappauto-1.0.2/pyappauto.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2023-06-20 01:02:27.000000 pyappauto-1.0.2/pyappauto.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 01:02:27.000000 pyappauto-1.0.2/pyappauto.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2023-06-20 01:02:27.000000 pyappauto-1.0.2/pyappauto.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-20 01:02:27.000000 pyappauto-1.0.2/pyappauto.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-20 01:02:27.780997 pyappauto-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1031 2023-06-20 01:02:12.000000 pyappauto-1.0.2/setup.py
```

### Comparing `pyappauto-1.0.1/LICENSE.txt` & `pyappauto-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyappauto-1.0.1/PKG-INFO` & `pyappauto-1.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyappauto
-Version: 1.0.1
+Version: 1.0.2
 Summary: Control an app without disturbing your everyday life.
 Home-page: https://github.com/User00092/PyAppAuto
 Author: User0092
 Author-email: unknownuser0092@protonmail.com
 License: MIT
 Keywords: Windows App control,App controller,PyAppAuto
 Classifier: Development Status :: 5 - Production/Stable
@@ -23,27 +23,31 @@
 Control an app without disturbing your everyday life.
 
 ## Requirements
 
 - Windows 10+
 - Python 3.7 or higher.
 
+## Latest Patch
+
+- Fixed `_close_handler` recursion error.
+
 ## Features
 
 - Attach to a created window by hwnd, or create one by path.
 - Left and right click the window. (Without using your mouse)
 - Keypress and typewrite directly to the window.
 - Find an image on the window without focusing it.
 - Set the monitor index of the window.
 - Enter and exit fullscreen.
 - Get the window size and position.
 - Set the window size and position.
 - Double click (Simulates a double click, sending a double click crashes the window)
 - pyappauto.utils.keys.KeyCodes
-
+ 
 ## Installation
 
 - Install with pip.
 
 ```cmd
   pip install pyappauto
 ```
```

### Comparing `pyappauto-1.0.1/README.md` & `pyappauto-1.0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -4,27 +4,31 @@
 Control an app without disturbing your everyday life.
 
 ## Requirements
 
 - Windows 10+
 - Python 3.7 or higher.
 
+## Latest Patch
+
+- Fixed `_close_handler` recursion error.
+
 ## Features
 
 - Attach to a created window by hwnd, or create one by path.
 - Left and right click the window. (Without using your mouse)
 - Keypress and typewrite directly to the window.
 - Find an image on the window without focusing it.
 - Set the monitor index of the window.
 - Enter and exit fullscreen.
 - Get the window size and position.
 - Set the window size and position.
 - Double click (Simulates a double click, sending a double click crashes the window)
 - pyappauto.utils.keys.KeyCodes
-
+ 
 ## Installation
 
 - Install with pip.
 
 ```cmd
   pip install pyappauto
 ```
```

### Comparing `pyappauto-1.0.1/pyappauto/__init__.py` & `pyappauto-1.0.2/pyappauto/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import win32gui
 import win32api
 import win32ui
 import time
 import cv2
 import os
 
-__version__ = '1.0.1'
+__version__ = '1.0.2'
 
 
 class Instance:
     def __init__(self, hwnd: int | None = None, debug: bool = False):
         """This is the constructor method for the class "Instance"
 
         Args:
@@ -24,27 +24,33 @@
             debug (bool, optional): if set to `True`, prints debug information to the console.
         """
         
         self._hwnd = hwnd
         self.__process = None
         self.__kill = False
         self._debug = debug
+        self.__watch_close_thread = None
 
         if hwnd:
             Thread(target=self._close_handler).start()
     
     def __debug(self, title: str, content: str) -> None:
         if not self._debug:
             return
         
         print(f'[DEBUG] {title}: {content}')
     
     def _close_handler(self):
+        if self.__watch_close_thread:
+            return
+        
         self.__debug('Info', 'Created close handler.')
 
+        self.__watch_close_thread = self._close_handler
+
         while not self.__kill:
             if not win32gui.IsWindow(self._hwnd):
                 break
             time.sleep(1)
 
         self.__debug('Info', 'Detected application close in close handler.')
         self.close()
@@ -105,14 +111,15 @@
             self.__process.terminate()
         else:
             win32gui.PostMessage(self._hwnd, win32con.WM_CLOSE, 0, 0)
 
         
         self.__process = None
         self._hwnd = None
+        self.__watch_close_thread = None
         self.__debug('Success', 'Closed application.')
 
     def set_monitor(self, monitor_number: int = 0) -> None:
         """This function sets the position of a window to a specified monitor.
 
         Args:
             monitor_number (int, optional):  An integer representing the index of the monitor to set the window
```

### Comparing `pyappauto-1.0.1/pyappauto/utils/keys.py` & `pyappauto-1.0.2/pyappauto/utils/keys.py`

 * *Files identical despite different names*

### Comparing `pyappauto-1.0.1/pyappauto.egg-info/PKG-INFO` & `pyappauto-1.0.2/pyappauto.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyappauto
-Version: 1.0.1
+Version: 1.0.2
 Summary: Control an app without disturbing your everyday life.
 Home-page: https://github.com/User00092/PyAppAuto
 Author: User0092
 Author-email: unknownuser0092@protonmail.com
 License: MIT
 Keywords: Windows App control,App controller,PyAppAuto
 Classifier: Development Status :: 5 - Production/Stable
@@ -23,27 +23,31 @@
 Control an app without disturbing your everyday life.
 
 ## Requirements
 
 - Windows 10+
 - Python 3.7 or higher.
 
+## Latest Patch
+
+- Fixed `_close_handler` recursion error.
+
 ## Features
 
 - Attach to a created window by hwnd, or create one by path.
 - Left and right click the window. (Without using your mouse)
 - Keypress and typewrite directly to the window.
 - Find an image on the window without focusing it.
 - Set the monitor index of the window.
 - Enter and exit fullscreen.
 - Get the window size and position.
 - Set the window size and position.
 - Double click (Simulates a double click, sending a double click crashes the window)
 - pyappauto.utils.keys.KeyCodes
-
+ 
 ## Installation
 
 - Install with pip.
 
 ```cmd
   pip install pyappauto
 ```
```

### Comparing `pyappauto-1.0.1/setup.py` & `pyappauto-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 DESCRIPTION = 'Control an app without disturbing your everyday life.'
 
 # Setting up
 setup(
 	name="pyappauto",
 	url="https://github.com/User00092/PyAppAuto",
-	version='1.0.1',
+	version='1.0.2',
 	license='MIT',
 	author="User0092",
 	author_email="unknownuser0092@protonmail.com",
 	description=DESCRIPTION,
 	long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
 	keywords=['Windows App control', 'App controller', 'PyAppAuto'],
```

