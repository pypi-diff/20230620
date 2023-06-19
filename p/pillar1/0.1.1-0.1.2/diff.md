# Comparing `tmp/pillar1-0.1.1.tar.gz` & `tmp/pillar1-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pillar1-0.1.1.tar", last modified: Mon Jun 19 22:34:37 2023, max compression
+gzip compressed data, was "pillar1-0.1.2.tar", last modified: Mon Jun 19 22:35:36 2023, max compression
```

## Comparing `pillar1-0.1.1.tar` & `pillar1-0.1.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-19 22:34:37.301640 pillar1-0.1.1/
--rw-r--r--   0 aymanhajja   (501) staff       (20)      317 2023-06-19 22:34:37.301514 pillar1-0.1.1/PKG-INFO
--rw-r--r--   0 aymanhajja   (501) staff       (20)     2842 2023-06-19 22:34:12.000000 pillar1-0.1.1/README.md
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-19 22:34:37.301325 pillar1-0.1.1/pillar1.egg-info/
--rw-r--r--   0 aymanhajja   (501) staff       (20)      317 2023-06-19 22:34:37.000000 pillar1-0.1.1/pillar1.egg-info/PKG-INFO
--rw-r--r--   0 aymanhajja   (501) staff       (20)      142 2023-06-19 22:34:37.000000 pillar1-0.1.1/pillar1.egg-info/SOURCES.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)        1 2023-06-19 22:34:37.000000 pillar1-0.1.1/pillar1.egg-info/dependency_links.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)        1 2023-06-19 22:34:37.000000 pillar1-0.1.1/pillar1.egg-info/top_level.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)       38 2023-06-19 22:34:37.301680 pillar1-0.1.1/setup.cfg
--rw-r--r--   0 aymanhajja   (501) staff       (20)      529 2023-06-19 22:34:31.000000 pillar1-0.1.1/setup.py
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-19 22:35:36.107558 pillar1-0.1.2/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     3200 2023-06-19 22:35:36.107433 pillar1-0.1.2/PKG-INFO
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     2842 2023-06-19 22:34:12.000000 pillar1-0.1.2/README.md
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-19 22:35:36.107240 pillar1-0.1.2/pillar1.egg-info/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     3200 2023-06-19 22:35:36.000000 pillar1-0.1.2/pillar1.egg-info/PKG-INFO
+-rw-r--r--   0 aymanhajja   (501) staff       (20)      142 2023-06-19 22:35:36.000000 pillar1-0.1.2/pillar1.egg-info/SOURCES.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)        1 2023-06-19 22:35:36.000000 pillar1-0.1.2/pillar1.egg-info/dependency_links.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)        1 2023-06-19 22:35:36.000000 pillar1-0.1.2/pillar1.egg-info/top_level.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)       38 2023-06-19 22:35:36.107601 pillar1-0.1.2/setup.cfg
+-rw-r--r--   0 aymanhajja   (501) staff       (20)      619 2023-06-19 22:35:33.000000 pillar1-0.1.2/setup.py
```

### Comparing `pillar1-0.1.1/README.md` & `pillar1-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pillar1-0.1.1/setup.py` & `pillar1-0.1.2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pillar1',
-    version='0.1.1',
+    version='0.1.2',
     packages=find_packages(),
     description='Official package for Pillar1 company',
+    long_description=long_description,
+    long_description_content_type='text/markdown',
     author='Ayman Hajja',
     author_email='amhajja@gmail.com',
     url='https://github.com/amhajja/pillar1',
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
     ],
```

