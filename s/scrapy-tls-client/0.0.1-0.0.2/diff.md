# Comparing `tmp/scrapy-tls-client-0.0.1.tar.gz` & `tmp/scrapy-tls-client-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapy-tls-client-0.0.1.tar", last modified: Wed Jun 14 13:43:27 2023, max compression
+gzip compressed data, was "scrapy-tls-client-0.0.2.tar", last modified: Tue Jun 20 13:01:26 2023, max compression
```

## Comparing `scrapy-tls-client-0.0.1.tar` & `scrapy-tls-client-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 13:43:27.325617 scrapy-tls-client-0.0.1/
--rw-rw-rw-   0        0        0     1088 2023-06-14 11:35:40.000000 scrapy-tls-client-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     4790 2023-06-14 13:43:27.325617 scrapy-tls-client-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3756 2023-06-14 11:51:08.000000 scrapy-tls-client-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-14 13:43:27.319180 scrapy-tls-client-0.0.1/scrapy_tls_client/
--rw-rw-rw-   0        0        0       63 2023-06-14 11:35:40.000000 scrapy-tls-client-0.0.1/scrapy_tls_client/__init__.py
--rw-rw-rw-   0        0        0      369 2023-06-14 11:41:45.000000 scrapy-tls-client-0.0.1/scrapy_tls_client/__version__.py
--rw-rw-rw-   0        0        0     9489 2023-06-14 11:35:40.000000 scrapy-tls-client-0.0.1/scrapy_tls_client/downloaderMiddleware.py
--rw-rw-rw-   0        0        0     4928 2023-06-14 11:48:46.000000 scrapy-tls-client-0.0.1/scrapy_tls_client/settings.py
-drwxrwxrwx   0        0        0        0 2023-06-14 13:43:27.319180 scrapy-tls-client-0.0.1/scrapy_tls_client.egg-info/
--rw-rw-rw-   0        0        0     4790 2023-06-14 13:43:27.000000 scrapy-tls-client-0.0.1/scrapy_tls_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      365 2023-06-14 13:43:27.000000 scrapy-tls-client-0.0.1/scrapy_tls_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 13:43:27.000000 scrapy-tls-client-0.0.1/scrapy_tls_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-06-14 13:43:27.000000 scrapy-tls-client-0.0.1/scrapy_tls_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-06-14 13:43:27.000000 scrapy-tls-client-0.0.1/scrapy_tls_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-14 13:43:27.325617 scrapy-tls-client-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     2844 2023-06-14 13:43:25.000000 scrapy-tls-client-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 13:01:26.818237 scrapy-tls-client-0.0.2/
+-rw-rw-rw-   0        0        0     1088 2023-06-14 11:35:40.000000 scrapy-tls-client-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     5470 2023-06-20 13:01:26.818237 scrapy-tls-client-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4436 2023-06-20 12:54:00.000000 scrapy-tls-client-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-20 13:01:26.818237 scrapy-tls-client-0.0.2/scrapy_tls_client/
+-rw-rw-rw-   0        0        0       63 2023-06-14 11:35:40.000000 scrapy-tls-client-0.0.2/scrapy_tls_client/__init__.py
+-rw-rw-rw-   0        0        0      369 2023-06-20 12:53:13.000000 scrapy-tls-client-0.0.2/scrapy_tls_client/__version__.py
+-rw-rw-rw-   0        0        0    10185 2023-06-20 12:53:13.000000 scrapy-tls-client-0.0.2/scrapy_tls_client/downloaderMiddleware.py
+-rw-rw-rw-   0        0        0     5458 2023-06-20 12:53:13.000000 scrapy-tls-client-0.0.2/scrapy_tls_client/settings.py
+drwxrwxrwx   0        0        0        0 2023-06-20 13:01:26.818237 scrapy-tls-client-0.0.2/scrapy_tls_client.egg-info/
+-rw-rw-rw-   0        0        0     5470 2023-06-20 13:01:26.000000 scrapy-tls-client-0.0.2/scrapy_tls_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      378 2023-06-20 13:01:26.000000 scrapy-tls-client-0.0.2/scrapy_tls_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 13:01:26.000000 scrapy-tls-client-0.0.2/scrapy_tls_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-06-20 13:01:26.000000 scrapy-tls-client-0.0.2/scrapy_tls_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-06-20 13:01:26.000000 scrapy-tls-client-0.0.2/scrapy_tls_client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-20 13:01:26.818237 scrapy-tls-client-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     2844 2023-06-14 13:43:25.000000 scrapy-tls-client-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 13:01:26.818237 scrapy-tls-client-0.0.2/test/
+-rw-rw-rw-   0        0        0      815 2023-06-20 12:44:19.000000 scrapy-tls-client-0.0.2/test/test.py
```

### Comparing `scrapy-tls-client-0.0.1/LICENSE` & `scrapy-tls-client-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `scrapy-tls-client-0.0.1/PKG-INFO` & `scrapy-tls-client-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapy-tls-client
-Version: 0.0.1
+Version: 0.0.2
 Summary: tls client downloader middleware for scrapy, send request by tls client.
 Home-page: https://github.com/dylankeepon/TlsClientMiddleware.git
 Author: Dylan Chen
 Author-email: dylankeep@163.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
@@ -39,26 +39,44 @@
 After add this middleware, all requests will be sent by tls_client.
 
 The usage is very simple, for tls client session, just add params in settings.py in scrapy project, 
 for request, specify params in meta. 
 
 PLEASE NOTE YOU DO NOT NEED TO SPECIFY ALL PARAMS SHOWS BELOW, JUST SPECIFY REQUIRED.
 
-For the preset usage of tls_client:
-
 ### Settings for Tls_Client Session
 
+For the preset usage of tls_client:
+
 ```python
 CLIENT_IDENTIFIER = 'chrome_112'
 RANDOM_TLS_EXTENSION_ORDER = True
 FORCE_HTTP1 = False #default False
 CATCH_PANICS = False #default False
 RAW_RESPONSE_TYPE = 'HtmlResponse' #HtmlResponse or TextResponse, default HtmlResponse
 ```
 
+or
+
+```python
+RANDOM_CHROME_IDENTIFIER = True
+RANDOM_TLS_EXTENSION_ORDER = True
+FORCE_HTTP1 = False #default False
+CATCH_PANICS = False #default False
+RAW_RESPONSE_TYPE = 'HtmlResponse' #HtmlResponse or TextResponse, default HtmlResponse
+```
+
+```python
+RANDOM_APP_IDENTIFIER = True
+RANDOM_TLS_EXTENSION_ORDER = True
+FORCE_HTTP1 = False #default False
+CATCH_PANICS = False #default False
+RAW_RESPONSE_TYPE = 'HtmlResponse' #HtmlResponse or TextResponse, default HtmlResponse
+```
+
 For the custom usage:
 
 ```python
 JA3_STRING = '771,4865-4866-4867-49195-49199-49196-49200-52393-52392-49171-49172-156-157-47-53,0-23-65281-10-11-35-16-5-13-18-51-45-43-27-17513,29-23-24,0'
 H2_SETTINGS = {
     "HEADER_TABLE_SIZE": 65536,
     "MAX_CONCURRENT_STREAMS": 1000,
@@ -160,14 +178,19 @@
     'key2': 'value2',
 }
 payload = {
     'key1': 'value1',
     'key2': 'value2'
 }
 proxy = 'http://username:password@ip:port' # https also works
+or 
+proxy = [
+    'http://username:password@ip:port',
+    'http://username:password@ip:port',
+] # if the type of proxy is list, every request will get a random proxy in the list
 meta_data = {
     'params': params,
     'data': data,
     'cookies': cookies,
     'json': payload,
     'allow_redirects': False,
     'insecure_skip_verify': False,
```

### Comparing `scrapy-tls-client-0.0.1/README.md` & `scrapy-tls-client-0.0.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -14,26 +14,44 @@
 After add this middleware, all requests will be sent by tls_client.
 
 The usage is very simple, for tls client session, just add params in settings.py in scrapy project, 
 for request, specify params in meta. 
 
 PLEASE NOTE YOU DO NOT NEED TO SPECIFY ALL PARAMS SHOWS BELOW, JUST SPECIFY REQUIRED.
 
-For the preset usage of tls_client:
-
 ### Settings for Tls_Client Session
 
+For the preset usage of tls_client:
+
 ```python
 CLIENT_IDENTIFIER = 'chrome_112'
 RANDOM_TLS_EXTENSION_ORDER = True
 FORCE_HTTP1 = False #default False
 CATCH_PANICS = False #default False
 RAW_RESPONSE_TYPE = 'HtmlResponse' #HtmlResponse or TextResponse, default HtmlResponse
 ```
 
+or
+
+```python
+RANDOM_CHROME_IDENTIFIER = True
+RANDOM_TLS_EXTENSION_ORDER = True
+FORCE_HTTP1 = False #default False
+CATCH_PANICS = False #default False
+RAW_RESPONSE_TYPE = 'HtmlResponse' #HtmlResponse or TextResponse, default HtmlResponse
+```
+
+```python
+RANDOM_APP_IDENTIFIER = True
+RANDOM_TLS_EXTENSION_ORDER = True
+FORCE_HTTP1 = False #default False
+CATCH_PANICS = False #default False
+RAW_RESPONSE_TYPE = 'HtmlResponse' #HtmlResponse or TextResponse, default HtmlResponse
+```
+
 For the custom usage:
 
 ```python
 JA3_STRING = '771,4865-4866-4867-49195-49199-49196-49200-52393-52392-49171-49172-156-157-47-53,0-23-65281-10-11-35-16-5-13-18-51-45-43-27-17513,29-23-24,0'
 H2_SETTINGS = {
     "HEADER_TABLE_SIZE": 65536,
     "MAX_CONCURRENT_STREAMS": 1000,
@@ -135,14 +153,19 @@
     'key2': 'value2',
 }
 payload = {
     'key1': 'value1',
     'key2': 'value2'
 }
 proxy = 'http://username:password@ip:port' # https also works
+or 
+proxy = [
+    'http://username:password@ip:port',
+    'http://username:password@ip:port',
+] # if the type of proxy is list, every request will get a random proxy in the list
 meta_data = {
     'params': params,
     'data': data,
     'cookies': cookies,
     'json': payload,
     'allow_redirects': False,
     'insecure_skip_verify': False,
```

### Comparing `scrapy-tls-client-0.0.1/scrapy_tls_client/downloaderMiddleware.py` & `scrapy-tls-client-0.0.2/scrapy_tls_client/downloaderMiddleware.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     TimeoutError,
 )
 from twisted.web.client import ResponseFailed
 from scrapy.core.downloader.handlers.http11 import TunnelError
 from scrapy.utils.python import global_object_name
 from scrapy.utils.response import response_status_message
 from scrapy_tls_client.settings import *
+import random
 import logging
 logger = logging.getLogger('TlsClientDownloaderMiddleware')
 
 
 class TlsClientDownloaderMiddleware:
 
     EXCEPTIONS_TO_RETRY = (
@@ -41,14 +42,18 @@
 
     @classmethod
     def from_crawler(cls, crawler):
         # This method is used by Scrapy to create your spiders.
         settings = crawler.settings
         s = cls()
         cls.client_identifier = settings.get('CLIENT_IDENTIFIER', CLIENT_IDENTIFIER)
+        cls.random_chrome_identifier = settings.get('RANDOM_CHROME_IDENTIFIER', RANDOM_CHROME_IDENTIFIER)
+        cls.random_app_identifier = settings.get('RANDOM_APP_IDENTIFIER', RANDOM_APP_IDENTIFIER)
+        cls.chrome_identifier = settings.get('CHROME_IDENTIFIER', CHROME_IDENTIFIER)
+        cls.app_identifier = settings.get('APP_IDENTIFIER', APP_IDENTIFIER)
         cls.ja3_string = settings.get('JA3_STRING', JA3_STRING)
         cls.h2_settings = settings.get('H2_SETTINGS', H2_SETTINGS)
         cls.h2_settings_order = settings.get('H2_SETTINGS_ORDER', H2_SETTINGS_ORDER)
         cls.supported_signature_algorithms = settings.get('SUPPORTED_SIGNATURE_ALGORITHMS',
                                                         SUPPORTED_SIGNATURE_ALGORITHMS)
         cls.supported_delegated_credentials_algorithms = settings.get('SUPPORTED_DELEGATED_CREDENTIALS_ALGORITHMS',
                                                                     SUPPORTED_DELEGATED_CREDENTIALS_ALGORITHMS)
@@ -106,14 +111,18 @@
             stats.inc_value('retry/max_reached')
             logger.error("Gave up retrying %(request)s (failed %(retry_times)d times): %(reason)s",
                          {'request': request, 'retry_times': retry_times, 'reason': reason},
                          extra={'spider': spider})
             return None
 
     def _process_request(self, request, spider):
+        if self.random_chrome_identifier:
+            self.client_identifier = random.choice(self.chrome_identifier)
+        elif self.random_app_identifier:
+            self.client_identifier = random.choice(self.app_identifier)
         if self.client_identifier:
             tls_session = tls_client.Session(
                 client_identifier=self.client_identifier,
                 additional_decode=self.additional_decode,
                 header_order=self.header_order,
                 random_tls_extension_order=self.random_tls_extension_order,
                 force_http1=self.force_http1,
@@ -145,14 +154,16 @@
         data = request.meta.get('data', None)
         cookies = request.meta.get('cookies', None)
         json = request.meta.get('json', None)
         allow_redirects = request.meta.get('allow_redirects', False)
         insecure_skip_verify = request.meta.get('insecure_skip_verify', False)
         timeout_seconds = request.meta.get('timeout_seconds', None)
         proxy = request.meta.get('proxy', None)
+        if isinstance(proxy, list):
+            proxy = random.choice(proxy)
         try:
             response = tls_session.execute_request(method=method, url=url, params=params, data=data,
                                                    headers=headers, cookies=cookies,
                                                    json=json, allow_redirects=allow_redirects,
                                                    insecure_skip_verify=insecure_skip_verify,
                                                    timeout_seconds=timeout_seconds, proxy=proxy)
         except Exception as e:
```

### Comparing `scrapy-tls-client-0.0.1/scrapy_tls_client/settings.py` & `scrapy-tls-client-0.0.2/scrapy_tls_client/settings.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,15 +8,22 @@
 # Safari --> safari_15_3, safari_15_6_1, safari_16_0
 # iOS --> safari_ios_15_5, safari_ios_15_6, safari_ios_16_0
 # iPadOS --> safari_ios_15_6
 # Android --> okhttp4_android_7, okhttp4_android_8, okhttp4_android_9, okhttp4_android_10, okhttp4_android_11,
 #             okhttp4_android_12, okhttp4_android_13
 # CLIENT_IDENTIFIER = 'chrome_112'
 CLIENT_IDENTIFIER = None
+RANDOM_CHROME_IDENTIFIER = False
+RANDOM_APP_IDENTIFIER = False
+CHROME_IDENTIFIER = ['chrome_103', 'chrome_104', 'chrome_105', 'chrome_106', 'chrome_107',
+                    'chrome_108', 'chrome_109', 'Chrome_110', 'chrome_111', 'chrome_112']
 
+APP_IDENTIFIER = ['safari_ios_15_5', 'safari_ios_15_6', 'safari_ios_16_0', 'safari_ios_15_6',
+                 'okhttp4_android_7', 'okhttp4_android_8', 'okhttp4_android_9', 'okhttp4_android_10',
+                 'okhttp4_android_11', 'okhttp4_android_12', 'okhttp4_android_13']
 # Set JA3 --> TLSVersion, Ciphers, Extensions, EllipticCurves, EllipticCurvePointFormats
 # Example:
 # JA3_STRING = '771,4865-4866-4867-49195-49199-49196-49200-52393-52392-49171-49172-156-157-47-53,0-23-65281-10-11-35-16-5-13-18-51-45-43-27-17513,29-23-24,0'
 JA3_STRING=None
 
 # HTTP2 Header Frame Settings
 # Possible Settings:
```

### Comparing `scrapy-tls-client-0.0.1/scrapy_tls_client.egg-info/PKG-INFO` & `scrapy-tls-client-0.0.2/scrapy_tls_client.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapy-tls-client
-Version: 0.0.1
+Version: 0.0.2
 Summary: tls client downloader middleware for scrapy, send request by tls client.
 Home-page: https://github.com/dylankeepon/TlsClientMiddleware.git
 Author: Dylan Chen
 Author-email: dylankeep@163.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
@@ -39,26 +39,44 @@
 After add this middleware, all requests will be sent by tls_client.
 
 The usage is very simple, for tls client session, just add params in settings.py in scrapy project, 
 for request, specify params in meta. 
 
 PLEASE NOTE YOU DO NOT NEED TO SPECIFY ALL PARAMS SHOWS BELOW, JUST SPECIFY REQUIRED.
 
-For the preset usage of tls_client:
-
 ### Settings for Tls_Client Session
 
+For the preset usage of tls_client:
+
 ```python
 CLIENT_IDENTIFIER = 'chrome_112'
 RANDOM_TLS_EXTENSION_ORDER = True
 FORCE_HTTP1 = False #default False
 CATCH_PANICS = False #default False
 RAW_RESPONSE_TYPE = 'HtmlResponse' #HtmlResponse or TextResponse, default HtmlResponse
 ```
 
+or
+
+```python
+RANDOM_CHROME_IDENTIFIER = True
+RANDOM_TLS_EXTENSION_ORDER = True
+FORCE_HTTP1 = False #default False
+CATCH_PANICS = False #default False
+RAW_RESPONSE_TYPE = 'HtmlResponse' #HtmlResponse or TextResponse, default HtmlResponse
+```
+
+```python
+RANDOM_APP_IDENTIFIER = True
+RANDOM_TLS_EXTENSION_ORDER = True
+FORCE_HTTP1 = False #default False
+CATCH_PANICS = False #default False
+RAW_RESPONSE_TYPE = 'HtmlResponse' #HtmlResponse or TextResponse, default HtmlResponse
+```
+
 For the custom usage:
 
 ```python
 JA3_STRING = '771,4865-4866-4867-49195-49199-49196-49200-52393-52392-49171-49172-156-157-47-53,0-23-65281-10-11-35-16-5-13-18-51-45-43-27-17513,29-23-24,0'
 H2_SETTINGS = {
     "HEADER_TABLE_SIZE": 65536,
     "MAX_CONCURRENT_STREAMS": 1000,
@@ -160,14 +178,19 @@
     'key2': 'value2',
 }
 payload = {
     'key1': 'value1',
     'key2': 'value2'
 }
 proxy = 'http://username:password@ip:port' # https also works
+or 
+proxy = [
+    'http://username:password@ip:port',
+    'http://username:password@ip:port',
+] # if the type of proxy is list, every request will get a random proxy in the list
 meta_data = {
     'params': params,
     'data': data,
     'cookies': cookies,
     'json': payload,
     'allow_redirects': False,
     'insecure_skip_verify': False,
```

### Comparing `scrapy-tls-client-0.0.1/setup.py` & `scrapy-tls-client-0.0.2/setup.py`

 * *Files identical despite different names*

