# Comparing `tmp/pillar1-0.1.2.tar.gz` & `tmp/pillar1-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pillar1-0.1.2.tar", last modified: Mon Jun 19 22:35:36 2023, max compression
+gzip compressed data, was "pillar1-0.1.3.tar", last modified: Mon Jun 19 22:55:26 2023, max compression
```

## Comparing `pillar1-0.1.2.tar` & `pillar1-0.1.3.tar`

### file list

```diff
@@ -1,10 +1,14 @@
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-19 22:35:36.107558 pillar1-0.1.2/
--rw-r--r--   0 aymanhajja   (501) staff       (20)     3200 2023-06-19 22:35:36.107433 pillar1-0.1.2/PKG-INFO
--rw-r--r--   0 aymanhajja   (501) staff       (20)     2842 2023-06-19 22:34:12.000000 pillar1-0.1.2/README.md
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-19 22:35:36.107240 pillar1-0.1.2/pillar1.egg-info/
--rw-r--r--   0 aymanhajja   (501) staff       (20)     3200 2023-06-19 22:35:36.000000 pillar1-0.1.2/pillar1.egg-info/PKG-INFO
--rw-r--r--   0 aymanhajja   (501) staff       (20)      142 2023-06-19 22:35:36.000000 pillar1-0.1.2/pillar1.egg-info/SOURCES.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)        1 2023-06-19 22:35:36.000000 pillar1-0.1.2/pillar1.egg-info/dependency_links.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)        1 2023-06-19 22:35:36.000000 pillar1-0.1.2/pillar1.egg-info/top_level.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)       38 2023-06-19 22:35:36.107601 pillar1-0.1.2/setup.cfg
--rw-r--r--   0 aymanhajja   (501) staff       (20)      619 2023-06-19 22:35:33.000000 pillar1-0.1.2/setup.py
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-19 22:55:26.331085 pillar1-0.1.3/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     3201 2023-06-19 22:55:26.330961 pillar1-0.1.3/PKG-INFO
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     2842 2023-06-19 22:34:12.000000 pillar1-0.1.3/README.md
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-19 22:55:26.329919 pillar1-0.1.3/pillar1/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)       27 2023-06-19 22:42:24.000000 pillar1-0.1.3/pillar1/__init__.py
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     1427 2023-06-19 22:51:40.000000 pillar1-0.1.3/pillar1/pillar1.py
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-19 22:55:26.330784 pillar1-0.1.3/pillar1.egg-info/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     3201 2023-06-19 22:55:26.000000 pillar1-0.1.3/pillar1.egg-info/PKG-INFO
+-rw-r--r--   0 aymanhajja   (501) staff       (20)      211 2023-06-19 22:55:26.000000 pillar1-0.1.3/pillar1.egg-info/SOURCES.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)        1 2023-06-19 22:55:26.000000 pillar1-0.1.3/pillar1.egg-info/dependency_links.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)       48 2023-06-19 22:55:26.000000 pillar1-0.1.3/pillar1.egg-info/requires.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)        8 2023-06-19 22:55:26.000000 pillar1-0.1.3/pillar1.egg-info/top_level.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)       38 2023-06-19 22:55:26.331125 pillar1-0.1.3/setup.cfg
+-rw-r--r--   0 aymanhajja   (501) staff       (20)      730 2023-06-19 22:53:59.000000 pillar1-0.1.3/setup.py
```

### Comparing `pillar1-0.1.2/PKG-INFO` & `pillar1-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: pillar1
-Version: 0.1.2
+Version: 0.1.3
 Summary: Official package for Pillar1 company
 Home-page: https://github.com/amhajja/pillar1
 Author: Ayman Hajja
 Author-email: amhajja@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.6
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 
 # Pillar1: AI Solution Implementation Consulting and Product Development
 
 Unlock the Power of AI with Pillar1. We specialize in leveraging the latest advancements in artificial intelligence to transform businesses and drive innovation. Pillar1 assists businesses in implementing AI solutions, achieving their strategic objectives, and unlocking the full potential of artificial intelligence.
 
 ## Features
```

### Comparing `pillar1-0.1.2/README.md` & `pillar1-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pillar1-0.1.2/pillar1.egg-info/PKG-INFO` & `pillar1-0.1.3/pillar1.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: pillar1
-Version: 0.1.2
+Version: 0.1.3
 Summary: Official package for Pillar1 company
 Home-page: https://github.com/amhajja/pillar1
 Author: Ayman Hajja
 Author-email: amhajja@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.6
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 
 # Pillar1: AI Solution Implementation Consulting and Product Development
 
 Unlock the Power of AI with Pillar1. We specialize in leveraging the latest advancements in artificial intelligence to transform businesses and drive innovation. Pillar1 assists businesses in implementing AI solutions, achieving their strategic objectives, and unlocking the full potential of artificial intelligence.
 
 ## Features
```

### Comparing `pillar1-0.1.2/setup.py` & `pillar1-0.1.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pillar1',
-    version='0.1.2',
+    version='0.1.3',
     packages=find_packages(),
     description='Official package for Pillar1 company',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Ayman Hajja',
     author_email='amhajja@gmail.com',
     url='https://github.com/amhajja/pillar1',
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
     ],
-    python_requires='>=3.6',
+    python_requires='>=3.11',
+    install_requires=[
+        'boto3>=1.26.156',
+        'matplotlib>=3.1.2',
+        'pandas>=1.0.1'
+    ],
 )
```

