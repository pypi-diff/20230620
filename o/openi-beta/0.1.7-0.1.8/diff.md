# Comparing `tmp/openi-beta-0.1.7.tar.gz` & `tmp/openi-beta-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openi-beta-0.1.7.tar", last modified: Mon Jun 19 08:02:55 2023, max compression
+gzip compressed data, was "openi-beta-0.1.8.tar", last modified: Tue Jun 20 01:20:28 2023, max compression
```

## Comparing `openi-beta-0.1.7.tar` & `openi-beta-0.1.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-19 08:02:55.457109 openi-beta-0.1.7/
--rw-r--r--   0 jochen10518   (501) staff       (20)     2102 2023-06-19 08:02:55.456969 openi-beta-0.1.7/PKG-INFO
--rw-r--r--   0 jochen10518   (501) staff       (20)     1473 2023-06-19 07:48:49.000000 openi-beta-0.1.7/README.md
--rw-r--r--   0 jochen10518   (501) staff       (20)       38 2023-06-19 08:02:55.457164 openi-beta-0.1.7/setup.cfg
--rw-r--r--   0 jochen10518   (501) staff       (20)     1145 2023-06-19 08:02:50.000000 openi-beta-0.1.7/setup.py
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-19 08:02:55.454261 openi-beta-0.1.7/src/
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-19 08:02:55.455076 openi-beta-0.1.7/src/openi/
--rw-r--r--   0 jochen10518   (501) staff       (20)       48 2023-06-19 07:48:49.000000 openi-beta-0.1.7/src/openi/__init__.py
--rw-r--r--   0 jochen10518   (501) staff       (20)      356 2023-06-19 07:48:49.000000 openi-beta-0.1.7/src/openi/constants.py
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-19 08:02:55.455564 openi-beta-0.1.7/src/openi/dataset/
--rw-r--r--   0 jochen10518   (501) staff       (20)       22 2023-06-15 09:50:35.000000 openi-beta-0.1.7/src/openi/dataset/__init__.py
--rw-r--r--   0 jochen10518   (501) staff       (20)    12807 2023-06-19 08:01:59.000000 openi-beta-0.1.7/src/openi/dataset/dataset.py
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-19 08:02:55.455812 openi-beta-0.1.7/src/openi/utils/
--rw-r--r--   0 jochen10518   (501) staff       (20)      419 2023-06-19 07:48:49.000000 openi-beta-0.1.7/src/openi/utils/logger.py
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-19 08:02:55.456565 openi-beta-0.1.7/src/openi_beta.egg-info/
--rw-r--r--   0 jochen10518   (501) staff       (20)     2102 2023-06-19 08:02:55.000000 openi-beta-0.1.7/src/openi_beta.egg-info/PKG-INFO
--rw-r--r--   0 jochen10518   (501) staff       (20)      363 2023-06-19 08:02:55.000000 openi-beta-0.1.7/src/openi_beta.egg-info/SOURCES.txt
--rw-r--r--   0 jochen10518   (501) staff       (20)        1 2023-06-19 08:02:55.000000 openi-beta-0.1.7/src/openi_beta.egg-info/dependency_links.txt
--rw-r--r--   0 jochen10518   (501) staff       (20)       14 2023-06-19 08:02:55.000000 openi-beta-0.1.7/src/openi_beta.egg-info/requires.txt
--rw-r--r--   0 jochen10518   (501) staff       (20)        6 2023-06-19 08:02:55.000000 openi-beta-0.1.7/src/openi_beta.egg-info/top_level.txt
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-19 08:02:55.456710 openi-beta-0.1.7/test/
--rw-r--r--   0 jochen10518   (501) staff       (20)      627 2023-06-19 07:48:49.000000 openi-beta-0.1.7/test/test_upload_multi.py
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-20 01:20:28.242139 openi-beta-0.1.8/
+-rw-r--r--   0 jochen10518   (501) staff       (20)     2102 2023-06-20 01:20:28.241989 openi-beta-0.1.8/PKG-INFO
+-rw-r--r--   0 jochen10518   (501) staff       (20)     1473 2023-06-20 01:19:17.000000 openi-beta-0.1.8/README.md
+-rw-r--r--   0 jochen10518   (501) staff       (20)       38 2023-06-20 01:20:28.242197 openi-beta-0.1.8/setup.cfg
+-rw-r--r--   0 jochen10518   (501) staff       (20)     1145 2023-06-20 01:19:36.000000 openi-beta-0.1.8/setup.py
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-20 01:20:28.239147 openi-beta-0.1.8/src/
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-20 01:20:28.239818 openi-beta-0.1.8/src/openi/
+-rw-r--r--   0 jochen10518   (501) staff       (20)       48 2023-06-20 01:19:17.000000 openi-beta-0.1.8/src/openi/__init__.py
+-rw-r--r--   0 jochen10518   (501) staff       (20)      356 2023-06-20 01:19:17.000000 openi-beta-0.1.8/src/openi/constants.py
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-20 01:20:28.240114 openi-beta-0.1.8/src/openi/dataset/
+-rw-r--r--   0 jochen10518   (501) staff       (20)       22 2023-06-20 01:19:17.000000 openi-beta-0.1.8/src/openi/dataset/__init__.py
+-rw-r--r--   0 jochen10518   (501) staff       (20)    12772 2023-06-20 01:19:50.000000 openi-beta-0.1.8/src/openi/dataset/dataset.py
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-20 01:20:28.240256 openi-beta-0.1.8/src/openi/utils/
+-rw-r--r--   0 jochen10518   (501) staff       (20)      419 2023-06-20 01:19:17.000000 openi-beta-0.1.8/src/openi/utils/logger.py
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-20 01:20:28.241592 openi-beta-0.1.8/src/openi_beta.egg-info/
+-rw-r--r--   0 jochen10518   (501) staff       (20)     2102 2023-06-20 01:20:28.000000 openi-beta-0.1.8/src/openi_beta.egg-info/PKG-INFO
+-rw-r--r--   0 jochen10518   (501) staff       (20)      363 2023-06-20 01:20:28.000000 openi-beta-0.1.8/src/openi_beta.egg-info/SOURCES.txt
+-rw-r--r--   0 jochen10518   (501) staff       (20)        1 2023-06-20 01:20:28.000000 openi-beta-0.1.8/src/openi_beta.egg-info/dependency_links.txt
+-rw-r--r--   0 jochen10518   (501) staff       (20)       14 2023-06-20 01:20:28.000000 openi-beta-0.1.8/src/openi_beta.egg-info/requires.txt
+-rw-r--r--   0 jochen10518   (501) staff       (20)        6 2023-06-20 01:20:28.000000 openi-beta-0.1.8/src/openi_beta.egg-info/top_level.txt
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-20 01:20:28.241767 openi-beta-0.1.8/test/
+-rw-r--r--   0 jochen10518   (501) staff       (20)      627 2023-06-20 01:19:17.000000 openi-beta-0.1.8/test/test_upload_multi.py
```

### Comparing `openi-beta-0.1.7/PKG-INFO` & `openi-beta-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openi-beta
-Version: 0.1.7
+Version: 0.1.8
 Summary: A test package for openi pypi
 Home-page: https://openi.pcl.ac.cn/OpenIOSSG/openi-pypi
 Author: chenzh05
 Author-email: chenzh.ds@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `openi-beta-0.1.7/README.md` & `openi-beta-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `openi-beta-0.1.7/setup.py` & `openi-beta-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='openi-beta',
-    version='0.1.7',
+    version='0.1.8',
     description='A test package for openi pypi',
     package_dir={'': 'src'},
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://openi.pcl.ac.cn/OpenIOSSG/openi-pypi',
     author='chenzh05',
     author_email='chenzh.ds@outlook.com',
```

### Comparing `openi-beta-0.1.7/src/openi/dataset/dataset.py` & `openi-beta-0.1.8/src/openi/dataset/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,24 +110,22 @@
             "file_name": self.filename,
             "type": self.upload_type,
             "totalChunkCounts": self.total_chunk_counts,
             "size": self.size
         }
         x = requests.get('{}attachments/new_multipart'.format(self.app_url), params=params)
 
-        try:
-        #if x.json()["result_code"] == "0":
+        if x.json()["result_code"] == "0":
             logging.info(f'{x.url} {x} {x.reason} | params return: {x.json()}')
             self.upload_id = x.json()["uploadID"]
             self.uuid = x.json()["uuid"]
-        #else:
-        except:
+        else:
             logging.error(f'{x.url} {x} {x.reason} | {x.json()}')
             raise ConnectionRefusedError(
-                f'❌ <{x.status_code} {x.reason}>') # {x.json()["msg"]}')
+                f'❌ <{x.status_code} {x.reason}> {x.json()["msg"]}')
 
     def getMultipartURL(self, chunk_number, chunk_size):
         params = {
             "access_token": self.token,
             "dataset_id": self.dataset_id,
             "file_name": self.filename,
             "type": self.upload_type,
```

### Comparing `openi-beta-0.1.7/src/openi_beta.egg-info/PKG-INFO` & `openi-beta-0.1.8/src/openi_beta.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openi-beta
-Version: 0.1.7
+Version: 0.1.8
 Summary: A test package for openi pypi
 Home-page: https://openi.pcl.ac.cn/OpenIOSSG/openi-pypi
 Author: chenzh05
 Author-email: chenzh.ds@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `openi-beta-0.1.7/test/test_upload_multi.py` & `openi-beta-0.1.8/test/test_upload_multi.py`

 * *Files identical despite different names*

