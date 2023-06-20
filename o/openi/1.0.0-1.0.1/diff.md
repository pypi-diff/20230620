# Comparing `tmp/openi-1.0.0.tar.gz` & `tmp/openi-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openi-1.0.0.tar", last modified: Mon Jun 12 09:05:26 2023, max compression
+gzip compressed data, was "openi-1.0.1.tar", last modified: Tue Jun 20 03:47:41 2023, max compression
```

## Comparing `openi-1.0.0.tar` & `openi-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,22 @@
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-12 09:05:26.716138 openi-1.0.0/
--rw-r--r--   0 jochen10518   (501) staff       (20)     2092 2023-06-12 09:05:26.715989 openi-1.0.0/PKG-INFO
--rw-r--r--   0 jochen10518   (501) staff       (20)     1473 2023-06-12 09:04:22.000000 openi-1.0.0/README.md
--rw-r--r--   0 jochen10518   (501) staff       (20)       38 2023-06-12 09:05:26.716195 openi-1.0.0/setup.cfg
--rw-r--r--   0 jochen10518   (501) staff       (20)      900 2023-06-12 09:05:19.000000 openi-1.0.0/setup.py
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-12 09:05:26.713797 openi-1.0.0/src/
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-12 09:05:26.714516 openi-1.0.0/src/openi/
--rw-r--r--   0 jochen10518   (501) staff       (20)       48 2023-06-12 09:04:22.000000 openi-1.0.0/src/openi/__init__.py
--rw-r--r--   0 jochen10518   (501) staff       (20)      290 2023-06-12 09:04:22.000000 openi-1.0.0/src/openi/constants.py
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-12 09:05:26.715722 openi-1.0.0/src/openi/dataset/
--rw-r--r--   0 jochen10518   (501) staff       (20)       22 2023-05-30 08:31:28.000000 openi-1.0.0/src/openi/dataset/__init__.py
--rw-r--r--   0 jochen10518   (501) staff       (20)     9661 2023-06-12 09:04:22.000000 openi-1.0.0/src/openi/dataset/dataset.py
-drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-12 09:05:26.715234 openi-1.0.0/src/openi.egg-info/
--rw-r--r--   0 jochen10518   (501) staff       (20)     2092 2023-06-12 09:05:26.000000 openi-1.0.0/src/openi.egg-info/PKG-INFO
--rw-r--r--   0 jochen10518   (501) staff       (20)      286 2023-06-12 09:05:26.000000 openi-1.0.0/src/openi.egg-info/SOURCES.txt
--rw-r--r--   0 jochen10518   (501) staff       (20)        1 2023-06-12 09:05:26.000000 openi-1.0.0/src/openi.egg-info/dependency_links.txt
--rw-r--r--   0 jochen10518   (501) staff       (20)       14 2023-06-12 09:05:26.000000 openi-1.0.0/src/openi.egg-info/requires.txt
--rw-r--r--   0 jochen10518   (501) staff       (20)        6 2023-06-12 09:05:26.000000 openi-1.0.0/src/openi.egg-info/top_level.txt
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-20 03:47:41.743189 openi-1.0.1/
+-rw-r--r--   0 jochen10518   (501) staff       (20)     2097 2023-06-20 03:47:41.743062 openi-1.0.1/PKG-INFO
+-rw-r--r--   0 jochen10518   (501) staff       (20)     1473 2023-06-20 03:39:14.000000 openi-1.0.1/README.md
+-rw-r--r--   0 jochen10518   (501) staff       (20)       38 2023-06-20 03:47:41.743236 openi-1.0.1/setup.cfg
+-rw-r--r--   0 jochen10518   (501) staff       (20)     1140 2023-06-20 03:42:59.000000 openi-1.0.1/setup.py
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-20 03:47:41.740115 openi-1.0.1/src/
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-20 03:47:41.741070 openi-1.0.1/src/openi/
+-rw-r--r--   0 jochen10518   (501) staff       (20)       48 2023-06-20 03:39:14.000000 openi-1.0.1/src/openi/__init__.py
+-rw-r--r--   0 jochen10518   (501) staff       (20)      356 2023-06-20 03:40:01.000000 openi-1.0.1/src/openi/constants.py
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-20 03:47:41.742231 openi-1.0.1/src/openi/dataset/
+-rw-r--r--   0 jochen10518   (501) staff       (20)       22 2023-06-20 03:39:14.000000 openi-1.0.1/src/openi/dataset/__init__.py
+-rw-r--r--   0 jochen10518   (501) staff       (20)    12697 2023-06-20 03:45:33.000000 openi-1.0.1/src/openi/dataset/dataset.py
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-20 03:47:41.742528 openi-1.0.1/src/openi/utils/
+-rw-r--r--   0 jochen10518   (501) staff       (20)      419 2023-06-20 03:40:01.000000 openi-1.0.1/src/openi/utils/logger.py
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-20 03:47:41.741874 openi-1.0.1/src/openi.egg-info/
+-rw-r--r--   0 jochen10518   (501) staff       (20)     2097 2023-06-20 03:47:41.000000 openi-1.0.1/src/openi.egg-info/PKG-INFO
+-rw-r--r--   0 jochen10518   (501) staff       (20)      338 2023-06-20 03:47:41.000000 openi-1.0.1/src/openi.egg-info/SOURCES.txt
+-rw-r--r--   0 jochen10518   (501) staff       (20)        1 2023-06-20 03:47:41.000000 openi-1.0.1/src/openi.egg-info/dependency_links.txt
+-rw-r--r--   0 jochen10518   (501) staff       (20)       14 2023-06-20 03:47:41.000000 openi-1.0.1/src/openi.egg-info/requires.txt
+-rw-r--r--   0 jochen10518   (501) staff       (20)        6 2023-06-20 03:47:41.000000 openi-1.0.1/src/openi.egg-info/top_level.txt
+drwxr-xr-x   0 jochen10518   (501) staff       (20)        0 2023-06-20 03:47:41.742767 openi-1.0.1/test/
+-rw-r--r--   0 jochen10518   (501) staff       (20)      627 2023-06-20 03:39:14.000000 openi-1.0.1/test/test_upload_multi.py
```

### Comparing `openi-1.0.0/PKG-INFO` & `openi-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: openi
-Version: 1.0.0
-Summary: A package for openi pypi
+Version: 1.0.1
+Summary: A test package for openi pypi
 Home-page: https://openi.pcl.ac.cn/OpenIOSSG/openi-pypi
 Author: chenzh05
 Author-email: chenzh.ds@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `openi-1.0.0/README.md` & `openi-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `openi-1.0.0/setup.py` & `openi-1.0.1/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,16 +1,21 @@
+# python setup.py sdist bdist_wheel
+# twine upload dist/*
+# twine upload --repository testpypi dist/*
+# pip install -i https://test.pypi.org/pypi/ --extra-index-url https://pypi.org/simple <your_package_in_testpypi>
+
 from setuptools import find_packages, setup
 
-with open('README.md', 'r') as f:
+with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='openi',
-    version='1.0.0',
-    description='A package for openi pypi',
+    version='1.0.1',
+    description='A test package for openi pypi',
     package_dir={'': 'src'},
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://openi.pcl.ac.cn/OpenIOSSG/openi-pypi',
     author='chenzh05',
     author_email='chenzh.ds@outlook.com',
     license='MIT',
```

### Comparing `openi-1.0.0/src/openi/dataset/dataset.py` & `openi-1.0.1/src/openi/dataset/dataset.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 import os
 import math
 import requests
 import hashlib
 from tqdm import tqdm
-from collections import OrderedDict
+import time
 from datetime import datetime
 from ..constants import *
 
 import logging
-
-LOG_FORMAT = "%(asctime)s [%(levelname)s] - %(funcName)s() %(lineno)d: %(message)s"
-DATE_FORMAT = "%Y/%m/%d %H:%M:%S"
-logging.basicConfig(filename='openi.log', level=logging.DEBUG, format=LOG_FORMAT, datefmt=DATE_FORMAT)
-
+from openi.utils.logger import setup_logging
+setup_logging()
 
 class DatasetUploadFile:
     """
     Build APIs calls for uploading a file to openi platform.
     This class will start upload process immediatelly once being initialized. 
     """
 
@@ -35,15 +32,14 @@
         self.username = username
         self.repo = repository
         self.token = token
         self.cluster = cluster
         self.app_url = app_url
 
         # preset variables
-        # self.max_chunk_size = MAX_CHUNK_SIZE
         if cluster == "NPU":
             self.upload_type = 1
         elif cluster == "GPU":
             self.upload_type = 0
         else:
             raise ValueError(
                 f"❌ please enter a valid cluster name, 'GPU' or 'NPU'")
@@ -55,201 +51,252 @@
 
         self.size = os.path.getsize(self.filepath)
         self.upload_url = dict()
 
     """
     APIs implementation
     """
-
     def getChunks(self):
         params = {
             "access_token": self.token,
             "dataset_id": self.dataset_id,
             "md5": self.md5,
             "file_name": self.filename,
             "type": self.upload_type,
         }
         x = requests.get('{}attachments/get_chunks'.format(self.app_url), params=params)
+
         if x.status_code == 200:
+            logging.info(f'{x.url} {x} {x.reason} | params return: {x.json()}')
             self.upload_id = x.json()["uploadID"]
             self.uuid = x.json()["uuid"]
             self.uploaded_chunks = x.json()["chunks"]
             if x.json()["uploaded"] == '1':
                 self.uploaded = True
             else:
                 self.uploaded = False
+            try:
+                return [int(i.split('-')[0]) for i in x.json()["chunks"].split(',') if i != '']
+            except:
+                logging.error(f' {x.url} {x} {x.reason} | getChunks.["chunks"] not returned.')
+                raise ValueError(
+                    " f'❌ getChunks failed.")
         else:
+            logging.error(f'{x.url} {x} {x.reason}')
             raise ConnectionRefusedError(
-                f'❌ <{x.status_code} {x.reason}> {x.text}')
+                f'❌ <{x.status_code} {x.reason}>')
 
     def getDatasetID(self):
         params = {"access_token": self.token}
         x = requests.get('{}datasets/{}/{}/'.format(self.app_url, self.username, self.repo), params=params)
         if x.status_code == 200:
             try:
+                logging.info(f'{x.url} {x} {x.reason} | params return: {x.json()}')
                 self.dataset_id = x.json()["data"][0]["id"]
-            except:
-                print(
+            except Exception as e:
+                logging.error(f'{x.url} {x} {x.reason} | dataset does not exist, please create dataset before uploading files.')
+                raise ValueError(
                     f'❌ repo [{self.username}/{self.repo}]: dataset does not exist, please create dataset before uploading files.')
         else:
+            logging.error(f'{x.url} {x} {x.reason}')
             raise ConnectionRefusedError(
-                f'❌ <{x.status_code} {x.reason}> {x.text}')
+                f'❌ <{x.status_code} {x.reason}>')
 
     def newMultipart(self):
         params = {
             "access_token": self.token,
             "dataset_id": self.dataset_id,
             "md5": self.md5,
             "file_name": self.filename,
             "type": self.upload_type,
             "totalChunkCounts": self.total_chunk_counts,
             "size": self.size
         }
         x = requests.get('{}attachments/new_multipart'.format(self.app_url), params=params)
+
         if x.json()["result_code"] == "0":
+            logging.info(f'{x.url} {x} {x.reason} | params return: {x.json()}')
             self.upload_id = x.json()["uploadID"]
             self.uuid = x.json()["uuid"]
         else:
+            logging.error(f'{x.url} {x} {x.reason} | {x.json()}')
             raise ConnectionRefusedError(
                 f'❌ <{x.status_code} {x.reason}> {x.json()["msg"]}')
 
     def getMultipartURL(self, chunk_number, chunk_size):
         params = {
             "access_token": self.token,
             "dataset_id": self.dataset_id,
             "file_name": self.filename,
             "type": self.upload_type,
             "chunkNumber": chunk_number,
             "size": chunk_size,
             "uploadID": self.upload_id,
             "uuid": self.uuid
         }
-        x = requests.get('{}attachments/get_multipart_url'.format(self.app_url), params=params)
-        if x.status_code == 200:
-            self.upload_url[chunk_number] = x.json()["url"]
-        else:
-            raise ConnectionRefusedError(
-                f'❌ <{x.status_code} {x.reason}> {x.text}')
 
-    def putUpload(self, chunk_number, start, chunk_size):
+        retry = 0
+        while retry < 3:
+            try:
+                x = requests.get('{}attachments/get_multipart_url'.format(self.app_url), params=params)
+                logging.info(f'{x.url} {x} {x.reason} | params return: {x.json()}')
+                return x.json()["url"]
+            except ConnectionError:
+                logging.error(f'getMultiUrl chunk [{chunk_number}], retry={retry+1} ')
+                print(f'getMultiUrl chunk [{chunk_number}], retry={retry+1}')
+            except RuntimeError:
+                logging.error(f'getMultiUrl chunk [{chunk_number}], retry={retry+1} ')
+                print(f'getMultiUrl chunk [{chunk_number}], retry={retry+1}')
+            retry += 1
+            time.sleep(0.5)
+        logging.error(f'reach max retry, getMultiUrl chunk [{chunk_number}] failed.')
+        raise ConnectionRefusedError(
+            f'❌ reach max retry {retry}, `getMultiUrl` chunk [{chunk_number}] failed. Checkpoint saved, please upload again.')
+
+    def putUpload(self, url, chunk_number, file_chunk_data):
         headers = {"Content-Type": "text/plain"} if self.upload_type == 0 else {}
-        file_chunk_data = None
-        with open(self.filepath, 'rb') as f:
-            f.seek(start)
-            file_chunk_data = f.read(chunk_size)
-        x = requests.put(self.upload_url[chunk_number], data=file_chunk_data, headers=headers)
-        if x.status_code != 200:
-            raise ConnectionRefusedError(
-                f'❌ <{x.status_code} {x.reason}> "upload chunk [{chunk_number}] failed."')
+
+        retry = 0
+        while retry < 3:
+            try:
+                x = requests.put(url, data=file_chunk_data, headers=headers)
+                logging.info(f'{x} {x.reason} {x.url} | etag: {x.headers["ETag"]}')
+                return x.headers["ETag"]
+            except ConnectionError:
+                logging.error(f'putUpload chunk [{chunk_number}], retry={retry+1}')
+                print(f'putUpload chunk [{chunk_number}], retry={retry+1}')
+            except RuntimeError:
+                logging.error(f'putUpload chunk [{chunk_number}], retry={retry+1}')
+                print(f'putUpload chunk [{chunk_number}], retry={retry+1}')
+            retry += 1
+            time.sleep(0.5)
+        logging.error(f'reach max retry, putUpload chunk [{chunk_number}] failed.')
+        raise ConnectionRefusedError(
+            f'❌ reach max retry {retry}, `putUpload` chunk [{chunk_number}] failed. Checkpoint saved, please upload again.')
 
     def completeMultipart(self):
         params = {
             "access_token": self.token,
             "dataset_id": self.dataset_id,
             "file_name": self.filename,
             "type": self.upload_type,
             "size": self.size,
             "uploadID": self.upload_id,
             "uuid": self.uuid
         }
         x = requests.post('{}attachments/complete_multipart'.format(self.app_url), params=params)
+        logging.info(f'{x.url} {x} {x.reason} | finished completeMultipart | Fileobject: {self.__dict__}')
         if x.status_code != 200:
+            logging.error(f'{x.url} {x} {x.reason} | {x.text}')
             raise ConnectionRefusedError(
                 f'❌ <{x.status_code} {x.reason}> {x.text}')
         if x.json()["result_code"] == "-1":
+            logging.error(f'{x} {x.reason} | {x.json()}')
             raise ConnectionRefusedError(
                 f'❌ <{x.status_code} {x.reason}> {x.json()["msg"]}')
-
     """
     utils functions
     """
 
-    def stdOut(self, message=""):
-        asctime = datetime.now().strftime("%H:%M:%S")
-        return (f'{asctime}|{self.filename}|{self.cluster}|{message}')
+    def get_time(self, message=""):
+        return datetime.now().strftime("%H:%M:%S")
 
     def filePreprocess(self):
+        self.getDatasetID()
         if self.size == 0:
+            logging.error(f'[{self.filename}] File size is 0 | FileObject: {self.__dict__}')
             raise ValueError(
                 f'❌ [{self.filename}] File size is 0')
         if self.size > MAX_FILE_SIZE:
+            logging.error(f'[{self.filename}] File size exceeds 200GB | FileObject: {self.__dict__}')
             raise ValueError(
                 f'❌ [{self.filename}] File size exceeds 200GB')
 
-        chunk_size = SMALL_FILE_CHUNK_SIZE if self.size < SMALL_FILE_SIZE else LARGE_FILE_CHUNK_SIZE
-        self.total_chunk_counts = math.ceil(self.size / chunk_size)
-        self.chunks = {n: (n - 1) * chunk_size for n in range(1, self.total_chunk_counts + 1)}
-
+        self.chunk_size = SMALL_FILE_CHUNK_SIZE if self.size < SMALL_FILE_SIZE else LARGE_FILE_CHUNK_SIZE
+        self.total_chunk_counts = math.ceil(self.size / self.chunk_size)
+        #self.chunks = {n: (n - 1) * self.chunk_size for n in range(1, self.total_chunk_counts + 1)}
         self.calculateMD5()
-        self.getDatasetID()
 
     def calculateMD5(self):
-        with open(self.filepath, 'rb') as f:
-            data = f.read()
-        self.md5 = hashlib.md5(data).hexdigest()
+        """
+        计算文件的md5
+        :param self.filepath:
+        :return:
+        """
+        m = hashlib.md5()  # 创建md5对象
+        with open(self.filepath, 'rb') as fobj:
+            while True:
+                data = fobj.read(4096)
+                if not data:
+                    break
+                m.update(data)  # 更新md5对象
+
+        self.md5 = m.hexdigest()  # 返回md5对象
 
     """
     Main functions
     uploadProgressBar(): upload file with progress bar.
     uploadMain(): control flow function.
     """
 
     def uploadProgressBar(self, chunks):
-        u = self.total_chunk_counts - len(chunks)
-
+        _progress = self.chunk_size * (self.total_chunk_counts - len(chunks))
         bar_format = '{desc}{percentage:3.0f}%|{bar}{r_bar}'
-        with tqdm(total=self.size, leave=True, unit='B', unit_scale=True, unit_divisor=1000, desc=self.stdOut(),
-                  bar_format=bar_format) as pbar:
-            chunk_size = SMALL_FILE_CHUNK_SIZE if self.size < SMALL_FILE_SIZE else LARGE_FILE_CHUNK_SIZE
-
-            # checkpoint
-            if u != 0:
-                pbar.update(chunk_size * u)
-
-            # upload chunks
-            for n, v in chunks.items():
-                chunk_size = min(self.size - v, self.size, chunk_size)
-                self.getMultipartURL(n, chunk_size)
-                self.putUpload(n, v, chunk_size)
+        desc = f'{self.get_time()} - Uploading: '
+        with tqdm(total=self.size, leave=True, unit='B', unit_scale=True, unit_divisor=1000, desc=desc,
+                  bar_format=bar_format, initial=_progress) as pbar:
+            for n in chunks:
+                start_position = (n - 1) * self.chunk_size
+                chunk_size = min(self.size, self.chunk_size, self.size - start_position)
+                with open(self.filepath, 'rb') as file:
+                    file.seek(start_position)  # Move the file pointer to the desired start position
+                    data = file.read(chunk_size)  # Read the specified chunk size from the current position
+                url = self.getMultipartURL(n, chunk_size)
+                etag = self.putUpload(url, n, data)
+                if etag is None:
+                    raise RuntimeError(
+                        f'❌ Upload failed: {self.filename}({self.cluster}) '
+                        f'chunk {n} failed to upload.')
                 pbar.update(chunk_size)
-                logging.info(f"[{self.filename}]: chunk {n} to {n + chunk_size}")
+                logging.info(f'chunk {n} uploaded. | FileObject: {self.__dict__}')
+
 
     def uploadMain(self):
 
-        print(self.stdOut('dataset file processing & checking...'))
+        print(f'{self.get_time()} - `{self.filename}({self.cluster})` dataset file processing & checking...')
         # preprocess
         self.filePreprocess()
+        logging.info(f'file check finished. | FileObject: {self.__dict__}')
+
         # checking upload status
-        self.getChunks()
+        uploaded_chunks = self.getChunks()
 
-        # upload starts
+
+        #upload starts
         if self.uuid != '':
             if self.uploaded:
+                logging.error(f'Upload failed: `{self.filename}({self.cluster})` already exists in `{self.datasetName}`, cannot be uploaded again. | FileObject: {self.__dict__}')
                 raise ValueError(
-                    f'❌ Upload failed: [{self.filename} - {self.cluster}], already exists, cannot be uploaded again.')
+                    f'❌ Upload failed: `{self.filename}({self.cluster})` already exists in `{self.datasetName}`, cannot be uploaded again. ')
             else:
-                print(self.stdOut('continue upload...'))
-                uploaded_chunks = [int(i.split('-')[0]) for i in self.uploaded_chunks.split(',') if i != '']
-                continue_chunks = {i: self.chunks[i] for i in self.chunks if i not in uploaded_chunks}
-                # re-upload last chunk from checkpoint
-                if uploaded_chunks:
-                    last_chunk_index = max(uploaded_chunks)
-                    continue_chunks[last_chunk_index] = self.chunks[last_chunk_index]
-                continue_chunks = OrderedDict(sorted(continue_chunks.items()))
+                uploaded_chunks = sorted(uploaded_chunks)[:-1]
+                continue_chunks = [i for i in range(1, self.total_chunk_counts+1) if i not in uploaded_chunks]
+                continue_chunks = sorted(continue_chunks)
                 self.uploadProgressBar(continue_chunks)
 
         else:
-            print(self.stdOut('start new upload...'))
+        #if not self.uploaded:
             self.newMultipart()
-            self.uploadProgressBar(self.chunks)
+            chunks = [i for i in range(1, self.total_chunk_counts + 1)]
+            self.uploadProgressBar(chunks)
 
         self.completeMultipart()
         url = f"{self.app_url.split('api')[0]}{self.username}/{self.repo}/datasets"
-        print(self.stdOut(f'🎉 Successfully uploaded, view on link: {url}'))
-
+        print(f'{self.get_time()} - 🎉 Successfully uploaded, view on link: {url}')
+        logging.info(f'successfully uploaded. | FileObject: {self.__dict__}')
 
 def upload_file(file, username, repository, token, cluster="NPU", app_url=APP_URL):
     d = DatasetUploadFile(
         file=file,
         username=username,
         repository=repository,
         token=token,
```

### Comparing `openi-1.0.0/src/openi.egg-info/PKG-INFO` & `openi-1.0.1/src/openi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: openi
-Version: 1.0.0
-Summary: A package for openi pypi
+Version: 1.0.1
+Summary: A test package for openi pypi
 Home-page: https://openi.pcl.ac.cn/OpenIOSSG/openi-pypi
 Author: chenzh05
 Author-email: chenzh.ds@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

