# Comparing `tmp/mlserver-mlflow-1.3.4rc2.tar.gz` & `tmp/mlserver-mlflow-1.4.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlserver-mlflow-1.3.4rc2.tar", last modified: Tue Jun 20 09:09:44 2023, max compression
+gzip compressed data, was "mlserver-mlflow-1.4.0.dev2.tar", last modified: Thu May  4 09:30:52 2023, max compression
```

## Comparing `mlserver-mlflow-1.3.4rc2.tar` & `mlserver-mlflow-1.4.0.dev2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:09:44.496017 mlserver-mlflow-1.3.4rc2/
--rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-06-20 09:08:55.000000 mlserver-mlflow-1.3.4rc2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-06-20 09:09:44.496017 mlserver-mlflow-1.3.4rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-20 09:08:55.000000 mlserver-mlflow-1.3.4rc2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:09:44.492017 mlserver-mlflow-1.3.4rc2/mlserver_mlflow/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-20 09:08:55.000000 mlserver-mlflow-1.3.4rc2/mlserver_mlflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-06-20 09:08:55.000000 mlserver-mlflow-1.3.4rc2/mlserver_mlflow/codecs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-06-20 09:08:55.000000 mlserver-mlflow-1.3.4rc2/mlserver_mlflow/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     7217 2023-06-20 09:08:55.000000 mlserver-mlflow-1.3.4rc2/mlserver_mlflow/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-20 09:08:55.000000 mlserver-mlflow-1.3.4rc2/mlserver_mlflow/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:09:44.496017 mlserver-mlflow-1.3.4rc2/mlserver_mlflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-06-20 09:09:44.000000 mlserver-mlflow-1.3.4rc2/mlserver_mlflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-20 09:09:44.000000 mlserver-mlflow-1.3.4rc2/mlserver_mlflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 09:09:44.000000 mlserver-mlflow-1.3.4rc2/mlserver_mlflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-20 09:09:44.000000 mlserver-mlflow-1.3.4rc2/mlserver_mlflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-20 09:09:44.000000 mlserver-mlflow-1.3.4rc2/mlserver_mlflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 09:09:44.496017 mlserver-mlflow-1.3.4rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-20 09:08:55.000000 mlserver-mlflow-1.3.4rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:52.716329 mlserver-mlflow-1.4.0.dev2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-05-04 09:30:02.000000 mlserver-mlflow-1.4.0.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-04 09:30:52.716329 mlserver-mlflow-1.4.0.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-04 09:30:02.000000 mlserver-mlflow-1.4.0.dev2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:52.716329 mlserver-mlflow-1.4.0.dev2/mlserver_mlflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-04 09:30:02.000000 mlserver-mlflow-1.4.0.dev2/mlserver_mlflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-05-04 09:30:02.000000 mlserver-mlflow-1.4.0.dev2/mlserver_mlflow/codecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-05-04 09:30:02.000000 mlserver-mlflow-1.4.0.dev2/mlserver_mlflow/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7217 2023-05-04 09:30:02.000000 mlserver-mlflow-1.4.0.dev2/mlserver_mlflow/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-04 09:30:02.000000 mlserver-mlflow-1.4.0.dev2/mlserver_mlflow/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:52.716329 mlserver-mlflow-1.4.0.dev2/mlserver_mlflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-04 09:30:52.000000 mlserver-mlflow-1.4.0.dev2/mlserver_mlflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-04 09:30:52.000000 mlserver-mlflow-1.4.0.dev2/mlserver_mlflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 09:30:52.000000 mlserver-mlflow-1.4.0.dev2/mlserver_mlflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-04 09:30:52.000000 mlserver-mlflow-1.4.0.dev2/mlserver_mlflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-04 09:30:52.000000 mlserver-mlflow-1.4.0.dev2/mlserver_mlflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 09:30:52.716329 mlserver-mlflow-1.4.0.dev2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-04 09:30:02.000000 mlserver-mlflow-1.4.0.dev2/setup.py
```

### Comparing `mlserver-mlflow-1.3.4rc2/LICENSE` & `mlserver-mlflow-1.4.0.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `mlserver-mlflow-1.3.4rc2/PKG-INFO` & `mlserver-mlflow-1.4.0.dev2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlserver-mlflow
-Version: 1.3.4rc2
+Version: 1.4.0.dev2
 Summary: MLflow runtime for MLServer
 Home-page: https://github.com/SeldonIO/MLServer.git
 Author: Seldon Technologies Ltd.
 Author-email: hello@seldon.io
 License: Apache 2.0
 Description: # MLflow runtime for MLServer
```

### Comparing `mlserver-mlflow-1.3.4rc2/README.md` & `mlserver-mlflow-1.4.0.dev2/README.md`

 * *Files identical despite different names*

### Comparing `mlserver-mlflow-1.3.4rc2/mlserver_mlflow/codecs.py` & `mlserver-mlflow-1.4.0.dev2/mlserver_mlflow/codecs.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 
 from typing import Optional, Dict
 
-from mlserver.types import InferenceRequest, InferenceResponse, Parameters
+from mlserver.types import InferenceRequest, InferenceResponse
 from mlserver.codecs import (
     NumpyCodec,
     RequestCodec,
     register_request_codec,
     get_decoded_or_raw,
 )
 from mlserver.codecs.lists import is_list_of
@@ -42,18 +42,15 @@
     ) -> InferenceResponse:
         outputs = [
             NumpyCodec.encode_output(name, value, **kwargs)
             for name, value in payload.items()
         ]
 
         return InferenceResponse(
-            model_name=model_name,
-            model_version=model_version,
-            outputs=outputs,
-            parameters=Parameters(content_type=cls.ContentType),
+            model_name=model_name, model_version=model_version, outputs=outputs
         )
 
     @classmethod
     def decode_response(cls, response: InferenceResponse) -> TensorDict:
         return {
             response_output.name: NumpyCodec.decode_output(response_output)
             for response_output in response.outputs
@@ -62,17 +59,15 @@
     @classmethod
     def encode_request(cls, payload: TensorDict, **kwargs) -> InferenceRequest:
         inputs = [
             NumpyCodec.encode_input(name, value, **kwargs)
             for name, value in payload.items()
         ]
 
-        return InferenceRequest(
-            inputs=inputs, parameters=Parameters(content_type=cls.ContentType)
-        )
+        return InferenceRequest(inputs=inputs)
 
     @classmethod
     def decode_request(cls, request: InferenceRequest) -> TensorDict:
         return {
             request_input.name: get_decoded_or_raw(request_input)
             for request_input in request.inputs
         }
```

### Comparing `mlserver-mlflow-1.3.4rc2/mlserver_mlflow/metadata.py` & `mlserver-mlflow-1.4.0.dev2/mlserver_mlflow/metadata.py`

 * *Files identical despite different names*

### Comparing `mlserver-mlflow-1.3.4rc2/mlserver_mlflow/runtime.py` & `mlserver-mlflow-1.4.0.dev2/mlserver_mlflow/runtime.py`

 * *Files identical despite different names*

### Comparing `mlserver-mlflow-1.3.4rc2/mlserver_mlflow.egg-info/PKG-INFO` & `mlserver-mlflow-1.4.0.dev2/mlserver_mlflow.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlserver-mlflow
-Version: 1.3.4rc2
+Version: 1.4.0.dev2
 Summary: MLflow runtime for MLServer
 Home-page: https://github.com/SeldonIO/MLServer.git
 Author: Seldon Technologies Ltd.
 Author-email: hello@seldon.io
 License: Apache 2.0
 Description: # MLflow runtime for MLServer
```

### Comparing `mlserver-mlflow-1.3.4rc2/setup.py` & `mlserver-mlflow-1.4.0.dev2/setup.py`

 * *Files identical despite different names*

