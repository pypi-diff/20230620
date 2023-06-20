# Comparing `tmp/pillar1-0.1.5.2.tar.gz` & `tmp/pillar1-0.1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pillar1-0.1.5.2.tar", last modified: Tue Jun 20 00:20:21 2023, max compression
+gzip compressed data, was "pillar1-0.1.5.3.tar", last modified: Tue Jun 20 00:23:05 2023, max compression
```

## Comparing `pillar1-0.1.5.2.tar` & `pillar1-0.1.5.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-20 00:20:21.215910 pillar1-0.1.5.2/
--rw-r--r--   0 aymanhajja   (501) staff       (20)     3202 2023-06-20 00:20:21.215798 pillar1-0.1.5.2/PKG-INFO
--rw-r--r--   0 aymanhajja   (501) staff       (20)     2842 2023-06-19 22:34:12.000000 pillar1-0.1.5.2/README.md
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-20 00:20:21.215031 pillar1-0.1.5.2/pillar1/
--rw-r--r--   0 aymanhajja   (501) staff       (20)       27 2023-06-19 22:42:24.000000 pillar1-0.1.5.2/pillar1/__init__.py
--rw-r--r--   0 aymanhajja   (501) staff       (20)     2490 2023-06-20 00:19:43.000000 pillar1-0.1.5.2/pillar1/pillar1.py
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-20 00:20:21.215635 pillar1-0.1.5.2/pillar1.egg-info/
--rw-r--r--   0 aymanhajja   (501) staff       (20)     3202 2023-06-20 00:20:21.000000 pillar1-0.1.5.2/pillar1.egg-info/PKG-INFO
--rw-r--r--   0 aymanhajja   (501) staff       (20)      181 2023-06-20 00:20:21.000000 pillar1-0.1.5.2/pillar1.egg-info/SOURCES.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)        1 2023-06-20 00:20:21.000000 pillar1-0.1.5.2/pillar1.egg-info/dependency_links.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)        8 2023-06-20 00:20:21.000000 pillar1-0.1.5.2/pillar1.egg-info/top_level.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)       38 2023-06-20 00:20:21.215948 pillar1-0.1.5.2/setup.cfg
--rw-r--r--   0 aymanhajja   (501) staff       (20)      621 2023-06-20 00:19:57.000000 pillar1-0.1.5.2/setup.py
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-20 00:23:05.051145 pillar1-0.1.5.3/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     3202 2023-06-20 00:23:05.051026 pillar1-0.1.5.3/PKG-INFO
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     2842 2023-06-19 22:34:12.000000 pillar1-0.1.5.3/README.md
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-20 00:23:05.050345 pillar1-0.1.5.3/pillar1/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)       27 2023-06-19 22:42:24.000000 pillar1-0.1.5.3/pillar1/__init__.py
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     2500 2023-06-20 00:22:57.000000 pillar1-0.1.5.3/pillar1/pillar1.py
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-20 00:23:05.050857 pillar1-0.1.5.3/pillar1.egg-info/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     3202 2023-06-20 00:23:05.000000 pillar1-0.1.5.3/pillar1.egg-info/PKG-INFO
+-rw-r--r--   0 aymanhajja   (501) staff       (20)      181 2023-06-20 00:23:05.000000 pillar1-0.1.5.3/pillar1.egg-info/SOURCES.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)        1 2023-06-20 00:23:05.000000 pillar1-0.1.5.3/pillar1.egg-info/dependency_links.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)        8 2023-06-20 00:23:05.000000 pillar1-0.1.5.3/pillar1.egg-info/top_level.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)       38 2023-06-20 00:23:05.051189 pillar1-0.1.5.3/setup.cfg
+-rw-r--r--   0 aymanhajja   (501) staff       (20)      621 2023-06-20 00:23:02.000000 pillar1-0.1.5.3/setup.py
```

### Comparing `pillar1-0.1.5.2/PKG-INFO` & `pillar1-0.1.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pillar1
-Version: 0.1.5.2
+Version: 0.1.5.3
 Summary: Official package for Pillar1 company
 Home-page: https://github.com/amhajja/pillar1
 Author: Ayman Hajja
 Author-email: amhajja@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
```

### Comparing `pillar1-0.1.5.2/README.md` & `pillar1-0.1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `pillar1-0.1.5.2/pillar1/pillar1.py` & `pillar1-0.1.5.3/pillar1/pillar1.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         self.client = boto3.client(
             'sagemaker-runtime',
             aws_access_key_id=user_name,
             aws_secret_access_key=password,
             region_name='us-west-2'
         )
 
-    def query(self, prompt):
+    def query(self, prompt: str = ''):
         def submit_request(prompt):
             payload = {
                 'inputs': prompt,
                 "parameters": {
                     "do_sample": True,
                     "top_p": 0.7,
                     "temperature": 0.7,
```

### Comparing `pillar1-0.1.5.2/pillar1.egg-info/PKG-INFO` & `pillar1-0.1.5.3/pillar1.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pillar1
-Version: 0.1.5.2
+Version: 0.1.5.3
 Summary: Official package for Pillar1 company
 Home-page: https://github.com/amhajja/pillar1
 Author: Ayman Hajja
 Author-email: amhajja@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
```

### Comparing `pillar1-0.1.5.2/setup.py` & `pillar1-0.1.5.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pillar1',
-    version='0.1.5.2',
+    version='0.1.5.3',
     packages=find_packages(),
     description='Official package for Pillar1 company',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Ayman Hajja',
     author_email='amhajja@gmail.com',
     url='https://github.com/amhajja/pillar1',
```

