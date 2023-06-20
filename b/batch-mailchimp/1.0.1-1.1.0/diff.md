# Comparing `tmp/batch-mailchimp-1.0.1.tar.gz` & `tmp/batch-mailchimp-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "batch-mailchimp-1.0.1.tar", last modified: Tue Jun 20 18:24:29 2023, max compression
+gzip compressed data, was "batch-mailchimp-1.1.0.tar", last modified: Tue Jun 20 18:38:54 2023, max compression
```

## Comparing `batch-mailchimp-1.0.1.tar` & `batch-mailchimp-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:24:29.460153 batch-mailchimp-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-20 18:24:21.000000 batch-mailchimp-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-06-20 18:24:29.460153 batch-mailchimp-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-06-20 18:24:21.000000 batch-mailchimp-1.0.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:24:29.460153 batch-mailchimp-1.0.1/batch_mailchimp/
--rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-06-20 18:24:21.000000 batch-mailchimp-1.0.1/batch_mailchimp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6479 2023-06-20 18:24:21.000000 batch-mailchimp-1.0.1/batch_mailchimp/batches_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:24:29.460153 batch-mailchimp-1.0.1/batch_mailchimp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-06-20 18:24:29.000000 batch-mailchimp-1.0.1/batch_mailchimp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-20 18:24:29.000000 batch-mailchimp-1.0.1/batch_mailchimp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 18:24:29.000000 batch-mailchimp-1.0.1/batch_mailchimp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-20 18:24:29.000000 batch-mailchimp-1.0.1/batch_mailchimp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-20 18:24:29.000000 batch-mailchimp-1.0.1/batch_mailchimp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 18:24:29.460153 batch-mailchimp-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-06-20 18:24:21.000000 batch-mailchimp-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:38:54.884643 batch-mailchimp-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-20 18:38:46.000000 batch-mailchimp-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-06-20 18:38:54.884643 batch-mailchimp-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-06-20 18:38:46.000000 batch-mailchimp-1.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:38:54.884643 batch-mailchimp-1.1.0/batch_mailchimp/
+-rw-r--r--   0 runner    (1001) docker     (123)     5438 2023-06-20 18:38:46.000000 batch-mailchimp-1.1.0/batch_mailchimp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-06-20 18:38:46.000000 batch-mailchimp-1.1.0/batch_mailchimp/batches_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-20 18:38:46.000000 batch-mailchimp-1.1.0/batch_mailchimp/collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-20 18:38:46.000000 batch-mailchimp-1.1.0/batch_mailchimp/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:38:54.884643 batch-mailchimp-1.1.0/batch_mailchimp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-06-20 18:38:54.000000 batch-mailchimp-1.1.0/batch_mailchimp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-20 18:38:54.000000 batch-mailchimp-1.1.0/batch_mailchimp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 18:38:54.000000 batch-mailchimp-1.1.0/batch_mailchimp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-20 18:38:54.000000 batch-mailchimp-1.1.0/batch_mailchimp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-20 18:38:54.000000 batch-mailchimp-1.1.0/batch_mailchimp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 18:38:54.884643 batch-mailchimp-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-06-20 18:38:46.000000 batch-mailchimp-1.1.0/setup.py
```

### Comparing `batch-mailchimp-1.0.1/LICENSE` & `batch-mailchimp-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `batch-mailchimp-1.0.1/PKG-INFO` & `batch-mailchimp-1.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: batch-mailchimp
-Version: 1.0.1
-Summary: A python client for v3 of MailChimp API, with batch support
+Version: 1.1.0
+Summary: A python client for MailChimp Marketing API, with batch support
 Home-page: https://github.com/FullFact/python-batchmailchimp
 Author: Andy Lulham
 Author-email: andy.lulham@fullfact.org
 License: MIT
-Keywords: mailchimp api v3 client wrapper
+Keywords: mailchimp marketing api client wrapper
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 License-File: LICENSE
 
 Python BatchMailchimp
 =====================
 
 .. image:: https://img.shields.io/pypi/v/batch-mailchimp.svg
     :alt: PyPI Package latest release
```

### Comparing `batch-mailchimp-1.0.1/README.rst` & `batch-mailchimp-1.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `batch-mailchimp-1.0.1/batch_mailchimp/__init__.py` & `batch-mailchimp-1.1.0/batch_mailchimp/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 from mailchimp_marketing.api.search_campaigns_api import SearchCampaignsApi
 from mailchimp_marketing.api.search_members_api import SearchMembersApi
 from mailchimp_marketing.api.template_folders_api import TemplateFoldersApi
 from mailchimp_marketing.api.templates_api import TemplatesApi
 from mailchimp_marketing.api.verified_domains_api import VerifiedDomainsApi
 from mailchimp_marketing import api_client
 from mailchimp_marketing import Client as MailChimpClient
-
 from .batches_api import BatchesApi
 
 
 class FakeRequest:
     def __init__(self, operation_id):
         self.ok = True
         self.headers = {
```

### Comparing `batch-mailchimp-1.0.1/batch_mailchimp/batches_api.py` & `batch-mailchimp-1.1.0/batch_mailchimp/batches_api.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,15 @@
-from collections import UserDict
 import json
 from io import BytesIO
 import tarfile
 from itertools import islice
 from mailchimp_marketing.api import batches_api
 import requests
-
-
-class MyCollection(UserDict):
-    def __repr__(self):
-        return "<{module}.{name}: {data}>".format(
-            module=self.__class__.__module__,
-            name=self.__class__.__name__,
-            data=list(self.data.values()),
-        )
-
-    def __getitem__(self, item):
-        if type(item) is str:
-            return super().__getitem__(item)
-        return list(self.data.values())[item]
-
-    def __iter__(self):
-        for item in self.data.values():
-            yield item
-
-
-class ResponseCollection(MyCollection):
-    ...
-
-
-class BatchCollection(MyCollection):
-    ...
+from .decorators import no_batch
+from .collections import BatchCollection, ResponseCollection
 
 
 class Response:
     def __init__(self, **kwargs):
         self.operation_id = kwargs["operation_id"]
         self.status_code = kwargs["status_code"]
         self.body = json.loads(kwargs["response"])
@@ -98,26 +73,14 @@
             })
             return self.response
 
     def delete(self):
         return self._batches_api.delete_request(self.batch_id)
 
 
-def no_batch(func):
-    def wrapper_no_batch(self, *args, **kwargs):
-        batch_mode = self.api_client.batch_mode
-        self.api_client.set_batch_mode(False)
-        try:
-            response = func(self, *args, **kwargs)
-        finally:
-            self.api_client.set_batch_mode(batch_mode)
-        return response
-    return wrapper_no_batch
-
-
 class BatchesApi(batches_api.BatchesApi):
     _max_operations = 1_000
 
     def __init__(self, api_client):
         super().__init__(api_client)
         self._batches = BatchCollection()
```

### Comparing `batch-mailchimp-1.0.1/batch_mailchimp.egg-info/PKG-INFO` & `batch-mailchimp-1.1.0/batch_mailchimp.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: batch-mailchimp
-Version: 1.0.1
-Summary: A python client for v3 of MailChimp API, with batch support
+Version: 1.1.0
+Summary: A python client for MailChimp Marketing API, with batch support
 Home-page: https://github.com/FullFact/python-batchmailchimp
 Author: Andy Lulham
 Author-email: andy.lulham@fullfact.org
 License: MIT
-Keywords: mailchimp api v3 client wrapper
+Keywords: mailchimp marketing api client wrapper
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 License-File: LICENSE
 
 Python BatchMailchimp
 =====================
 
 .. image:: https://img.shields.io/pypi/v/batch-mailchimp.svg
     :alt: PyPI Package latest release
```

