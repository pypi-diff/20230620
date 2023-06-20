# Comparing `tmp/coinpaprika_async-3.0.0.tar.gz` & `tmp/coinpaprika_async-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coinpaprika_async-3.0.0.tar", last modified: Tue Jun 20 21:14:57 2023, max compression
+gzip compressed data, was "coinpaprika_async-3.0.1.tar", last modified: Tue Jun 20 21:40:33 2023, max compression
```

## Comparing `coinpaprika_async-3.0.0.tar` & `coinpaprika_async-3.0.1.tar`

### file list

```diff
@@ -1,19 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 21:14:57.926778 coinpaprika_async-3.0.0/
--rw-rw-rw-   0        0        0     1084 2023-05-21 17:45:15.000000 coinpaprika_async-3.0.0/LICENSE
--rw-rw-rw-   0        0        0     2169 2023-06-20 21:14:57.927779 coinpaprika_async-3.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1400 2023-06-20 20:27:13.000000 coinpaprika_async-3.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-20 21:14:57.907777 coinpaprika_async-3.0.0/coinpaprika_async/
--rw-rw-rw-   0        0        0      147 2023-06-17 19:38:46.000000 coinpaprika_async-3.0.0/coinpaprika_async/__init__.py
--rw-rw-rw-   0        0        0      125 2023-06-20 20:16:17.000000 coinpaprika_async-3.0.0/coinpaprika_async/_version__.py
--rw-rw-rw-   0        0        0     1315 2023-06-20 18:32:49.000000 coinpaprika_async-3.0.0/coinpaprika_async/coinpaprika_async_client.py
-drwxrwxrwx   0        0        0        0 2023-06-20 21:14:57.920778 coinpaprika_async-3.0.0/coinpaprika_async.egg-info/
--rw-rw-rw-   0        0        0     2169 2023-06-20 21:14:57.000000 coinpaprika_async-3.0.0/coinpaprika_async.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      384 2023-06-20 21:14:57.000000 coinpaprika_async-3.0.0/coinpaprika_async.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 21:14:57.000000 coinpaprika_async-3.0.0/coinpaprika_async.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-20 21:14:57.000000 coinpaprika_async-3.0.0/coinpaprika_async.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-06-20 21:14:57.000000 coinpaprika_async-3.0.0/coinpaprika_async.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      209 2023-05-21 17:49:30.000000 coinpaprika_async-3.0.0/pyproject.toml
--rw-rw-rw-   0        0        0      139 2023-06-20 21:14:57.934795 coinpaprika_async-3.0.0/setup.cfg
--rw-rw-rw-   0        0        0      859 2023-06-20 20:16:11.000000 coinpaprika_async-3.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-20 21:14:57.924779 coinpaprika_async-3.0.0/tests/
--rw-rw-rw-   0        0        0     1893 2023-06-20 18:16:17.000000 coinpaprika_async-3.0.0/tests/test_client.py
+drwxrwxrwx   0        0        0        0 2023-06-20 21:40:33.905603 coinpaprika_async-3.0.1/
+-rw-rw-rw-   0        0        0     1084 2023-05-21 17:45:15.000000 coinpaprika_async-3.0.1/LICENSE
+-rw-rw-rw-   0        0        0     2169 2023-06-20 21:40:33.905603 coinpaprika_async-3.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1400 2023-06-20 20:27:13.000000 coinpaprika_async-3.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-20 21:40:33.861601 coinpaprika_async-3.0.1/coinpaprika_async/
+-rw-rw-rw-   0        0        0      449 2023-06-20 21:32:25.000000 coinpaprika_async-3.0.1/coinpaprika_async/__init__.py
+-rw-rw-rw-   0        0        0      125 2023-06-20 21:38:00.000000 coinpaprika_async-3.0.1/coinpaprika_async/_version__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 21:40:33.893603 coinpaprika_async-3.0.1/coinpaprika_async/api/
+-rw-rw-rw-   0        0        0      245 2023-06-20 18:10:10.000000 coinpaprika_async-3.0.1/coinpaprika_async/api/__init__.py
+-rw-rw-rw-   0        0        0      235 2023-06-18 16:35:59.000000 coinpaprika_async-3.0.1/coinpaprika_async/api/coinpaprika_api.py
+-rw-rw-rw-   0        0        0     1314 2023-06-20 21:30:06.000000 coinpaprika_async-3.0.1/coinpaprika_async/coinpaprika_async_client.py
+drwxrwxrwx   0        0        0        0 2023-06-20 21:40:33.888602 coinpaprika_async-3.0.1/coinpaprika_async.egg-info/
+-rw-rw-rw-   0        0        0     2169 2023-06-20 21:40:33.000000 coinpaprika_async-3.0.1/coinpaprika_async.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      459 2023-06-20 21:40:33.000000 coinpaprika_async-3.0.1/coinpaprika_async.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 21:40:33.000000 coinpaprika_async-3.0.1/coinpaprika_async.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-20 21:40:33.000000 coinpaprika_async-3.0.1/coinpaprika_async.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-06-20 21:40:33.000000 coinpaprika_async-3.0.1/coinpaprika_async.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      209 2023-05-21 17:49:30.000000 coinpaprika_async-3.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0      139 2023-06-20 21:40:33.907609 coinpaprika_async-3.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      899 2023-06-20 21:37:54.000000 coinpaprika_async-3.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 21:40:33.902600 coinpaprika_async-3.0.1/tests/
+-rw-rw-rw-   0        0        0     1893 2023-06-20 18:16:17.000000 coinpaprika_async-3.0.1/tests/test_client.py
```

### Comparing `coinpaprika_async-3.0.0/LICENSE` & `coinpaprika_async-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `coinpaprika_async-3.0.0/PKG-INFO` & `coinpaprika_async-3.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coinpaprika_async
-Version: 3.0.0
+Version: 3.0.1
 Summary: An asynchronous client for the coinpaprika API.
 Home-page: https://github.com/DroidZed/coinpaprika-async-client.git
 Author: DroidZed
 Author-email: droid.zed77@outlook.com
 License: MIT
 Keywords: coinpaprika_async api cryptocurrency async httpx client
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `coinpaprika_async-3.0.0/README.md` & `coinpaprika_async-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `coinpaprika_async-3.0.0/coinpaprika_async/coinpaprika_async_client.py` & `coinpaprika_async-3.0.1/coinpaprika_async/coinpaprika_async_client.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional, Dict, Any
+from typing import Optional
 
 from .api.networking_layer import HttpAsyncClient
 
 
 class CoinPaprikaAsyncClient:
 
     """
@@ -10,15 +10,15 @@
 
     """
 
     __FREE_API_URL = "https://api.coinpaprika.com/v1"
 
     __PRO_API_URL = "https://api-pro.coinpaprika.com/v1"
 
-    def __init__(self, http: HttpAsyncClient = HttpAsyncClient(), api_key: str = None):
+    def __init__(self, http: HttpAsyncClient = HttpAsyncClient(), api_key: Optional[str] = None):
         self._http_client = http
         self._is_paid = api_key != None
         self._api_key = api_key
 
     async def call_api(self, path: str, **query_params):
         uri = self.__create_api_uri(path)
         headers = self.__create_headers()
```

### Comparing `coinpaprika_async-3.0.0/coinpaprika_async.egg-info/PKG-INFO` & `coinpaprika_async-3.0.1/coinpaprika_async.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coinpaprika-async
-Version: 3.0.0
+Version: 3.0.1
 Summary: An asynchronous client for the coinpaprika API.
 Home-page: https://github.com/DroidZed/coinpaprika-async-client.git
 Author: DroidZed
 Author-email: droid.zed77@outlook.com
 License: MIT
 Keywords: coinpaprika_async api cryptocurrency async httpx client
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `coinpaprika_async-3.0.0/setup.py` & `coinpaprika_async-3.0.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from setuptools import setup
+from setuptools import setup, find_packages
 
 setup(
     name="coinpaprika_async",
-    version="3.0.0",
+    version="3.0.1",
     author="DroidZed",
     author_email="droid.zed77@outlook.com",
     description="An asynchronous client for the coinpaprika API.",
-    packages=["coinpaprika_async"],
+    packages=["coinpaprika_async", "coinpaprika_async.api"],
     url="https://github.com/DroidZed/coinpaprika-async-client.git",
     license="MIT",
     install_requires=["httpx"],
     keywords="coinpaprika_async api cryptocurrency async httpx client",
     classifiers=[
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
```

### Comparing `coinpaprika_async-3.0.0/tests/test_client.py` & `coinpaprika_async-3.0.1/tests/test_client.py`

 * *Files identical despite different names*

