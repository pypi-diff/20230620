# Comparing `tmp/eodc-2023.6.1.tar.gz` & `tmp/eodc-2023.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eodc-2023.6.1.tar", max compression
+gzip compressed data, was "eodc-2023.6.2.tar", max compression
```

## Comparing `eodc-2023.6.1.tar` & `eodc-2023.6.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      513 2023-06-16 13:02:05.166212 eodc-2023.6.1/README.md
--rw-r--r--   0        0        0      213 2023-06-16 13:02:05.166212 eodc-2023.6.1/eodc/__init__.py
--rw-r--r--   0        0        0     1102 2023-06-16 13:02:05.166212 eodc-2023.6.1/eodc/dask.py
--rw-r--r--   0        0        0     7865 2023-06-16 13:02:05.166212 eodc-2023.6.1/eodc/faas.py
--rw-r--r--   0        0        0      469 2023-06-16 13:02:05.166212 eodc-2023.6.1/eodc/settings.py
--rw-r--r--   0        0        0     1161 2023-06-16 13:02:05.166212 eodc-2023.6.1/pyproject.toml
--rw-r--r--   0        0        0     1680 1970-01-01 00:00:00.000000 eodc-2023.6.1/PKG-INFO
+-rw-r--r--   0        0        0      513 2023-06-20 08:50:46.924532 eodc-2023.6.2/README.md
+-rw-r--r--   0        0        0      213 2023-06-20 08:50:46.924532 eodc-2023.6.2/eodc/__init__.py
+-rw-r--r--   0        0        0     1102 2023-06-20 08:50:46.924532 eodc-2023.6.2/eodc/dask.py
+-rw-r--r--   0        0        0     7909 2023-06-20 08:50:46.924532 eodc-2023.6.2/eodc/faas.py
+-rw-r--r--   0        0        0      469 2023-06-20 08:50:46.924532 eodc-2023.6.2/eodc/settings.py
+-rw-r--r--   0        0        0     1161 2023-06-20 08:50:46.924532 eodc-2023.6.2/pyproject.toml
+-rw-r--r--   0        0        0     1680 1970-01-01 00:00:00.000000 eodc-2023.6.2/PKG-INFO
```

### Comparing `eodc-2023.6.1/README.md` & `eodc-2023.6.2/README.md`

 * *Files identical despite different names*

### Comparing `eodc-2023.6.1/eodc/dask.py` & `eodc-2023.6.2/eodc/dask.py`

 * *Files identical despite different names*

### Comparing `eodc-2023.6.1/eodc/faas.py` & `eodc-2023.6.2/eodc/faas.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import logging
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from enum import Enum
 from time import sleep
 
 import argo_workflows
+from argo_workflows.api import workflow_service_api
 from argo_workflows.model.io_argoproj_workflow_v1alpha1_arguments import (
     IoArgoprojWorkflowV1alpha1Arguments,
 )
 from argo_workflows.model.io_argoproj_workflow_v1alpha1_parameter import (
     IoArgoprojWorkflowV1alpha1Parameter,
 )
 from argo_workflows.model.io_argoproj_workflow_v1alpha1_workflow import (
@@ -55,22 +56,20 @@
 
 class FaasProcessorBase(ABC):
     @classmethod
     def get_instance(cls, processor_details):
         return cls(processor_details=processor_details)
 
     def __init__(self, processor_details: FaasProcessorDetails) -> None:
-        self.configuration = argo_workflows.Configuration(
-            host=settings.FAAS_URL, disabled_client_side_validations=True
-        )
+        self.configuration = argo_workflows.Configuration(host=settings.FAAS_URL)
         self.configuration.verify_ssl = False
 
         self.api_client = argo_workflows.ApiClient(self.configuration)
-        self.api_instance_workflows = (
-            argo_workflows.api.workflow_service_api.WorkflowServiceApi(self.api_client)
+        self.api_instance_workflows = workflow_service_api.WorkflowServiceApi(
+            self.api_client
         )
         self.processor_details = processor_details
         # TODO: Check here that this workflow template even exists on the server
 
     def submit_workflow(self, **kwargs):
         parameters = [
             IoArgoprojWorkflowV1alpha1Parameter(name=k, value=v)
@@ -214,7 +213,10 @@
         openeo_job_id: str,
     ):
         return super().submit_workflow(
             openeo_executor_parameters=openeo_parameters.json(),
             openeo_user_id=openeo_user_id,
             openeo_job_id=openeo_job_id,
         )
+
+    def get_output_stac_items(self):
+        raise NotImplementedError()
```

### Comparing `eodc-2023.6.1/pyproject.toml` & `eodc-2023.6.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eodc"
-version = "2023.6.1"
+version = "2023.6.2"
 description = "Python SDK for interacting with EODC services."
 authors = ["Lukas Weidenholzer <lukas.weidenholzer@eodc.eu>"]
 maintainers = ["EODC Staff <support@eodc.eu>"]
 readme = "README.md"
 repository = "https://github.com/eodcgmbh/eodc-sdk"
 classifiers = [
     "Development Status :: 1 - Planning",
```

### Comparing `eodc-2023.6.1/PKG-INFO` & `eodc-2023.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eodc
-Version: 2023.6.1
+Version: 2023.6.2
 Summary: Python SDK for interacting with EODC services.
 Home-page: https://github.com/eodcgmbh/eodc-sdk
 Author: Lukas Weidenholzer
 Author-email: lukas.weidenholzer@eodc.eu
 Maintainer: EODC Staff
 Maintainer-email: support@eodc.eu
 Requires-Python: >=3.9,<3.12
```

