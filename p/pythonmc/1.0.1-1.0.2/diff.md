# Comparing `tmp/pythonmc-1.0.1.tar.gz` & `tmp/pythonmc-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythonmc-1.0.1.tar", last modified: Tue Jun 20 00:54:30 2023, max compression
+gzip compressed data, was "pythonmc-1.0.2.tar", last modified: Tue Jun 20 01:31:13 2023, max compression
```

## Comparing `pythonmc-1.0.1.tar` & `pythonmc-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 00:54:30.347332 pythonmc-1.0.1/
--rw-rw-rw-   0        0        0     4674 2023-06-20 00:54:30.347332 pythonmc-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     4161 2023-06-19 22:16:33.000000 pythonmc-1.0.1/README.md
--rw-rw-rw-   0        0        0      108 2023-06-20 00:42:26.000000 pythonmc-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      675 2023-06-20 00:54:30.347332 pythonmc-1.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-20 00:54:30.331712 pythonmc-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-20 00:54:30.331712 pythonmc-1.0.1/src/pythonmc/
--rw-rw-rw-   0        0        0    95343 2023-06-20 00:52:33.000000 pythonmc-1.0.1/src/pythonmc/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 00:54:30.347332 pythonmc-1.0.1/src/pythonmc.egg-info/
--rw-rw-rw-   0        0        0     4674 2023-06-20 00:54:30.000000 pythonmc-1.0.1/src/pythonmc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      203 2023-06-20 00:54:30.000000 pythonmc-1.0.1/src/pythonmc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 00:54:30.000000 pythonmc-1.0.1/src/pythonmc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-20 00:54:30.000000 pythonmc-1.0.1/src/pythonmc.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-20 01:31:13.642351 pythonmc-1.0.2/
+-rw-rw-rw-   0        0        0     4674 2023-06-20 01:31:13.642351 pythonmc-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4161 2023-06-19 22:16:33.000000 pythonmc-1.0.2/README.md
+-rw-rw-rw-   0        0        0      108 2023-06-20 00:42:26.000000 pythonmc-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0      675 2023-06-20 01:31:13.643351 pythonmc-1.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-20 01:31:13.634533 pythonmc-1.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-06-20 01:31:13.641347 pythonmc-1.0.2/src/pythonmc.egg-info/
+-rw-rw-rw-   0        0        0     4674 2023-06-20 01:31:13.000000 pythonmc-1.0.2/src/pythonmc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      178 2023-06-20 01:31:13.000000 pythonmc-1.0.2/src/pythonmc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 01:31:13.000000 pythonmc-1.0.2/src/pythonmc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 01:31:13.000000 pythonmc-1.0.2/src/pythonmc.egg-info/top_level.txt
```

### Comparing `pythonmc-1.0.1/PKG-INFO` & `pythonmc-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythonmc
-Version: 1.0.1
+Version: 1.0.2
 Summary: The python library for PythonMC
 Home-page: https://github.com/RevolvingMadness/PythonMC
 Author: RevolvingMadness
 Author-email: revolvingmad@gmail.com
 Project-URL: Bug Tracker, https://github.com/RevolvingMadness/PythonMC/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pythonmc Version: 1.0.1 Summary: The python library
+Metadata-Version: 2.1 Name: pythonmc Version: 1.0.2 Summary: The python library
 for PythonMC Home-page: https://github.com/RevolvingMadness/PythonMC Author:
 RevolvingMadness Author-email: revolvingmad@gmail.com Project-URL: Bug Tracker,
 https://github.com/RevolvingMadness/PythonMC/issues Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.9
 Description-Content-Type: text/markdown  [![Contributors][contributors-shield]]
 [contributors-url] [![Forks][forks-shield]][forks-url] [![Stargazers][stars-
```

### Comparing `pythonmc-1.0.1/README.md` & `pythonmc-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pythonmc-1.0.1/setup.cfg` & `pythonmc-1.0.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 7974 686f 6e6d 630d 0a76 6572   = pythonmc..ver
-00000020: 7369 6f6e 203d 2031 2e30 2e31 0d0a 6175  sion = 1.0.1..au
+00000020: 7369 6f6e 203d 2031 2e30 2e32 0d0a 6175  sion = 1.0.2..au
 00000030: 7468 6f72 203d 2052 6576 6f6c 7669 6e67  thor = Revolving
 00000040: 4d61 646e 6573 730d 0a61 7574 686f 725f  Madness..author_
 00000050: 656d 6169 6c20 3d20 7265 766f 6c76 696e  email = revolvin
 00000060: 676d 6164 4067 6d61 696c 2e63 6f6d 0d0a  gmad@gmail.com..
 00000070: 6465 7363 7269 7074 696f 6e20 3d20 5468  description = Th
 00000080: 6520 7079 7468 6f6e 206c 6962 7261 7279  e python library
 00000090: 2066 6f72 2050 7974 686f 6e4d 430d 0a6c   for PythonMC..l
```

### Comparing `pythonmc-1.0.1/src/pythonmc.egg-info/PKG-INFO` & `pythonmc-1.0.2/src/pythonmc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythonmc
-Version: 1.0.1
+Version: 1.0.2
 Summary: The python library for PythonMC
 Home-page: https://github.com/RevolvingMadness/PythonMC
 Author: RevolvingMadness
 Author-email: revolvingmad@gmail.com
 Project-URL: Bug Tracker, https://github.com/RevolvingMadness/PythonMC/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pythonmc Version: 1.0.1 Summary: The python library
+Metadata-Version: 2.1 Name: pythonmc Version: 1.0.2 Summary: The python library
 for PythonMC Home-page: https://github.com/RevolvingMadness/PythonMC Author:
 RevolvingMadness Author-email: revolvingmad@gmail.com Project-URL: Bug Tracker,
 https://github.com/RevolvingMadness/PythonMC/issues Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.9
 Description-Content-Type: text/markdown  [![Contributors][contributors-shield]]
 [contributors-url] [![Forks][forks-shield]][forks-url] [![Stargazers][stars-
```

