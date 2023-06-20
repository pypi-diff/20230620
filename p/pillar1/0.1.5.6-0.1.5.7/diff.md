# Comparing `tmp/pillar1-0.1.5.6.tar.gz` & `tmp/pillar1-0.1.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pillar1-0.1.5.6.tar", last modified: Tue Jun 20 00:44:49 2023, max compression
+gzip compressed data, was "pillar1-0.1.5.7.tar", last modified: Tue Jun 20 21:36:06 2023, max compression
```

## Comparing `pillar1-0.1.5.6.tar` & `pillar1-0.1.5.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-20 00:44:49.178505 pillar1-0.1.5.6/
--rw-r--r--   0 aymanhajja   (501) staff       (20)     3202 2023-06-20 00:44:49.178349 pillar1-0.1.5.6/PKG-INFO
--rw-r--r--   0 aymanhajja   (501) staff       (20)     2842 2023-06-19 22:34:12.000000 pillar1-0.1.5.6/README.md
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-20 00:44:49.177404 pillar1-0.1.5.6/pillar1/
--rw-r--r--   0 aymanhajja   (501) staff       (20)       27 2023-06-19 22:42:24.000000 pillar1-0.1.5.6/pillar1/__init__.py
--rw-r--r--   0 aymanhajja   (501) staff       (20)     2585 2023-06-20 00:32:34.000000 pillar1-0.1.5.6/pillar1/pillar1.py
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-20 00:44:49.178130 pillar1-0.1.5.6/pillar1.egg-info/
--rw-r--r--   0 aymanhajja   (501) staff       (20)     3202 2023-06-20 00:44:49.000000 pillar1-0.1.5.6/pillar1.egg-info/PKG-INFO
--rw-r--r--   0 aymanhajja   (501) staff       (20)      181 2023-06-20 00:44:49.000000 pillar1-0.1.5.6/pillar1.egg-info/SOURCES.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)        1 2023-06-20 00:44:49.000000 pillar1-0.1.5.6/pillar1.egg-info/dependency_links.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)        8 2023-06-20 00:44:49.000000 pillar1-0.1.5.6/pillar1.egg-info/top_level.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)       38 2023-06-20 00:44:49.178550 pillar1-0.1.5.6/setup.cfg
--rw-r--r--   0 aymanhajja   (501) staff       (20)      621 2023-06-20 00:44:45.000000 pillar1-0.1.5.6/setup.py
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-20 21:36:06.267908 pillar1-0.1.5.7/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     3202 2023-06-20 21:36:06.267776 pillar1-0.1.5.7/PKG-INFO
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     2842 2023-06-19 22:34:12.000000 pillar1-0.1.5.7/README.md
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-20 21:36:06.266893 pillar1-0.1.5.7/pillar1/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)       27 2023-06-19 22:42:24.000000 pillar1-0.1.5.7/pillar1/__init__.py
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     2348 2023-06-20 21:33:54.000000 pillar1-0.1.5.7/pillar1/pillar1.py
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-20 21:36:06.267550 pillar1-0.1.5.7/pillar1.egg-info/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     3202 2023-06-20 21:36:06.000000 pillar1-0.1.5.7/pillar1.egg-info/PKG-INFO
+-rw-r--r--   0 aymanhajja   (501) staff       (20)      181 2023-06-20 21:36:06.000000 pillar1-0.1.5.7/pillar1.egg-info/SOURCES.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)        1 2023-06-20 21:36:06.000000 pillar1-0.1.5.7/pillar1.egg-info/dependency_links.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)        8 2023-06-20 21:36:06.000000 pillar1-0.1.5.7/pillar1.egg-info/top_level.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)       38 2023-06-20 21:36:06.267950 pillar1-0.1.5.7/setup.cfg
+-rw-r--r--   0 aymanhajja   (501) staff       (20)      621 2023-06-20 21:34:02.000000 pillar1-0.1.5.7/setup.py
```

### Comparing `pillar1-0.1.5.6/PKG-INFO` & `pillar1-0.1.5.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pillar1
-Version: 0.1.5.6
+Version: 0.1.5.7
 Summary: Official package for Pillar1 company
 Home-page: https://github.com/amhajja/pillar1
 Author: Ayman Hajja
 Author-email: amhajja@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
```

### Comparing `pillar1-0.1.5.6/README.md` & `pillar1-0.1.5.7/README.md`

 * *Files identical despite different names*

### Comparing `pillar1-0.1.5.6/pillar1/pillar1.py` & `pillar1-0.1.5.7/pillar1/pillar1.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,20 @@
 import json
 import boto3
 import ipywidgets as widgets
 from IPython.display import display
 
-MODEL_META = {
-    'falcon-7b-instruct': {
-        'endpoint_name': 'huggingface-pytorch-tgi-inference-2023-06-19-20-08-19-092',
-    }
-}
-
 
 class Model:
-    def __init__(self, user_name: str = '', password: str = '', model_name: str = 'falcon-7b-instruct', max_new_tokens: int = 200):
-        self.model_name = model_name
+    def __init__(self, user_name: str = '', password: str = '', end_point: str = '', max_new_tokens: int = 200):
+        self.end_point = end_point
         self.prompt = None
         self.response = None
         self.max_new_tokens = max_new_tokens
 
-        self.endpoint_name = MODEL_META[self.model_name]['endpoint_name']
         self.client = boto3.client(
             'sagemaker-runtime',
             aws_access_key_id=user_name,
             aws_secret_access_key=password,
             region_name='us-west-2'
         )
 
@@ -37,15 +30,15 @@
                     "max_new_tokens": self.max_new_tokens,
                     "repetition_penalty": 1.03,
                     "stop": ["<|endoftext|>"]
                 }
             }
 
             response = self.client.invoke_endpoint(
-                EndpointName=self.endpoint_name,
+                EndpointName=self.end_point,
                 ContentType='application/json',
                 Body=json.dumps(payload)
             )
 
             self.response = json.loads(response['Body'].read())[0]['generated_text']
             print(self.response)
```

### Comparing `pillar1-0.1.5.6/pillar1.egg-info/PKG-INFO` & `pillar1-0.1.5.7/pillar1.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pillar1
-Version: 0.1.5.6
+Version: 0.1.5.7
 Summary: Official package for Pillar1 company
 Home-page: https://github.com/amhajja/pillar1
 Author: Ayman Hajja
 Author-email: amhajja@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
```

### Comparing `pillar1-0.1.5.6/setup.py` & `pillar1-0.1.5.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pillar1',
-    version='0.1.5.6',
+    version='0.1.5.7',
     packages=find_packages(),
     description='Official package for Pillar1 company',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Ayman Hajja',
     author_email='amhajja@gmail.com',
     url='https://github.com/amhajja/pillar1',
```

