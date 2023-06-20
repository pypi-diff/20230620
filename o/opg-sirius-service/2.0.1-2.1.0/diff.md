# Comparing `tmp/opg_sirius_service-2.0.1.tar.gz` & `tmp/opg_sirius_service-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/opg_sirius_service-2.0.1.tar", last modified: Fri Feb 25 15:32:57 2022, max compression
+gzip compressed data, was "opg_sirius_service-2.1.0.tar", last modified: Tue Jun 20 16:57:26 2023, max compression
```

## Comparing `opg_sirius_service-2.0.1.tar` & `opg_sirius_service-2.1.0.tar`

### file list

```diff
@@ -1,14 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 15:32:57.000000 opg_sirius_service-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1074 2022-02-25 15:29:42.000000 opg_sirius_service-2.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      550 2022-02-25 15:32:57.000000 opg_sirius_service-2.0.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 15:32:57.000000 opg_sirius_service-2.0.1/opg_sirius_service/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-25 15:29:42.000000 opg_sirius_service-2.0.1/opg_sirius_service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9405 2022-02-25 15:29:42.000000 opg_sirius_service-2.0.1/opg_sirius_service/sirius_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 15:32:57.000000 opg_sirius_service-2.0.1/opg_sirius_service.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      550 2022-02-25 15:32:57.000000 opg_sirius_service-2.0.1/opg_sirius_service.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      293 2022-02-25 15:32:57.000000 opg_sirius_service-2.0.1/opg_sirius_service.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-25 15:32:57.000000 opg_sirius_service-2.0.1/opg_sirius_service.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       44 2022-02-25 15:32:57.000000 opg_sirius_service-2.0.1/opg_sirius_service.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-02-25 15:32:57.000000 opg_sirius_service-2.0.1/opg_sirius_service.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-25 15:32:57.000000 opg_sirius_service-2.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      813 2022-02-25 15:29:42.000000 opg_sirius_service-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:57:26.168427 opg_sirius_service-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-20 16:54:13.000000 opg_sirius_service-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-20 16:57:26.168427 opg_sirius_service-2.1.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:57:26.164427 opg_sirius_service-2.1.0/opg_sirius_service/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 16:54:13.000000 opg_sirius_service-2.1.0/opg_sirius_service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9718 2023-06-20 16:54:13.000000 opg_sirius_service-2.1.0/opg_sirius_service/sirius_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:57:26.168427 opg_sirius_service-2.1.0/opg_sirius_service.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-20 16:57:26.000000 opg_sirius_service-2.1.0/opg_sirius_service.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-06-20 16:57:26.000000 opg_sirius_service-2.1.0/opg_sirius_service.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 16:57:26.000000 opg_sirius_service-2.1.0/opg_sirius_service.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-20 16:57:26.000000 opg_sirius_service-2.1.0/opg_sirius_service.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-20 16:57:26.000000 opg_sirius_service-2.1.0/opg_sirius_service.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 16:57:26.168427 opg_sirius_service-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-20 16:54:13.000000 opg_sirius_service-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:57:26.168427 opg_sirius_service-2.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-06-20 16:54:13.000000 opg_sirius_service-2.1.0/tests/test_build_sirius_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-20 16:54:13.000000 opg_sirius_service-2.1.0/tests/test_build_sirius_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-20 16:54:13.000000 opg_sirius_service-2.1.0/tests/test_cache_available.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-06-20 16:54:13.000000 opg_sirius_service-2.1.0/tests/test_constructor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-06-20 16:54:13.000000 opg_sirius_service-2.1.0/tests/test_get_data_from_sirius.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-20 16:54:13.000000 opg_sirius_service-2.1.0/tests/test_get_secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-06-20 16:54:13.000000 opg_sirius_service-2.1.0/tests/test_get_sirius_data_from_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-20 16:54:13.000000 opg_sirius_service-2.1.0/tests/test_handle_sirius_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-06-20 16:54:13.000000 opg_sirius_service-2.1.0/tests/test_put_sirius_data_in_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7757 2023-06-20 16:54:13.000000 opg_sirius_service-2.1.0/tests/test_send_request_to_sirius.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-06-20 16:54:13.000000 opg_sirius_service-2.1.0/tests/test_sirius_available.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `opg_sirius_service-2.0.1/LICENSE` & `opg_sirius_service-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `opg_sirius_service-2.0.1/PKG-INFO` & `opg_sirius_service-2.1.0/opg_sirius_service.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 Metadata-Version: 2.1
-Name: opg_sirius_service
-Version: 2.0.1
+Name: opg-sirius-service
+Version: 2.1.0
 Summary: Sirius Service
 Home-page: https://github.com/ministryofjustice/opg-data
 Author: OPG
 Author-email: opg-integrations@digital.justice.gov.uk
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Sirius Service
 
 This is some information about the Sirius Service.
 
 
 
-
-
```

### Comparing `opg_sirius_service-2.0.1/opg_sirius_service/sirius_handler.py` & `opg_sirius_service-2.1.0/opg_sirius_service/sirius_handler.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,27 +4,24 @@
 
 import boto3
 import jwt
 import localstack_client.session
 import requests
 from botocore.exceptions import ClientError
 
-# from ..api.helpers import custom_logger
-
-# logger = custom_logger("opg_sirius_service")
 import logging
 
 logger = logging
 
 
 class SiriusService:
     def __init__(self, config_params, cache):
-
         try:
             self.cache = cache
+            self.use_cache = False
             self.sirius_base_url = config_params.SIRIUS_BASE_URL
             self.environment = config_params.ENVIRONMENT
             self.session_data = config_params.SESSION_DATA
             self.request_timeout = config_params.REQUEST_TIMEOUT
             self.request_caching = (
                 config_params.REQUEST_CACHING if cache else "disabled"
             )
@@ -35,15 +32,15 @@
             )
             self.request_caching_ttl = (
                 config_params.REQUEST_CACHING_TTL
                 if config_params.REQUEST_CACHING_TTL
                 else 48
             )
         except Exception as e:
-            logger.info(f"Error loading config e: {e}")
+            raise Exception(f"Error loading config e: {e}")
 
     def build_sirius_url(self, endpoint, url_params=None):
         """
         Builds the url for the endpoint from variables (probably saved in env vars)
 
         Args:
             base_url: URL of the Sirius server
@@ -75,34 +72,35 @@
         Returns:
             JWT secret
         Raises:
             ClientError
         """
 
         environment = self.environment
+        print(self.environment)
         secret_name = f"{environment}/jwt-key"
+        print(secret_name)
         region_name = "eu-west-1"
 
         if environment == "local":  # pragma: no cover
-            logger.info("Using local AWS Secrets Manager")  # pragma: no cover
+            logger.debug("Using local AWS Secrets Manager")  # pragma: no cover
             current_session = localstack_client.session.Session()  # pragma: no cover
 
         else:
             current_session = boto3.session.Session()
 
         client = current_session.client(
             service_name="secretsmanager", region_name=region_name
         )
 
         try:
             get_secret_value_response = client.get_secret_value(SecretId=secret_name)
             secret = get_secret_value_response["SecretString"]
         except ClientError as e:
-            logger.info(f"Unable to get secret from Secrets Manager {e}")
-            raise e
+            raise Exception(f"Unable to get secret from Secrets Manager: {e}")
 
         return secret
 
     def _build_sirius_headers(self, content_type="application/json"):
         """
         Builds headers for Sirius request, including JWT auth
 
@@ -125,85 +123,94 @@
             },
             self._get_secret(),
             algorithm="HS256",
         )
 
         return {
             "Content-Type": content_type,
-            "Authorization": "Bearer " + encoded_jwt.decode("UTF8"),
+            "Authorization": "Bearer " + encoded_jwt,
         }
 
     def _handle_sirius_error(
         self, error_code=None, error_message=None, error_details=None
     ):
         error_code = error_code if error_code else 500
         error_message = (
-            error_message if error_message else "Unknown error talking to " "Sirius"
+            error_message if error_message else "Unknown error talking to Sirius"
         )
 
         try:
             error_details = error_details["detail"]
 
         except (KeyError, TypeError):
             error_details = (
                 str(error_details) if len(str(error_details)) > 0 else "None"
             )
 
         message = f"{error_message}, details: {str(error_details)}"
-        logger.error(message)
         return error_code, message
 
     def check_sirius_available(self):
         healthcheck_url = f"{self.sirius_base_url}/api/health-check"
         try:
-            return True if requests.get(url=healthcheck_url,timeout=self.request_timeout).status_code == 200 else False
+            return (
+                True
+                if requests.get(
+                    url=healthcheck_url, timeout=self.request_timeout
+                ).status_code
+                == 200
+                else False
+            )
         except Exception as e:
             logger.error(f"Sirius Unavailable: {e}")
             return False
 
     def check_cache_available(self):
         try:
             return self.cache.ping()
         except Exception as e:
             logger.error(f"Unable to connect to cache: {e}")
             return False
 
     def send_request_to_sirius(self, key, url, method, content_type=None, data=None):
-
         cache_enabled = True if self.request_caching == "enabled" else False
-
+        self.use_cache = False
         if self.check_sirius_available():
             sirius_status_code, sirius_data = self._get_data_from_sirius(
                 url, method, content_type, data
             )
-            logger.info(f"sirius_status_code: {sirius_status_code}")
-            logger.info(f"cache_enables: {cache_enabled}")
-            logger.info(f"method: {method}")
+            logger.debug(f"sirius_status_code: {sirius_status_code}")
+            logger.debug(f"cache_enabled: {cache_enabled}")
+            logger.debug(f"method: {method}")
             if cache_enabled and method == "GET":
                 if sirius_status_code == 200 or sirius_status_code == 410:
-                    logger.info(f"Putting data in cache with key: {key}")
-                    self._put_sirius_data_in_cache(key=key, data=sirius_data, status=sirius_status_code)
+                    logger.debug(f"Putting data in cache with key: {key}")
+                    self._put_sirius_data_in_cache(
+                        key=key, data=sirius_data, status=sirius_status_code
+                    )
 
             return sirius_status_code, sirius_data
         else:
             if cache_enabled and method == "GET":
-                logger.info(f"Getting data from cache with key: {key}")
+                self.use_cache = True
+                logger.debug(f"Getting data from cache with key: {key}")
                 sirius_status_code, sirius_data = self._get_sirius_data_from_cache(
                     key=key
                 )
 
                 return sirius_status_code, sirius_data
             else:
-                return self._handle_sirius_error(
-                    error_message=f"Unable to send request to Sirius",
-                    error_details=f"Sirius not available",
+                sirius_status_code, sirius_data = self._handle_sirius_error(
+                    error_message="Unable to send request to Sirius",
+                    error_details="Sirius not available - cache not enabled or incorrect method for cache",
                 )
+                return sirius_status_code, sirius_data
 
     def _get_data_from_sirius(self, url, method, content_type=None, data=None):
-        logger.info("_get_data_from_sirius")
+        logger.debug("_get_data_from_sirius")
         headers = self._build_sirius_headers(content_type)
 
         try:
             if method == "PUT":
                 r = requests.put(url=url, data=data, headers=headers)
                 return r.status_code, r.json()
 
@@ -211,62 +218,60 @@
                 r = requests.post(url=url, data=data, headers=headers)
                 if r.status_code == 204:
                     return r.status_code, ""
 
                 return r.status_code, r.json()
             elif method == "GET":
                 r = requests.get(url=url, headers=headers, timeout=self.request_timeout)
-
                 return r.status_code, r.json()
             else:
                 return self._handle_sirius_error(
-                    error_message=f"Unable to send request to Sirius",
+                    error_message="Unable to send request to Sirius",
                     error_details=f"Method {method} not allowed on Sirius route",
                 )
 
         except Exception as e:
             return self._handle_sirius_error(
-                error_message=f"Unable to send request to Sirius", error_details=e
+                error_message="Unable to send request to Sirius", error_details=e
             )
 
     def _put_sirius_data_in_cache(self, key, data, status):
-        logger.info(f"_put_sirius_data_in_cache")
+        logger.debug("_put_sirius_data_in_cache")
         cache_name = self.request_caching_name
         cache_ref = f"{cache_name}-{key}"
 
         cache_ttl_in_seconds = self.request_caching_ttl * 60 * 60
 
         data = json.dumps(data)
 
         try:
             self.cache.set(
                 name=f"{cache_ref}-{status}", value=data, ex=cache_ttl_in_seconds
             )
-            logger.info(f"setting redis: {cache_ref}-{status}")
+            logger.debug(f"setting redis: {cache_ref}-{status}")
         except Exception as e:
             logger.error(f"Unable to set cache: {cache_ref}-{status}, error {e}")
 
     def _get_sirius_data_from_cache(self, key):
-
         cache_name = self.request_caching_name
         cache_ref = f"{cache_name}-{key}"
 
         try:
             if self.cache.exists(f"{cache_ref}-200"):
-                logger.info(f"found redis cache: {cache_ref}-200")
+                logger.debug(f"found redis cache: {cache_ref}-200")
                 status_code = 200
                 result = self.cache.get(f"{cache_ref}-200")
                 result = json.loads(result)
             elif self.cache.exists(f"{cache_ref}-410"):
-                logger.info(f"found redis cache: {cache_ref}-410")
+                logger.debug(f"found redis cache: {cache_ref}-410")
                 status_code = 410
                 result = self.cache.get(f"{cache_ref}-410")
                 result = json.loads(result)
             else:
-                logger.info(f"no-cache exists for: {cache_ref}-[200, 410]")
+                logger.debug(f"no-cache exists for: {cache_ref}-[200, 410]")
                 status_code = 500
                 result = None
         except Exception as e:
             logger.error(f"Unable to get from cache: {cache_ref}, error {e}")
             status_code = 500
             result = None
```

