# Comparing `tmp/dagster-hex-0.1.2.tar.gz` & `tmp/dagster-hex-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-hex-0.1.2.tar", last modified: Tue Nov  8 00:57:21 2022, max compression
+gzip compressed data, was "dagster-hex-0.1.3.tar", last modified: Tue Jun 20 18:01:13 2023, max compression
```

## Comparing `dagster-hex-0.1.2.tar` & `dagster-hex-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-11-08 00:57:21.231321 dagster-hex-0.1.2/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       20 2022-11-08 00:57:07.000000 dagster-hex-0.1.2/MANIFEST.in
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1811 2022-11-08 00:57:21.235321 dagster-hex-0.1.2/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1112 2022-11-08 00:57:07.000000 dagster-hex-0.1.2/README.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)        6 2022-11-08 00:57:07.000000 dagster-hex-0.1.2/VERSION.txt
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-11-08 00:57:21.231321 dagster-hex-0.1.2/dagster_hex/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-11-08 00:57:07.000000 dagster-hex-0.1.2/dagster_hex/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      381 2022-11-08 00:57:07.000000 dagster-hex-0.1.2/dagster_hex/consts.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3309 2022-11-08 00:57:07.000000 dagster-hex-0.1.2/dagster_hex/ops.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11105 2022-11-08 00:57:07.000000 dagster-hex-0.1.2/dagster_hex/resources.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      675 2022-11-08 00:57:07.000000 dagster-hex-0.1.2/dagster_hex/types.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-11-08 00:57:21.231321 dagster-hex-0.1.2/dagster_hex.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1811 2022-11-08 00:57:21.000000 dagster-hex-0.1.2/dagster_hex.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      371 2022-11-08 00:57:21.000000 dagster-hex-0.1.2/dagster_hex.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-11-08 00:57:21.000000 dagster-hex-0.1.2/dagster_hex.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-11-08 00:57:20.000000 dagster-hex-0.1.2/dagster_hex.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (3434) circleci  (3434)      126 2022-11-08 00:57:21.000000 dagster-hex-0.1.2/dagster_hex.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       12 2022-11-08 00:57:21.000000 dagster-hex-0.1.2/dagster_hex.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1572 2022-11-08 00:57:21.235321 dagster-hex-0.1.2/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2022-11-08 00:57:07.000000 dagster-hex-0.1.2/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-20 18:01:13.021990 dagster-hex-0.1.3/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       20 2023-06-20 18:01:01.000000 dagster-hex-0.1.3/MANIFEST.in
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1811 2023-06-20 18:01:13.021990 dagster-hex-0.1.3/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1113 2023-06-20 18:01:01.000000 dagster-hex-0.1.3/README.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        6 2023-06-20 18:01:01.000000 dagster-hex-0.1.3/VERSION.txt
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-20 18:01:13.021990 dagster-hex-0.1.3/dagster_hex/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-20 18:01:01.000000 dagster-hex-0.1.3/dagster_hex/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      381 2023-06-20 18:01:01.000000 dagster-hex-0.1.3/dagster_hex/consts.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3628 2023-06-20 18:01:01.000000 dagster-hex-0.1.3/dagster_hex/ops.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11447 2023-06-20 18:01:01.000000 dagster-hex-0.1.3/dagster_hex/resources.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1178 2023-06-20 18:01:01.000000 dagster-hex-0.1.3/dagster_hex/types.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-20 18:01:13.021990 dagster-hex-0.1.3/dagster_hex.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1811 2023-06-20 18:01:13.000000 dagster-hex-0.1.3/dagster_hex.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      389 2023-06-20 18:01:13.000000 dagster-hex-0.1.3/dagster_hex.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-06-20 18:01:13.000000 dagster-hex-0.1.3/dagster_hex.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-06-20 18:01:12.000000 dagster-hex-0.1.3/dagster_hex.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      126 2023-06-20 18:01:13.000000 dagster-hex-0.1.3/dagster_hex.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       12 2023-06-20 18:01:13.000000 dagster-hex-0.1.3/dagster_hex.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1572 2023-06-20 18:01:13.025990 dagster-hex-0.1.3/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-06-20 18:01:01.000000 dagster-hex-0.1.3/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-20 18:01:13.021990 dagster-hex-0.1.3/tests/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1423 2023-06-20 18:01:01.000000 dagster-hex-0.1.3/tests/test_hex.py
```

### Comparing `dagster-hex-0.1.2/PKG-INFO` & `dagster-hex-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-hex
-Version: 0.1.2
+Version: 0.1.3
 Summary: Dagster library for Hex
 Home-page: https://github.com/hex-inc/dagster-hex
 Author: Pedram Navid
 Author-email: pedram@pedramnavid.com
 License: Apache License 2.0
 Project-URL: Source Code, https://github.com/hex-inc/dagster-hex
 Project-URL: Homepage, https://github.com/hex-inc/dagster-hex
@@ -20,15 +20,15 @@
 # Hex Dagster Library
 
 ### Installation
 
 To install the library, use pip alongside your existing Dagster environment.
 
 ```bash
-pip install dagster_hex
+pip install dagster-hex
 ```
 
 ### Configuration
 
 First, you'll need to specify your Hex API Token key as a resource.
 
 ```python
```

### Comparing `dagster-hex-0.1.2/README.md` & `dagster-hex-0.1.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Hex Dagster Library
 
 ### Installation
 
 To install the library, use pip alongside your existing Dagster environment.
 
 ```bash
-pip install dagster_hex
+pip install dagster-hex
 ```
 
 ### Configuration
 
 First, you'll need to specify your Hex API Token key as a resource.
 
 ```python
@@ -48,8 +48,8 @@
 
 ```
 run_url	
 run_status_url	
 trace_id	
 run_id	
 elapsed_time	
-```
+```
```

### Comparing `dagster-hex-0.1.2/dagster_hex/ops.py` & `dagster-hex-0.1.3/dagster_hex/ops.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,14 +28,21 @@
         ),
         "inputs": Field(
             Noneable(dict),
             is_required=False,
             default_value=None,
             description="Additional inputs for the Hex Project",
         ),
+        "notifications": Field(
+            Noneable(list),
+            is_required=False,
+            default_value=None,
+            description="A list of notification details that will be delivered "
+            + "once a project run completes",
+        ),
         "update_cache": Field(
             bool,
             is_required=False,
             default_value=False,
             description="When true, this run will update the cached state of the "
             "published app with the latest run results.",
         ),
@@ -67,14 +74,15 @@
     completes, raising an error if it is unsuccessful. It outputs a StatusResponse
     which contains the details of the Hex project after the run completes.
     """
 
     hex_output: HexOutput = context.resources.hex.run_and_poll(
         project_id=context.op_config["project_id"],
         inputs=context.op_config["inputs"],
+        notifications=context.op_config["notifications"],
         update_cache=context.op_config["update_cache"],
         kill_on_timeout=context.op_config["kill_on_timeout"],
         poll_interval=context.op_config["poll_interval"],
         poll_timeout=context.op_config["poll_timeout"],
     )
     asset_name = ["hex", hex_output.run_response["projectId"]]
```

### Comparing `dagster-hex-0.1.2/dagster_hex/resources.py` & `dagster-hex-0.1.3/dagster_hex/resources.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 import datetime
 import logging
 import time
 from importlib.metadata import PackageNotFoundError, version
-from typing import Any, Dict, Optional, cast
+from typing import Any, Dict, List, Optional, cast
 from urllib.parse import urljoin
 
 import requests
 from dagster import Failure, Field, StringSource, get_dagster_logger, resource
 
-from dagster_hex.types import HexOutput, RunResponse, StatusResponse
+from dagster_hex.types import (
+    HexOutput,
+    NotificationDetails,
+    RunResponse,
+    StatusResponse,
+)
 
 from .consts import (
     COMPLETE,
     DEFAULT_POLL_INTERVAL,
     DEFAULT_POLL_TIMEOUT,
     HEX_API_BASE,
     TERMINAL_STATUSES,
@@ -35,15 +40,14 @@
         self,
         api_key: str,
         base_url: str = HEX_API_BASE,
         log: logging.Logger = get_dagster_logger(),
         request_max_retries: int = 3,
         request_retry_delay: float = 0.25,
     ):
-
         self._log = log
         self._api_key = api_key
         self._request_max_retries = request_max_retries
         self._request_retry_delay = request_retry_delay
         self.api_base_url = base_url
 
     def make_request(
@@ -125,14 +129,15 @@
         raise Failure("Exceeded max number of retries.")
 
     def run_project(
         self,
         project_id: str,
         inputs: Optional[Dict[str, Any]] = None,
         update_cache: bool = False,
+        notifications: List[NotificationDetails] = [],
     ) -> RunResponse:
         """Trigger a sync and initiate a sync run
 
         Args:
             project_id (str): The Hex Project ID
             inputs (dict): additional input parameters, a json-serializable dictionary
                 of variable_name: value pairs.
@@ -147,14 +152,17 @@
         """
         method = "POST"
         endpoint = f"/api/v1/project/{project_id}/run"
         data: Dict[str, Any] = {"updateCache": update_cache}
         if inputs:
             data["inputParams"] = inputs
 
+        if notifications:
+            data["notifications"] = notifications
+
         response = cast(
             RunResponse,
             self.make_request(
                 method=method,
                 endpoint=endpoint,
                 data=data,
             ),
@@ -199,14 +207,15 @@
         self.make_request(method=method, endpoint=endpoint)
         return run_id
 
     def run_and_poll(
         self,
         project_id: str,
         inputs: Optional[dict],
+        notifications: List[NotificationDetails] = [],
         update_cache: bool = False,
         kill_on_timeout: bool = True,
         poll_interval: float = DEFAULT_POLL_INTERVAL,
         poll_timeout: Optional[float] = DEFAULT_POLL_TIMEOUT,
     ) -> HexOutput:
         """Trigger a project and poll until complete
 
@@ -224,15 +233,20 @@
                 background until completion.
             poll_interval (int): time to wait in between polls to the API
             poll_timeout (int): maximum time to wait for the project to complete
 
         Returns:
             Dict[str, Any]: Parsed json output from the API
         """
-        run_response = self.run_project(project_id, inputs, update_cache)
+        run_response = self.run_project(
+            project_id,
+            inputs=inputs,
+            notifications=notifications,
+            update_cache=update_cache,
+        )
         run_id = run_response["runId"]
         poll_start = datetime.datetime.now()
         while True:
             run_status = self.run_status(project_id, run_id)
             project_status = run_status["status"]
 
             self._log.debug(run_status)
```

### Comparing `dagster-hex-0.1.2/dagster_hex.egg-info/PKG-INFO` & `dagster-hex-0.1.3/dagster_hex.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-hex
-Version: 0.1.2
+Version: 0.1.3
 Summary: Dagster library for Hex
 Home-page: https://github.com/hex-inc/dagster-hex
 Author: Pedram Navid
 Author-email: pedram@pedramnavid.com
 License: Apache License 2.0
 Project-URL: Source Code, https://github.com/hex-inc/dagster-hex
 Project-URL: Homepage, https://github.com/hex-inc/dagster-hex
@@ -20,15 +20,15 @@
 # Hex Dagster Library
 
 ### Installation
 
 To install the library, use pip alongside your existing Dagster environment.
 
 ```bash
-pip install dagster_hex
+pip install dagster-hex
 ```
 
 ### Configuration
 
 First, you'll need to specify your Hex API Token key as a resource.
 
 ```python
```

### Comparing `dagster-hex-0.1.2/setup.cfg` & `dagster-hex-0.1.3/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 	Changelog=https://github.com/hex-inc/dagster-hex/blob/main/CHANGELOG.md
 
 [options]
 python_requires = >=3.8
 packages = find_namespace:
 include_package_data = true
 install_requires = 
-	dagster>=1.0
+	dagster>=1.3
 	dagit
 	requests>=2
 zip_safe = false
 
 [options.extras_require]
 dev = 
 	mypy>=0.8
```

