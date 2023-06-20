# Comparing `tmp/icn3dpy-3.8.1.tar.gz` & `tmp/icn3dpy-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/icn3dpy-3.8.1.tar", last modified: Fri Jan 28 17:50:27 2022, max compression
+gzip compressed data, was "dist/icn3dpy-3.9.0.tar", last modified: Mon Feb 28 14:28:14 2022, max compression
```

## Comparing `icn3dpy-3.8.1.tar` & `icn3dpy-3.9.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 joewang    (501) staff       (20)        0 2022-01-28 17:50:27.000000 icn3dpy-3.8.1/
--rw-r--r--   0 joewang    (501) staff       (20)     3661 2022-01-28 17:50:27.000000 icn3dpy-3.8.1/PKG-INFO
--rw-r--r--   0 joewang    (501) staff       (20)      128 2022-01-27 13:39:07.000000 icn3dpy-3.8.1/README
--rw-r--r--   0 joewang    (501) staff       (20)     2117 2022-01-07 14:18:12.000000 icn3dpy-3.8.1/README.md
-drwxr-xr-x   0 joewang    (501) staff       (20)        0 2022-01-28 17:50:27.000000 icn3dpy-3.8.1/icn3dpy/
--rw-r--r--   0 joewang    (501) staff       (20)     4397 2021-07-04 12:20:28.000000 icn3dpy-3.8.1/icn3dpy/__init__.py
--rw-r--r--   0 joewang    (501) staff       (20)     4029 2020-07-11 01:14:12.000000 icn3dpy-3.8.1/icn3dpy/__init__v1.py
--rw-r--r--   0 joewang    (501) staff       (20)     3647 2020-07-11 01:14:12.000000 icn3dpy-3.8.1/icn3dpy/__init__v2.py
--rw-r--r--   0 joewang    (501) staff       (20)     4772 2020-07-16 02:35:40.000000 icn3dpy-3.8.1/icn3dpy/__init__v3.py
-drwxr-xr-x   0 joewang    (501) staff       (20)        0 2022-01-28 17:50:27.000000 icn3dpy-3.8.1/icn3dpy.egg-info/
--rw-r--r--   0 joewang    (501) staff       (20)     3661 2022-01-28 17:50:26.000000 icn3dpy-3.8.1/icn3dpy.egg-info/PKG-INFO
--rw-r--r--   0 joewang    (501) staff       (20)      265 2022-01-28 17:50:26.000000 icn3dpy-3.8.1/icn3dpy.egg-info/SOURCES.txt
--rw-r--r--   0 joewang    (501) staff       (20)        1 2022-01-28 17:50:26.000000 icn3dpy-3.8.1/icn3dpy.egg-info/dependency_links.txt
--rw-r--r--   0 joewang    (501) staff       (20)       17 2022-01-28 17:50:26.000000 icn3dpy-3.8.1/icn3dpy.egg-info/requires.txt
--rw-r--r--   0 joewang    (501) staff       (20)        8 2022-01-28 17:50:26.000000 icn3dpy-3.8.1/icn3dpy.egg-info/top_level.txt
--rw-r--r--   0 joewang    (501) staff       (20)       38 2022-01-28 17:50:27.000000 icn3dpy-3.8.1/setup.cfg
--rw-r--r--   0 joewang    (501) staff       (20)     2784 2022-01-28 17:50:20.000000 icn3dpy-3.8.1/setup.py
+drwxr-xr-x   0 joewang    (501) staff       (20)        0 2022-02-28 14:28:14.000000 icn3dpy-3.9.0/
+-rw-r--r--   0 joewang    (501) staff       (20)     3661 2022-02-28 14:28:14.000000 icn3dpy-3.9.0/PKG-INFO
+-rw-r--r--   0 joewang    (501) staff       (20)      128 2022-01-27 13:39:07.000000 icn3dpy-3.9.0/README
+-rw-r--r--   0 joewang    (501) staff       (20)     2117 2022-01-07 14:18:12.000000 icn3dpy-3.9.0/README.md
+drwxr-xr-x   0 joewang    (501) staff       (20)        0 2022-02-28 14:28:14.000000 icn3dpy-3.9.0/icn3dpy/
+-rw-r--r--   0 joewang    (501) staff       (20)     4397 2021-07-04 12:20:28.000000 icn3dpy-3.9.0/icn3dpy/__init__.py
+-rw-r--r--   0 joewang    (501) staff       (20)     4029 2020-07-11 01:14:12.000000 icn3dpy-3.9.0/icn3dpy/__init__v1.py
+-rw-r--r--   0 joewang    (501) staff       (20)     3647 2020-07-11 01:14:12.000000 icn3dpy-3.9.0/icn3dpy/__init__v2.py
+-rw-r--r--   0 joewang    (501) staff       (20)     4772 2020-07-16 02:35:40.000000 icn3dpy-3.9.0/icn3dpy/__init__v3.py
+drwxr-xr-x   0 joewang    (501) staff       (20)        0 2022-02-28 14:28:14.000000 icn3dpy-3.9.0/icn3dpy.egg-info/
+-rw-r--r--   0 joewang    (501) staff       (20)     3661 2022-02-28 14:28:13.000000 icn3dpy-3.9.0/icn3dpy.egg-info/PKG-INFO
+-rw-r--r--   0 joewang    (501) staff       (20)      265 2022-02-28 14:28:13.000000 icn3dpy-3.9.0/icn3dpy.egg-info/SOURCES.txt
+-rw-r--r--   0 joewang    (501) staff       (20)        1 2022-02-28 14:28:13.000000 icn3dpy-3.9.0/icn3dpy.egg-info/dependency_links.txt
+-rw-r--r--   0 joewang    (501) staff       (20)       17 2022-02-28 14:28:13.000000 icn3dpy-3.9.0/icn3dpy.egg-info/requires.txt
+-rw-r--r--   0 joewang    (501) staff       (20)        8 2022-02-28 14:28:13.000000 icn3dpy-3.9.0/icn3dpy.egg-info/top_level.txt
+-rw-r--r--   0 joewang    (501) staff       (20)       38 2022-02-28 14:28:14.000000 icn3dpy-3.9.0/setup.cfg
+-rw-r--r--   0 joewang    (501) staff       (20)     2784 2022-02-28 14:27:54.000000 icn3dpy-3.9.0/setup.py
```

### Comparing `icn3dpy-3.8.1/PKG-INFO` & `icn3dpy-3.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icn3dpy
-Version: 3.8.1
+Version: 3.9.0
 Summary: An IPython interface for embedding iCn3D viewer
 Home-page: https://github.com/ncbi/icn3d
 Author: Jiyao Wang
 Author-email: wangjiy@ncbi.lm.nih.gov
 License: MIT License
 Description: icn3dpy
         =======
```

### Comparing `icn3dpy-3.8.1/README.md` & `icn3dpy-3.9.0/README.md`

 * *Files identical despite different names*

### Comparing `icn3dpy-3.8.1/icn3dpy/__init__.py` & `icn3dpy-3.9.0/icn3dpy/__init__.py`

 * *Files identical despite different names*

### Comparing `icn3dpy-3.8.1/icn3dpy/__init__v1.py` & `icn3dpy-3.9.0/icn3dpy/__init__v1.py`

 * *Files identical despite different names*

### Comparing `icn3dpy-3.8.1/icn3dpy/__init__v2.py` & `icn3dpy-3.9.0/icn3dpy/__init__v2.py`

 * *Files identical despite different names*

### Comparing `icn3dpy-3.8.1/icn3dpy/__init__v3.py` & `icn3dpy-3.9.0/icn3dpy/__init__v3.py`

 * *Files identical despite different names*

### Comparing `icn3dpy-3.8.1/icn3dpy.egg-info/PKG-INFO` & `icn3dpy-3.9.0/icn3dpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icn3dpy
-Version: 3.8.1
+Version: 3.9.0
 Summary: An IPython interface for embedding iCn3D viewer
 Home-page: https://github.com/ncbi/icn3d
 Author: Jiyao Wang
 Author-email: wangjiy@ncbi.lm.nih.gov
 License: MIT License
 Description: icn3dpy
         =======
```

### Comparing `icn3dpy-3.8.1/setup.py` & `icn3dpy-3.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 setup(
     name='icn3dpy',
 
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='3.8.1',
+    version='3.9.0',
 
     description='An IPython interface for embedding iCn3D viewer',
     long_description=long_description,
     long_description_content_type='text/markdown',
 
     # The project's main homepage.
     url='https://github.com/ncbi/icn3d',
```

