# Comparing `tmp/py2appsigner-0.5.0.tar.gz` & `tmp/py2appsigner-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py2appsigner-0.5.0.tar", last modified: Mon Jun 19 21:08:14 2023, max compression
+gzip compressed data, was "py2appsigner-0.5.2.tar", last modified: Tue Jun 20 03:07:28 2023, max compression
```

## Comparing `py2appsigner-0.5.0.tar` & `py2appsigner-0.5.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-19 21:08:14.068340 py2appsigner-0.5.0/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    34523 2023-05-17 20:07:47.000000 py2appsigner-0.5.0/LICENSE
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    44603 2023-06-19 21:08:14.068211 py2appsigner-0.5.0/PKG-INFO
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4408 2023-06-19 21:06:01.000000 py2appsigner-0.5.0/README.md
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-19 21:08:14.065753 py2appsigner-0.5.0/py2appsigner/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2595 2023-06-03 20:42:54.000000 py2appsigner-0.5.0/py2appsigner/ApplicationNotarize.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6701 2023-06-03 20:22:26.000000 py2appsigner-0.5.0/py2appsigner/ApplicationSign.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      711 2023-06-02 20:02:20.000000 py2appsigner-0.5.0/py2appsigner/ApplicationStaple.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      505 2023-06-02 20:02:20.000000 py2appsigner-0.5.0/py2appsigner/ApplicationVerify.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1016 2023-06-04 22:47:50.000000 py2appsigner-0.5.0/py2appsigner/BaseCommand.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1758 2023-06-03 17:59:25.000000 py2appsigner-0.5.0/py2appsigner/CommandBasic.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      737 2023-06-02 20:02:20.000000 py2appsigner-0.5.0/py2appsigner/CommandExtended.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    10033 2023-06-04 23:39:53.000000 py2appsigner-0.5.0/py2appsigner/Commands.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      113 2023-06-03 20:21:23.000000 py2appsigner-0.5.0/py2appsigner/Common.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2316 2023-06-19 20:48:07.000000 py2appsigner-0.5.0/py2appsigner/Notary.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6225 2023-06-03 20:22:37.000000 py2appsigner-0.5.0/py2appsigner/ZipSign.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       46 2023-05-17 20:18:22.000000 py2appsigner-0.5.0/py2appsigner/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       22 2023-05-17 20:18:38.000000 py2appsigner-0.5.0/py2appsigner/_version.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-19 21:08:14.067611 py2appsigner-0.5.0/py2appsigner/environment/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2094 2023-05-31 01:40:56.000000 py2appsigner-0.5.0/py2appsigner/environment/BasicEnvironment.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1519 2023-06-03 20:04:40.000000 py2appsigner-0.5.0/py2appsigner/environment/Environment.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      219 2023-06-04 22:46:26.000000 py2appsigner-0.5.0/py2appsigner/environment/NotaryEnvironment.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-02 19:06:14.000000 py2appsigner-0.5.0/py2appsigner/environment/__init__.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-19 21:08:14.067812 py2appsigner-0.5.0/py2appsigner/resources/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-17 20:20:16.000000 py2appsigner-0.5.0/py2appsigner/resources/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      854 2023-05-19 16:43:35.000000 py2appsigner-0.5.0/py2appsigner/resources/loggingConfiguration.json
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-19 21:08:14.066707 py2appsigner-0.5.0/py2appsigner.egg-info/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    44603 2023-06-19 21:08:14.000000 py2appsigner-0.5.0/py2appsigner.egg-info/PKG-INFO
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      866 2023-06-19 21:08:14.000000 py2appsigner-0.5.0/py2appsigner.egg-info/SOURCES.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        1 2023-06-19 21:08:14.000000 py2appsigner-0.5.0/py2appsigner.egg-info/dependency_links.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      246 2023-06-19 21:08:14.000000 py2appsigner-0.5.0/py2appsigner.egg-info/entry_points.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       26 2023-06-19 21:08:14.000000 py2appsigner-0.5.0/py2appsigner.egg-info/requires.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       13 2023-06-19 21:08:14.000000 py2appsigner-0.5.0/py2appsigner.egg-info/top_level.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       38 2023-06-19 21:08:14.068379 py2appsigner-0.5.0/setup.cfg
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1363 2023-06-04 22:36:05.000000 py2appsigner-0.5.0/setup.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-20 03:07:28.682803 py2appsigner-0.5.2/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    34523 2023-05-17 20:07:47.000000 py2appsigner-0.5.2/LICENSE
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    44603 2023-06-20 03:07:28.682672 py2appsigner-0.5.2/PKG-INFO
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4408 2023-06-19 21:06:01.000000 py2appsigner-0.5.2/README.md
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-20 03:07:28.680960 py2appsigner-0.5.2/py2appsigner/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2595 2023-06-03 20:42:54.000000 py2appsigner-0.5.2/py2appsigner/ApplicationNotarize.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6785 2023-06-19 21:47:06.000000 py2appsigner-0.5.2/py2appsigner/ApplicationSign.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      711 2023-06-02 20:02:20.000000 py2appsigner-0.5.2/py2appsigner/ApplicationStaple.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      505 2023-06-02 20:02:20.000000 py2appsigner-0.5.2/py2appsigner/ApplicationVerify.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1016 2023-06-04 22:47:50.000000 py2appsigner-0.5.2/py2appsigner/BaseCommand.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1758 2023-06-03 17:59:25.000000 py2appsigner-0.5.2/py2appsigner/CommandBasic.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      737 2023-06-02 20:02:20.000000 py2appsigner-0.5.2/py2appsigner/CommandExtended.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    10033 2023-06-04 23:39:53.000000 py2appsigner-0.5.2/py2appsigner/Commands.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      113 2023-06-03 20:21:23.000000 py2appsigner-0.5.2/py2appsigner/Common.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2316 2023-06-19 20:48:07.000000 py2appsigner-0.5.2/py2appsigner/Notary.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6225 2023-06-03 20:22:37.000000 py2appsigner-0.5.2/py2appsigner/ZipSign.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       46 2023-05-17 20:18:22.000000 py2appsigner-0.5.2/py2appsigner/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       22 2023-06-20 02:48:04.000000 py2appsigner-0.5.2/py2appsigner/_version.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-20 03:07:28.682230 py2appsigner-0.5.2/py2appsigner/environment/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2094 2023-05-31 01:40:56.000000 py2appsigner-0.5.2/py2appsigner/environment/BasicEnvironment.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1519 2023-06-03 20:04:40.000000 py2appsigner-0.5.2/py2appsigner/environment/Environment.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      219 2023-06-04 22:46:26.000000 py2appsigner-0.5.2/py2appsigner/environment/NotaryEnvironment.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-02 19:06:14.000000 py2appsigner-0.5.2/py2appsigner/environment/__init__.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-20 03:07:28.682455 py2appsigner-0.5.2/py2appsigner/resources/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-17 20:20:16.000000 py2appsigner-0.5.2/py2appsigner/resources/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      854 2023-05-19 16:43:35.000000 py2appsigner-0.5.2/py2appsigner/resources/loggingConfiguration.json
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-20 03:07:28.681783 py2appsigner-0.5.2/py2appsigner.egg-info/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    44603 2023-06-20 03:07:28.000000 py2appsigner-0.5.2/py2appsigner.egg-info/PKG-INFO
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      866 2023-06-20 03:07:28.000000 py2appsigner-0.5.2/py2appsigner.egg-info/SOURCES.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        1 2023-06-20 03:07:28.000000 py2appsigner-0.5.2/py2appsigner.egg-info/dependency_links.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      246 2023-06-20 03:07:28.000000 py2appsigner-0.5.2/py2appsigner.egg-info/entry_points.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       26 2023-06-20 03:07:28.000000 py2appsigner-0.5.2/py2appsigner.egg-info/requires.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       13 2023-06-20 03:07:28.000000 py2appsigner-0.5.2/py2appsigner.egg-info/top_level.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       38 2023-06-20 03:07:28.682837 py2appsigner-0.5.2/setup.cfg
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1363 2023-06-04 22:36:05.000000 py2appsigner-0.5.2/setup.py
```

### Comparing `py2appsigner-0.5.0/LICENSE` & `py2appsigner-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `py2appsigner-0.5.0/PKG-INFO` & `py2appsigner-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py2appsigner
-Version: 0.5.0
+Version: 0.5.2
 Summary: Scripts to Code Sign py2app applications
 Home-page: https://github.com/py2appsigner
 Author: Humberto A. Sanchez II
 Author-email: humberto.a.sanchez.ii@gmail.com
 Maintainer: Humberto A. Sanchez II
 Maintainer-email: humberto.a.sanchez.ii@gmail.com
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
```

### Comparing `py2appsigner-0.5.0/README.md` & `py2appsigner-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `py2appsigner-0.5.0/py2appsigner/ApplicationNotarize.py` & `py2appsigner-0.5.2/py2appsigner/ApplicationNotarize.py`

 * *Files identical despite different names*

### Comparing `py2appsigner-0.5.0/py2appsigner/ApplicationSign.py` & `py2appsigner-0.5.2/py2appsigner/ApplicationSign.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,16 @@
     'Contents/Resources/lib/python3.10/numpy/f2py/tests/src/assumed_shape/.f2py_f2cmap',
     'Contents/Resources/lib/python3.10/site.pyo'
 ]
 
 SHARED_OBJECT_LIBRARY_WILDCARD:       str = '*.so'
 MACH_OBJECT_DYNAMIC_LIBRARY_WILDCARD: str = '*.dylib'
 
+PRE_FRAMEWORK_PATH: str = '/Contents/Frameworks/Python.framework'
+
 
 class ApplicationSign(CommandExtended):
 
     def __init__(self, environment: Environment, fixLib: bool):
 
         super().__init__(environment=environment)
         self.logger: Logger = getLogger(__name__)
@@ -116,15 +118,18 @@
         """
          Assumes Xcode 13 is installed
         """
         #
         # codesign --sign "${IDENTITY}" ${OPTIONS} "${FULL_APP_NAME}/Contents/Frameworks/Python.framework/Versions/3.10/Python"
         #
         secho('Sign Framework')
-        framework:     str = f'{self._applicationName}/Contents/Frameworks/Python.framework/Versions/3.10/Python'
+
+        framework:     str = (
+            f'{self._applicationName}/{PRE_FRAMEWORK_PATH}/{self._pythonVersion}/Python'
+        )
         signFramework: str = f'{self._codeSignCommand} {framework}'
         self._runCommand(signFramework)
 
     def _signPythonApp(self):
         # codesign --sign "${IDENTITY}" ${OPTIONS} "${FULL_APP_NAME}/Contents/MacOS/python"
         pythonApp:  str = f'{self._applicationName}/Contents/MacOS/python'
         signPython: str = f'{self._codeSignCommand} {pythonApp}'
```

### Comparing `py2appsigner-0.5.0/py2appsigner/ApplicationStaple.py` & `py2appsigner-0.5.2/py2appsigner/ApplicationStaple.py`

 * *Files identical despite different names*

### Comparing `py2appsigner-0.5.0/py2appsigner/BaseCommand.py` & `py2appsigner-0.5.2/py2appsigner/BaseCommand.py`

 * *Files identical despite different names*

### Comparing `py2appsigner-0.5.0/py2appsigner/CommandBasic.py` & `py2appsigner-0.5.2/py2appsigner/CommandBasic.py`

 * *Files identical despite different names*

### Comparing `py2appsigner-0.5.0/py2appsigner/CommandExtended.py` & `py2appsigner-0.5.2/py2appsigner/CommandExtended.py`

 * *Files identical despite different names*

### Comparing `py2appsigner-0.5.0/py2appsigner/Commands.py` & `py2appsigner-0.5.2/py2appsigner/Commands.py`

 * *Files identical despite different names*

### Comparing `py2appsigner-0.5.0/py2appsigner/Notary.py` & `py2appsigner-0.5.2/py2appsigner/Notary.py`

 * *Files identical despite different names*

### Comparing `py2appsigner-0.5.0/py2appsigner/ZipSign.py` & `py2appsigner-0.5.2/py2appsigner/ZipSign.py`

 * *Files identical despite different names*

### Comparing `py2appsigner-0.5.0/py2appsigner/environment/BasicEnvironment.py` & `py2appsigner-0.5.2/py2appsigner/environment/BasicEnvironment.py`

 * *Files identical despite different names*

### Comparing `py2appsigner-0.5.0/py2appsigner/environment/Environment.py` & `py2appsigner-0.5.2/py2appsigner/environment/Environment.py`

 * *Files identical despite different names*

### Comparing `py2appsigner-0.5.0/py2appsigner/resources/loggingConfiguration.json` & `py2appsigner-0.5.2/py2appsigner/resources/loggingConfiguration.json`

 * *Files identical despite different names*

### Comparing `py2appsigner-0.5.0/py2appsigner.egg-info/PKG-INFO` & `py2appsigner-0.5.2/py2appsigner.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py2appsigner
-Version: 0.5.0
+Version: 0.5.2
 Summary: Scripts to Code Sign py2app applications
 Home-page: https://github.com/py2appsigner
 Author: Humberto A. Sanchez II
 Author-email: humberto.a.sanchez.ii@gmail.com
 Maintainer: Humberto A. Sanchez II
 Maintainer-email: humberto.a.sanchez.ii@gmail.com
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
```

### Comparing `py2appsigner-0.5.0/py2appsigner.egg-info/SOURCES.txt` & `py2appsigner-0.5.2/py2appsigner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py2appsigner-0.5.0/setup.py` & `py2appsigner-0.5.2/setup.py`

 * *Files identical despite different names*

