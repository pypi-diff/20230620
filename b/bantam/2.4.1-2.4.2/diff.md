# Comparing `tmp/bantam-2.4.1.tar.gz` & `tmp/bantam-2.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bantam-2.4.1.tar", last modified: Sun Jun 18 01:09:01 2023, max compression
+gzip compressed data, was "bantam-2.4.2.tar", last modified: Tue Jun 20 02:14:40 2023, max compression
```

## Comparing `bantam-2.4.1.tar` & `bantam-2.4.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-18 01:09:01.884757 bantam-2.4.1/
--rw-rw-r--   0 pi        (1000) pi        (1000)      780 2023-06-18 01:09:01.884757 bantam-2.4.1/PKG-INFO
--rw-rw-r--   0 pi        (1000) pi        (1000)      370 2023-06-03 15:15:17.000000 bantam-2.4.1/README
--rw-rw-r--   0 pi        (1000) pi        (1000)       54 2023-06-11 03:58:58.000000 bantam-2.4.1/requirements.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)       70 2023-06-18 01:09:01.884757 bantam-2.4.1/setup.cfg
--rwxrwxr-x   0 pi        (1000) pi        (1000)     1425 2023-06-18 01:06:44.000000 bantam-2.4.1/setup.py
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-18 01:09:01.880757 bantam-2.4.1/src/
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-18 01:09:01.884757 bantam-2.4.1/src/bantam/
--rw-rw-r--   0 pi        (1000) pi        (1000)     4616 2023-06-11 16:48:25.000000 bantam-2.4.1/src/bantam/__init__.py
--rw-rw-r--   0 pi        (1000) pi        (1000)    11963 2023-06-17 16:30:44.000000 bantam-2.4.1/src/bantam/api.py
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-18 01:09:01.884757 bantam-2.4.1/src/bantam/autogen/
--rw-rw-r--   0 pi        (1000) pi        (1000)        0 2023-06-03 15:15:17.000000 bantam-2.4.1/src/bantam/autogen/__init__.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     3399 2023-06-03 15:15:17.000000 bantam-2.4.1/src/bantam/autogen/main.py
--rw-rw-r--   0 pi        (1000) pi        (1000)    21101 2023-06-17 16:17:43.000000 bantam-2.4.1/src/bantam/client.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     5705 2023-06-17 16:33:30.000000 bantam-2.4.1/src/bantam/conversions.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     4684 2023-06-04 23:41:07.000000 bantam-2.4.1/src/bantam/decorators.py
--rw-rw-r--   0 pi        (1000) pi        (1000)    50491 2023-06-18 01:07:41.000000 bantam-2.4.1/src/bantam/http.py
--rw-rw-r--   0 pi        (1000) pi        (1000)    22114 2023-06-17 16:10:55.000000 bantam-2.4.1/src/bantam/js.py
--rw-rw-r--   0 pi        (1000) pi        (1000)    20369 2023-06-04 03:38:29.000000 bantam-2.4.1/src/bantam/js_async.py
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-18 01:09:01.884757 bantam-2.4.1/src/bantam.egg-info/
--rw-rw-r--   0 pi        (1000) pi        (1000)      780 2023-06-18 01:09:01.000000 bantam-2.4.1/src/bantam.egg-info/PKG-INFO
--rw-rw-r--   0 pi        (1000) pi        (1000)      672 2023-06-18 01:09:01.000000 bantam-2.4.1/src/bantam.egg-info/SOURCES.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)        1 2023-06-18 01:09:01.000000 bantam-2.4.1/src/bantam.egg-info/dependency_links.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)       61 2023-06-18 01:09:01.000000 bantam-2.4.1/src/bantam.egg-info/entry_points.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)       54 2023-06-18 01:09:01.000000 bantam-2.4.1/src/bantam.egg-info/requires.txt
--rw-rw-r--   0 pi        (1000) pi        (1000)        7 2023-06-18 01:09:01.000000 bantam-2.4.1/src/bantam.egg-info/top_level.txt
-drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-18 01:09:01.884757 bantam-2.4.1/test/
--rw-rw-r--   0 pi        (1000) pi        (1000)     4821 2023-06-17 16:39:40.000000 bantam-2.4.1/test/test_client_get.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     4670 2023-06-17 15:47:27.000000 bantam-2.4.1/test/test_client_post.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     6038 2023-06-11 01:57:09.000000 bantam-2.4.1/test/test_client_post_inherited_apis.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     3469 2023-06-04 03:12:58.000000 bantam-2.4.1/test/test_conversions.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     3217 2023-06-04 03:13:40.000000 bantam-2.4.1/test/test_decorators.py
--rw-rw-r--   0 pi        (1000) pi        (1000)      191 2023-06-04 14:25:43.000000 bantam-2.4.1/test/test_http.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     3001 2023-06-11 03:15:10.000000 bantam-2.4.1/test/test_js.py
--rw-rw-r--   0 pi        (1000) pi        (1000)     2856 2023-06-10 16:58:56.000000 bantam-2.4.1/test/test_js_async.py
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-20 02:14:40.132470 bantam-2.4.2/
+-rw-rw-r--   0 pi        (1000) pi        (1000)      780 2023-06-20 02:14:40.132470 bantam-2.4.2/PKG-INFO
+-rw-rw-r--   0 pi        (1000) pi        (1000)      370 2023-06-03 15:15:17.000000 bantam-2.4.2/README
+-rw-rw-r--   0 pi        (1000) pi        (1000)       54 2023-06-11 03:58:58.000000 bantam-2.4.2/requirements.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)       70 2023-06-20 02:14:40.132470 bantam-2.4.2/setup.cfg
+-rwxrwxr-x   0 pi        (1000) pi        (1000)     1425 2023-06-20 02:13:31.000000 bantam-2.4.2/setup.py
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-20 02:14:40.132470 bantam-2.4.2/src/
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-20 02:14:40.132470 bantam-2.4.2/src/bantam/
+-rw-rw-r--   0 pi        (1000) pi        (1000)     4616 2023-06-11 16:48:25.000000 bantam-2.4.2/src/bantam/__init__.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    11963 2023-06-17 16:30:44.000000 bantam-2.4.2/src/bantam/api.py
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-20 02:14:40.132470 bantam-2.4.2/src/bantam/autogen/
+-rw-rw-r--   0 pi        (1000) pi        (1000)        0 2023-06-03 15:15:17.000000 bantam-2.4.2/src/bantam/autogen/__init__.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     3399 2023-06-03 15:15:17.000000 bantam-2.4.2/src/bantam/autogen/main.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    21101 2023-06-17 16:17:43.000000 bantam-2.4.2/src/bantam/client.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     5705 2023-06-17 16:33:30.000000 bantam-2.4.2/src/bantam/conversions.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     4684 2023-06-04 23:41:07.000000 bantam-2.4.2/src/bantam/decorators.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    50846 2023-06-20 02:13:08.000000 bantam-2.4.2/src/bantam/http.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    22114 2023-06-17 16:10:55.000000 bantam-2.4.2/src/bantam/js.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    20369 2023-06-04 03:38:29.000000 bantam-2.4.2/src/bantam/js_async.py
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-20 02:14:40.132470 bantam-2.4.2/src/bantam.egg-info/
+-rw-rw-r--   0 pi        (1000) pi        (1000)      780 2023-06-20 02:14:40.000000 bantam-2.4.2/src/bantam.egg-info/PKG-INFO
+-rw-rw-r--   0 pi        (1000) pi        (1000)      672 2023-06-20 02:14:40.000000 bantam-2.4.2/src/bantam.egg-info/SOURCES.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)        1 2023-06-20 02:14:40.000000 bantam-2.4.2/src/bantam.egg-info/dependency_links.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)       61 2023-06-20 02:14:40.000000 bantam-2.4.2/src/bantam.egg-info/entry_points.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)       54 2023-06-20 02:14:40.000000 bantam-2.4.2/src/bantam.egg-info/requires.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)        7 2023-06-20 02:14:40.000000 bantam-2.4.2/src/bantam.egg-info/top_level.txt
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2023-06-20 02:14:40.132470 bantam-2.4.2/test/
+-rw-rw-r--   0 pi        (1000) pi        (1000)     4821 2023-06-17 16:39:40.000000 bantam-2.4.2/test/test_client_get.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     4670 2023-06-17 15:47:27.000000 bantam-2.4.2/test/test_client_post.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     6038 2023-06-11 01:57:09.000000 bantam-2.4.2/test/test_client_post_inherited_apis.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     3469 2023-06-04 03:12:58.000000 bantam-2.4.2/test/test_conversions.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     3217 2023-06-04 03:13:40.000000 bantam-2.4.2/test/test_decorators.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)      191 2023-06-04 14:25:43.000000 bantam-2.4.2/test/test_http.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     3001 2023-06-11 03:15:10.000000 bantam-2.4.2/test/test_js.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     2856 2023-06-10 16:58:56.000000 bantam-2.4.2/test/test_js_async.py
```

### Comparing `bantam-2.4.1/PKG-INFO` & `bantam-2.4.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: bantam
-Version: 2.4.1
+Version: 2.4.2
 Summary: small utils to automate web interface in Python
 Home-page: https://github.com/nak/bantam
-Download-URL: https://github.com/bantam/dist/2.4.1
+Download-URL: https://github.com/bantam/dist/2.4.2
 Author: John Rusnak
 Author-email: john.j.rusnak@att.net
 License: BSD 2-CLAUSE
 Keywords: auto web api python
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `bantam-2.4.1/setup.py` & `bantam-2.4.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 
 import setuptools
 
-VERSION = "2.4.1"
+VERSION = "2.4.2"
 
 setuptools.setup(
     name='bantam',
     author='John Rusnak',
     author_email='john.j.rusnak@att.net',
     version=VERSION,
     data_files=[('.', ['requirements.txt'])],
```

### Comparing `bantam-2.4.1/src/bantam/__init__.py` & `bantam-2.4.2/src/bantam/__init__.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.1/src/bantam/api.py` & `bantam-2.4.2/src/bantam/api.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.1/src/bantam/autogen/main.py` & `bantam-2.4.2/src/bantam/autogen/main.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.1/src/bantam/client.py` & `bantam-2.4.2/src/bantam/client.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.1/src/bantam/conversions.py` & `bantam-2.4.2/src/bantam/conversions.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.1/src/bantam/decorators.py` & `bantam-2.4.2/src/bantam/decorators.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.1/src/bantam/http.py` & `bantam-2.4.2/src/bantam/http.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,15 +99,18 @@
         request_q = asynciomultiplexer.AsyncAdaptorQueue(MAX_SIMULTANEOUS_REQUESTS)
 
         @classmethod
         async def start(cls, coro: Awaitable, resp_q: asynciomultiplexer.AsyncAdaptorQueue):
             await cls.request_q.put((coro, resp_q))
 
         @classmethod
-        async def main(cls):
+        async def main(cls, initializer: Optional[Callable[[], None]] = None):
+            if initializer:
+                initializer()
+
             async def task(coro: Awaitable, resp_q: asynciomultiplexer.AsyncAdaptorQueue):
                 try:
                     resp = await coro
                 except Exception as e:
                     resp = e
                 await resp_q.put(resp)
 
@@ -347,40 +350,43 @@
 
     # noinspection PyProtectedMember
     async def start(self,
                     modules: List[str],
                     host: Optional[str] = None,
                     port: Optional[int] = None,
                     path: Optional[str] = None,
+                    initializer: Optional[Callable[[], None]] = None,
                     shutdown_timeout: float = 60.0,
                     ssl_context: Optional[SSLContext] = None,
                     backlog: int = 128,
                     handle_signals: bool = True,
                     reuse_address: Optional[bool] = None,
                     reuse_port: Optional[bool] = None,) -> None:
         """
         start the app
 
         :param modules: list of name of modules to import that contain the @web_api definitions to use, must not be
            empty and will be imported to load the @web_api definitions
         :param host: optional host of app, defaults to '127.0.0.1'
         :param port: optional port to listen on (TCP)
         :param path: path, if using UNIX domain sockets to listen on (cannot specify both TCP and domain parameters)
+        :param initializer: optional function (no params, no return) to call on first bring-up, inside the
+            thread associated with the app's asyncio loop
         :param shutdown_timeout: force shutdown if a shutdown call fails to take hold after this many seconds
         :param ssl_context: for HTTPS server; if not provided, will default to HTTP connection
         :param backlog: number of unaccepted connections before system will refuse new connections
         :param handle_signals: gracefully handle TERM signal or not
         :param reuse_address: tells the kernel to reuse a local socket in TIME_WAIT state, without waiting for its
            natural timeout to expire. If not specified will automatically be set to True on UNIX.
         :param reuse_port: tells the kernel to allow this endpoint to be bound to the same port as other existing
             endpoints are bound to, so long as they all set this flag when being created. This option is not supported
             on Windows.
         """
         # noinspection PyProtectedMember
-        self._main_task = asyncio.create_task(self.MainThread.main())
+        self._main_task = asyncio.create_task(self.MainThread.main(initializer))
         from aiohttp.web import _run_app as web_run_app
         for module in modules:
             self.preprocess_module(module)
             if module not in sys.modules:
                 mod = importlib.import_module(module)
             else:
                 mod = sys.modules.get(module)
```

### Comparing `bantam-2.4.1/src/bantam/js.py` & `bantam-2.4.2/src/bantam/js.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.1/src/bantam/js_async.py` & `bantam-2.4.2/src/bantam/js_async.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.1/src/bantam.egg-info/PKG-INFO` & `bantam-2.4.2/src/bantam.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: bantam
-Version: 2.4.1
+Version: 2.4.2
 Summary: small utils to automate web interface in Python
 Home-page: https://github.com/nak/bantam
-Download-URL: https://github.com/bantam/dist/2.4.1
+Download-URL: https://github.com/bantam/dist/2.4.2
 Author: John Rusnak
 Author-email: john.j.rusnak@att.net
 License: BSD 2-CLAUSE
 Keywords: auto web api python
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `bantam-2.4.1/src/bantam.egg-info/SOURCES.txt` & `bantam-2.4.2/src/bantam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bantam-2.4.1/test/test_client_get.py` & `bantam-2.4.2/test/test_client_get.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.1/test/test_client_post.py` & `bantam-2.4.2/test/test_client_post.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.1/test/test_client_post_inherited_apis.py` & `bantam-2.4.2/test/test_client_post_inherited_apis.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.1/test/test_conversions.py` & `bantam-2.4.2/test/test_conversions.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.1/test/test_decorators.py` & `bantam-2.4.2/test/test_decorators.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.1/test/test_js.py` & `bantam-2.4.2/test/test_js.py`

 * *Files identical despite different names*

### Comparing `bantam-2.4.1/test/test_js_async.py` & `bantam-2.4.2/test/test_js_async.py`

 * *Files identical despite different names*

