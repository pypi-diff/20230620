# Comparing `tmp/algocash-sdk-1.1.1.tar.gz` & `tmp/algocash-sdk-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "algocash-sdk-1.1.1.tar", last modified: Mon Jun 19 19:04:21 2023, max compression
+gzip compressed data, was "algocash-sdk-1.2.0.tar", last modified: Tue Jun 20 09:15:45 2023, max compression
```

## Comparing `algocash-sdk-1.1.1.tar` & `algocash-sdk-1.2.0.tar`

### file list

```diff
@@ -1,47 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 19:04:21.324744 algocash-sdk-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-19 19:04:21.324744 algocash-sdk-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-06-19 19:04:10.000000 algocash-sdk-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 19:04:21.316744 algocash-sdk-1.1.1/algocash_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-06-19 19:04:10.000000 algocash-sdk-1.1.1/algocash_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 19:04:21.320744 algocash-sdk-1.1.1/algocash_sdk/api/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-19 19:04:10.000000 algocash-sdk-1.1.1/algocash_sdk/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6601 2023-06-19 19:04:10.000000 algocash-sdk-1.1.1/algocash_sdk/api/deposit_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7183 2023-06-19 19:04:10.000000 algocash-sdk-1.1.1/algocash_sdk/api/payout_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    27984 2023-06-19 19:04:10.000000 algocash-sdk-1.1.1/algocash_sdk/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8128 2023-06-19 19:04:10.000000 algocash-sdk-1.1.1/algocash_sdk/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 19:04:21.320744 algocash-sdk-1.1.1/algocash_sdk/models/
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-19 19:04:10.000000 algocash-sdk-1.1.1/algocash_sdk/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-06-19 19:04:10.000000 algocash-sdk-1.1.1/algocash_sdk/models/address.py
--rw-r--r--   0 runner    (1001) docker     (123)     6398 2023-06-19 19:04:10.000000 algocash-sdk-1.1.1/algocash_sdk/models/bank.py
--rw-r--r--   0 runner    (1001) docker     (123)     8417 2023-06-19 19:04:10.000000 algocash-sdk-1.1.1/algocash_sdk/models/callback_payload.py
--rw-r--r--   0 runner    (1001) docker     (123)     6081 2023-06-19 19:04:10.000000 algocash-sdk-1.1.1/algocash_sdk/models/deposit_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-06-19 19:04:10.000000 algocash-sdk-1.1.1/algocash_sdk/models/deposit_success.py
--rw-r--r--   0 runner    (1001) docker     (123)     4151 2023-06-19 19:04:10.000000 algocash-sdk-1.1.1/algocash_sdk/models/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     6877 2023-06-19 19:04:10.000000 algocash-sdk-1.1.1/algocash_sdk/models/payer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6801 2023-06-19 19:04:10.000000 algocash-sdk-1.1.1/algocash_sdk/models/payout_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-06-19 19:04:10.000000 algocash-sdk-1.1.1/algocash_sdk/models/payout_success.py
--rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-06-19 19:04:10.000000 algocash-sdk-1.1.1/algocash_sdk/models/url.py
--rw-r--r--   0 runner    (1001) docker     (123)    12974 2023-06-19 19:04:10.000000 algocash-sdk-1.1.1/algocash_sdk/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 19:04:21.320744 algocash-sdk-1.1.1/algocash_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-19 19:04:21.000000 algocash-sdk-1.1.1/algocash_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-19 19:04:21.000000 algocash-sdk-1.1.1/algocash_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 19:04:21.000000 algocash-sdk-1.1.1/algocash_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-19 19:04:21.000000 algocash-sdk-1.1.1/algocash_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-19 19:04:21.000000 algocash-sdk-1.1.1/algocash_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 19:04:21.324744 algocash-sdk-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-19 19:04:10.000000 algocash-sdk-1.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 19:04:21.320744 algocash-sdk-1.1.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-19 19:04:10.000000 algocash-sdk-1.1.1/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-19 19:04:10.000000 algocash-sdk-1.1.1/test/server.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-19 19:04:10.000000 algocash-sdk-1.1.1/test/test_address.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-19 19:04:10.000000 algocash-sdk-1.1.1/test/test_bank.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-19 19:04:10.000000 algocash-sdk-1.1.1/test/test_callback_payload.py
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-06-19 19:04:10.000000 algocash-sdk-1.1.1/test/test_deposit_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-06-19 19:04:10.000000 algocash-sdk-1.1.1/test/test_deposit_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-06-19 19:04:10.000000 algocash-sdk-1.1.1/test/test_deposit_success.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-19 19:04:10.000000 algocash-sdk-1.1.1/test/test_error.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-19 19:04:10.000000 algocash-sdk-1.1.1/test/test_payer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-06-19 19:04:10.000000 algocash-sdk-1.1.1/test/test_payout_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-19 19:04:10.000000 algocash-sdk-1.1.1/test/test_payout_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-19 19:04:10.000000 algocash-sdk-1.1.1/test/test_payout_success.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-06-19 19:04:10.000000 algocash-sdk-1.1.1/test/test_url.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:15:45.487049 algocash-sdk-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-20 09:15:45.487049 algocash-sdk-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-06-20 09:15:35.000000 algocash-sdk-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:15:45.483049 algocash-sdk-1.2.0/algocash_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-20 09:15:35.000000 algocash-sdk-1.2.0/algocash_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:15:45.483049 algocash-sdk-1.2.0/algocash_sdk/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-20 09:15:35.000000 algocash-sdk-1.2.0/algocash_sdk/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-06-20 09:15:35.000000 algocash-sdk-1.2.0/algocash_sdk/api/deposit_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-06-20 09:15:35.000000 algocash-sdk-1.2.0/algocash_sdk/api/payout_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27823 2023-06-20 09:15:35.000000 algocash-sdk-1.2.0/algocash_sdk/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8724 2023-06-20 09:15:35.000000 algocash-sdk-1.2.0/algocash_sdk/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:15:45.483049 algocash-sdk-1.2.0/algocash_sdk/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-20 09:15:35.000000 algocash-sdk-1.2.0/algocash_sdk/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-06-20 09:15:35.000000 algocash-sdk-1.2.0/algocash_sdk/models/address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6268 2023-06-20 09:15:35.000000 algocash-sdk-1.2.0/algocash_sdk/models/bank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8287 2023-06-20 09:15:35.000000 algocash-sdk-1.2.0/algocash_sdk/models/callback_payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-06-20 09:15:35.000000 algocash-sdk-1.2.0/algocash_sdk/models/deposit_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7837 2023-06-20 09:15:35.000000 algocash-sdk-1.2.0/algocash_sdk/models/deposit_status_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-06-20 09:15:35.000000 algocash-sdk-1.2.0/algocash_sdk/models/deposit_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-06-20 09:15:35.000000 algocash-sdk-1.2.0/algocash_sdk/models/deposit_success.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-06-20 09:15:35.000000 algocash-sdk-1.2.0/algocash_sdk/models/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6747 2023-06-20 09:15:35.000000 algocash-sdk-1.2.0/algocash_sdk/models/payer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-06-20 09:15:35.000000 algocash-sdk-1.2.0/algocash_sdk/models/payout_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6903 2023-06-20 09:15:35.000000 algocash-sdk-1.2.0/algocash_sdk/models/payout_status_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-06-20 09:15:35.000000 algocash-sdk-1.2.0/algocash_sdk/models/payout_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-06-20 09:15:35.000000 algocash-sdk-1.2.0/algocash_sdk/models/payout_success.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5874 2023-06-20 09:15:35.000000 algocash-sdk-1.2.0/algocash_sdk/models/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12905 2023-06-20 09:15:35.000000 algocash-sdk-1.2.0/algocash_sdk/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:15:45.483049 algocash-sdk-1.2.0/algocash_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-20 09:15:45.000000 algocash-sdk-1.2.0/algocash_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-06-20 09:15:45.000000 algocash-sdk-1.2.0/algocash_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 09:15:45.000000 algocash-sdk-1.2.0/algocash_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-20 09:15:45.000000 algocash-sdk-1.2.0/algocash_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-20 09:15:45.000000 algocash-sdk-1.2.0/algocash_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 09:15:45.487049 algocash-sdk-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-20 09:15:35.000000 algocash-sdk-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:15:45.487049 algocash-sdk-1.2.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-20 09:15:35.000000 algocash-sdk-1.2.0/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-20 09:15:35.000000 algocash-sdk-1.2.0/test/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-20 09:15:35.000000 algocash-sdk-1.2.0/test/test_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-20 09:15:35.000000 algocash-sdk-1.2.0/test/test_bank.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-20 09:15:35.000000 algocash-sdk-1.2.0/test/test_callback_payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-06-20 09:15:35.000000 algocash-sdk-1.2.0/test/test_deposit_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-20 09:15:35.000000 algocash-sdk-1.2.0/test/test_deposit_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-06-20 09:15:35.000000 algocash-sdk-1.2.0/test/test_deposit_status_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-20 09:15:35.000000 algocash-sdk-1.2.0/test/test_deposit_success.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-20 09:15:35.000000 algocash-sdk-1.2.0/test/test_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-20 09:15:35.000000 algocash-sdk-1.2.0/test/test_payer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-06-20 09:15:35.000000 algocash-sdk-1.2.0/test/test_payout_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-20 09:15:35.000000 algocash-sdk-1.2.0/test/test_payout_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-06-20 09:15:35.000000 algocash-sdk-1.2.0/test/test_payout_status_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-20 09:15:35.000000 algocash-sdk-1.2.0/test/test_payout_success.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-20 09:15:35.000000 algocash-sdk-1.2.0/test/test_url.py
```

### Comparing `algocash-sdk-1.1.1/README.md` & `algocash-sdk-1.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 amount = '12' # str | 
 payer = algocash_sdk.Payer('email', 'phone number') # Payer 
 payment_method = 'UPI' # str | 
 url = algocash_sdk.Url('callback_url', 'pending_url', 'success_url', 'error_url') # Url | 
 
 try:
     # create a deposit
-    api_response = api_instance.create_deposit(invoice_id, amount, payer, payment_method, url)
+    api_response = api_instance.create_deposit(invoice_id, amount, payer, url, payment_method)
     pprint(api_response)
 except ValueError as e:
             print("ValueError Exception when calling DepositApi->create_deposit: %s\n" % e)
 except ApiException as e:
     print("Exception when calling DepositApi->create_deposit: %s\n" % e)
     pprint(json.loads(e.body))
 ```
```

### Comparing `algocash-sdk-1.1.1/algocash_sdk/__init__.py` & `algocash-sdk-1.2.0/algocash_sdk/models/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,30 @@
 # coding: utf-8
 
 # flake8: noqa
-
 """
     Algocash API
 
     This is a Algocash API  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     Contact: loganph.work@gmail.com
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
+    
 """
 
 from __future__ import absolute_import
 
-# import apis into sdk package
-from algocash_sdk.api.deposit_api import DepositApi
-from algocash_sdk.api.payout_api import PayoutApi
-# import ApiClient
-from algocash_sdk.api_client import ApiClient
-from algocash_sdk.configuration import Configuration
-# import models into sdk package
+# import models into model package
 from algocash_sdk.models.address import Address
 from algocash_sdk.models.bank import Bank
 from algocash_sdk.models.callback_payload import CallbackPayload
 from algocash_sdk.models.deposit_request import DepositRequest
 from algocash_sdk.models.deposit_success import DepositSuccess
+from algocash_sdk.models.deposit_status_response import DepositStatusResponse
+from algocash_sdk.models.deposit_status_info import DepositStatusInfo
 from algocash_sdk.models.error import Error
 from algocash_sdk.models.payer import Payer
 from algocash_sdk.models.payout_request import PayoutRequest
 from algocash_sdk.models.payout_success import PayoutSuccess
+from algocash_sdk.models.payout_status_response import PayoutStatusResponse
+from algocash_sdk.models.payout_status_info import PayoutStatusInfo
 from algocash_sdk.models.url import Url
```

### Comparing `algocash-sdk-1.1.1/algocash_sdk/api_client.py` & `algocash-sdk-1.2.0/algocash_sdk/api_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 """
     Algocash API
 
     This is a Algocash API  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     Contact: loganph.work@gmail.com
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
+    
 """
 from __future__ import absolute_import
 
 import datetime
 import json
 import mimetypes
 from multiprocessing.pool import ThreadPool
@@ -31,15 +31,15 @@
     """Generic API client for Swagger client library builds.
 
     Swagger generic API client. This client handles the client-
     server communication, and is invariant across implementations. Specifics of
     the methods and models for each application are generated from the Swagger
     templates.
 
-    NOTE: This class is auto generated by the swagger code generator program.
+    .
     Ref: https://github.com/swagger-api/swagger-codegen
     Do not edit the class manually.
 
     :param configuration: .Configuration object for this client
     :param header_name: a header to pass when making calls to the API.
     :param header_value: a header value to pass when making calls to
         the API.
@@ -89,15 +89,15 @@
 
     def set_default_header(self, header_name, header_value):
         self.default_headers[header_name] = header_value
 
     def __call_api(
             self, resource_path, method, path_params=None,
             query_params=None, header_params=None, body=None, post_params=None,
-            files=None, response_type=None, auth_settings=None,
+            files=None, response_type=None, auth_requested=True,
             _return_http_data_only=None, collection_formats=None,
             _preload_content=True, _request_timeout=None):
 
         config = self.configuration
 
         # header parameters
         header_params = header_params or {}
@@ -134,18 +134,19 @@
         
         # body
         if body:
             body = self.sanitize_for_serialization(body)
             body = self.parameters_to_dicts(body)
 
         # auth setting
-        self.update_params_for_auth(header_params, body, query_params, auth_settings)
+        if auth_requested:
+            self.update_params_for_auth(header_params, body, query_params)
         
         # request url
-        url = self.configuration.host + resource_path
+        url = self.configuration.get_host() + resource_path
 
         # perform request and return response
         response_data = self.request(
             method, url, query_params=query_params, headers=header_params,
             post_params=post_params, body=body,
             _preload_content=_preload_content,
             _request_timeout=_request_timeout)
@@ -193,20 +194,20 @@
         elif isinstance(obj, (datetime.datetime, datetime.date)):
             return obj.isoformat()
 
         if isinstance(obj, dict):
             obj_dict = obj
         else:
             # Convert model obj to dict except
-            # attributes `swagger_types`, `attribute_map`
+            # attributes `attribute_types`, `attribute_map`
             # and attributes which value is not None.
             # Convert attribute name to json key in
             # model definition for request.
             obj_dict = {obj.attribute_map[attr]: getattr(obj, attr)
-                        for attr, _ in six.iteritems(obj.swagger_types)
+                        for attr, _ in six.iteritems(obj.attribute_types)
                         if getattr(obj, attr) is not None}
 
         return {key: self.sanitize_for_serialization(val)
                 for key, val in six.iteritems(obj_dict)}
 
     def deserialize(self, response, response_type):
         """Deserializes response into an object.
@@ -267,22 +268,16 @@
             return self.__deserialize_object(data)
         elif klass == datetime.date:
             return self.__deserialize_date(data)
         elif klass == datetime.datetime:
             return self.__deserialize_datatime(data)
         else:
             return self.__deserialize_model(data, klass)
-
-    def call_api(self, resource_path, method,
-                 path_params=None, query_params=None, header_params=None,
-                 body=None, post_params=None, files=None,
-                 response_type=None, auth_settings=None, async_req=None,
-                 _return_http_data_only=None, collection_formats=None,
-                 _preload_content=True, _request_timeout=None):
-        """Makes the HTTP request (synchronous) and returns deserialized data.
+        
+    """Makes the HTTP request (synchronous) and returns deserialized data.
 
         To make an async request, set the async_req parameter.
 
         :param resource_path: Path to method endpoint.
         :param method: Method to call.
         :param path_params: Path parameters in the url.
         :param query_params: Query parameters in the url.
@@ -310,27 +305,35 @@
         :return:
             If async_req parameter is True,
             the request will be called asynchronously.
             The method will return the request thread.
             If parameter async_req is False or missing,
             then the method will return the response directly.
         """
+
+    def call_api(self, resource_path, method,
+                 path_params=None, query_params=None, header_params=None,
+                 body=None, post_params=None, files=None,
+                 response_type=None, auth_requested=True, async_req=None,
+                 _return_http_data_only=True, collection_formats=None,
+                 _preload_content=True, _request_timeout=None):
+        
         if not async_req:
             return self.__call_api(resource_path, method,
                                    path_params, query_params, header_params,
                                    body, post_params, files,
-                                   response_type, auth_settings,
+                                   response_type, auth_requested,
                                    _return_http_data_only, collection_formats,
                                    _preload_content, _request_timeout)
         else:
             thread = self.pool.apply_async(self.__call_api, (resource_path,
                                            method, path_params, query_params,
                                            header_params, body,
                                            post_params, files,
-                                           response_type, auth_settings,
+                                           response_type, auth_requested,
                                            _return_http_data_only,
                                            collection_formats,
                                            _preload_content, _request_timeout))
         return thread
 
     def request(self, method, url, query_params=None, headers=None,
                 post_params=None, body=None, _preload_content=True,
@@ -543,25 +546,25 @@
         content_types = [x.lower() for x in content_types]
 
         if 'application/json' in content_types or '*/*' in content_types:
             return 'application/json'
         else:
             return content_types[0]
 
-    def update_params_for_auth(self, headers, post_params, querys, auth_settings):
-        """Updates header and query params based on authentication setting.
+    """Updates header and query params based on authentication setting.
 
-        :param headers: Header parameters dict to be updated.
-        :param querys: Query parameters tuple list to be updated.
-        :param auth_settings: Authentication setting identifiers list.
-        """
-        if not auth_settings:
+    :param headers: Header parameters dict to be updated.
+    :param querys: Query parameters tuple list to be updated.
+    """
+    def update_params_for_auth(self, headers, post_params, querys):
+
+        if not self.configuration.auths:
             return
 
-        for auth in auth_settings:
+        for auth in self.configuration.auths:
             auth_setting = self.configuration.auth_settings(auth, post_params)
             if auth_setting:
                 if not auth_setting['value']:
                     continue
                 elif auth_setting['in'] == 'header':
                     headers[auth_setting['key']] = auth_setting['value']
                 elif auth_setting['in'] == 'query':
@@ -667,32 +670,32 @@
         """Deserializes list or dict to model.
 
         :param data: dict, list.
         :param klass: class literal.
         :return: model object.
         """
 
-        if not klass.swagger_types and not self.__hasattr(klass, 'get_real_child_model'):
+        if not klass.attribute_types and not self.__hasattr(klass, 'get_real_child_model'):
             return data
 
         kwargs = {}
-        if klass.swagger_types is not None:
-            for attr, attr_type in six.iteritems(klass.swagger_types):
+        if klass.attribute_types is not None:
+            for attr, attr_type in six.iteritems(klass.attribute_types):
                 if (data is not None and
                         klass.attribute_map[attr] in data and
                         isinstance(data, (list, dict))):
                     value = data[klass.attribute_map[attr]]
                     kwargs[attr] = self.__deserialize(value, attr_type)
 
         instance = klass(**kwargs)
 
         if (isinstance(instance, dict) and
-                klass.swagger_types is not None and
+                klass.attribute_types is not None and
                 isinstance(data, dict)):
             for key, value in data.items():
-                if key not in klass.swagger_types:
+                if key not in klass.attribute_types:
                     instance[key] = value
         if self.__hasattr(instance, 'get_real_child_model'):
             klass_name = instance.get_real_child_model(data)
             if klass_name:
                 instance = self.__deserialize(data, klass_name)
         return instance
```

### Comparing `algocash-sdk-1.1.1/algocash_sdk/configuration.py` & `algocash-sdk-1.2.0/algocash_sdk/configuration.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
     Algocash API
 
     This is a Algocash API  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     Contact: loganph.work@gmail.com
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
+    
 """
 
 from __future__ import absolute_import
 
 import copy
 import logging
 import multiprocessing
@@ -36,15 +36,15 @@
         return copy.copy(cls._default)
 
     def set_default(cls, default):
         cls._default = copy.copy(default)
 
 
 class Configuration(six.with_metaclass(TypeWithDefault, object)):
-    """NOTE: This class is auto generated by the swagger code generator program.
+    """.
 
     Ref: https://github.com/swagger-api/swagger-codegen
     Do not edit the class manually.
     """
 
     def __init__(self):
         """Constructor"""
@@ -57,14 +57,25 @@
         # Authentication Settings
         # generate signature
         self.api_access_token = ""
         # merchant_key for HTTP basic authentication
         self.merchant_key = ""
         # merchant_secret for HTTP basic authentication
         self.merchant_secret = ""
+        
+        self.header_params = {}
+        # HTTP header `Accept`
+        self.header_params['Accept'] = 'application/json'
+
+        # HTTP header `Content-Type`
+        self.header_params['Content-Type'] = 'application/json'
+
+        # Authentication setting
+        self.auths = ['basicAuth', 'signatureAuth']  # noqa: E501
+        
         # Logging Settings
         self.logger = {}
         self.logger["package_logger"] = logging.getLogger("algocash_sdk")
         self.logger["urllib3_logger"] = logging.getLogger("urllib3")
         # Log format
         self.logger_format = '%(asctime)s %(levelname)s %(message)s'
         # Log stream handler
@@ -198,22 +209,31 @@
         self.logger_formatter = logging.Formatter(self.__logger_format)
 
     def get_basic_auth_token(self):
         """Gets HTTP basic authentication header (string).
 
         :return: The token for basic HTTP authentication.
         """
+        if self.merchant_key == '' or self.merchant_secret == '':
+            raise ValueError("Missing the required merchant_key and merchant_secret")
+        
         return urllib3.util.make_headers(
             basic_auth=self.merchant_key + ':' + self.merchant_secret
         ).get('authorization')
     
     def generateSignature(self, post_params):
         
+        if self.api_access_token == '':
+            raise ValueError("Missing the required api_access_token")
+        
         signature = hmac.new(self.api_access_token.encode('utf-8'), json.dumps(post_params, separators=(',', ':')).encode('utf-8'), hashlib.sha256).hexdigest()
         return signature
+    
+    def get_host(self):
+        return "https://testapi2.algorithmic.cash" if self.devmode else self.host
 
     def auth_settings(self, auth, post_params):
         """Gets Auth Settings dict for api client.
 
         :return: The Auth Settings information dict.
         """
```

### Comparing `algocash-sdk-1.1.1/algocash_sdk/models/address.py` & `algocash-sdk-1.2.0/algocash_sdk/models/address.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,36 +3,36 @@
 """
     Algocash API
 
     This is a Algocash API  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     Contact: loganph.work@gmail.com
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
+    
 """
 
 import pprint
 import re  # noqa: F401
 import json
 
 import six
 
 class Address(object):
-    """NOTE: This class is auto generated by the swagger code generator program.
+    """.
 
     Do not edit the class manually.
     """
     """
     Attributes:
-      swagger_types (dict): The key is attribute name
+      attribute_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
-    swagger_types = {
+    attribute_types = {
         'street': 'str',
         'city': 'str',
         'state': 'str',
         'zip_code': 'str'
     }
 
     attribute_map = {
@@ -142,15 +142,15 @@
 
         self._zip_code = zip_code
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
-        for attr, _ in six.iteritems(self.swagger_types):
+        for attr, _ in six.iteritems(self.attribute_types):
             value = getattr(self, attr)
             if isinstance(value, list):
                 result[attr] = list(map(
                     lambda x: x.to_dict() if hasattr(x, "to_dict") else x,
                     value
                 ))
             elif hasattr(value, "to_dict"):
```

### Comparing `algocash-sdk-1.1.1/algocash_sdk/models/bank.py` & `algocash-sdk-1.2.0/algocash_sdk/models/bank.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,36 +3,36 @@
 """
     Algocash API
 
     This is a Algocash API  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     Contact: loganph.work@gmail.com
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
+    
 """
 
 import pprint
 import re  # noqa: F401
 import json
 
 import six
 
 class Bank(object):
-    """NOTE: This class is auto generated by the swagger code generator program.
+    """.
 
     Do not edit the class manually.
     """
     """
     Attributes:
-      swagger_types (dict): The key is attribute name
+      attribute_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
-    swagger_types = {
+    attribute_types = {
         'bank_account_number': 'str',
         'bank_code': 'str',
         'bank_beneficiary': 'str',
         'bank_branch': 'str',
         'bank_account_type': 'str'
     }
 
@@ -171,15 +171,15 @@
 
         self._bank_account_type = bank_account_type
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
-        for attr, _ in six.iteritems(self.swagger_types):
+        for attr, _ in six.iteritems(self.attribute_types):
             value = getattr(self, attr)
             if isinstance(value, list):
                 result[attr] = list(map(
                     lambda x: x.to_dict() if hasattr(x, "to_dict") else x,
                     value
                 ))
             elif hasattr(value, "to_dict"):
```

### Comparing `algocash-sdk-1.1.1/algocash_sdk/models/callback_payload.py` & `algocash-sdk-1.2.0/algocash_sdk/models/callback_payload.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,35 +3,35 @@
 """
     Algocash API
 
     This is a Algocash API  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     Contact: loganph.work@gmail.com
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
+    
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 class CallbackPayload(object):
-    """NOTE: This class is auto generated by the swagger code generator program.
+    """.
 
     Do not edit the class manually.
     """
     """
     Attributes:
-      swagger_types (dict): The key is attribute name
+      attribute_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
-    swagger_types = {
+    attribute_types = {
         'status': 'str',
         'transaction_id': 'str',
         'merchant_invoice_id': 'str',
         'amount': 'str',
         'currency': 'str',
         'fee_amount': 'str',
         'fee_currency': 'str'
@@ -233,15 +233,15 @@
 
         self._fee_currency = fee_currency
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
-        for attr, _ in six.iteritems(self.swagger_types):
+        for attr, _ in six.iteritems(self.attribute_types):
             value = getattr(self, attr)
             if isinstance(value, list):
                 result[attr] = list(map(
                     lambda x: x.to_dict() if hasattr(x, "to_dict") else x,
                     value
                 ))
             elif hasattr(value, "to_dict"):
```

### Comparing `algocash-sdk-1.1.1/algocash_sdk/models/deposit_request.py` & `algocash-sdk-1.2.0/algocash_sdk/models/deposit_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,35 +3,35 @@
 """
     Algocash API
 
     This is a Algocash API  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     Contact: loganph.work@gmail.com
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
+    
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 class DepositRequest(object):
-    """NOTE: This class is auto generated by the swagger code generator program.
+    """.
 
     Do not edit the class manually.
     """
     """
     Attributes:
-      swagger_types (dict): The key is attribute name
+      attribute_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
-    swagger_types = {
+    attribute_types = {
         'invoice_id': 'str',
         'amount': 'str',
         'payer': 'Payer',
         'payment_method': 'str',
         'url': 'Url'
     }
 
@@ -172,15 +172,15 @@
 
         self._url = url
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
-        for attr, _ in six.iteritems(self.swagger_types):
+        for attr, _ in six.iteritems(self.attribute_types):
             value = getattr(self, attr)
             if isinstance(value, list):
                 result[attr] = list(map(
                     lambda x: x.to_dict() if hasattr(x, "to_dict") else x,
                     value
                 ))
             elif hasattr(value, "to_dict"):
```

### Comparing `algocash-sdk-1.1.1/algocash_sdk/models/deposit_success.py` & `algocash-sdk-1.2.0/algocash_sdk/models/deposit_success.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,35 +3,35 @@
 """
     Algocash API
 
     This is a Algocash API  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     Contact: loganph.work@gmail.com
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
+    
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 class DepositSuccess(object):
-    """NOTE: This class is auto generated by the swagger code generator program.
+    """.
 
     Do not edit the class manually.
     """
     """
     Attributes:
-      swagger_types (dict): The key is attribute name
+      attribute_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
-    swagger_types = {
+    attribute_types = {
         'redirect_url': 'str',
         'merchant_invoice_id': 'str',
         'transaction_id': 'str'
     }
 
     attribute_map = {
         'redirect_url': 'redirect_url',
@@ -115,15 +115,15 @@
 
         self._transaction_id = transaction_id
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
-        for attr, _ in six.iteritems(self.swagger_types):
+        for attr, _ in six.iteritems(self.attribute_types):
             value = getattr(self, attr)
             if isinstance(value, list):
                 result[attr] = list(map(
                     lambda x: x.to_dict() if hasattr(x, "to_dict") else x,
                     value
                 ))
             elif hasattr(value, "to_dict"):
```

### Comparing `algocash-sdk-1.1.1/algocash_sdk/models/error.py` & `algocash-sdk-1.2.0/algocash_sdk/models/error.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,35 +3,35 @@
 """
     Algocash API
 
     This is a Algocash API  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     Contact: loganph.work@gmail.com
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
+    
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 class Error(object):
-    """NOTE: This class is auto generated by the swagger code generator program.
+    """.
 
     Do not edit the class manually.
     """
     """
     Attributes:
-      swagger_types (dict): The key is attribute name
+      attribute_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
-    swagger_types = {
+    attribute_types = {
         'code': 'str',
         'description': 'str',
         'type': 'str'
     }
 
     attribute_map = {
         'code': 'code',
@@ -115,15 +115,15 @@
 
         self._type = type
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
-        for attr, _ in six.iteritems(self.swagger_types):
+        for attr, _ in six.iteritems(self.attribute_types):
             value = getattr(self, attr)
             if isinstance(value, list):
                 result[attr] = list(map(
                     lambda x: x.to_dict() if hasattr(x, "to_dict") else x,
                     value
                 ))
             elif hasattr(value, "to_dict"):
```

### Comparing `algocash-sdk-1.1.1/algocash_sdk/models/payer.py` & `algocash-sdk-1.2.0/algocash_sdk/models/payer.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,36 +3,36 @@
 """
     Algocash API
 
     This is a Algocash API  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     Contact: loganph.work@gmail.com
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
+    
 """
 
 import pprint
 import re  # noqa: F401
 import json
 
 import six
 
 class Payer(object):
-    """NOTE: This class is auto generated by the swagger code generator program.
+    """.
 
     Do not edit the class manually.
     """
     """
     Attributes:
-      swagger_types (dict): The key is attribute name
+      attribute_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
-    swagger_types = {
+    attribute_types = {
         'email': 'str',
         'phone': 'str',
         'id': 'str',
         'document': 'str',
         'first_name': 'str',
         'last_name': 'str',
         'address': 'Address'
@@ -224,15 +224,15 @@
 
         self._address = address
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
-        for attr, _ in six.iteritems(self.swagger_types):
+        for attr, _ in six.iteritems(self.attribute_types):
             value = getattr(self, attr)
             if isinstance(value, list):
                 result[attr] = list(map(
                     lambda x: x.to_dict() if hasattr(x, "to_dict") else x,
                     value
                 ))
             elif hasattr(value, "to_dict"):
```

### Comparing `algocash-sdk-1.1.1/algocash_sdk/models/payout_request.py` & `algocash-sdk-1.2.0/algocash_sdk/models/payout_request.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,35 +3,35 @@
 """
     Algocash API
 
     This is a Algocash API  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     Contact: loganph.work@gmail.com
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
+    
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 class PayoutRequest(object):
-    """NOTE: This class is auto generated by the swagger code generator program.
+    """.
 
     Do not edit the class manually.
     """
     """
     Attributes:
-      swagger_types (dict): The key is attribute name
+      attribute_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
-    swagger_types = {
+    attribute_types = {
         'invoice_id': 'str',
         'amount': 'str',
         'payer': 'Payer',
         'payment_method': 'str',
         'bank_account': 'Bank',
         'url': 'Url'
     }
@@ -198,15 +198,15 @@
 
         self._url = url
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
-        for attr, _ in six.iteritems(self.swagger_types):
+        for attr, _ in six.iteritems(self.attribute_types):
             value = getattr(self, attr)
             if isinstance(value, list):
                 result[attr] = list(map(
                     lambda x: x.to_dict() if hasattr(x, "to_dict") else x,
                     value
                 ))
             elif hasattr(value, "to_dict"):
```

### Comparing `algocash-sdk-1.1.1/algocash_sdk/models/payout_success.py` & `algocash-sdk-1.2.0/algocash_sdk/models/payout_success.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,35 +3,35 @@
 """
     Algocash API
 
     This is a Algocash API  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     Contact: loganph.work@gmail.com
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
+    
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 class PayoutSuccess(object):
-    """NOTE: This class is auto generated by the swagger code generator program.
+    """.
 
     Do not edit the class manually.
     """
     """
     Attributes:
-      swagger_types (dict): The key is attribute name
+      attribute_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
-    swagger_types = {
+    attribute_types = {
         'merchant_invoice_id': 'str',
         'transaction_id': 'str'
     }
 
     attribute_map = {
         'merchant_invoice_id': 'merchant_invoice_id',
         'transaction_id': 'transaction_id'
@@ -89,15 +89,15 @@
 
         self._transaction_id = transaction_id
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
-        for attr, _ in six.iteritems(self.swagger_types):
+        for attr, _ in six.iteritems(self.attribute_types):
             value = getattr(self, attr)
             if isinstance(value, list):
                 result[attr] = list(map(
                     lambda x: x.to_dict() if hasattr(x, "to_dict") else x,
                     value
                 ))
             elif hasattr(value, "to_dict"):
```

### Comparing `algocash-sdk-1.1.1/algocash_sdk/models/url.py` & `algocash-sdk-1.2.0/algocash_sdk/models/url.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,36 +3,36 @@
 """
     Algocash API
 
     This is a Algocash API  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     Contact: loganph.work@gmail.com
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
+    
 """
 
 import pprint
 import re  # noqa: F401
 import json
 
 import six
 
 class Url(object):
-    """NOTE: This class is auto generated by the swagger code generator program.
+    """.
 
     Do not edit the class manually.
     """
     """
     Attributes:
-      swagger_types (dict): The key is attribute name
+      attribute_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
-    swagger_types = {
+    attribute_types = {
         'callback_url': 'str',
         'pending_url': 'str',
         'success_url': 'str',
         'error_url': 'str',
         'back_url': 'str'
     }
 
@@ -171,15 +171,15 @@
 
         self._back_url = back_url
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
-        for attr, _ in six.iteritems(self.swagger_types):
+        for attr, _ in six.iteritems(self.attribute_types):
             value = getattr(self, attr)
             if isinstance(value, list):
                 result[attr] = list(map(
                     lambda x: x.to_dict() if hasattr(x, "to_dict") else x,
                     value
                 ))
             elif hasattr(value, "to_dict"):
```

### Comparing `algocash-sdk-1.1.1/algocash_sdk/rest.py` & `algocash-sdk-1.2.0/algocash_sdk/rest.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
     Algocash API
 
     This is a Algocash API  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     Contact: loganph.work@gmail.com
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
+    
 """
 
 from __future__ import absolute_import
 
 import io
 import json
 import logging
@@ -38,15 +38,15 @@
         self.urllib3_response = resp
         self.status = resp.status
         self.reason = resp.reason
         self.data = resp.data
 
     def getheaders(self):
         """Returns a dictionary of the response headers."""
-        return self.urllib3_response.getheaders()
+        return self.urllib3_response.headers
 
     def getheader(self, name, default=None):
         """Returns a given response header."""
         return self.urllib3_response.getheader(name, default)
 
 
 class RESTClientObject(object):
```

### Comparing `algocash-sdk-1.1.1/algocash_sdk.egg-info/SOURCES.txt` & `algocash-sdk-1.2.0/algocash_sdk.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -13,27 +13,33 @@
 algocash_sdk/api/deposit_api.py
 algocash_sdk/api/payout_api.py
 algocash_sdk/models/__init__.py
 algocash_sdk/models/address.py
 algocash_sdk/models/bank.py
 algocash_sdk/models/callback_payload.py
 algocash_sdk/models/deposit_request.py
+algocash_sdk/models/deposit_status_info.py
+algocash_sdk/models/deposit_status_response.py
 algocash_sdk/models/deposit_success.py
 algocash_sdk/models/error.py
 algocash_sdk/models/payer.py
 algocash_sdk/models/payout_request.py
+algocash_sdk/models/payout_status_info.py
+algocash_sdk/models/payout_status_response.py
 algocash_sdk/models/payout_success.py
 algocash_sdk/models/url.py
 test/__init__.py
 test/server.py
 test/test_address.py
 test/test_bank.py
 test/test_callback_payload.py
 test/test_deposit_api.py
 test/test_deposit_request.py
+test/test_deposit_status_api.py
 test/test_deposit_success.py
 test/test_error.py
 test/test_payer.py
 test/test_payout_api.py
 test/test_payout_request.py
+test/test_payout_status_api.py
 test/test_payout_success.py
 test/test_url.py
```

### Comparing `algocash-sdk-1.1.1/setup.py` & `algocash-sdk-1.2.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     OpenAPI spec version: 1.0.0
     Contact: loganph.work@gmail.com
 """
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "algocash-sdk"
-VERSION = "1.1.1"
+VERSION = "1.2.0"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `algocash-sdk-1.1.1/test/server.py` & `algocash-sdk-1.2.0/test/server.py`

 * *Files identical despite different names*

### Comparing `algocash-sdk-1.1.1/test/test_address.py` & `algocash-sdk-1.2.0/test/test_address.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
     Algocash API
 
     This is a Algocash API  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     Contact: loganph.work@gmail.com
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
+    
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import algocash_sdk
```

### Comparing `algocash-sdk-1.1.1/test/test_bank.py` & `algocash-sdk-1.2.0/test/test_error.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,37 +3,37 @@
 """
     Algocash API
 
     This is a Algocash API  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     Contact: loganph.work@gmail.com
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
+    
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import algocash_sdk
-from algocash_sdk.models.bank import Bank  # noqa: E501
+from algocash_sdk.models.error import Error  # noqa: E501
 from algocash_sdk.rest import ApiException
 
 
-class TestBank(unittest.TestCase):
-    """Bank unit test stubs"""
+class TestError(unittest.TestCase):
+    """Error unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testBank(self):
-        """Test Bank"""
+    def testError(self):
+        """Test Error"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = algocash_sdk.models.bank.Bank()  # noqa: E501
+        # model = algocash_sdk.models.error.Error()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `algocash-sdk-1.1.1/test/test_callback_payload.py` & `algocash-sdk-1.2.0/test/test_callback_payload.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
     Algocash API
 
     This is a Algocash API  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     Contact: loganph.work@gmail.com
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
+    
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import algocash_sdk
```

### Comparing `algocash-sdk-1.1.1/test/test_deposit_api.py` & `algocash-sdk-1.2.0/test/test_deposit_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
     Algocash API
 
     This is a Algocash API  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     Contact: loganph.work@gmail.com
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
+    
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import algocash_sdk
@@ -35,34 +35,36 @@
     def test_create_deposit(self):
         """Test case for create_deposit
 
         create a deposit  # noqa: E501
         """
 
         configuration = Configuration()
-        configuration.host = 'https://dd1e-5-31-3-154.ngrok-free.app'
+        # configuration.host = 'https://dd1e-5-31-3-154.ngrok-free.app'
         configuration.merchant_key = 'sWBYGvzA61ITU4Vh'
         configuration.merchant_secret = 'OfeR3xi59rLAM9c1'
         configuration.api_access_token = '4q4epHrbUHykQwnc'
         configuration.devmode = True
 
         client = ApiClient(configuration)
 
         # create an instance of the API class
         api_instance = DepositApi(client)
-        invoice_id = '1000000001' # str | 
-        amount = '20' # str | 
+        invoice_id = '46560389502' # str | 
+        amount = '100' # str | 
         payer = algocash_sdk.Payer('test@gmail.com', '+918885916123') # Payer 
         payment_method = 'UPI' # str | 
         url = algocash_sdk.Url('https://localhost:8080/callback', 'https://localhost:8080/pending', 'https://localhost:8080/success', 'https://localhost:8080/error') # Url | 
 
         try:
             # create a deposit
-            api_response = api_instance.create_deposit(invoice_id, amount, payer, payment_method, url)
+            api_response = api_instance.create_deposit(invoice_id, amount, payer, url, payment_method)
             pprint(api_response)
+        except ValueError as e:
+            print("ValueError Exception when calling DepositApi->create_deposit: %s\n" % e)
         except ApiException as e:
             print("Exception when calling DepositApi->create_deposit: %s\n" % e)
             pprint(json.loads(e.body))
         pass
 
 
 if __name__ == '__main__':
```

### Comparing `algocash-sdk-1.1.1/test/test_deposit_success.py` & `algocash-sdk-1.2.0/test/test_deposit_success.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
     Algocash API
 
     This is a Algocash API  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     Contact: loganph.work@gmail.com
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
+    
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import algocash_sdk
```

### Comparing `algocash-sdk-1.1.1/test/test_payer.py` & `algocash-sdk-1.2.0/test/test_payer.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
     Algocash API
 
     This is a Algocash API  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     Contact: loganph.work@gmail.com
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
+    
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import algocash_sdk
```

### Comparing `algocash-sdk-1.1.1/test/test_payout_api.py` & `algocash-sdk-1.2.0/test/test_payout_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
     Algocash API
 
     This is a Algocash API  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     Contact: loganph.work@gmail.com
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
+    
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import algocash_sdk
@@ -32,33 +32,35 @@
 
     def test_create_payout(self):
         """Test case for create_payout
 
         create payout  # noqa: E501
         """
         configuration = algocash_sdk.Configuration()
-        configuration.host = 'https://dd1e-5-31-3-154.ngrok-free.app'
+        # configuration.host = 'https://dd1e-5-31-3-154.ngrok-free.app'
         configuration.merchant_key = 'sWBYGvzA61ITU4Vh'
         configuration.merchant_secret = 'OfeR3xi59rLAM9c1'
         configuration.api_access_token = '4q4epHrbUHykQwnc'
         configuration.devmode = True
 
         # create an instance of the API class
         api_instance = algocash_sdk.PayoutApi(algocash_sdk.ApiClient(configuration))
-        invoice_id = '1000038351' # str | 
+        invoice_id = '100003438351' # str | 
         amount = '100' # str | 
         payer = algocash_sdk.Payer('test@gmail.com', '+918885916123') # Payer 
         payment_method = 'UPI' # str | 
         bank_account = algocash_sdk.Bank('712442638', '84932568207', 'first name last name') # Bank | 
         url = algocash_sdk.Url('https://localhost:8080/callback') # Url | 
 
         try:
             # create payout
-            api_response = api_instance.create_payout(invoice_id, amount, payer, payment_method, bank_account, url)
+            api_response = api_instance.create_payout(invoice_id, amount, payer, bank_account, url, payment_method)
             pprint(api_response)
+        except ValueError as e:
+            print("ValueError Exception when calling PayoutApi->create_payout: %s\n" % e)
         except ApiException as e:
             print("Exception when calling PayoutApi->create_payout: %s\n" % e)
             pprint(json.loads(e.body))
         pass
 
 
 if __name__ == '__main__':
```

### Comparing `algocash-sdk-1.1.1/test/test_payout_request.py` & `algocash-sdk-1.2.0/test/test_payout_request.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
     Algocash API
 
     This is a Algocash API  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     Contact: loganph.work@gmail.com
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
+    
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import algocash_sdk
```

### Comparing `algocash-sdk-1.1.1/test/test_payout_success.py` & `algocash-sdk-1.2.0/test/test_payout_success.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
     Algocash API
 
     This is a Algocash API  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     Contact: loganph.work@gmail.com
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
+    
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import algocash_sdk
```

### Comparing `algocash-sdk-1.1.1/test/test_url.py` & `algocash-sdk-1.2.0/test/test_url.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
     Algocash API
 
     This is a Algocash API  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     Contact: loganph.work@gmail.com
-    Generated by: https://github.com/swagger-api/swagger-codegen.git
+    
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import algocash_sdk
```

