# Comparing `tmp/sagemaker_inference-1.9.2.tar.gz` & `tmp/sagemaker_inference-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sagemaker_inference-1.9.2.tar", last modified: Tue Apr  4 09:19:56 2023, max compression
+gzip compressed data, was "dist/sagemaker_inference-1.9.3.tar", last modified: Tue Jun 20 09:18:41 2023, max compression
```

## Comparing `sagemaker_inference-1.9.2.tar` & `sagemaker_inference-1.9.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 09:19:56.000000 sagemaker_inference-1.9.2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 09:19:56.000000 sagemaker_inference-1.9.2/sagemaker_inference.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11088 2023-04-04 09:19:55.000000 sagemaker_inference-1.9.2/sagemaker_inference.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      923 2023-04-04 09:19:55.000000 sagemaker_inference-1.9.2/sagemaker_inference.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-04 09:19:55.000000 sagemaker_inference-1.9.2/sagemaker_inference.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      108 2023-04-04 09:19:55.000000 sagemaker_inference-1.9.2/sagemaker_inference.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-04-04 09:19:55.000000 sagemaker_inference-1.9.2/sagemaker_inference.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 09:19:56.000000 sagemaker_inference-1.9.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 09:19:56.000000 sagemaker_inference-1.9.2/src/sagemaker_inference/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 09:19:56.000000 sagemaker_inference-1.9.2/src/sagemaker_inference/etc/
--rw-rw-r--   0 root         (0) root         (0)      162 2023-04-03 20:26:18.000000 sagemaker_inference-1.9.2/src/sagemaker_inference/etc/default-mms.properties
--rw-rw-r--   0 root         (0) root         (0)     3535 2023-04-03 20:26:18.000000 sagemaker_inference-1.9.2/src/sagemaker_inference/etc/log4j2.xml
--rw-rw-r--   0 root         (0) root         (0)      161 2023-04-03 20:26:18.000000 sagemaker_inference-1.9.2/src/sagemaker_inference/etc/mme-mms.properties
--rw-rw-r--   0 root         (0) root         (0)        0 2023-04-03 20:26:18.000000 sagemaker_inference-1.9.2/src/sagemaker_inference/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      813 2023-04-03 20:26:18.000000 sagemaker_inference-1.9.2/src/sagemaker_inference/content_types.py
--rw-rw-r--   0 root         (0) root         (0)     3365 2023-04-03 20:26:18.000000 sagemaker_inference-1.9.2/src/sagemaker_inference/decoder.py
--rw-rw-r--   0 root         (0) root         (0)     2644 2023-04-03 20:26:18.000000 sagemaker_inference-1.9.2/src/sagemaker_inference/default_handler_service.py
--rw-rw-r--   0 root         (0) root         (0)     3434 2023-04-03 20:26:18.000000 sagemaker_inference-1.9.2/src/sagemaker_inference/default_inference_handler.py
--rw-rw-r--   0 root         (0) root         (0)     3459 2023-04-03 20:26:18.000000 sagemaker_inference-1.9.2/src/sagemaker_inference/encoder.py
--rw-rw-r--   0 root         (0) root         (0)     6692 2023-04-03 20:26:18.000000 sagemaker_inference-1.9.2/src/sagemaker_inference/environment.py
--rw-rw-r--   0 root         (0) root         (0)     2863 2023-04-03 20:26:18.000000 sagemaker_inference-1.9.2/src/sagemaker_inference/errors.py
--rw-rw-r--   0 root         (0) root         (0)     1264 2023-04-03 20:26:18.000000 sagemaker_inference-1.9.2/src/sagemaker_inference/logging.py
--rw-rw-r--   0 root         (0) root         (0)     8020 2023-04-03 20:26:18.000000 sagemaker_inference-1.9.2/src/sagemaker_inference/model_server.py
--rw-rw-r--   0 root         (0) root         (0)     1457 2023-04-03 20:26:18.000000 sagemaker_inference-1.9.2/src/sagemaker_inference/parameters.py
--rw-rw-r--   0 root         (0) root         (0)    11258 2023-04-03 20:26:18.000000 sagemaker_inference-1.9.2/src/sagemaker_inference/transformer.py
--rw-rw-r--   0 root         (0) root         (0)     2774 2023-04-03 20:26:18.000000 sagemaker_inference-1.9.2/src/sagemaker_inference/utils.py
--rw-rw-r--   0 root         (0) root         (0)    10142 2023-04-03 20:26:18.000000 sagemaker_inference-1.9.2/LICENSE
--rw-rw-r--   0 root         (0) root         (0)      128 2023-04-03 20:26:18.000000 sagemaker_inference-1.9.2/MANIFEST.in
--rw-rw-r--   0 root         (0) root         (0)      101 2023-04-03 20:26:18.000000 sagemaker_inference-1.9.2/NOTICE
--rw-rw-r--   0 root         (0) root         (0)     9009 2023-04-03 20:26:18.000000 sagemaker_inference-1.9.2/README.md
--rw-rw-r--   0 root         (0) root         (0)        6 2023-04-04 09:18:24.000000 sagemaker_inference-1.9.2/VERSION
--rw-rw-r--   0 root         (0) root         (0)      108 2023-04-04 09:19:56.000000 sagemaker_inference-1.9.2/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     2333 2023-04-03 20:26:18.000000 sagemaker_inference-1.9.2/setup.py
--rw-r--r--   0 root         (0) root         (0)    11088 2023-04-04 09:19:56.000000 sagemaker_inference-1.9.2/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 09:18:41.000000 sagemaker_inference-1.9.3/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 09:18:41.000000 sagemaker_inference-1.9.3/sagemaker_inference.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11088 2023-06-20 09:18:40.000000 sagemaker_inference-1.9.3/sagemaker_inference.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      923 2023-06-20 09:18:40.000000 sagemaker_inference-1.9.3/sagemaker_inference.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 09:18:40.000000 sagemaker_inference-1.9.3/sagemaker_inference.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      108 2023-06-20 09:18:40.000000 sagemaker_inference-1.9.3/sagemaker_inference.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-06-20 09:18:40.000000 sagemaker_inference-1.9.3/sagemaker_inference.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 09:18:41.000000 sagemaker_inference-1.9.3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 09:18:41.000000 sagemaker_inference-1.9.3/src/sagemaker_inference/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 09:18:41.000000 sagemaker_inference-1.9.3/src/sagemaker_inference/etc/
+-rw-rw-r--   0 root         (0) root         (0)      162 2023-06-19 18:40:34.000000 sagemaker_inference-1.9.3/src/sagemaker_inference/etc/default-mms.properties
+-rw-rw-r--   0 root         (0) root         (0)     3535 2023-06-19 18:40:34.000000 sagemaker_inference-1.9.3/src/sagemaker_inference/etc/log4j2.xml
+-rw-rw-r--   0 root         (0) root         (0)      161 2023-06-19 18:40:34.000000 sagemaker_inference-1.9.3/src/sagemaker_inference/etc/mme-mms.properties
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-06-19 18:40:34.000000 sagemaker_inference-1.9.3/src/sagemaker_inference/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      813 2023-06-19 18:40:34.000000 sagemaker_inference-1.9.3/src/sagemaker_inference/content_types.py
+-rw-rw-r--   0 root         (0) root         (0)     3365 2023-06-19 18:40:34.000000 sagemaker_inference-1.9.3/src/sagemaker_inference/decoder.py
+-rw-rw-r--   0 root         (0) root         (0)     2644 2023-06-19 18:40:34.000000 sagemaker_inference-1.9.3/src/sagemaker_inference/default_handler_service.py
+-rw-rw-r--   0 root         (0) root         (0)     3434 2023-06-19 18:40:34.000000 sagemaker_inference-1.9.3/src/sagemaker_inference/default_inference_handler.py
+-rw-rw-r--   0 root         (0) root         (0)     3459 2023-06-19 18:40:34.000000 sagemaker_inference-1.9.3/src/sagemaker_inference/encoder.py
+-rw-rw-r--   0 root         (0) root         (0)     7248 2023-06-19 18:40:34.000000 sagemaker_inference-1.9.3/src/sagemaker_inference/environment.py
+-rw-rw-r--   0 root         (0) root         (0)     2863 2023-06-19 18:40:34.000000 sagemaker_inference-1.9.3/src/sagemaker_inference/errors.py
+-rw-rw-r--   0 root         (0) root         (0)     1264 2023-06-19 18:40:34.000000 sagemaker_inference-1.9.3/src/sagemaker_inference/logging.py
+-rw-rw-r--   0 root         (0) root         (0)     8190 2023-06-19 18:40:34.000000 sagemaker_inference-1.9.3/src/sagemaker_inference/model_server.py
+-rw-rw-r--   0 root         (0) root         (0)     1546 2023-06-19 18:40:34.000000 sagemaker_inference-1.9.3/src/sagemaker_inference/parameters.py
+-rw-rw-r--   0 root         (0) root         (0)    11258 2023-06-19 18:40:34.000000 sagemaker_inference-1.9.3/src/sagemaker_inference/transformer.py
+-rw-rw-r--   0 root         (0) root         (0)     2774 2023-06-19 18:40:34.000000 sagemaker_inference-1.9.3/src/sagemaker_inference/utils.py
+-rw-rw-r--   0 root         (0) root         (0)    10142 2023-06-19 18:40:34.000000 sagemaker_inference-1.9.3/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)      128 2023-06-19 18:40:34.000000 sagemaker_inference-1.9.3/MANIFEST.in
+-rw-rw-r--   0 root         (0) root         (0)      101 2023-06-19 18:40:34.000000 sagemaker_inference-1.9.3/NOTICE
+-rw-rw-r--   0 root         (0) root         (0)     9009 2023-06-19 18:40:34.000000 sagemaker_inference-1.9.3/README.md
+-rw-rw-r--   0 root         (0) root         (0)        6 2023-06-20 09:17:09.000000 sagemaker_inference-1.9.3/VERSION
+-rw-rw-r--   0 root         (0) root         (0)      108 2023-06-20 09:18:41.000000 sagemaker_inference-1.9.3/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     2333 2023-06-19 18:40:34.000000 sagemaker_inference-1.9.3/setup.py
+-rw-r--r--   0 root         (0) root         (0)    11088 2023-06-20 09:18:41.000000 sagemaker_inference-1.9.3/PKG-INFO
```

### Comparing `sagemaker_inference-1.9.2/sagemaker_inference.egg-info/PKG-INFO` & `sagemaker_inference-1.9.3/sagemaker_inference.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sagemaker-inference
-Version: 1.9.2
+Version: 1.9.3
 Summary: Open source toolkit for helping create serving containers to run on Amazon SageMaker.
 Home-page: https://github.com/aws/sagemaker-inference-toolkit/
 Author: Amazon Web Services
 License: Apache License 2.0
 Description: ![SageMaker](https://github.com/aws/sagemaker-inference-toolkit/raw/master/branding/icon/sagemaker-banner.png)
         
         # SageMaker Inference Toolkit
```

### Comparing `sagemaker_inference-1.9.2/sagemaker_inference.egg-info/SOURCES.txt` & `sagemaker_inference-1.9.3/sagemaker_inference.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sagemaker_inference-1.9.2/src/sagemaker_inference/etc/log4j2.xml` & `sagemaker_inference-1.9.3/src/sagemaker_inference/etc/log4j2.xml`

 * *Files identical despite different names*

### Comparing `sagemaker_inference-1.9.2/src/sagemaker_inference/content_types.py` & `sagemaker_inference-1.9.3/src/sagemaker_inference/content_types.py`

 * *Files identical despite different names*

### Comparing `sagemaker_inference-1.9.2/src/sagemaker_inference/decoder.py` & `sagemaker_inference-1.9.3/src/sagemaker_inference/decoder.py`

 * *Files identical despite different names*

### Comparing `sagemaker_inference-1.9.2/src/sagemaker_inference/default_handler_service.py` & `sagemaker_inference-1.9.3/src/sagemaker_inference/default_handler_service.py`

 * *Files identical despite different names*

### Comparing `sagemaker_inference-1.9.2/src/sagemaker_inference/default_inference_handler.py` & `sagemaker_inference-1.9.3/src/sagemaker_inference/default_inference_handler.py`

 * *Files identical despite different names*

### Comparing `sagemaker_inference-1.9.2/src/sagemaker_inference/encoder.py` & `sagemaker_inference-1.9.3/src/sagemaker_inference/encoder.py`

 * *Files identical despite different names*

### Comparing `sagemaker_inference-1.9.2/src/sagemaker_inference/environment.py` & `sagemaker_inference-1.9.3/src/sagemaker_inference/environment.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # language governing permissions and limitations under the License.
 """This module contains functionality that provides access to system
 characteristics, environment variables and configuration settings.
 """
 from __future__ import absolute_import
 
 import os
+from typing import Optional
 
 from sagemaker_inference import content_types, logging, parameters
 
 logger = logging.get_logger()
 
 DEFAULT_MODULE_NAME = "inference.py"
 DEFAULT_MODEL_SERVER_TIMEOUT = "60"
@@ -47,15 +48,17 @@
     including system characteristics, environment variables and configuration settings.
 
     The Environment is a read-only snapshot of the container environment.
     It is a dictionary-like object, allowing any builtin function that works with dictionary.
 
     Attributes:
         module_name (str): The name of the user-provided module. Default is inference.py.
-        model_server_timeout (int): Timeout in seconds for the model server. Default is 60.
+        model_server_timeout (int): Timeout for the model server. Default is 60.
+        model_server_timeout_seconds (Optional[int]): Timeout in seconds for the model server.
+            Default is None.
         model_server_workers (str): Number of worker processes the model server will use.
 
         default_accept (str): The desired default MIME type of the inference in the response
             as specified in the user-supplied SAGEMAKER_DEFAULT_INVOCATIONS_ACCEPT environment
             variable. Otherwise, returns 'application/json' by default.
             For example: application/json
         http_port (str): Port that SageMaker will use to handle invocations and pings against the
@@ -67,15 +70,21 @@
     """
 
     def __init__(self):
         self._module_name = os.environ.get(parameters.USER_PROGRAM_ENV, DEFAULT_MODULE_NAME)
         self._model_server_timeout = int(
             os.environ.get(parameters.MODEL_SERVER_TIMEOUT_ENV, DEFAULT_MODEL_SERVER_TIMEOUT)
         )
+        timeout_seconds_var = os.environ.get(parameters.MODEL_SERVER_TIMEOUT_SECONDS_ENV)
+        self._model_server_timeout_seconds = (
+            int(timeout_seconds_var) if timeout_seconds_var is not None else None
+        )
+
         self._model_server_workers = os.environ.get(parameters.MODEL_SERVER_WORKERS_ENV)
+
         self._startup_timeout = int(
             os.environ.get(parameters.STARTUP_TIMEOUT_ENV, DEFAULT_STARTUP_TIMEOUT)
         )
         self._default_accept = os.environ.get(
             parameters.DEFAULT_INVOCATIONS_ACCEPT_ENV, content_types.JSON
         )
         self._inference_http_port = os.environ.get(parameters.BIND_TO_PORT_ENV, DEFAULT_HTTP_PORT)
@@ -103,59 +112,67 @@
 
     @property
     def module_name(self):  # type: () -> str
         """str: Name of the user-provided module."""
         return self._parse_module_name(self._module_name)
 
     @property
-    def model_server_timeout(self):  # type: () -> int
+    def model_server_timeout(self) -> int:
+        """int: Timeout used for model server's backend workers before they are
+        deemed unresponsive and rebooted.
+
+        """
+        return self._model_server_timeout
+
+    @property
+    def model_server_timeout_seconds(self) -> Optional[int]:
         """int: Timeout, in seconds, used for model server's backend workers before
         they are deemed unresponsive and rebooted.
         """
-        return self._model_server_timeout
+        return self._model_server_timeout_seconds
 
     @property
-    def model_server_workers(self):  # type: () -> str
+    def model_server_workers(self) -> Optional[str]:
         """str: Number of worker processes the model server is configured to use."""
         return self._model_server_workers
 
     @property
-    def startup_timeout(self):  # type () -> int
+    def startup_timeout(self) -> int:
         """int: Timeout, in seconds, used for starting up the model server and fetching
         its process id, before giving up and throwing error.
         """
         return self._startup_timeout
 
     @property
-    def default_accept(self):  # type: () -> str
+    def default_accept(self) -> str:
         """str: The desired default MIME type of the inference in the response."""
         return self._default_accept
 
     @property
-    def inference_http_port(self):  # type: () -> str
+    def inference_http_port(self) -> str:
         """str: HTTP port that SageMaker uses to handle invocations and pings."""
         return self._inference_http_port
 
     @property
-    def management_http_port(self):  # type: () -> str
+    def management_http_port(self) -> str:
         """str: HTTP port that SageMaker uses to handle model management requests."""
         return self._management_http_port
 
     @property
-    def safe_port_range(self):  # type: () -> str
+    def safe_port_range(self) -> Optional[str]:
         """str: HTTP port range that can be used by users to avoid collisions with the HTTP port
         specified by SageMaker for handling pings and invocations.
         """
         return self._safe_port_range
 
     @property
-    def vmargs(self):  # type: () -> str
+    def vmargs(self) -> str:
         """str: vmargs can be provided for the JVM, to be overriden"""
         return self._vmargs
 
     @property
-    def max_request_size(self):  # type: () -> str
+    def max_request_size(self) -> Optional[int]:
         """str: max request size set by Sagemaker platform in bytes"""
         if self._max_request_size_in_mb is not None:
             return int(self._max_request_size_in_mb) * 1024 * 1024
         else:
             return None
```

### Comparing `sagemaker_inference-1.9.2/src/sagemaker_inference/errors.py` & `sagemaker_inference-1.9.3/src/sagemaker_inference/errors.py`

 * *Files identical despite different names*

### Comparing `sagemaker_inference-1.9.2/src/sagemaker_inference/logging.py` & `sagemaker_inference-1.9.3/src/sagemaker_inference/logging.py`

 * *Files identical despite different names*

### Comparing `sagemaker_inference-1.9.2/src/sagemaker_inference/model_server.py` & `sagemaker_inference-1.9.3/src/sagemaker_inference/model_server.py`

 * *Files 3% similar despite different names*

```diff
@@ -162,14 +162,19 @@
         "vmargs": env.vmargs,
         "max_request_size": env.max_request_size,
     }
     # If provided, add handler service to user config
     if handler_service:
         user_defined_configuration["default_service_handler"] = handler_service
 
+    if env.model_server_timeout_seconds:
+        user_defined_configuration[
+            "default_response_timeout_seconds"
+        ] = env.model_server_timeout_seconds
+
     custom_configuration = str()
 
     for key in user_defined_configuration:
         value = user_defined_configuration.get(key)
         if value:
             custom_configuration += "{}={}\n".format(key, value)
```

### Comparing `sagemaker_inference-1.9.2/src/sagemaker_inference/parameters.py` & `sagemaker_inference-1.9.3/src/sagemaker_inference/parameters.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,13 +16,14 @@
 
 BASE_PATH_ENV = "SAGEMAKER_BASE_DIR"  # type: str
 USER_PROGRAM_ENV = "SAGEMAKER_PROGRAM"  # type: str
 LOG_LEVEL_ENV = "SAGEMAKER_CONTAINER_LOG_LEVEL"  # type: str
 DEFAULT_INVOCATIONS_ACCEPT_ENV = "SAGEMAKER_DEFAULT_INVOCATIONS_ACCEPT"  # type: str
 MODEL_SERVER_WORKERS_ENV = "SAGEMAKER_MODEL_SERVER_WORKERS"  # type: str
 MODEL_SERVER_TIMEOUT_ENV = "SAGEMAKER_MODEL_SERVER_TIMEOUT"  # type: str
+MODEL_SERVER_TIMEOUT_SECONDS_ENV = "SAGEMAKER_MODEL_SERVER_TIMEOUT_SECONDS"  # type: str
 MODEL_SERVER_VMARGS = "SAGEMAKER_MODEL_SERVER_VMARGS"  # type: str
 STARTUP_TIMEOUT_ENV = "SAGEMAKER_STARTUP_TIMEOUT"  # type: str
 BIND_TO_PORT_ENV = "SAGEMAKER_BIND_TO_PORT"  # type: str
 SAFE_PORT_RANGE_ENV = "SAGEMAKER_SAFE_PORT_RANGE"  # type: str
 MULTI_MODEL_ENV = "SAGEMAKER_MULTI_MODEL"  # type: str
 MAX_REQUEST_SIZE = "SAGEMAKER_MAX_PAYLOAD_IN_MB"  # type: str
```

### Comparing `sagemaker_inference-1.9.2/src/sagemaker_inference/transformer.py` & `sagemaker_inference-1.9.3/src/sagemaker_inference/transformer.py`

 * *Files identical despite different names*

### Comparing `sagemaker_inference-1.9.2/src/sagemaker_inference/utils.py` & `sagemaker_inference-1.9.3/src/sagemaker_inference/utils.py`

 * *Files identical despite different names*

### Comparing `sagemaker_inference-1.9.2/LICENSE` & `sagemaker_inference-1.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sagemaker_inference-1.9.2/README.md` & `sagemaker_inference-1.9.3/README.md`

 * *Files identical despite different names*

### Comparing `sagemaker_inference-1.9.2/setup.py` & `sagemaker_inference-1.9.3/setup.py`

 * *Files identical despite different names*

### Comparing `sagemaker_inference-1.9.2/PKG-INFO` & `sagemaker_inference-1.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sagemaker_inference
-Version: 1.9.2
+Version: 1.9.3
 Summary: Open source toolkit for helping create serving containers to run on Amazon SageMaker.
 Home-page: https://github.com/aws/sagemaker-inference-toolkit/
 Author: Amazon Web Services
 License: Apache License 2.0
 Description: ![SageMaker](https://github.com/aws/sagemaker-inference-toolkit/raw/master/branding/icon/sagemaker-banner.png)
         
         # SageMaker Inference Toolkit
```

