# Comparing `tmp/pillar1-0.1.5.5.tar.gz` & `tmp/pillar1-0.1.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pillar1-0.1.5.5.tar", last modified: Tue Jun 20 00:32:49 2023, max compression
+gzip compressed data, was "pillar1-0.1.5.6.tar", last modified: Tue Jun 20 00:44:49 2023, max compression
```

## Comparing `pillar1-0.1.5.5.tar` & `pillar1-0.1.5.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-20 00:32:49.984423 pillar1-0.1.5.5/
--rw-r--r--   0 aymanhajja   (501) staff       (20)     3202 2023-06-20 00:32:49.984293 pillar1-0.1.5.5/PKG-INFO
--rw-r--r--   0 aymanhajja   (501) staff       (20)     2842 2023-06-19 22:34:12.000000 pillar1-0.1.5.5/README.md
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-20 00:32:49.983431 pillar1-0.1.5.5/pillar1/
--rw-r--r--   0 aymanhajja   (501) staff       (20)       27 2023-06-19 22:42:24.000000 pillar1-0.1.5.5/pillar1/__init__.py
--rw-r--r--   0 aymanhajja   (501) staff       (20)     2585 2023-06-20 00:32:34.000000 pillar1-0.1.5.5/pillar1/pillar1.py
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-20 00:32:49.984096 pillar1-0.1.5.5/pillar1.egg-info/
--rw-r--r--   0 aymanhajja   (501) staff       (20)     3202 2023-06-20 00:32:49.000000 pillar1-0.1.5.5/pillar1.egg-info/PKG-INFO
--rw-r--r--   0 aymanhajja   (501) staff       (20)      181 2023-06-20 00:32:49.000000 pillar1-0.1.5.5/pillar1.egg-info/SOURCES.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)        1 2023-06-20 00:32:49.000000 pillar1-0.1.5.5/pillar1.egg-info/dependency_links.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)        8 2023-06-20 00:32:49.000000 pillar1-0.1.5.5/pillar1.egg-info/top_level.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)       38 2023-06-20 00:32:49.984465 pillar1-0.1.5.5/setup.cfg
--rw-r--r--   0 aymanhajja   (501) staff       (20)      621 2023-06-20 00:32:45.000000 pillar1-0.1.5.5/setup.py
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-20 00:44:49.178505 pillar1-0.1.5.6/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     3202 2023-06-20 00:44:49.178349 pillar1-0.1.5.6/PKG-INFO
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     2842 2023-06-19 22:34:12.000000 pillar1-0.1.5.6/README.md
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-20 00:44:49.177404 pillar1-0.1.5.6/pillar1/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)       27 2023-06-19 22:42:24.000000 pillar1-0.1.5.6/pillar1/__init__.py
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     2585 2023-06-20 00:32:34.000000 pillar1-0.1.5.6/pillar1/pillar1.py
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-20 00:44:49.178130 pillar1-0.1.5.6/pillar1.egg-info/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     3202 2023-06-20 00:44:49.000000 pillar1-0.1.5.6/pillar1.egg-info/PKG-INFO
+-rw-r--r--   0 aymanhajja   (501) staff       (20)      181 2023-06-20 00:44:49.000000 pillar1-0.1.5.6/pillar1.egg-info/SOURCES.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)        1 2023-06-20 00:44:49.000000 pillar1-0.1.5.6/pillar1.egg-info/dependency_links.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)        8 2023-06-20 00:44:49.000000 pillar1-0.1.5.6/pillar1.egg-info/top_level.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)       38 2023-06-20 00:44:49.178550 pillar1-0.1.5.6/setup.cfg
+-rw-r--r--   0 aymanhajja   (501) staff       (20)      621 2023-06-20 00:44:45.000000 pillar1-0.1.5.6/setup.py
```

### Comparing `pillar1-0.1.5.5/PKG-INFO` & `pillar1-0.1.5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pillar1
-Version: 0.1.5.5
+Version: 0.1.5.6
 Summary: Official package for Pillar1 company
 Home-page: https://github.com/amhajja/pillar1
 Author: Ayman Hajja
 Author-email: amhajja@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
```

### Comparing `pillar1-0.1.5.5/README.md` & `pillar1-0.1.5.6/README.md`

 * *Files identical despite different names*

### Comparing `pillar1-0.1.5.5/pillar1/pillar1.py` & `pillar1-0.1.5.6/pillar1/pillar1.py`

 * *Files identical despite different names*

### Comparing `pillar1-0.1.5.5/pillar1.egg-info/PKG-INFO` & `pillar1-0.1.5.6/pillar1.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pillar1
-Version: 0.1.5.5
+Version: 0.1.5.6
 Summary: Official package for Pillar1 company
 Home-page: https://github.com/amhajja/pillar1
 Author: Ayman Hajja
 Author-email: amhajja@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
```

### Comparing `pillar1-0.1.5.5/setup.py` & `pillar1-0.1.5.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pillar1',
-    version='0.1.5.5',
+    version='0.1.5.6',
     packages=find_packages(),
     description='Official package for Pillar1 company',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Ayman Hajja',
     author_email='amhajja@gmail.com',
     url='https://github.com/amhajja/pillar1',
```

