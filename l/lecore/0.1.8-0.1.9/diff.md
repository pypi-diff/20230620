# Comparing `tmp/lecore-0.1.8.tar.gz` & `tmp/lecore-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\work\gitlab\le-py-core\package-lecore\dist\.tmp-qhqjkxsw\lecore-0.1.8.tar", last modified: Tue Jun 13 14:44:02 2023, max compression
+gzip compressed data, was "D:\work\gitlab\le-py-core\package-lecore\dist\.tmp-rrvftim3\lecore-0.1.9.tar", last modified: Tue Jun 13 15:11:17 2023, max compression
```

## Comparing `lecore-0.1.8.tar` & `lecore-0.1.9.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 14:44:02.000000 lecore-0.1.8/
--rw-rw-rw-   0        0        0     1091 2023-03-24 15:23:12.000000 lecore-0.1.8/LICENSE
--rw-rw-rw-   0        0        0     1558 2023-06-13 14:44:02.000000 lecore-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     1067 2023-03-27 13:17:27.000000 lecore-0.1.8/README.md
--rw-rw-rw-   0        0        0      704 2023-06-13 14:43:42.000000 lecore-0.1.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-13 14:44:02.000000 lecore-0.1.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-13 14:44:02.000000 lecore-0.1.8/src/
-drwxrwxrwx   0        0        0        0 2023-06-13 14:44:02.000000 lecore-0.1.8/src/lecore/
-drwxrwxrwx   0        0        0        0 2023-06-13 14:44:02.000000 lecore-0.1.8/src/lecore/LeBin/
--rw-rw-rw-   0        0        0    12112 2023-01-16 14:47:23.000000 lecore-0.1.8/src/lecore/LeBin/RegisterMap.py
--rw-rw-rw-   0        0        0     4563 2021-08-12 11:01:11.000000 lecore-0.1.8/src/lecore/LeBin/SerialCom.py
--rw-rw-rw-   0        0        0     2933 2020-11-27 14:22:56.000000 lecore-0.1.8/src/lecore/LeBin/UpgradeFirmware.py
--rw-rw-rw-   0        0        0     5334 2023-06-06 09:06:28.000000 lecore-0.1.8/src/lecore/LeBin/VisualLeBin.py
--rw-rw-rw-   0        0        0      156 2023-06-06 09:02:40.000000 lecore-0.1.8/src/lecore/LeBin/__init__.py
--rw-rw-rw-   0        0        0     4973 2023-06-05 14:39:42.000000 lecore-0.1.8/src/lecore/Looger.py
-drwxrwxrwx   0        0        0        0 2023-06-13 14:44:02.000000 lecore-0.1.8/src/lecore/TestFrame/
--rw-rw-rw-   0        0        0     1886 2023-06-13 14:37:57.000000 lecore-0.1.8/src/lecore/TestFrame/CoreTest.py
--rw-rw-rw-   0        0        0      184 2023-06-13 14:37:57.000000 lecore-0.1.8/src/lecore/TestFrame/ModbusUnitTest.py
--rw-rw-rw-   0        0        0     2848 2023-06-13 14:37:57.000000 lecore-0.1.8/src/lecore/TestFrame/RtuClient.py
--rw-rw-rw-   0        0        0     2136 2023-02-20 13:11:31.000000 lecore-0.1.8/src/lecore/TestFrame/TestUtils.py
--rw-rw-rw-   0        0        0      224 2023-06-13 14:37:57.000000 lecore-0.1.8/src/lecore/TestFrame/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 14:44:02.000000 lecore-0.1.8/src/lecore/VisualModbus/
--rw-rw-rw-   0        0        0     3452 2020-11-18 16:02:58.000000 lecore-0.1.8/src/lecore/VisualModbus/AppLogging.py
--rw-rw-rw-   0        0        0     1648 2020-11-18 16:02:58.000000 lecore-0.1.8/src/lecore/VisualModbus/Crc32.py
--rw-rw-rw-   0        0        0     2903 2020-05-05 14:10:01.000000 lecore-0.1.8/src/lecore/VisualModbus/HelpAbout.py
--rw-rw-rw-   0        0        0     6975 2023-02-06 16:45:12.000000 lecore-0.1.8/src/lecore/VisualModbus/MbClient.py
--rw-rw-rw-   0        0        0     7821 2023-02-06 16:17:38.000000 lecore-0.1.8/src/lecore/VisualModbus/MbUpgrade.py
--rw-rw-rw-   0        0        0     5034 2023-06-13 08:40:17.000000 lecore-0.1.8/src/lecore/VisualModbus/ReadWrite.py
--rw-rw-rw-   0        0        0    14943 2022-02-25 08:52:05.000000 lecore-0.1.8/src/lecore/VisualModbus/RegMap.py
--rw-rw-rw-   0        0        0     8611 2023-06-13 09:26:48.000000 lecore-0.1.8/src/lecore/VisualModbus/VisualMbApp.py
--rw-rw-rw-   0        0        0     2080 2020-11-18 17:05:27.000000 lecore-0.1.8/src/lecore/VisualModbus/VmSettings.py
--rw-rw-rw-   0        0        0      170 2023-06-07 10:26:20.000000 lecore-0.1.8/src/lecore/VisualModbus/__init__.py
--rw-rw-rw-   0        0        0       28 2023-06-05 14:45:48.000000 lecore-0.1.8/src/lecore/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 14:44:02.000000 lecore-0.1.8/src/lecore.egg-info/
--rw-rw-rw-   0        0        0     1558 2023-06-13 14:44:02.000000 lecore-0.1.8/src/lecore.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1024 2023-06-13 14:44:02.000000 lecore-0.1.8/src/lecore.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 14:44:02.000000 lecore-0.1.8/src/lecore.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-06-13 14:44:02.000000 lecore-0.1.8/src/lecore.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-13 14:44:02.000000 lecore-0.1.8/src/lecore.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-13 14:44:02.000000 lecore-0.1.8/tests/
--rw-rw-rw-   0        0        0      849 2023-06-13 14:37:57.000000 lecore-0.1.8/tests/test_frame.py
--rw-rw-rw-   0        0        0     1127 2023-06-13 08:49:10.000000 lecore-0.1.8/tests/test_lebin.py
--rw-rw-rw-   0        0        0     1452 2023-06-05 14:53:08.000000 lecore-0.1.8/tests/test_looger.py
--rw-rw-rw-   0        0        0     1193 2023-06-13 09:32:50.000000 lecore-0.1.8/tests/test_modbus.py
+drwxrwxrwx   0        0        0        0 2023-06-13 15:11:17.000000 lecore-0.1.9/
+-rw-rw-rw-   0        0        0     1091 2023-03-24 15:23:12.000000 lecore-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0     1558 2023-06-13 15:11:17.000000 lecore-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1067 2023-03-27 13:17:27.000000 lecore-0.1.9/README.md
+-rw-rw-rw-   0        0        0      704 2023-06-13 15:11:00.000000 lecore-0.1.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-13 15:11:17.000000 lecore-0.1.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-13 15:11:17.000000 lecore-0.1.9/src/
+drwxrwxrwx   0        0        0        0 2023-06-13 15:11:17.000000 lecore-0.1.9/src/lecore/
+drwxrwxrwx   0        0        0        0 2023-06-13 15:11:17.000000 lecore-0.1.9/src/lecore/LeBin/
+-rw-rw-rw-   0        0        0    12112 2023-01-16 14:47:23.000000 lecore-0.1.9/src/lecore/LeBin/RegisterMap.py
+-rw-rw-rw-   0        0        0     4563 2021-08-12 11:01:11.000000 lecore-0.1.9/src/lecore/LeBin/SerialCom.py
+-rw-rw-rw-   0        0        0     2933 2020-11-27 14:22:56.000000 lecore-0.1.9/src/lecore/LeBin/UpgradeFirmware.py
+-rw-rw-rw-   0        0        0     5392 2023-06-13 15:10:45.000000 lecore-0.1.9/src/lecore/LeBin/VisualLeBin.py
+-rw-rw-rw-   0        0        0      156 2023-06-06 09:02:40.000000 lecore-0.1.9/src/lecore/LeBin/__init__.py
+-rw-rw-rw-   0        0        0     4973 2023-06-05 14:39:42.000000 lecore-0.1.9/src/lecore/Looger.py
+drwxrwxrwx   0        0        0        0 2023-06-13 15:11:17.000000 lecore-0.1.9/src/lecore/TestFrame/
+-rw-rw-rw-   0        0        0     1886 2023-06-13 14:37:57.000000 lecore-0.1.9/src/lecore/TestFrame/CoreTest.py
+-rw-rw-rw-   0        0        0      184 2023-06-13 14:37:57.000000 lecore-0.1.9/src/lecore/TestFrame/ModbusUnitTest.py
+-rw-rw-rw-   0        0        0     2848 2023-06-13 14:37:57.000000 lecore-0.1.9/src/lecore/TestFrame/RtuClient.py
+-rw-rw-rw-   0        0        0     2136 2023-02-20 13:11:31.000000 lecore-0.1.9/src/lecore/TestFrame/TestUtils.py
+-rw-rw-rw-   0        0        0      224 2023-06-13 14:37:57.000000 lecore-0.1.9/src/lecore/TestFrame/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 15:11:17.000000 lecore-0.1.9/src/lecore/VisualModbus/
+-rw-rw-rw-   0        0        0     3452 2020-11-18 16:02:58.000000 lecore-0.1.9/src/lecore/VisualModbus/AppLogging.py
+-rw-rw-rw-   0        0        0     1648 2020-11-18 16:02:58.000000 lecore-0.1.9/src/lecore/VisualModbus/Crc32.py
+-rw-rw-rw-   0        0        0     2903 2020-05-05 14:10:01.000000 lecore-0.1.9/src/lecore/VisualModbus/HelpAbout.py
+-rw-rw-rw-   0        0        0     6975 2023-02-06 16:45:12.000000 lecore-0.1.9/src/lecore/VisualModbus/MbClient.py
+-rw-rw-rw-   0        0        0     7821 2023-02-06 16:17:38.000000 lecore-0.1.9/src/lecore/VisualModbus/MbUpgrade.py
+-rw-rw-rw-   0        0        0     5034 2023-06-13 08:40:17.000000 lecore-0.1.9/src/lecore/VisualModbus/ReadWrite.py
+-rw-rw-rw-   0        0        0    14943 2022-02-25 08:52:05.000000 lecore-0.1.9/src/lecore/VisualModbus/RegMap.py
+-rw-rw-rw-   0        0        0     8673 2023-06-13 15:10:45.000000 lecore-0.1.9/src/lecore/VisualModbus/VisualMbApp.py
+-rw-rw-rw-   0        0        0     2080 2020-11-18 17:05:27.000000 lecore-0.1.9/src/lecore/VisualModbus/VmSettings.py
+-rw-rw-rw-   0        0        0      170 2023-06-07 10:26:20.000000 lecore-0.1.9/src/lecore/VisualModbus/__init__.py
+-rw-rw-rw-   0        0        0       28 2023-06-05 14:45:48.000000 lecore-0.1.9/src/lecore/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 15:11:17.000000 lecore-0.1.9/src/lecore.egg-info/
+-rw-rw-rw-   0        0        0     1558 2023-06-13 15:11:17.000000 lecore-0.1.9/src/lecore.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1024 2023-06-13 15:11:17.000000 lecore-0.1.9/src/lecore.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 15:11:17.000000 lecore-0.1.9/src/lecore.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-06-13 15:11:17.000000 lecore-0.1.9/src/lecore.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-13 15:11:17.000000 lecore-0.1.9/src/lecore.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-13 15:11:17.000000 lecore-0.1.9/tests/
+-rw-rw-rw-   0        0        0      849 2023-06-13 14:37:57.000000 lecore-0.1.9/tests/test_frame.py
+-rw-rw-rw-   0        0        0     1165 2023-06-13 15:10:45.000000 lecore-0.1.9/tests/test_lebin.py
+-rw-rw-rw-   0        0        0     1452 2023-06-05 14:53:08.000000 lecore-0.1.9/tests/test_looger.py
+-rw-rw-rw-   0        0        0     1193 2023-06-13 09:32:50.000000 lecore-0.1.9/tests/test_modbus.py
```

### Comparing `lecore-0.1.8/LICENSE` & `lecore-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `lecore-0.1.8/PKG-INFO` & `lecore-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lecore
-Version: 0.1.8
+Version: 0.1.9
 Summary: Logic Elements core utilities
 Author-email: Jan Bartovský <jan.bartovsky@logicelements.cz>
 Project-URL: Homepage, http://www.logicelements.cz
 Keywords: logicelements,looger,development
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lecore-0.1.8/README.md` & `lecore-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `lecore-0.1.8/pyproject.toml` & `lecore-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lecore"
 description = "Logic Elements core utilities"
-version = "0.1.8"
+version = "0.1.9"
 authors = [
   { name="Jan Bartovský", email="jan.bartovsky@logicelements.cz" },
 ]
 readme = "README.md"
 
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `lecore-0.1.8/src/lecore/LeBin/RegisterMap.py` & `lecore-0.1.9/src/lecore/LeBin/RegisterMap.py`

 * *Files identical despite different names*

### Comparing `lecore-0.1.8/src/lecore/LeBin/SerialCom.py` & `lecore-0.1.9/src/lecore/LeBin/SerialCom.py`

 * *Files identical despite different names*

### Comparing `lecore-0.1.8/src/lecore/LeBin/UpgradeFirmware.py` & `lecore-0.1.9/src/lecore/LeBin/UpgradeFirmware.py`

 * *Files identical despite different names*

### Comparing `lecore-0.1.8/src/lecore/LeBin/VisualLeBin.py` & `lecore-0.1.9/src/lecore/LeBin/VisualLeBin.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 from .RegisterMap import *
-import PySimpleGUI as SG
+try:
+    import PySimpleGUI as SG
+except ImportError:
+    import datetime as SG
 
 
 class VisualLeBin:
     """
     Visual application for LeBin protocol with serial communication
     """
     HEX_SUFFIX = "_H"
```

### Comparing `lecore-0.1.8/src/lecore/Looger.py` & `lecore-0.1.9/src/lecore/Looger.py`

 * *Files identical despite different names*

### Comparing `lecore-0.1.8/src/lecore/TestFrame/CoreTest.py` & `lecore-0.1.9/src/lecore/TestFrame/CoreTest.py`

 * *Files identical despite different names*

### Comparing `lecore-0.1.8/src/lecore/TestFrame/RtuClient.py` & `lecore-0.1.9/src/lecore/TestFrame/RtuClient.py`

 * *Files identical despite different names*

### Comparing `lecore-0.1.8/src/lecore/TestFrame/TestUtils.py` & `lecore-0.1.9/src/lecore/TestFrame/TestUtils.py`

 * *Files identical despite different names*

### Comparing `lecore-0.1.8/src/lecore/VisualModbus/AppLogging.py` & `lecore-0.1.9/src/lecore/VisualModbus/AppLogging.py`

 * *Files identical despite different names*

### Comparing `lecore-0.1.8/src/lecore/VisualModbus/Crc32.py` & `lecore-0.1.9/src/lecore/VisualModbus/Crc32.py`

 * *Files identical despite different names*

### Comparing `lecore-0.1.8/src/lecore/VisualModbus/HelpAbout.py` & `lecore-0.1.9/src/lecore/VisualModbus/HelpAbout.py`

 * *Files identical despite different names*

### Comparing `lecore-0.1.8/src/lecore/VisualModbus/MbClient.py` & `lecore-0.1.9/src/lecore/VisualModbus/MbClient.py`

 * *Files identical despite different names*

### Comparing `lecore-0.1.8/src/lecore/VisualModbus/MbUpgrade.py` & `lecore-0.1.9/src/lecore/VisualModbus/MbUpgrade.py`

 * *Files identical despite different names*

### Comparing `lecore-0.1.8/src/lecore/VisualModbus/ReadWrite.py` & `lecore-0.1.9/src/lecore/VisualModbus/ReadWrite.py`

 * *Files identical despite different names*

### Comparing `lecore-0.1.8/src/lecore/VisualModbus/RegMap.py` & `lecore-0.1.9/src/lecore/VisualModbus/RegMap.py`

 * *Files identical despite different names*

### Comparing `lecore-0.1.8/src/lecore/VisualModbus/VisualMbApp.py` & `lecore-0.1.9/src/lecore/VisualModbus/VisualMbApp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 # import build-in modules
-import PySimpleGUI as SG
+try:
+    import PySimpleGUI as SG
+except ImportError:
+    import datetime as SG    
 # import own modules
 from .AppLogging import *
 from .RegMap import RegMap
 from .MbClient import MbClient
 from .HelpAbout import *
 from .VmSettings import *
 from .MbUpgrade import *
```

### Comparing `lecore-0.1.8/src/lecore/VisualModbus/VmSettings.py` & `lecore-0.1.9/src/lecore/VisualModbus/VmSettings.py`

 * *Files identical despite different names*

### Comparing `lecore-0.1.8/src/lecore.egg-info/PKG-INFO` & `lecore-0.1.9/src/lecore.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lecore
-Version: 0.1.8
+Version: 0.1.9
 Summary: Logic Elements core utilities
 Author-email: Jan Bartovský <jan.bartovsky@logicelements.cz>
 Project-URL: Homepage, http://www.logicelements.cz
 Keywords: logicelements,looger,development
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lecore-0.1.8/src/lecore.egg-info/SOURCES.txt` & `lecore-0.1.9/src/lecore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lecore-0.1.8/tests/test_frame.py` & `lecore-0.1.9/tests/test_frame.py`

 * *Files identical despite different names*

### Comparing `lecore-0.1.8/tests/test_lebin.py` & `lecore-0.1.9/tests/test_lebin.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 try:
     import lecore.LeBin as LeBin
 except ImportError:
     import src.lecore.LeBin as LeBin
 
 
+# import src.lecore.LeBin as LeBin
+
 pth = os.path.dirname(os.path.abspath(__file__))
 
 
 class TestSimple(unittest.TestCase):
 
     @classmethod
     def setUpClass(cls):
```

### Comparing `lecore-0.1.8/tests/test_looger.py` & `lecore-0.1.9/tests/test_looger.py`

 * *Files identical despite different names*

### Comparing `lecore-0.1.8/tests/test_modbus.py` & `lecore-0.1.9/tests/test_modbus.py`

 * *Files identical despite different names*

