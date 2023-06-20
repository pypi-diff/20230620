# Comparing `tmp/mecode_viewer-0.2.0.tar.gz` & `tmp/mecode_viewer-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mecode_viewer-0.2.0.tar", last modified: Fri Jun 16 05:04:14 2023, max compression
+gzip compressed data, was "mecode_viewer-0.2.1.tar", last modified: Tue Jun 20 19:13:01 2023, max compression
```

## Comparing `mecode_viewer-0.2.0.tar` & `mecode_viewer-0.2.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 rtelles    (502) staff       (20)        0 2023-06-16 05:04:14.738235 mecode_viewer-0.2.0/
--rw-r--r--   0 rtelles    (502) staff       (20)     3602 2022-11-21 22:26:04.000000 mecode_viewer-0.2.0/CONTRIBUTING.rst
--rw-r--r--   0 rtelles    (502) staff       (20)       89 2022-11-21 22:26:04.000000 mecode_viewer-0.2.0/HISTORY.rst
--rw-r--r--   0 rtelles    (502) staff       (20)     1073 2022-11-21 22:26:04.000000 mecode_viewer-0.2.0/LICENSE
--rw-r--r--   0 rtelles    (502) staff       (20)      242 2022-11-21 22:26:04.000000 mecode_viewer-0.2.0/MANIFEST.in
--rw-r--r--   0 rtelles    (502) staff       (20)     2061 2023-06-16 05:04:14.738402 mecode_viewer-0.2.0/PKG-INFO
--rw-r--r--   0 rtelles    (502) staff       (20)     1261 2023-06-13 00:32:44.000000 mecode_viewer-0.2.0/README.rst
-drwxr-xr-x   0 rtelles    (502) staff       (20)        0 2023-06-16 05:04:14.726642 mecode_viewer-0.2.0/docs/
--rw-r--r--   0 rtelles    (502) staff       (20)      614 2022-11-21 22:26:04.000000 mecode_viewer-0.2.0/docs/Makefile
--rwxr-xr-x   0 rtelles    (502) staff       (20)     4862 2022-11-21 22:26:04.000000 mecode_viewer-0.2.0/docs/conf.py
--rw-r--r--   0 rtelles    (502) staff       (20)       33 2022-11-21 22:26:04.000000 mecode_viewer-0.2.0/docs/contributing.rst
--rw-r--r--   0 rtelles    (502) staff       (20)       28 2022-11-21 22:26:04.000000 mecode_viewer-0.2.0/docs/history.rst
--rw-r--r--   0 rtelles    (502) staff       (20)      299 2022-11-21 22:26:04.000000 mecode_viewer-0.2.0/docs/index.rst
--rw-r--r--   0 rtelles    (502) staff       (20)     1170 2022-11-21 22:26:04.000000 mecode_viewer-0.2.0/docs/installation.rst
--rw-r--r--   0 rtelles    (502) staff       (20)      811 2022-11-21 22:26:04.000000 mecode_viewer-0.2.0/docs/make.bat
--rw-r--r--   0 rtelles    (502) staff       (20)       27 2022-11-21 22:26:04.000000 mecode_viewer-0.2.0/docs/readme.rst
--rw-r--r--   0 rtelles    (502) staff       (20)       81 2022-11-21 22:26:04.000000 mecode_viewer-0.2.0/docs/usage.rst
-drwxr-xr-x   0 rtelles    (502) staff       (20)        0 2023-06-16 05:04:14.728497 mecode_viewer-0.2.0/mecode_viewer/
--rw-r--r--   0 rtelles    (502) staff       (20)      165 2023-06-16 05:01:44.000000 mecode_viewer-0.2.0/mecode_viewer/__init__.py
--rw-r--r--   0 rtelles    (502) staff       (20)      454 2022-11-21 22:26:04.000000 mecode_viewer-0.2.0/mecode_viewer/cli.py
--rw-r--r--   0 rtelles    (502) staff       (20)    21238 2023-06-16 04:54:30.000000 mecode_viewer-0.2.0/mecode_viewer/mecode_viewer.py
-drwxr-xr-x   0 rtelles    (502) staff       (20)        0 2023-06-16 05:04:14.736636 mecode_viewer-0.2.0/mecode_viewer.egg-info/
--rw-r--r--   0 rtelles    (502) staff       (20)     2061 2023-06-16 05:04:14.000000 mecode_viewer-0.2.0/mecode_viewer.egg-info/PKG-INFO
--rw-r--r--   0 rtelles    (502) staff       (20)      610 2023-06-16 05:04:14.000000 mecode_viewer-0.2.0/mecode_viewer.egg-info/SOURCES.txt
--rw-r--r--   0 rtelles    (502) staff       (20)        1 2023-06-16 05:04:14.000000 mecode_viewer-0.2.0/mecode_viewer.egg-info/dependency_links.txt
--rw-r--r--   0 rtelles    (502) staff       (20)       57 2023-06-16 05:04:14.000000 mecode_viewer-0.2.0/mecode_viewer.egg-info/entry_points.txt
--rw-r--r--   0 rtelles    (502) staff       (20)        1 2023-06-12 21:06:47.000000 mecode_viewer-0.2.0/mecode_viewer.egg-info/not-zip-safe
--rw-r--r--   0 rtelles    (502) staff       (20)       39 2023-06-16 05:04:14.000000 mecode_viewer-0.2.0/mecode_viewer.egg-info/requires.txt
--rw-r--r--   0 rtelles    (502) staff       (20)       14 2023-06-16 05:04:14.000000 mecode_viewer-0.2.0/mecode_viewer.egg-info/top_level.txt
--rw-r--r--   0 rtelles    (502) staff       (20)      385 2023-06-16 05:04:14.739132 mecode_viewer-0.2.0/setup.cfg
--rw-r--r--   0 rtelles    (502) staff       (20)     1482 2023-06-16 05:01:44.000000 mecode_viewer-0.2.0/setup.py
-drwxr-xr-x   0 rtelles    (502) staff       (20)        0 2023-06-16 05:04:14.737818 mecode_viewer-0.2.0/tests/
--rw-r--r--   0 rtelles    (502) staff       (20)       43 2022-11-21 22:26:04.000000 mecode_viewer-0.2.0/tests/__init__.py
--rw-r--r--   0 rtelles    (502) staff       (20)      417 2022-11-21 22:26:04.000000 mecode_viewer-0.2.0/tests/test_mecode_viewer.py
+drwxr-xr-x   0 rtelles    (502) staff       (20)        0 2023-06-20 19:13:01.222608 mecode_viewer-0.2.1/
+-rw-r--r--   0 rtelles    (502) staff       (20)     3602 2022-11-21 22:26:04.000000 mecode_viewer-0.2.1/CONTRIBUTING.rst
+-rw-r--r--   0 rtelles    (502) staff       (20)       89 2022-11-21 22:26:04.000000 mecode_viewer-0.2.1/HISTORY.rst
+-rw-r--r--   0 rtelles    (502) staff       (20)     1073 2022-11-21 22:26:04.000000 mecode_viewer-0.2.1/LICENSE
+-rw-r--r--   0 rtelles    (502) staff       (20)      242 2022-11-21 22:26:04.000000 mecode_viewer-0.2.1/MANIFEST.in
+-rw-r--r--   0 rtelles    (502) staff       (20)     2061 2023-06-20 19:13:01.222758 mecode_viewer-0.2.1/PKG-INFO
+-rw-r--r--   0 rtelles    (502) staff       (20)     1261 2023-06-13 00:32:44.000000 mecode_viewer-0.2.1/README.rst
+drwxr-xr-x   0 rtelles    (502) staff       (20)        0 2023-06-20 19:13:01.209787 mecode_viewer-0.2.1/docs/
+-rw-r--r--   0 rtelles    (502) staff       (20)      614 2022-11-21 22:26:04.000000 mecode_viewer-0.2.1/docs/Makefile
+-rwxr-xr-x   0 rtelles    (502) staff       (20)     4862 2022-11-21 22:26:04.000000 mecode_viewer-0.2.1/docs/conf.py
+-rw-r--r--   0 rtelles    (502) staff       (20)       33 2022-11-21 22:26:04.000000 mecode_viewer-0.2.1/docs/contributing.rst
+-rw-r--r--   0 rtelles    (502) staff       (20)       28 2022-11-21 22:26:04.000000 mecode_viewer-0.2.1/docs/history.rst
+-rw-r--r--   0 rtelles    (502) staff       (20)      299 2022-11-21 22:26:04.000000 mecode_viewer-0.2.1/docs/index.rst
+-rw-r--r--   0 rtelles    (502) staff       (20)     1170 2022-11-21 22:26:04.000000 mecode_viewer-0.2.1/docs/installation.rst
+-rw-r--r--   0 rtelles    (502) staff       (20)      811 2022-11-21 22:26:04.000000 mecode_viewer-0.2.1/docs/make.bat
+-rw-r--r--   0 rtelles    (502) staff       (20)       27 2022-11-21 22:26:04.000000 mecode_viewer-0.2.1/docs/readme.rst
+-rw-r--r--   0 rtelles    (502) staff       (20)       81 2022-11-21 22:26:04.000000 mecode_viewer-0.2.1/docs/usage.rst
+drwxr-xr-x   0 rtelles    (502) staff       (20)        0 2023-06-20 19:13:01.212278 mecode_viewer-0.2.1/mecode_viewer/
+-rw-r--r--   0 rtelles    (502) staff       (20)      165 2023-06-20 19:12:37.000000 mecode_viewer-0.2.1/mecode_viewer/__init__.py
+-rw-r--r--   0 rtelles    (502) staff       (20)      454 2022-11-21 22:26:04.000000 mecode_viewer-0.2.1/mecode_viewer/cli.py
+-rw-r--r--   0 rtelles    (502) staff       (20)    21228 2023-06-20 19:11:16.000000 mecode_viewer-0.2.1/mecode_viewer/mecode_viewer.py
+drwxr-xr-x   0 rtelles    (502) staff       (20)        0 2023-06-20 19:13:01.221077 mecode_viewer-0.2.1/mecode_viewer.egg-info/
+-rw-r--r--   0 rtelles    (502) staff       (20)     2061 2023-06-20 19:13:00.000000 mecode_viewer-0.2.1/mecode_viewer.egg-info/PKG-INFO
+-rw-r--r--   0 rtelles    (502) staff       (20)      610 2023-06-20 19:13:00.000000 mecode_viewer-0.2.1/mecode_viewer.egg-info/SOURCES.txt
+-rw-r--r--   0 rtelles    (502) staff       (20)        1 2023-06-20 19:13:00.000000 mecode_viewer-0.2.1/mecode_viewer.egg-info/dependency_links.txt
+-rw-r--r--   0 rtelles    (502) staff       (20)       57 2023-06-20 19:13:00.000000 mecode_viewer-0.2.1/mecode_viewer.egg-info/entry_points.txt
+-rw-r--r--   0 rtelles    (502) staff       (20)        1 2023-06-12 21:06:47.000000 mecode_viewer-0.2.1/mecode_viewer.egg-info/not-zip-safe
+-rw-r--r--   0 rtelles    (502) staff       (20)       39 2023-06-20 19:13:00.000000 mecode_viewer-0.2.1/mecode_viewer.egg-info/requires.txt
+-rw-r--r--   0 rtelles    (502) staff       (20)       14 2023-06-20 19:13:00.000000 mecode_viewer-0.2.1/mecode_viewer.egg-info/top_level.txt
+-rw-r--r--   0 rtelles    (502) staff       (20)      385 2023-06-20 19:13:01.223570 mecode_viewer-0.2.1/setup.cfg
+-rw-r--r--   0 rtelles    (502) staff       (20)     1482 2023-06-20 19:12:37.000000 mecode_viewer-0.2.1/setup.py
+drwxr-xr-x   0 rtelles    (502) staff       (20)        0 2023-06-20 19:13:01.222221 mecode_viewer-0.2.1/tests/
+-rw-r--r--   0 rtelles    (502) staff       (20)       43 2022-11-21 22:26:04.000000 mecode_viewer-0.2.1/tests/__init__.py
+-rw-r--r--   0 rtelles    (502) staff       (20)      417 2022-11-21 22:26:04.000000 mecode_viewer-0.2.1/tests/test_mecode_viewer.py
```

### Comparing `mecode_viewer-0.2.0/CONTRIBUTING.rst` & `mecode_viewer-0.2.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `mecode_viewer-0.2.0/LICENSE` & `mecode_viewer-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mecode_viewer-0.2.0/PKG-INFO` & `mecode_viewer-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mecode_viewer
-Version: 0.2.0
+Version: 0.2.1
 Summary: Simple GCode Viewer
 Home-page: https://github.com/rtellez700/mecode_viewer
 Author: Rodrigo Telles
 Author-email: rtelles@g.harvard.edu
 License: MIT license
 Keywords: mecode_viewer
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `mecode_viewer-0.2.0/README.rst` & `mecode_viewer-0.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `mecode_viewer-0.2.0/docs/Makefile` & `mecode_viewer-0.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mecode_viewer-0.2.0/docs/conf.py` & `mecode_viewer-0.2.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `mecode_viewer-0.2.0/docs/installation.rst` & `mecode_viewer-0.2.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `mecode_viewer-0.2.0/docs/make.bat` & `mecode_viewer-0.2.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mecode_viewer-0.2.0/mecode_viewer/mecode_viewer.py` & `mecode_viewer-0.2.1/mecode_viewer/mecode_viewer.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,38 +7,38 @@
 from gcode_helpers import get_accel_decel, get_print_mode, get_pressure_config, get_print_move, are_we_printing
 import numpy as np
 from typing import List, Optional, Union, Tuple
 from mpl_toolkits.mplot3d.art3d import Line3DCollection
 
 def mecode_viewer(file_name: str,
                   rel_mode: bool=False,
-                  animation: bool=False,
+                  animate: bool=False,
                   verbose: bool=False,
                   raw_gcode: List[str]=None,
                   origin: Union[List[Union[int, float]], Tuple[Union[int, float]]]=(0,0,0),
                   **kwargs) -> Optional[List[Dict]]:
     '''Visualize gcode file
 
         Args:
             file_name (str): name of gcode file
             rel_mode (bool): True if relative coordinates, False if absolute coordinates
-            animation (bool): True for 3D animation, False for static matplotlib figure
+            animate (bool): True for 3D animation, False for static matplotlib figure
             verbose (bool): If True, will return print history as a list of dict's
             raw_gcode (List[str]): Can provide list of gcode str commands in lieu of file_name
             origin (Union[List[Union[int, float]], Tuple[Union[int, float]]]): Specify origin as initial starting point
 
         Returns:
             Optional[List[Dict]]: If verbose is true, will return print history
 
         Examples:
             >>> mecode_viewer(file_name='gcode_file.pgm') # simplest case
 
             >>> mecode_viewer(file_name='gcode_file.pgm', rel_mode=True) # specify relative coordinates are being used
 
-            >>> mecode_viewer(file_name='gcode_file.pgm', animation=True) # show vpython 3D animation
+            >>> mecode_viewer(file_name='gcode_file.pgm', animate=True) # show vpython 3D animation
 
 
     '''
     # variables
     REL_MODE = rel_mode #True if mode == 'rel' else False
 
     ACCEL_RATE = 2000
@@ -103,17 +103,17 @@
                         'P_COM_PORT': P_COM_PORT,
                         'PRINTING': PRINTING,
                         'COORDS': COORDS,
                         'PRINT_SPEED' : PRINT_SPEED
                     })
                     move_counter += 1
 
-    if not animation:
+    if not animate:
         plot3d(history, **kwargs)
-    elif animation:
+    elif animate:
         animation(history, **kwargs)
     else:
         raise ValueError("Invalid plotting backend! Choose one of mayavi or matplotlib or matplotlib2d or vpython.")
     
     if verbose:
         return history
```

### Comparing `mecode_viewer-0.2.0/mecode_viewer.egg-info/PKG-INFO` & `mecode_viewer-0.2.1/mecode_viewer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mecode-viewer
-Version: 0.2.0
+Version: 0.2.1
 Summary: Simple GCode Viewer
 Home-page: https://github.com/rtellez700/mecode_viewer
 Author: Rodrigo Telles
 Author-email: rtelles@g.harvard.edu
 License: MIT license
 Keywords: mecode_viewer
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `mecode_viewer-0.2.0/mecode_viewer.egg-info/SOURCES.txt` & `mecode_viewer-0.2.1/mecode_viewer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mecode_viewer-0.2.0/setup.py` & `mecode_viewer-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,10 +43,10 @@
     include_package_data=True,
     keywords='mecode_viewer',
     name='mecode_viewer',
     packages=find_packages(include=['mecode_viewer', 'mecode_viewer.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/rtellez700/mecode_viewer',
-    version='0.2.0',
+    version='0.2.1',
     zip_safe=False,
 )
```

