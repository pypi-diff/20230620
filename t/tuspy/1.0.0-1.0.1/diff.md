# Comparing `tmp/tuspy-1.0.0.tar.gz` & `tmp/tuspy-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tuspy-1.0.0.tar", last modified: Thu Jul 21 01:31:54 2022, max compression
+gzip compressed data, was "tuspy-1.0.1.tar", last modified: Tue Jun 20 08:53:09 2023, max compression
```

## Comparing `tuspy-1.0.0.tar` & `tuspy-1.0.1.tar`

### file list

```diff
@@ -1,31 +1,38 @@
-drwxrwxr-x   0 kiloreux  (1000) kiloreux  (1000)        0 2022-07-21 01:31:54.096053 tuspy-1.0.0/
--rw-rw-r--   0 kiloreux  (1000) kiloreux  (1000)       56 2022-06-21 11:43:11.000000 tuspy-1.0.0/AUTHORS
--rw-rw-r--   0 kiloreux  (1000) kiloreux  (1000)     1078 2022-06-21 11:43:11.000000 tuspy-1.0.0/LICENSE
--rw-rw-r--   0 kiloreux  (1000) kiloreux  (1000)       18 2022-06-21 11:43:11.000000 tuspy-1.0.0/MANIFEST.in
--rw-rw-r--   0 kiloreux  (1000) kiloreux  (1000)     2949 2022-07-21 01:31:54.096053 tuspy-1.0.0/PKG-INFO
--rw-rw-r--   0 kiloreux  (1000) kiloreux  (1000)     2050 2022-06-21 11:43:11.000000 tuspy-1.0.0/README.md
--rw-rw-r--   0 kiloreux  (1000) kiloreux  (1000)       38 2022-07-21 01:31:54.096053 tuspy-1.0.0/setup.cfg
--rw-rw-r--   0 kiloreux  (1000) kiloreux  (1000)     1649 2022-06-21 11:43:11.000000 tuspy-1.0.0/setup.py
-drwxrwxr-x   0 kiloreux  (1000) kiloreux  (1000)        0 2022-07-21 01:31:54.096053 tuspy-1.0.0/tusclient/
--rw-rw-r--   0 kiloreux  (1000) kiloreux  (1000)       22 2022-06-21 11:43:11.000000 tuspy-1.0.0/tusclient/__init__.py
--rw-rw-r--   0 kiloreux  (1000) kiloreux  (1000)     1968 2022-06-21 11:43:11.000000 tuspy-1.0.0/tusclient/client.py
--rw-rw-r--   0 kiloreux  (1000) kiloreux  (1000)     1065 2022-06-21 11:43:11.000000 tuspy-1.0.0/tusclient/exceptions.py
-drwxrwxr-x   0 kiloreux  (1000) kiloreux  (1000)        0 2022-07-21 01:31:54.096053 tuspy-1.0.0/tusclient/fingerprint/
--rw-rw-r--   0 kiloreux  (1000) kiloreux  (1000)        0 2022-06-21 11:43:11.000000 tuspy-1.0.0/tusclient/fingerprint/__init__.py
--rw-rw-r--   0 kiloreux  (1000) kiloreux  (1000)     1187 2022-06-21 11:43:11.000000 tuspy-1.0.0/tusclient/fingerprint/fingerprint.py
--rw-rw-r--   0 kiloreux  (1000) kiloreux  (1000)      542 2022-06-21 11:43:11.000000 tuspy-1.0.0/tusclient/fingerprint/interface.py
--rw-rw-r--   0 kiloreux  (1000) kiloreux  (1000)     3911 2022-06-21 11:43:11.000000 tuspy-1.0.0/tusclient/request.py
-drwxrwxr-x   0 kiloreux  (1000) kiloreux  (1000)        0 2022-07-21 01:31:54.096053 tuspy-1.0.0/tusclient/storage/
--rw-rw-r--   0 kiloreux  (1000) kiloreux  (1000)        0 2022-06-21 11:43:11.000000 tuspy-1.0.0/tusclient/storage/__init__.py
--rw-rw-r--   0 kiloreux  (1000) kiloreux  (1000)     1424 2022-06-21 11:43:11.000000 tuspy-1.0.0/tusclient/storage/filestorage.py
--rw-rw-r--   0 kiloreux  (1000) kiloreux  (1000)      897 2022-06-21 11:43:11.000000 tuspy-1.0.0/tusclient/storage/interface.py
-drwxrwxr-x   0 kiloreux  (1000) kiloreux  (1000)        0 2022-07-21 01:31:54.096053 tuspy-1.0.0/tusclient/uploader/
--rw-rw-r--   0 kiloreux  (1000) kiloreux  (1000)       64 2022-06-21 11:43:11.000000 tuspy-1.0.0/tusclient/uploader/__init__.py
--rw-rw-r--   0 kiloreux  (1000) kiloreux  (1000)    10780 2022-06-21 11:43:11.000000 tuspy-1.0.0/tusclient/uploader/baseuploader.py
--rw-rw-r--   0 kiloreux  (1000) kiloreux  (1000)     5411 2022-06-21 11:43:11.000000 tuspy-1.0.0/tusclient/uploader/uploader.py
-drwxrwxr-x   0 kiloreux  (1000) kiloreux  (1000)        0 2022-07-21 01:31:54.096053 tuspy-1.0.0/tuspy.egg-info/
--rw-rw-r--   0 kiloreux  (1000) kiloreux  (1000)     2949 2022-07-21 01:31:54.000000 tuspy-1.0.0/tuspy.egg-info/PKG-INFO
--rw-rw-r--   0 kiloreux  (1000) kiloreux  (1000)      574 2022-07-21 01:31:54.000000 tuspy-1.0.0/tuspy.egg-info/SOURCES.txt
--rw-rw-r--   0 kiloreux  (1000) kiloreux  (1000)        1 2022-07-21 01:31:54.000000 tuspy-1.0.0/tuspy.egg-info/dependency_links.txt
--rw-rw-r--   0 kiloreux  (1000) kiloreux  (1000)      229 2022-07-21 01:31:54.000000 tuspy-1.0.0/tuspy.egg-info/requires.txt
--rw-rw-r--   0 kiloreux  (1000) kiloreux  (1000)       10 2022-07-21 01:31:54.000000 tuspy-1.0.0/tuspy.egg-info/top_level.txt
+drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-06-20 08:53:09.230502 tuspy-1.0.1/
+-rw-r--r--   0 marius     (501) staff       (20)       56 2023-06-20 08:44:44.000000 tuspy-1.0.1/AUTHORS
+-rw-r--r--   0 marius     (501) staff       (20)     1078 2023-06-20 08:44:44.000000 tuspy-1.0.1/LICENSE
+-rw-r--r--   0 marius     (501) staff       (20)       18 2023-06-20 08:44:44.000000 tuspy-1.0.1/MANIFEST.in
+-rw-r--r--   0 marius     (501) staff       (20)     2954 2023-06-20 08:53:09.230410 tuspy-1.0.1/PKG-INFO
+-rw-r--r--   0 marius     (501) staff       (20)     2057 2023-06-20 08:44:44.000000 tuspy-1.0.1/README.md
+-rw-r--r--   0 marius     (501) staff       (20)       38 2023-06-20 08:53:09.230538 tuspy-1.0.1/setup.cfg
+-rw-r--r--   0 marius     (501) staff       (20)     1649 2023-06-20 08:44:44.000000 tuspy-1.0.1/setup.py
+drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-06-20 08:53:09.228479 tuspy-1.0.1/tests/
+-rw-r--r--   0 marius     (501) staff       (20)     4233 2023-06-20 08:44:44.000000 tuspy-1.0.1/tests/test_async_uploader.py
+-rw-r--r--   0 marius     (501) staff       (20)     1689 2023-06-20 08:44:44.000000 tuspy-1.0.1/tests/test_client.py
+-rw-r--r--   0 marius     (501) staff       (20)      858 2023-06-20 08:44:44.000000 tuspy-1.0.1/tests/test_filestorage.py
+-rw-r--r--   0 marius     (501) staff       (20)     1111 2023-06-20 08:44:44.000000 tuspy-1.0.1/tests/test_fingerprint.py
+-rw-r--r--   0 marius     (501) staff       (20)     2080 2023-06-20 08:44:44.000000 tuspy-1.0.1/tests/test_request.py
+-rw-r--r--   0 marius     (501) staff       (20)     6787 2023-06-20 08:44:44.000000 tuspy-1.0.1/tests/test_uploader.py
+drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-06-20 08:53:09.228880 tuspy-1.0.1/tusclient/
+-rw-r--r--   0 marius     (501) staff       (20)       22 2023-06-20 08:52:26.000000 tuspy-1.0.1/tusclient/__init__.py
+-rw-r--r--   0 marius     (501) staff       (20)     1968 2023-06-20 08:44:44.000000 tuspy-1.0.1/tusclient/client.py
+-rw-r--r--   0 marius     (501) staff       (20)     1065 2023-06-20 08:44:44.000000 tuspy-1.0.1/tusclient/exceptions.py
+drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-06-20 08:53:09.229169 tuspy-1.0.1/tusclient/fingerprint/
+-rw-r--r--   0 marius     (501) staff       (20)        0 2023-06-20 08:44:44.000000 tuspy-1.0.1/tusclient/fingerprint/__init__.py
+-rw-r--r--   0 marius     (501) staff       (20)     1187 2023-06-20 08:44:44.000000 tuspy-1.0.1/tusclient/fingerprint/fingerprint.py
+-rw-r--r--   0 marius     (501) staff       (20)      542 2023-06-20 08:44:44.000000 tuspy-1.0.1/tusclient/fingerprint/interface.py
+-rw-r--r--   0 marius     (501) staff       (20)     3911 2023-06-20 08:44:44.000000 tuspy-1.0.1/tusclient/request.py
+drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-06-20 08:53:09.229464 tuspy-1.0.1/tusclient/storage/
+-rw-r--r--   0 marius     (501) staff       (20)        0 2023-06-20 08:44:44.000000 tuspy-1.0.1/tusclient/storage/__init__.py
+-rw-r--r--   0 marius     (501) staff       (20)     1424 2023-06-20 08:44:44.000000 tuspy-1.0.1/tusclient/storage/filestorage.py
+-rw-r--r--   0 marius     (501) staff       (20)      897 2023-06-20 08:44:44.000000 tuspy-1.0.1/tusclient/storage/interface.py
+drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-06-20 08:53:09.229764 tuspy-1.0.1/tusclient/uploader/
+-rw-r--r--   0 marius     (501) staff       (20)       64 2023-06-20 08:44:44.000000 tuspy-1.0.1/tusclient/uploader/__init__.py
+-rw-r--r--   0 marius     (501) staff       (20)    10809 2023-06-20 08:44:44.000000 tuspy-1.0.1/tusclient/uploader/baseuploader.py
+-rw-r--r--   0 marius     (501) staff       (20)     5622 2023-06-20 08:44:44.000000 tuspy-1.0.1/tusclient/uploader/uploader.py
+drwxr-xr-x   0 marius     (501) staff       (20)        0 2023-06-20 08:53:09.230263 tuspy-1.0.1/tuspy.egg-info/
+-rw-r--r--   0 marius     (501) staff       (20)     2954 2023-06-20 08:53:09.000000 tuspy-1.0.1/tuspy.egg-info/PKG-INFO
+-rw-r--r--   0 marius     (501) staff       (20)      721 2023-06-20 08:53:09.000000 tuspy-1.0.1/tuspy.egg-info/SOURCES.txt
+-rw-r--r--   0 marius     (501) staff       (20)        1 2023-06-20 08:53:09.000000 tuspy-1.0.1/tuspy.egg-info/dependency_links.txt
+-rw-r--r--   0 marius     (501) staff       (20)      229 2023-06-20 08:53:09.000000 tuspy-1.0.1/tuspy.egg-info/requires.txt
+-rw-r--r--   0 marius     (501) staff       (20)       10 2023-06-20 08:53:09.000000 tuspy-1.0.1/tuspy.egg-info/top_level.txt
```

### Comparing `tuspy-1.0.0/LICENSE` & `tuspy-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tuspy-1.0.0/PKG-INFO` & `tuspy-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tuspy
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python client for the tus resumable upload protocol ->  http://tus.io
 Home-page: http://github.com/tus/tus-py-client/
 Author: Ifedapo Olarewaju
 Author-email: ifedapoolarewaju@gmail.com
 License: MIT
 Platform: any
 Classifier: Programming Language :: Python
@@ -14,16 +14,16 @@
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Internet :: File Transfer Protocol (FTP)
 Classifier: Topic :: Communications :: File Sharing
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 Provides-Extra: test
+Provides-Extra: dev
 License-File: LICENSE
 License-File: AUTHORS
 
 # tus-py-client [![Build Status](https://github.com/tus/tus-py-client/actions/workflows/CI.yml/badge.svg)](https://github.com/tus/tus-py-client/actions/workflows/CI.yml)
 
 > **tus** is a protocol based on HTTP for *resumable file uploads*. Resumable
 > means that an upload can be interrupted at any moment and can be resumed without
@@ -55,15 +55,15 @@
 
 # Set more headers.
 my_client.set_headers({'HEADER_NAME': 'HEADER_VALUE'})
 
 uploader = my_client.uploader('path/to/file.ext', chunk_size=200)
 
 # A file stream may also be passed in place of a file path.
-fs = open('path/to/file.ext')
+fs = open('path/to/file.ext', mode=)
 uploader = my_client.uploader(file_stream=fs, chunk_size=200)
 
 # Upload a chunk i.e 200 bytes.
 uploader.upload_chunk()
 
 # Uploads the entire file.
 # This uploads chunk by chunk.
@@ -87,9 +87,7 @@
                        url='http://tusd.tusdemo.net/files/abcdef123456',
                        chunk_size=200)
 ```
 
 ## License
 
 MIT
-
-
```

### Comparing `tuspy-1.0.0/README.md` & `tuspy-1.0.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 # Set more headers.
 my_client.set_headers({'HEADER_NAME': 'HEADER_VALUE'})
 
 uploader = my_client.uploader('path/to/file.ext', chunk_size=200)
 
 # A file stream may also be passed in place of a file path.
-fs = open('path/to/file.ext')
+fs = open('path/to/file.ext', mode=)
 uploader = my_client.uploader(file_stream=fs, chunk_size=200)
 
 # Upload a chunk i.e 200 bytes.
 uploader.upload_chunk()
 
 # Uploads the entire file.
 # This uploads chunk by chunk.
```

### Comparing `tuspy-1.0.0/setup.py` & `tuspy-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `tuspy-1.0.0/tusclient/client.py` & `tuspy-1.0.1/tusclient/client.py`

 * *Files identical despite different names*

### Comparing `tuspy-1.0.0/tusclient/exceptions.py` & `tuspy-1.0.1/tusclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `tuspy-1.0.0/tusclient/fingerprint/fingerprint.py` & `tuspy-1.0.1/tusclient/fingerprint/fingerprint.py`

 * *Files identical despite different names*

### Comparing `tuspy-1.0.0/tusclient/fingerprint/interface.py` & `tuspy-1.0.1/tusclient/fingerprint/interface.py`

 * *Files identical despite different names*

### Comparing `tuspy-1.0.0/tusclient/request.py` & `tuspy-1.0.1/tusclient/request.py`

 * *Files identical despite different names*

### Comparing `tuspy-1.0.0/tusclient/storage/filestorage.py` & `tuspy-1.0.1/tusclient/storage/filestorage.py`

 * *Files identical despite different names*

### Comparing `tuspy-1.0.0/tusclient/storage/interface.py` & `tuspy-1.0.1/tusclient/storage/interface.py`

 * *Files identical despite different names*

### Comparing `tuspy-1.0.0/tusclient/uploader/baseuploader.py` & `tuspy-1.0.1/tusclient/uploader/baseuploader.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,28 +110,28 @@
         if url is None and client is None:
             raise ValueError("Either 'url' or 'client' cannot be None.")
 
         if store_url and url_storage is None:
             raise ValueError(
                 "Please specify a storage instance to enable resumablility.")
 
+        self.verify_tls_cert = verify_tls_cert
         self.file_path = file_path
         self.file_stream = file_stream
         self.stop_at = self.get_file_size()
         self.client = client
         self.metadata = metadata or {}
         self.metadata_encoding = metadata_encoding
         self.store_url = store_url
         self.url_storage = url_storage
         self.fingerprinter = fingerprinter or fingerprint.Fingerprint()
         self.offset = 0
         self.url = None
         self.__init_url_and_offset(url)
         self.chunk_size = chunk_size
-        self.verify_tls_cert = verify_tls_cert
         self.retries = retries
         self.request = None
         self._retried = 0
         self.retry_delay = retry_delay
         self.upload_checksum = upload_checksum
         self.__checksum_algorithm_name, self.__checksum_algorithm = \
             self.CHECKSUM_ALGORITHM_PAIR
@@ -168,15 +168,15 @@
     def get_offset(self):
         """
         Return offset from tus server.
 
         This is different from the instance attribute 'offset' because this makes an
         http request to the tus server to retrieve the offset.
         """
-        resp = requests.head(self.url, headers=self.get_headers())
+        resp = requests.head(self.url, headers=self.get_headers(), verify=self.verify_tls_cert)
         offset = resp.headers.get('upload-offset')
         if offset is None:
             msg = 'Attempt to retrieve offset fails with status {}'.format(
                 resp.status_code)
             raise TusCommunicationError(msg, resp.status_code, resp.content)
         return int(offset)
```

### Comparing `tuspy-1.0.0/tusclient/uploader/uploader.py` & `tuspy-1.0.1/tusclient/uploader/uploader.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,25 +31,30 @@
         :Args:
             - stop_at (Optional[int]):
                 Determines at what offset value the upload should stop. If not specified this
                 defaults to the file size.
         """
         self.stop_at = stop_at or self.get_file_size()
 
+        if not self.url:
+            # Ensure the POST request is performed even for empty files.
+            # This ensures even empty files can be uploaded; in this case
+            # only the POST request needs to be performed.
+            self.set_url(self.create_url())
+            self.offset = 0
+
         while self.offset < self.stop_at:
             self.upload_chunk()
 
     def upload_chunk(self):
         """
         Upload chunk of file.
         """
         self._retried = 0
-        if not self.url:
-            self.set_url(self.create_url())
-            self.offset = 0
+
         self._do_request()
         self.offset = int(self.request.response_headers.get('upload-offset'))
 
     @catch_requests_error
     def create_url(self):
         """
         Return upload url.
@@ -102,25 +107,28 @@
 
         :Args:
             - stop_at (Optional[int]):
                 Determines at what offset value the upload should stop. If not specified this
                 defaults to the file size.
         """
         self.stop_at = stop_at or self.get_file_size()
+
+        if not self.url:
+            self.set_url(await self.create_url())
+            self.offset = 0
+
         while self.offset < self.stop_at:
             await self.upload_chunk()
 
     async def upload_chunk(self):
         """
         Upload chunk of file.
         """
         self._retried = 0
-        if not self.url:
-            self.set_url(await self.create_url())
-            self.offset = 0
+
         await self._do_request()
         self.offset = int(self.request.response_headers.get('upload-offset'))
 
     async def create_url(self):
         """
         Return upload url.
```

### Comparing `tuspy-1.0.0/tuspy.egg-info/PKG-INFO` & `tuspy-1.0.1/tuspy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tuspy
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python client for the tus resumable upload protocol ->  http://tus.io
 Home-page: http://github.com/tus/tus-py-client/
 Author: Ifedapo Olarewaju
 Author-email: ifedapoolarewaju@gmail.com
 License: MIT
 Platform: any
 Classifier: Programming Language :: Python
@@ -14,16 +14,16 @@
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Internet :: File Transfer Protocol (FTP)
 Classifier: Topic :: Communications :: File Sharing
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 Provides-Extra: test
+Provides-Extra: dev
 License-File: LICENSE
 License-File: AUTHORS
 
 # tus-py-client [![Build Status](https://github.com/tus/tus-py-client/actions/workflows/CI.yml/badge.svg)](https://github.com/tus/tus-py-client/actions/workflows/CI.yml)
 
 > **tus** is a protocol based on HTTP for *resumable file uploads*. Resumable
 > means that an upload can be interrupted at any moment and can be resumed without
@@ -55,15 +55,15 @@
 
 # Set more headers.
 my_client.set_headers({'HEADER_NAME': 'HEADER_VALUE'})
 
 uploader = my_client.uploader('path/to/file.ext', chunk_size=200)
 
 # A file stream may also be passed in place of a file path.
-fs = open('path/to/file.ext')
+fs = open('path/to/file.ext', mode=)
 uploader = my_client.uploader(file_stream=fs, chunk_size=200)
 
 # Upload a chunk i.e 200 bytes.
 uploader.upload_chunk()
 
 # Uploads the entire file.
 # This uploads chunk by chunk.
@@ -87,9 +87,7 @@
                        url='http://tusd.tusdemo.net/files/abcdef123456',
                        chunk_size=200)
 ```
 
 ## License
 
 MIT
-
-
```

### Comparing `tuspy-1.0.0/tuspy.egg-info/SOURCES.txt` & `tuspy-1.0.1/tuspy.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 AUTHORS
 LICENSE
 MANIFEST.in
 README.md
 setup.py
+tests/test_async_uploader.py
+tests/test_client.py
+tests/test_filestorage.py
+tests/test_fingerprint.py
+tests/test_request.py
+tests/test_uploader.py
 tusclient/__init__.py
 tusclient/client.py
 tusclient/exceptions.py
 tusclient/request.py
 tusclient/fingerprint/__init__.py
 tusclient/fingerprint/fingerprint.py
 tusclient/fingerprint/interface.py
```

