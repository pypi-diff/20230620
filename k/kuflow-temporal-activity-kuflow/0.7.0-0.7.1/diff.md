# Comparing `tmp/kuflow_temporal_activity_kuflow-0.7.0.tar.gz` & `tmp/kuflow_temporal_activity_kuflow-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kuflow_temporal_activity_kuflow-0.7.0.tar", max compression
+gzip compressed data, was "kuflow_temporal_activity_kuflow-0.7.1.tar", max compression
```

## Comparing `kuflow_temporal_activity_kuflow-0.7.0.tar` & `kuflow_temporal_activity_kuflow-0.7.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      878 2023-06-20 06:25:31.590348 kuflow_temporal_activity_kuflow-0.7.0/README.md
--rw-r--r--   0        0        0        6 2023-06-20 06:25:31.590348 kuflow_temporal_activity_kuflow-0.7.0/VERSION
--rw-r--r--   0        0        0     1320 2023-06-20 06:25:31.590348 kuflow_temporal_activity_kuflow-0.7.0/kuflow_temporal_activity_kuflow/__init__.py
--rw-r--r--   0        0        0     8623 2023-06-20 06:25:31.590348 kuflow_temporal_activity_kuflow-0.7.0/kuflow_temporal_activity_kuflow/_validation.py
--rw-r--r--   0        0        0     5176 2023-06-20 06:25:31.590348 kuflow_temporal_activity_kuflow-0.7.0/kuflow_temporal_activity_kuflow/converter.py
--rw-r--r--   0        0        0     2226 2023-06-20 06:25:31.590348 kuflow_temporal_activity_kuflow-0.7.0/kuflow_temporal_activity_kuflow/kuflow_async_activities.py
--rw-r--r--   0        0        0    15503 2023-06-20 06:25:31.590348 kuflow_temporal_activity_kuflow-0.7.0/kuflow_temporal_activity_kuflow/kuflow_sync_activities.py
--rw-r--r--   0        0        0     3553 2023-06-20 06:25:31.590348 kuflow_temporal_activity_kuflow-0.7.0/kuflow_temporal_activity_kuflow/models/__init__.py
--rw-r--r--   0        0        0     1949 2023-06-20 06:26:41.671973 kuflow_temporal_activity_kuflow-0.7.0/kuflow_temporal_activity_kuflow/models/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0    22540 2023-06-20 06:26:41.675974 kuflow_temporal_activity_kuflow-0.7.0/kuflow_temporal_activity_kuflow/models/__pycache__/_models.cpython-38.pyc
--rw-r--r--   0        0        0    22235 2023-06-20 06:25:31.590348 kuflow_temporal_activity_kuflow-0.7.0/kuflow_temporal_activity_kuflow/models/_models.py
--rw-r--r--   0        0        0     1478 2023-06-20 06:25:31.594348 kuflow_temporal_activity_kuflow-0.7.0/kuflow_temporal_activity_kuflow/utils/__init__.py
--rw-r--r--   0        0        0      499 2023-06-20 06:26:41.679974 kuflow_temporal_activity_kuflow-0.7.0/kuflow_temporal_activity_kuflow/utils/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0    10493 2023-06-20 06:26:41.683974 kuflow_temporal_activity_kuflow-0.7.0/kuflow_temporal_activity_kuflow/utils/__pycache__/_save_process_element_utils.cpython-38.pyc
--rw-r--r--   0        0        0    13245 2023-06-20 06:26:41.687975 kuflow_temporal_activity_kuflow-0.7.0/kuflow_temporal_activity_kuflow/utils/__pycache__/_save_task_element_utils.cpython-38.pyc
--rw-r--r--   0        0        0    14343 2023-06-20 06:26:41.687975 kuflow_temporal_activity_kuflow-0.7.0/kuflow_temporal_activity_kuflow/utils/__pycache__/_save_task_json_forms_value_data_request_utils.cpython-38.pyc
--rw-r--r--   0        0        0    11220 2023-06-20 06:25:31.594348 kuflow_temporal_activity_kuflow-0.7.0/kuflow_temporal_activity_kuflow/utils/_save_process_element_utils.py
--rw-r--r--   0        0        0    14103 2023-06-20 06:25:31.594348 kuflow_temporal_activity_kuflow-0.7.0/kuflow_temporal_activity_kuflow/utils/_save_task_element_utils.py
--rw-r--r--   0        0        0    15436 2023-06-20 06:25:31.594348 kuflow_temporal_activity_kuflow-0.7.0/kuflow_temporal_activity_kuflow/utils/_save_task_json_forms_value_data_request_utils.py
--rw-r--r--   0        0        0     1037 2023-06-20 06:26:59.285395 kuflow_temporal_activity_kuflow-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     1705 1970-01-01 00:00:00.000000 kuflow_temporal_activity_kuflow-0.7.0/setup.py
--rw-r--r--   0        0        0     1667 1970-01-01 00:00:00.000000 kuflow_temporal_activity_kuflow-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0      878 2023-06-20 07:20:29.819020 kuflow_temporal_activity_kuflow-0.7.1/README.md
+-rw-r--r--   0        0        0        6 2023-06-20 07:20:29.819020 kuflow_temporal_activity_kuflow-0.7.1/VERSION
+-rw-r--r--   0        0        0     1320 2023-06-20 07:20:29.819020 kuflow_temporal_activity_kuflow-0.7.1/kuflow_temporal_activity_kuflow/__init__.py
+-rw-r--r--   0        0        0     8623 2023-06-20 07:20:29.819020 kuflow_temporal_activity_kuflow-0.7.1/kuflow_temporal_activity_kuflow/_validation.py
+-rw-r--r--   0        0        0     5176 2023-06-20 07:20:29.819020 kuflow_temporal_activity_kuflow-0.7.1/kuflow_temporal_activity_kuflow/converter.py
+-rw-r--r--   0        0        0     2226 2023-06-20 07:20:29.819020 kuflow_temporal_activity_kuflow-0.7.1/kuflow_temporal_activity_kuflow/kuflow_async_activities.py
+-rw-r--r--   0        0        0    15503 2023-06-20 07:20:29.819020 kuflow_temporal_activity_kuflow-0.7.1/kuflow_temporal_activity_kuflow/kuflow_sync_activities.py
+-rw-r--r--   0        0        0     3553 2023-06-20 07:20:29.819020 kuflow_temporal_activity_kuflow-0.7.1/kuflow_temporal_activity_kuflow/models/__init__.py
+-rw-r--r--   0        0        0     1949 2023-06-20 07:21:29.632378 kuflow_temporal_activity_kuflow-0.7.1/kuflow_temporal_activity_kuflow/models/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0    22540 2023-06-20 07:21:29.632378 kuflow_temporal_activity_kuflow-0.7.1/kuflow_temporal_activity_kuflow/models/__pycache__/_models.cpython-38.pyc
+-rw-r--r--   0        0        0    22235 2023-06-20 07:20:29.819020 kuflow_temporal_activity_kuflow-0.7.1/kuflow_temporal_activity_kuflow/models/_models.py
+-rw-r--r--   0        0        0     1478 2023-06-20 07:20:29.819020 kuflow_temporal_activity_kuflow-0.7.1/kuflow_temporal_activity_kuflow/utils/__init__.py
+-rw-r--r--   0        0        0      499 2023-06-20 07:21:29.640379 kuflow_temporal_activity_kuflow-0.7.1/kuflow_temporal_activity_kuflow/utils/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0    10493 2023-06-20 07:21:29.640379 kuflow_temporal_activity_kuflow-0.7.1/kuflow_temporal_activity_kuflow/utils/__pycache__/_save_process_element_utils.cpython-38.pyc
+-rw-r--r--   0        0        0    13245 2023-06-20 07:21:29.644379 kuflow_temporal_activity_kuflow-0.7.1/kuflow_temporal_activity_kuflow/utils/__pycache__/_save_task_element_utils.cpython-38.pyc
+-rw-r--r--   0        0        0    14343 2023-06-20 07:21:29.644379 kuflow_temporal_activity_kuflow-0.7.1/kuflow_temporal_activity_kuflow/utils/__pycache__/_save_task_json_forms_value_data_request_utils.cpython-38.pyc
+-rw-r--r--   0        0        0    11220 2023-06-20 07:20:29.819020 kuflow_temporal_activity_kuflow-0.7.1/kuflow_temporal_activity_kuflow/utils/_save_process_element_utils.py
+-rw-r--r--   0        0        0    14103 2023-06-20 07:20:29.819020 kuflow_temporal_activity_kuflow-0.7.1/kuflow_temporal_activity_kuflow/utils/_save_task_element_utils.py
+-rw-r--r--   0        0        0    15436 2023-06-20 07:20:29.819020 kuflow_temporal_activity_kuflow-0.7.1/kuflow_temporal_activity_kuflow/utils/_save_task_json_forms_value_data_request_utils.py
+-rw-r--r--   0        0        0     1017 2023-06-20 07:21:48.218041 kuflow_temporal_activity_kuflow-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     1705 1970-01-01 00:00:00.000000 kuflow_temporal_activity_kuflow-0.7.1/setup.py
+-rw-r--r--   0        0        0     1667 1970-01-01 00:00:00.000000 kuflow_temporal_activity_kuflow-0.7.1/PKG-INFO
```

### Comparing `kuflow_temporal_activity_kuflow-0.7.0/README.md` & `kuflow_temporal_activity_kuflow-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `kuflow_temporal_activity_kuflow-0.7.0/kuflow_temporal_activity_kuflow/__init__.py` & `kuflow_temporal_activity_kuflow-0.7.1/kuflow_temporal_activity_kuflow/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,8 +23,8 @@
 # SOFTWARE.
 #
 
 from .kuflow_async_activities import KuFlowAsyncActivities
 from .kuflow_sync_activities import KuFlowSyncActivities
 
 __all__ = ["KuFlowAsyncActivities", "KuFlowSyncActivities"]
-__version__ = "0.7.0"
+__version__ = "0.7.1"
```

### Comparing `kuflow_temporal_activity_kuflow-0.7.0/kuflow_temporal_activity_kuflow/_validation.py` & `kuflow_temporal_activity_kuflow-0.7.1/kuflow_temporal_activity_kuflow/_validation.py`

 * *Files identical despite different names*

### Comparing `kuflow_temporal_activity_kuflow-0.7.0/kuflow_temporal_activity_kuflow/converter.py` & `kuflow_temporal_activity_kuflow-0.7.1/kuflow_temporal_activity_kuflow/converter.py`

 * *Files identical despite different names*

### Comparing `kuflow_temporal_activity_kuflow-0.7.0/kuflow_temporal_activity_kuflow/kuflow_async_activities.py` & `kuflow_temporal_activity_kuflow-0.7.1/kuflow_temporal_activity_kuflow/kuflow_async_activities.py`

 * *Files identical despite different names*

### Comparing `kuflow_temporal_activity_kuflow-0.7.0/kuflow_temporal_activity_kuflow/kuflow_sync_activities.py` & `kuflow_temporal_activity_kuflow-0.7.1/kuflow_temporal_activity_kuflow/kuflow_sync_activities.py`

 * *Files identical despite different names*

### Comparing `kuflow_temporal_activity_kuflow-0.7.0/kuflow_temporal_activity_kuflow/models/__init__.py` & `kuflow_temporal_activity_kuflow-0.7.1/kuflow_temporal_activity_kuflow/models/__init__.py`

 * *Files identical despite different names*

### Comparing `kuflow_temporal_activity_kuflow-0.7.0/kuflow_temporal_activity_kuflow/models/__pycache__/__init__.cpython-38.pyc` & `kuflow_temporal_activity_kuflow-0.7.1/kuflow_temporal_activity_kuflow/models/__pycache__/__init__.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Jun 20 06:25:31 2023 UTC, .py size: 3553 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 5b46 9164 e10d 0000  U.......[F.d....
+00000000: 550d 0d0a 0000 0000 3d53 9164 e10d 0000  U.......=S.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0028 0000 0040 0000 0073 0001 0000 6400  .(...@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 6d04 5a04 6d05 5a05 6d06 5a06 6d07 5a07  m.Z.m.Z.m.Z.m.Z.
 00000050: 6d08 5a08 6d09 5a09 6d0a 5a0a 6d0b 5a0b  m.Z.m.Z.m.Z.m.Z.
 00000060: 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e 6d0f 5a0f  m.Z.m.Z.m.Z.m.Z.
 00000070: 6d10 5a10 6d11 5a11 6d12 5a12 6d13 5a13  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `kuflow_temporal_activity_kuflow-0.7.0/kuflow_temporal_activity_kuflow/models/__pycache__/_models.cpython-38.pyc` & `kuflow_temporal_activity_kuflow-0.7.1/kuflow_temporal_activity_kuflow/models/__pycache__/_models.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Jun 20 06:25:31 2023 UTC, .py size: 22235 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 5b46 9164 db56 0000  U.......[F.d.V..
+00000000: 550d 0d0a 0000 0000 3d53 9164 db56 0000  U.......=S.d.V..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 0403 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 6d04 5a04 0100 6400 6402 6c05 6d06 5a06  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6403 6c07 6d08 5a09 0100 4700  ..d.d.l.m.Z...G.
 00000060: 6404 6405 8400 6405 6506 6a0a 8303 5a0b  d.d...d.e.j...Z.
 00000070: 4700 6406 6407 8400 6407 6506 6a0a 8303  G.d.d...d.e.j...
```

### Comparing `kuflow_temporal_activity_kuflow-0.7.0/kuflow_temporal_activity_kuflow/models/_models.py` & `kuflow_temporal_activity_kuflow-0.7.1/kuflow_temporal_activity_kuflow/models/_models.py`

 * *Files identical despite different names*

### Comparing `kuflow_temporal_activity_kuflow-0.7.0/kuflow_temporal_activity_kuflow/utils/__init__.py` & `kuflow_temporal_activity_kuflow-0.7.1/kuflow_temporal_activity_kuflow/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `kuflow_temporal_activity_kuflow-0.7.0/kuflow_temporal_activity_kuflow/utils/__pycache__/_save_process_element_utils.cpython-38.pyc` & `kuflow_temporal_activity_kuflow-0.7.1/kuflow_temporal_activity_kuflow/utils/__pycache__/_save_process_element_utils.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Jun 20 06:25:31 2023 UTC, .py size: 11220 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 5b46 9164 d42b 0000  U.......[F.d.+..
+00000000: 550d 0d0a 0000 0000 3d53 9164 d42b 0000  U.......=S.d.+..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 c200 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 6d04 5a04 0100 6400 6403 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6400 6404 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 6d09 5a09 6d0a 5a0a 0100 6400 6405 6c0b  m.Z.m.Z...d.d.l.
 00000070: 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e 6d0f 5a0f  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `kuflow_temporal_activity_kuflow-0.7.0/kuflow_temporal_activity_kuflow/utils/__pycache__/_save_task_element_utils.cpython-38.pyc` & `kuflow_temporal_activity_kuflow-0.7.1/kuflow_temporal_activity_kuflow/utils/__pycache__/_save_task_element_utils.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Jun 20 06:25:31 2023 UTC, .py size: 14103 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 5b46 9164 1737 0000  U.......[F.d.7..
+00000000: 550d 0d0a 0000 0000 3d53 9164 1737 0000  U.......=S.d.7..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 e200 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 6d04 5a04 0100 6400 6403 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 6d07 5a07 6d08 5a08 0100 6400  m.Z.m.Z.m.Z...d.
 00000060: 6404 6c09 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c  d.l.m.Z.m.Z.m.Z.
 00000070: 0100 6400 6405 6c0d 6d0e 5a0e 6d0f 5a0f  ..d.d.l.m.Z.m.Z.
```

### Comparing `kuflow_temporal_activity_kuflow-0.7.0/kuflow_temporal_activity_kuflow/utils/__pycache__/_save_task_json_forms_value_data_request_utils.cpython-38.pyc` & `kuflow_temporal_activity_kuflow-0.7.1/kuflow_temporal_activity_kuflow/utils/__pycache__/_save_task_json_forms_value_data_request_utils.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Jun 20 06:25:31 2023 UTC, .py size: 15436 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 5b46 9164 4c3c 0000  U.......[F.dL<..
+00000000: 550d 0d0a 0000 0000 3d53 9164 4c3c 0000  U.......=S.dL<..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 be00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 0100 6400 6402 6c04 6d05 5a05 6d04 5a04  ..d.d.l.m.Z.m.Z.
 00000050: 0100 6400 6403 6c06 6d07 5a07 6d08 5a08  ..d.d.l.m.Z.m.Z.
 00000060: 6d09 5a09 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c  m.Z.m.Z.m.Z.m.Z.
 00000070: 6d0d 5a0d 6d0e 5a0e 6d0f 5a0f 6d10 5a10  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `kuflow_temporal_activity_kuflow-0.7.0/kuflow_temporal_activity_kuflow/utils/_save_process_element_utils.py` & `kuflow_temporal_activity_kuflow-0.7.1/kuflow_temporal_activity_kuflow/utils/_save_process_element_utils.py`

 * *Files identical despite different names*

### Comparing `kuflow_temporal_activity_kuflow-0.7.0/kuflow_temporal_activity_kuflow/utils/_save_task_element_utils.py` & `kuflow_temporal_activity_kuflow-0.7.1/kuflow_temporal_activity_kuflow/utils/_save_task_element_utils.py`

 * *Files identical despite different names*

### Comparing `kuflow_temporal_activity_kuflow-0.7.0/kuflow_temporal_activity_kuflow/utils/_save_task_json_forms_value_data_request_utils.py` & `kuflow_temporal_activity_kuflow-0.7.1/kuflow_temporal_activity_kuflow/utils/_save_task_json_forms_value_data_request_utils.py`

 * *Files identical despite different names*

### Comparing `kuflow_temporal_activity_kuflow-0.7.0/pyproject.toml` & `kuflow_temporal_activity_kuflow-0.7.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kuflow-temporal-activity-kuflow"
-version = "0.7.0"
+version = "0.7.1"
 description = "KuFlow SDK :: Temporal.io activities to interact with KuFlow"
 license = "MIT"
 authors = ["KuFlow S.L. <kuflow@kuflow.com>"]
 homepage = "https://kuflow.com/"
 documentation = "https://docs.kuflow.com/"
 repository = "https://github.com/kuflow/kuflow-sdk-python"
 readme = "README.md"
@@ -13,19 +13,18 @@
 
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-kuflow-temporal-common = "^0.7.0"
+kuflow-temporal-common = "^0.7.1"
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.3.0"
-ipython = "^7.34.0"
 flake8 = "^5.0.4"
 black = "^23.3.0"
 pytest = "^7.3.1"
 pyyaml = "^6.0"
 
 [tool.pytest.ini_options]
 log_cli = true
```

### Comparing `kuflow_temporal_activity_kuflow-0.7.0/setup.py` & `kuflow_temporal_activity_kuflow-0.7.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,19 +6,19 @@
  'kuflow_temporal_activity_kuflow.models',
  'kuflow_temporal_activity_kuflow.utils']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['kuflow-temporal-common>=0.7.0,<0.8.0']
+['kuflow-temporal-common>=0.7.1,<0.8.0']
 
 setup_kwargs = {
     'name': 'kuflow-temporal-activity-kuflow',
-    'version': '0.7.0',
+    'version': '0.7.1',
     'description': 'KuFlow SDK :: Temporal.io activities to interact with KuFlow',
     'long_description': '[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://github.com/kuflow/kuflow-sdk-python/blob/master/LICENSE)\n[![Python](https://img.shields.io/pypi/pyversions/kuflow-temporal-activity-kuflow.svg)](https://pypi.org/project/kuflow-temporal-activity-kuflow)\n[![PyPI](https://img.shields.io/pypi/v/kuflow-temporal-activity-kuflow.svg)](https://pypi.org/project/kuflow-temporal-activity-kuflow)\n\n# KuFlow Temporal Activities KuFlow\n\nTemporal.io activities to interact with KuFlow\n\n## Documentation\n\nMore detailed docs are available in the [documentation pages](https://docs.kuflow.com/developers/).\n\n## Contributing\n\nWe are happy to receive your help and comments, together we will dance a wonderful KuFlow. Please review our [contribution guide](CONTRIBUTING.md).\n\n## License\n\n[MIT License](https://github.com/kuflow/kuflow-sdk-python/blob/master/LICENSE)\n',
     'author': 'KuFlow S.L.',
     'author_email': 'kuflow@kuflow.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://kuflow.com/',
```

### Comparing `kuflow_temporal_activity_kuflow-0.7.0/PKG-INFO` & `kuflow_temporal_activity_kuflow-0.7.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: kuflow-temporal-activity-kuflow
-Version: 0.7.0
+Version: 0.7.1
 Summary: KuFlow SDK :: Temporal.io activities to interact with KuFlow
 Home-page: https://kuflow.com/
 License: MIT
 Author: KuFlow S.L.
 Author-email: kuflow@kuflow.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: kuflow-temporal-common (>=0.7.0,<0.8.0)
+Requires-Dist: kuflow-temporal-common (>=0.7.1,<0.8.0)
 Project-URL: Documentation, https://docs.kuflow.com/
 Project-URL: Repository, https://github.com/kuflow/kuflow-sdk-python
 Description-Content-Type: text/markdown
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://github.com/kuflow/kuflow-sdk-python/blob/master/LICENSE)
 [![Python](https://img.shields.io/pypi/pyversions/kuflow-temporal-activity-kuflow.svg)](https://pypi.org/project/kuflow-temporal-activity-kuflow)
 [![PyPI](https://img.shields.io/pypi/v/kuflow-temporal-activity-kuflow.svg)](https://pypi.org/project/kuflow-temporal-activity-kuflow)
```

