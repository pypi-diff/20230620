# Comparing `tmp/quantum_serverless-0.1.2.tar.gz` & `tmp/quantum_serverless-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantum_serverless-0.1.2.tar", last modified: Tue Jun  6 15:31:55 2023, max compression
+gzip compressed data, was "quantum_serverless-0.2.0.tar", last modified: Tue Jun 20 15:51:59 2023, max compression
```

## Comparing `quantum_serverless-0.1.2.tar` & `quantum_serverless-0.2.0.tar`

### file list

```diff
@@ -1,55 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:31:55.448205 quantum_serverless-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-06-06 15:31:55.448205 quantum_serverless-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-06-06 15:31:45.000000 quantum_serverless-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-06 15:31:45.000000 quantum_serverless-0.1.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:31:55.444205 quantum_serverless-0.1.2/quantum_serverless/
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-06 15:31:45.000000 quantum_serverless-0.1.2/quantum_serverless/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:31:55.444205 quantum_serverless-0.1.2/quantum_serverless/core/
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-06-06 15:31:45.000000 quantum_serverless-0.1.2/quantum_serverless/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-06-06 15:31:45.000000 quantum_serverless-0.1.2/quantum_serverless/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     9071 2023-06-06 15:31:45.000000 quantum_serverless-0.1.2/quantum_serverless/core/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-06-06 15:31:45.000000 quantum_serverless-0.1.2/quantum_serverless/core/events.py
--rw-r--r--   0 runner    (1001) docker     (123)    14645 2023-06-06 15:31:45.000000 quantum_serverless-0.1.2/quantum_serverless/core/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     7281 2023-06-06 15:31:45.000000 quantum_serverless-0.1.2/quantum_serverless/core/program.py
--rw-r--r--   0 runner    (1001) docker     (123)    19786 2023-06-06 15:31:45.000000 quantum_serverless-0.1.2/quantum_serverless/core/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-06-06 15:31:45.000000 quantum_serverless-0.1.2/quantum_serverless/core/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-06-06 15:31:45.000000 quantum_serverless-0.1.2/quantum_serverless/core/tracing.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-06-06 15:31:45.000000 quantum_serverless-0.1.2/quantum_serverless/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:31:55.444205 quantum_serverless-0.1.2/quantum_serverless/library/
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-06 15:31:45.000000 quantum_serverless-0.1.2/quantum_serverless/library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-06-06 15:31:45.000000 quantum_serverless-0.1.2/quantum_serverless/library/transpiler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12371 2023-06-06 15:31:45.000000 quantum_serverless-0.1.2/quantum_serverless/quantum_serverless.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:31:55.448205 quantum_serverless-0.1.2/quantum_serverless/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-06-06 15:31:45.000000 quantum_serverless-0.1.2/quantum_serverless/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-06-06 15:31:45.000000 quantum_serverless-0.1.2/quantum_serverless/serializers/program_serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-06-06 15:31:45.000000 quantum_serverless-0.1.2/quantum_serverless/serializers/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:31:55.448205 quantum_serverless-0.1.2/quantum_serverless/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-06-06 15:31:45.000000 quantum_serverless-0.1.2/quantum_serverless/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-06-06 15:31:45.000000 quantum_serverless-0.1.2/quantum_serverless/utils/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-06-06 15:31:45.000000 quantum_serverless-0.1.2/quantum_serverless/utils/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-06-06 15:31:45.000000 quantum_serverless-0.1.2/quantum_serverless/utils/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:31:55.444205 quantum_serverless-0.1.2/quantum_serverless.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-06-06 15:31:55.000000 quantum_serverless-0.1.2/quantum_serverless.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-06-06 15:31:55.000000 quantum_serverless-0.1.2/quantum_serverless.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 15:31:55.000000 quantum_serverless-0.1.2/quantum_serverless.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-06 15:31:55.000000 quantum_serverless-0.1.2/quantum_serverless.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-06 15:31:55.000000 quantum_serverless-0.1.2/quantum_serverless.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-06 15:31:55.448205 quantum_serverless-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-06-06 15:31:45.000000 quantum_serverless-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:31:55.448205 quantum_serverless-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 15:31:45.000000 quantum_serverless-0.1.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:31:55.448205 quantum_serverless-0.1.2/tests/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 15:31:45.000000 quantum_serverless-0.1.2/tests/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4734 2023-06-06 15:31:45.000000 quantum_serverless-0.1.2/tests/core/test_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-06-06 15:31:45.000000 quantum_serverless-0.1.2/tests/core/test_program.py
--rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-06-06 15:31:45.000000 quantum_serverless-0.1.2/tests/core/test_program_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-06-06 15:31:45.000000 quantum_serverless-0.1.2/tests/core/test_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:31:55.448205 quantum_serverless-0.1.2/tests/library/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 15:31:45.000000 quantum_serverless-0.1.2/tests/library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-06-06 15:31:45.000000 quantum_serverless-0.1.2/tests/library/test_transpiler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:31:55.448205 quantum_serverless-0.1.2/tests/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 15:31:45.000000 quantum_serverless-0.1.2/tests/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-06-06 15:31:45.000000 quantum_serverless-0.1.2/tests/serializers/test_program_serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-06-06 15:31:45.000000 quantum_serverless-0.1.2/tests/serializers/test_serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-06-06 15:31:45.000000 quantum_serverless-0.1.2/tests/test_quantum_serverless.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-06 15:31:45.000000 quantum_serverless-0.1.2/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:51:59.908800 quantum_serverless-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-06-20 15:51:59.908800 quantum_serverless-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-06-20 15:51:47.000000 quantum_serverless-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-20 15:51:47.000000 quantum_serverless-0.2.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:51:59.904800 quantum_serverless-0.2.0/quantum_serverless/
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-20 15:51:47.000000 quantum_serverless-0.2.0/quantum_serverless/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:51:59.904800 quantum_serverless-0.2.0/quantum_serverless/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-06-20 15:51:47.000000 quantum_serverless-0.2.0/quantum_serverless/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-06-20 15:51:47.000000 quantum_serverless-0.2.0/quantum_serverless/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9071 2023-06-20 15:51:47.000000 quantum_serverless-0.2.0/quantum_serverless/core/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-06-20 15:51:47.000000 quantum_serverless-0.2.0/quantum_serverless/core/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14891 2023-06-20 15:51:47.000000 quantum_serverless-0.2.0/quantum_serverless/core/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7281 2023-06-20 15:51:47.000000 quantum_serverless-0.2.0/quantum_serverless/core/program.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19786 2023-06-20 15:51:47.000000 quantum_serverless-0.2.0/quantum_serverless/core/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-06-20 15:51:47.000000 quantum_serverless-0.2.0/quantum_serverless/core/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-06-20 15:51:47.000000 quantum_serverless-0.2.0/quantum_serverless/core/tracing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-06-20 15:51:47.000000 quantum_serverless-0.2.0/quantum_serverless/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:51:59.904800 quantum_serverless-0.2.0/quantum_serverless/library/
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-20 15:51:47.000000 quantum_serverless-0.2.0/quantum_serverless/library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-06-20 15:51:47.000000 quantum_serverless-0.2.0/quantum_serverless/library/transpiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12562 2023-06-20 15:51:47.000000 quantum_serverless-0.2.0/quantum_serverless/quantum_serverless.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:51:59.904800 quantum_serverless-0.2.0/quantum_serverless/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-06-20 15:51:47.000000 quantum_serverless-0.2.0/quantum_serverless/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-06-20 15:51:47.000000 quantum_serverless-0.2.0/quantum_serverless/serializers/program_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-06-20 15:51:47.000000 quantum_serverless-0.2.0/quantum_serverless/serializers/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:51:59.904800 quantum_serverless-0.2.0/quantum_serverless/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-06-20 15:51:47.000000 quantum_serverless-0.2.0/quantum_serverless/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-06-20 15:51:47.000000 quantum_serverless-0.2.0/quantum_serverless/utils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-06-20 15:51:47.000000 quantum_serverless-0.2.0/quantum_serverless/utils/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-06-20 15:51:47.000000 quantum_serverless-0.2.0/quantum_serverless/utils/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:51:59.904800 quantum_serverless-0.2.0/quantum_serverless/visualizaiton/
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-06-20 15:51:47.000000 quantum_serverless-0.2.0/quantum_serverless/visualizaiton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6931 2023-06-20 15:51:47.000000 quantum_serverless-0.2.0/quantum_serverless/visualizaiton/widget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:51:59.904800 quantum_serverless-0.2.0/quantum_serverless.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-06-20 15:51:59.000000 quantum_serverless-0.2.0/quantum_serverless.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-06-20 15:51:59.000000 quantum_serverless-0.2.0/quantum_serverless.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 15:51:59.000000 quantum_serverless-0.2.0/quantum_serverless.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-20 15:51:59.000000 quantum_serverless-0.2.0/quantum_serverless.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-20 15:51:59.000000 quantum_serverless-0.2.0/quantum_serverless.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-20 15:51:59.908800 quantum_serverless-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-06-20 15:51:47.000000 quantum_serverless-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:51:59.904800 quantum_serverless-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 15:51:47.000000 quantum_serverless-0.2.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:51:59.904800 quantum_serverless-0.2.0/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 15:51:47.000000 quantum_serverless-0.2.0/tests/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-06-20 15:51:47.000000 quantum_serverless-0.2.0/tests/core/test_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-06-20 15:51:47.000000 quantum_serverless-0.2.0/tests/core/test_program.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-06-20 15:51:47.000000 quantum_serverless-0.2.0/tests/core/test_program_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-06-20 15:51:47.000000 quantum_serverless-0.2.0/tests/core/test_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:51:59.904800 quantum_serverless-0.2.0/tests/library/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 15:51:47.000000 quantum_serverless-0.2.0/tests/library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-06-20 15:51:47.000000 quantum_serverless-0.2.0/tests/library/test_transpiler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:51:59.908800 quantum_serverless-0.2.0/tests/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 15:51:47.000000 quantum_serverless-0.2.0/tests/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-06-20 15:51:47.000000 quantum_serverless-0.2.0/tests/serializers/test_program_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-06-20 15:51:47.000000 quantum_serverless-0.2.0/tests/serializers/test_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-06-20 15:51:47.000000 quantum_serverless-0.2.0/tests/test_quantum_serverless.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-20 15:51:47.000000 quantum_serverless-0.2.0/tests/utils.py
```

### Comparing `quantum_serverless-0.1.2/PKG-INFO` & `quantum_serverless-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantum_serverless
-Version: 0.1.2
+Version: 0.2.0
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Keywords: quantum serverless qiskit
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `quantum_serverless-0.1.2/README.md` & `quantum_serverless-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.1.2/quantum_serverless/__init__.py` & `quantum_serverless-0.2.0/quantum_serverless/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.1.2/quantum_serverless/core/__init__.py` & `quantum_serverless-0.2.0/quantum_serverless/core/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.1.2/quantum_serverless/core/constants.py` & `quantum_serverless-0.2.0/quantum_serverless/core/constants.py`

 * *Files 11% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 # repository
 REPO_HOST_KEY = "REPO_HOST_KEY"
 REPO_PORT_KEY = "REPO_PORT_KEY"
 
 
 # container image
-RAY_IMAGE = "qiskit/quantum-serverless-ray-node:latest-py39"
+RAY_IMAGE = "icr.io/quantum-public/quantum-serverless-ray-node:latest-py39"
 
 # keycloak
 ENV_KEYCLOAK_REALM = "ENV_KEYCLOAK_REALM"
 ENV_KEYCLOAK_CLIENT_ID = "ENV_KEYCLOAK_CLIENT_ID"
 
 # request timeout
 REQUESTS_TIMEOUT: int = 30
```

### Comparing `quantum_serverless-0.1.2/quantum_serverless/core/decorators.py` & `quantum_serverless-0.2.0/quantum_serverless/core/decorators.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.1.2/quantum_serverless/core/events.py` & `quantum_serverless-0.2.0/quantum_serverless/core/events.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.1.2/quantum_serverless/core/job.py` & `quantum_serverless-0.2.0/quantum_serverless/core/job.py`

 * *Files 2% similar despite different names*

```diff
@@ -344,39 +344,47 @@
                 job_id=response_data.get("id"),
                 job_client=self,
             )
 
         return job
 
     def list(self, **kwargs) -> List["Job"]:
+        limit = kwargs.get("limit", 10)
+        offset = kwargs.get("offset", 0)
         response_data = safe_json_request(
             request=lambda: requests.get(
-                f"{self.host}/api/{self.version}/jobs/",
+                f"{self.host}/api/{self.version}/jobs/?limit={limit}&offset={offset}",
                 headers={"Authorization": f"Bearer {self._token}"},
                 timeout=REQUESTS_TIMEOUT,
             )
         )
         return [
-            Job(job.get("id"), job_client=self)
+            Job(job.get("id"), job_client=self, raw_data=job)
             for job in response_data.get("results", [])
         ]
 
 
 class Job:
     """Job."""
 
-    def __init__(self, job_id: str, job_client: BaseJobClient):
+    def __init__(
+        self,
+        job_id: str,
+        job_client: BaseJobClient,
+        raw_data: Optional[Dict[str, Any]] = None,
+    ):
         """Job class for async script execution.
 
         Args:
             job_id: if of the job
             job_client: job client
         """
         self.job_id = job_id
         self._job_client = job_client
+        self.raw_data = raw_data or {}
 
     def status(self):
         """Returns status of the job."""
         return self._job_client.status(self.job_id)
 
     def stop(self):
         """Stops the job from running."""
```

### Comparing `quantum_serverless-0.1.2/quantum_serverless/core/program.py` & `quantum_serverless-0.2.0/quantum_serverless/core/program.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.1.2/quantum_serverless/core/provider.py` & `quantum_serverless-0.2.0/quantum_serverless/core/provider.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.1.2/quantum_serverless/core/state.py` & `quantum_serverless-0.2.0/quantum_serverless/core/state.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.1.2/quantum_serverless/core/tracing.py` & `quantum_serverless-0.2.0/quantum_serverless/core/tracing.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.1.2/quantum_serverless/exception.py` & `quantum_serverless-0.2.0/quantum_serverless/exception.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.1.2/quantum_serverless/library/__init__.py` & `quantum_serverless-0.2.0/quantum_serverless/library/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.1.2/quantum_serverless/library/transpiler.py` & `quantum_serverless-0.2.0/quantum_serverless/library/transpiler.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.1.2/quantum_serverless/quantum_serverless.py` & `quantum_serverless-0.2.0/quantum_serverless/quantum_serverless.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 import requests
 from ray._private.worker import BaseContext
 
 from quantum_serverless.core.job import Job
 from quantum_serverless.core.program import Program
 from quantum_serverless.core.provider import Provider, ComputeResource
 from quantum_serverless.exception import QuantumServerlessException
+from quantum_serverless.visualizaiton import Widget
 
 Context = Union[BaseContext]
 
 
 class QuantumServerless:
     """QuantumServerless class."""
 
@@ -265,14 +266,18 @@
         """Returns list of available providers.
 
         Returns:
             list of providers
         """
         return self._providers
 
+    def widget(self):
+        """Widget for information about provider and jobs."""
+        return Widget(self._selected_provider).show()
+
     def __repr__(self):
         providers = ", ".join(provider.name for provider in self.providers())
         return f"<QuantumServerless | providers [{providers}]>"
 
 
 def load_config(config: Optional[Dict[str, Any]] = None) -> List[Provider]:
     """Loads providers from configuration."""
```

### Comparing `quantum_serverless-0.1.2/quantum_serverless/serializers/__init__.py` & `quantum_serverless-0.2.0/quantum_serverless/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.1.2/quantum_serverless/serializers/program_serializers.py` & `quantum_serverless-0.2.0/quantum_serverless/serializers/program_serializers.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.1.2/quantum_serverless/serializers/serializers.py` & `quantum_serverless-0.2.0/quantum_serverless/serializers/serializers.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.1.2/quantum_serverless/utils/__init__.py` & `quantum_serverless-0.2.0/quantum_serverless/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.1.2/quantum_serverless/utils/errors.py` & `quantum_serverless-0.2.0/quantum_serverless/utils/errors.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.1.2/quantum_serverless/utils/json.py` & `quantum_serverless-0.2.0/quantum_serverless/utils/json.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.1.2/quantum_serverless/utils/storage.py` & `quantum_serverless-0.2.0/quantum_serverless/utils/storage.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.1.2/quantum_serverless.egg-info/PKG-INFO` & `quantum_serverless-0.2.0/quantum_serverless.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantum-serverless
-Version: 0.1.2
+Version: 0.2.0
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Keywords: quantum serverless qiskit
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `quantum_serverless-0.1.2/quantum_serverless.egg-info/SOURCES.txt` & `quantum_serverless-0.2.0/quantum_serverless.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -24,14 +24,16 @@
 quantum_serverless/serializers/__init__.py
 quantum_serverless/serializers/program_serializers.py
 quantum_serverless/serializers/serializers.py
 quantum_serverless/utils/__init__.py
 quantum_serverless/utils/errors.py
 quantum_serverless/utils/json.py
 quantum_serverless/utils/storage.py
+quantum_serverless/visualizaiton/__init__.py
+quantum_serverless/visualizaiton/widget.py
 tests/__init__.py
 tests/test_quantum_serverless.py
 tests/utils.py
 tests/core/__init__.py
 tests/core/test_decorator.py
 tests/core/test_program.py
 tests/core/test_program_repository.py
```

### Comparing `quantum_serverless-0.1.2/setup.py` & `quantum_serverless-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.1.2/tests/core/test_decorator.py` & `quantum_serverless-0.2.0/tests/core/test_decorator.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,23 +15,22 @@
 from unittest import TestCase
 
 from qiskit import QuantumCircuit
 from qiskit.circuit.random import random_circuit
 
 from quantum_serverless import QuantumServerless, get
 from quantum_serverless.core.decorators import (
-    run_qiskit_remote,
     distribute_task,
     Target,
     fetch_execution_meta,
 )
 from quantum_serverless.core.state import StateHandler
 
 
-class TestHandler(StateHandler):
+class DemoHandler(StateHandler):
     """TestHandler"""
 
     def __init__(self):
         self.memory: Dict[str, Any] = {}
 
     def set(self, key: str, value: Dict[str, Any]):
         self.memory[key] = value
@@ -39,42 +38,14 @@
     def get(self, key: str):
         return self.memory.get(key)
 
 
 class TestDecorators(TestCase):
     """Test decorators."""
 
-    def test_run_qiskit_remote(self):
-        """Test for run_qiskit_remote."""
-
-        serverless = QuantumServerless()
-
-        @run_qiskit_remote()
-        def another_function(
-            circuit: List[QuantumCircuit], other_circuit: QuantumCircuit
-        ):
-            """Another test function."""
-            return circuit[0].compose(other_circuit, range(5)).depth()
-
-        @run_qiskit_remote(target={"cpu": 1})
-        def ultimate_function(ultimate_argument: int):
-            """Test function."""
-            print("Printing function argument:", ultimate_argument)
-            mid_result = get(
-                another_function(
-                    [random_circuit(5, 2)], other_circuit=random_circuit(5, 2)
-                )
-            )
-            return mid_result
-
-        with self.assertWarns(Warning), serverless.context():
-            reference = ultimate_function(1)
-            result = get(reference)
-            self.assertEqual(result, 4)
-
     def test_distribute_task(self):
         """Test for run_qiskit_remote."""
 
         serverless = QuantumServerless()
 
         @distribute_task()
         def another_function(
@@ -104,15 +75,15 @@
         target_expected = Target(pip=["requests", "qiskit==0.39.2"])
         target = Target.from_dict({"pip": ["requests", "qiskit==0.39.2"]})
         self.assertEqual(target.pip, target_expected.pip)
 
     def test_remote_with_state_injection(self):
         """Tests remote with state injection."""
         serverless = QuantumServerless()
-        state_handler = TestHandler()
+        state_handler = DemoHandler()
 
         @distribute_task(target={"cpu": 1}, state=state_handler)
         def ultimate_function_with_state(state: StateHandler, ultimate_argument: int):
             """Test function."""
             state.set("some_key", {"result": ultimate_argument})
             return state.get("some_key")
```

### Comparing `quantum_serverless-0.1.2/tests/core/test_program_repository.py` & `quantum_serverless-0.2.0/tests/core/test_program_repository.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.1.2/tests/core/test_state.py` & `quantum_serverless-0.2.0/tests/core/test_state.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.1.2/tests/library/test_transpiler.py` & `quantum_serverless-0.2.0/tests/library/test_transpiler.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
         circuit1 = random_circuit(5, 3)
         circuit2 = random_circuit(5, 3)
 
         backend1 = FakeAlmadenV2()
         backend2 = FakeBrooklynV2()
 
-        with QuantumServerless():
+        with QuantumServerless().context():
             transpiled_circuits = parallel_transpile(
                 circuits=[circuit1, [circuit1, circuit2]], backends=[backend1, backend2]
             )
             self.assertIsInstance(transpiled_circuits[0], QuantumCircuit)
             self.assertIsInstance(transpiled_circuits[1], list)
             self.assertEqual(len(transpiled_circuits[1]), 2)
             for tcirc in transpiled_circuits[1]:
@@ -47,11 +47,11 @@
     def test_transpile_fail(self):
         """Test failing cases for parallel transpile."""
         circuit1 = random_circuit(5, 3)
 
         backend1 = FakeAlmadenV2()
         backend2 = FakeBrooklynV2()
 
-        with QuantumServerless():
+        with QuantumServerless().context():
             # inconsistent number of circuits and backends
             with self.assertRaises(QuantumServerlessException):
                 parallel_transpile(circuits=[circuit1], backends=[backend1, backend2])
```

### Comparing `quantum_serverless-0.1.2/tests/serializers/test_program_serializers.py` & `quantum_serverless-0.2.0/tests/serializers/test_program_serializers.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.1.2/tests/serializers/test_serializers.py` & `quantum_serverless-0.2.0/tests/serializers/test_serializers.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,22 +14,22 @@
 
 from unittest import TestCase
 
 from ray.util import register_serializer
 from qiskit import QuantumCircuit
 from qiskit.circuit.random import random_circuit
 
-from quantum_serverless import QuantumServerless, run_qiskit_remote, get
+from quantum_serverless import QuantumServerless, distribute_task, get
 from quantum_serverless.serializers.serializers import (
     circuit_serializer,
     circuit_deserializer,
 )
 
 
-@run_qiskit_remote()
+@distribute_task()
 def circuit_function(circuit: QuantumCircuit):
     """Test function."""
     return circuit.name
 
 
 class TestSerializers(TestCase):
     """TestSerializers."""
```

### Comparing `quantum_serverless-0.1.2/tests/test_quantum_serverless.py` & `quantum_serverless-0.2.0/tests/test_quantum_serverless.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.1.2/tests/utils.py` & `quantum_serverless-0.2.0/tests/utils.py`

 * *Files identical despite different names*

