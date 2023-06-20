# Comparing `tmp/pymexc-1.0.7.tar.gz` & `tmp/pymexc-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pymexc-1.0.7.tar", last modified: Tue Jun 20 14:13:00 2023, max compression
+gzip compressed data, was "dist\pymexc-1.0.8.tar", last modified: Tue Jun 20 19:37:43 2023, max compression
```

## Comparing `pymexc-1.0.7.tar` & `pymexc-1.0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 14:13:00.136821 pymexc-1.0.7/
--rw-rw-rw-   0        0        0     1088 2022-10-20 18:54:22.000000 pymexc-1.0.7/LICENSE
--rw-rw-rw-   0        0        0     3321 2023-06-20 14:13:00.136821 pymexc-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     2221 2023-05-30 13:04:58.000000 pymexc-1.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-20 14:13:00.117817 pymexc-1.0.7/pymexc/
--rw-rw-rw-   0        0        0     1431 2023-05-30 13:22:30.000000 pymexc-1.0.7/pymexc/__init__.py
--rw-rw-rw-   0        0        0     6130 2023-06-20 14:09:23.000000 pymexc-1.0.7/pymexc/base.py
--rw-rw-rw-   0        0        0    18102 2023-06-02 19:53:45.000000 pymexc-1.0.7/pymexc/base_websocket.py
--rw-rw-rw-   0        0        0    67666 2023-06-02 19:56:06.000000 pymexc-1.0.7/pymexc/futures.py
--rw-rw-rw-   0        0        0    68220 2023-06-02 19:56:58.000000 pymexc-1.0.7/pymexc/spot.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:13:00.135821 pymexc-1.0.7/pymexc.egg-info/
--rw-rw-rw-   0        0        0     3321 2023-06-20 14:12:59.000000 pymexc-1.0.7/pymexc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2023-06-20 14:13:00.000000 pymexc-1.0.7/pymexc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 14:12:59.000000 pymexc-1.0.7/pymexc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-20 14:12:59.000000 pymexc-1.0.7/pymexc.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       26 2023-06-20 14:12:59.000000 pymexc-1.0.7/pymexc.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-20 14:12:59.000000 pymexc-1.0.7/pymexc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-20 14:13:00.141822 pymexc-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1697 2023-06-20 14:11:56.000000 pymexc-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 19:37:43.415840 pymexc-1.0.8/
+-rw-rw-rw-   0        0        0     1088 2022-10-20 18:54:22.000000 pymexc-1.0.8/LICENSE
+-rw-rw-rw-   0        0        0     3321 2023-06-20 19:37:43.415840 pymexc-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2221 2023-05-30 13:04:58.000000 pymexc-1.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-06-20 19:37:43.391836 pymexc-1.0.8/pymexc/
+-rw-rw-rw-   0        0        0     1431 2023-05-30 13:22:30.000000 pymexc-1.0.8/pymexc/__init__.py
+-rw-rw-rw-   0        0        0     6190 2023-06-20 19:33:14.000000 pymexc-1.0.8/pymexc/base.py
+-rw-rw-rw-   0        0        0    18102 2023-06-02 19:53:45.000000 pymexc-1.0.8/pymexc/base_websocket.py
+-rw-rw-rw-   0        0        0    67666 2023-06-02 19:56:06.000000 pymexc-1.0.8/pymexc/futures.py
+-rw-rw-rw-   0        0        0    68220 2023-06-02 19:56:58.000000 pymexc-1.0.8/pymexc/spot.py
+drwxrwxrwx   0        0        0        0 2023-06-20 19:37:43.414841 pymexc-1.0.8/pymexc.egg-info/
+-rw-rw-rw-   0        0        0     3321 2023-06-20 19:37:43.000000 pymexc-1.0.8/pymexc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2023-06-20 19:37:43.000000 pymexc-1.0.8/pymexc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 19:37:43.000000 pymexc-1.0.8/pymexc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-20 19:37:43.000000 pymexc-1.0.8/pymexc.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       26 2023-06-20 19:37:43.000000 pymexc-1.0.8/pymexc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-20 19:37:43.000000 pymexc-1.0.8/pymexc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-20 19:37:43.416841 pymexc-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1697 2023-06-20 19:33:41.000000 pymexc-1.0.8/setup.py
```

### Comparing `pymexc-1.0.7/LICENSE` & `pymexc-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pymexc-1.0.7/PKG-INFO` & `pymexc-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pymexc
-Version: 1.0.7
+Version: 1.0.8
 Summary: Unofficial python library for interacting with the MEXC crypto exchange
 Home-page: https://github.com/makarworld/pymexc.git
-Download-URL: https://github.com/makarworld/pymexc/archive/refs/tags/v1.0.7.zip
+Download-URL: https://github.com/makarworld/pymexc/archive/refs/tags/v1.0.8.zip
 Author: abuztrade
 Author-email: abuztrade.work@gmail.com
 License: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Communications :: Email
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pymexc-1.0.7/README.md` & `pymexc-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `pymexc-1.0.7/pymexc/__init__.py` & `pymexc-1.0.8/pymexc/__init__.py`

 * *Files identical despite different names*

### Comparing `pymexc-1.0.7/pymexc/base.py` & `pymexc-1.0.8/pymexc/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from abc import ABC, abstractclassmethod
 from typing import Union, Literal
 import hmac, hashlib
 import requests
+from urllib.parse import urlencode
 import logging
 import time
 
 logger = logging.getLogger(__name__)
 
 class MexcAPIError(Exception): pass
 
@@ -46,26 +47,25 @@
     def __init__(self, api_key: str = None, api_secret: str = None, proxies: dict = None):
         super().__init__(api_key, api_secret, "https://api.mexc.com", proxies = proxies)
 
         self.session.headers.update({
             "X-MEXC-APIKEY": self.api_key
         })
 
-    def sign(self, **kwargs) -> str:
+    def sign(self, query_string: str) -> str:
         """
         Generates a signature for an API request using HMAC SHA256 encryption.
 
         Args:
             **kwargs: Arbitrary keyword arguments representing request parameters.
 
         Returns:
             A hexadecimal string representing the signature of the request.
         """
         # Generate signature
-        query_string = "&".join([f"{k}={v}" for k, v in kwargs.items()]) 
         signature = hmac.new(self.api_secret.encode('utf-8'), query_string.encode('utf-8'), hashlib.sha256).hexdigest()
         return signature
 
     def call(self, method: Union[Literal["GET"], Literal["POST"], Literal["PUT"], Literal["DELETE"]], router: str, *args, **kwargs) -> dict:
         if not router.startswith("/"):
             router = f"/{router}"
 
@@ -79,17 +79,19 @@
 
         if self.api_key and self.api_secret:
             # add signature
             timestamp = str(int(time.time() * 1000))
         kwargs['params']['recvWindow'] = self.recvWindow
         kwargs['params']['timestamp']  = timestamp
         kwargs['params'] = {k: v for k, v in sorted(kwargs['params'].items())}
-        kwargs['params']['signature']  = self.sign(**kwargs['params'])
+        
+        params = urlencode(kwargs.pop('params'), doseq=True).replace('+', '%20')
+        params += "&signature=" + self.sign(params)
 
-        response = self.session.request(method, f"{self.base_url}{router}", *args, **kwargs)
+        response = self.session.request(method, f"{self.base_url}{router}", params = params, *args, **kwargs)
 
         if not response.ok:
             raise MexcAPIError(f'(code={response.json()["code"]}): {response.json()["msg"]}')
 
         return response.json()
     
 class _FuturesHTTP(MexcSDK):
```

### Comparing `pymexc-1.0.7/pymexc/base_websocket.py` & `pymexc-1.0.8/pymexc/base_websocket.py`

 * *Files identical despite different names*

### Comparing `pymexc-1.0.7/pymexc/futures.py` & `pymexc-1.0.8/pymexc/futures.py`

 * *Files identical despite different names*

### Comparing `pymexc-1.0.7/pymexc/spot.py` & `pymexc-1.0.8/pymexc/spot.py`

 * *Files identical despite different names*

### Comparing `pymexc-1.0.7/pymexc.egg-info/PKG-INFO` & `pymexc-1.0.8/pymexc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pymexc
-Version: 1.0.7
+Version: 1.0.8
 Summary: Unofficial python library for interacting with the MEXC crypto exchange
 Home-page: https://github.com/makarworld/pymexc.git
-Download-URL: https://github.com/makarworld/pymexc/archive/refs/tags/v1.0.7.zip
+Download-URL: https://github.com/makarworld/pymexc/archive/refs/tags/v1.0.8.zip
 Author: abuztrade
 Author-email: abuztrade.work@gmail.com
 License: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Communications :: Email
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pymexc-1.0.7/setup.py` & `pymexc-1.0.8/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 :author: abuztrade
 :license: MIT License, see LICENSE file.
 :copyright: (c) 2022 by abuztrade.
 """
 
 
-version = '1.0.7'
+version = '1.0.8'
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="pymexc",
     version=version,
```

