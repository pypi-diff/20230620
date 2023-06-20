# Comparing `tmp/devcycle-python-server-sdk-2.0.0.tar.gz` & `tmp/devcycle-python-server-sdk-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devcycle-python-server-sdk-2.0.0.tar", last modified: Tue Jun 13 17:45:43 2023, max compression
+gzip compressed data, was "devcycle-python-server-sdk-2.0.1.tar", last modified: Tue Jun 20 18:48:38 2023, max compression
```

## Comparing `devcycle-python-server-sdk-2.0.0.tar` & `devcycle-python-server-sdk-2.0.1.tar`

### file list

```diff
@@ -1,39 +1,56 @@
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-06-13 17:45:43.851686 devcycle-python-server-sdk-2.0.0/
--rw-r--r--   0 chris      (501) staff       (20)     1071 2023-06-01 17:48:25.000000 devcycle-python-server-sdk-2.0.0/LICENSE
--rw-r--r--   0 chris      (501) staff       (20)      277 2023-06-13 17:45:43.851748 devcycle-python-server-sdk-2.0.0/PKG-INFO
--rw-r--r--   0 chris      (501) staff       (20)     2013 2023-06-13 17:41:34.000000 devcycle-python-server-sdk-2.0.0/README.md
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-06-13 17:45:43.848900 devcycle-python-server-sdk-2.0.0/devcycle_python_sdk/
--rw-r--r--   0 chris      (501) staff       (20)        5 2023-06-13 17:44:48.000000 devcycle-python-server-sdk-2.0.0/devcycle_python_sdk/VERSION.txt
--rw-r--r--   0 chris      (501) staff       (20)      186 2023-06-13 17:41:34.000000 devcycle-python-server-sdk-2.0.0/devcycle_python_sdk/__init__.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-06-13 17:45:43.849181 devcycle-python-server-sdk-2.0.0/devcycle_python_sdk/api/
--rw-r--r--   0 chris      (501) staff       (20)        1 2023-06-13 17:41:34.000000 devcycle-python-server-sdk-2.0.0/devcycle_python_sdk/api/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)     5186 2023-06-13 17:41:34.000000 devcycle-python-server-sdk-2.0.0/devcycle_python_sdk/api/bucketing_client.py
--rw-r--r--   0 chris      (501) staff       (20)     5637 2023-06-13 17:41:34.000000 devcycle-python-server-sdk-2.0.0/devcycle_python_sdk/dvc_cloud_client.py
--rw-r--r--   0 chris      (501) staff       (20)      783 2023-06-13 17:41:34.000000 devcycle-python-server-sdk-2.0.0/devcycle_python_sdk/dvc_options.py
--rw-r--r--   0 chris      (501) staff       (20)      522 2023-06-13 17:41:34.000000 devcycle-python-server-sdk-2.0.0/devcycle_python_sdk/exceptions.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-06-13 17:45:43.849898 devcycle-python-server-sdk-2.0.0/devcycle_python_sdk/models/
--rw-r--r--   0 chris      (501) staff       (20)        0 2023-06-13 17:41:34.000000 devcycle-python-server-sdk-2.0.0/devcycle_python_sdk/models/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)      442 2023-06-13 17:41:34.000000 devcycle-python-server-sdk-2.0.0/devcycle_python_sdk/models/error_response.py
--rw-r--r--   0 chris      (501) staff       (20)      551 2023-06-13 17:41:34.000000 devcycle-python-server-sdk-2.0.0/devcycle_python_sdk/models/event.py
--rw-r--r--   0 chris      (501) staff       (20)      480 2023-06-13 17:41:34.000000 devcycle-python-server-sdk-2.0.0/devcycle_python_sdk/models/feature.py
--rw-r--r--   0 chris      (501) staff       (20)     1002 2023-06-13 17:41:34.000000 devcycle-python-server-sdk-2.0.0/devcycle_python_sdk/models/user.py
--rw-r--r--   0 chris      (501) staff       (20)     1380 2023-06-13 17:41:34.000000 devcycle-python-server-sdk-2.0.0/devcycle_python_sdk/models/variable.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-06-13 17:45:43.850155 devcycle-python-server-sdk-2.0.0/devcycle_python_sdk/util/
--rw-r--r--   0 chris      (501) staff       (20)        1 2023-06-13 17:41:34.000000 devcycle-python-server-sdk-2.0.0/devcycle_python_sdk/util/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)      253 2023-06-13 17:41:34.000000 devcycle-python-server-sdk-2.0.0/devcycle_python_sdk/util/version.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-06-13 17:45:43.850713 devcycle-python-server-sdk-2.0.0/devcycle_python_server_sdk.egg-info/
--rw-r--r--   0 chris      (501) staff       (20)      277 2023-06-13 17:45:43.000000 devcycle-python-server-sdk-2.0.0/devcycle_python_server_sdk.egg-info/PKG-INFO
--rw-r--r--   0 chris      (501) staff       (20)      980 2023-06-13 17:45:43.000000 devcycle-python-server-sdk-2.0.0/devcycle_python_server_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 chris      (501) staff       (20)        1 2023-06-13 17:45:43.000000 devcycle-python-server-sdk-2.0.0/devcycle_python_server_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 chris      (501) staff       (20)       75 2023-06-13 17:45:43.000000 devcycle-python-server-sdk-2.0.0/devcycle_python_server_sdk.egg-info/requires.txt
--rw-r--r--   0 chris      (501) staff       (20)       33 2023-06-13 17:45:43.000000 devcycle-python-server-sdk-2.0.0/devcycle_python_server_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-06-13 17:45:43.850899 devcycle-python-server-sdk-2.0.0/example/
--rw-r--r--   0 chris      (501) staff       (20)        0 2023-06-01 17:48:25.000000 devcycle-python-server-sdk-2.0.0/example/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)     2289 2023-06-13 17:41:34.000000 devcycle-python-server-sdk-2.0.0/example/example.py
--rw-r--r--   0 chris      (501) staff       (20)       79 2023-06-13 17:45:43.851930 devcycle-python-server-sdk-2.0.0/setup.cfg
--rw-r--r--   0 chris      (501) staff       (20)      853 2023-06-13 17:41:34.000000 devcycle-python-server-sdk-2.0.0/setup.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-06-13 17:45:43.851442 devcycle-python-server-sdk-2.0.0/test/
--rw-r--r--   0 chris      (501) staff       (20)        0 2023-06-01 17:48:25.000000 devcycle-python-server-sdk-2.0.0/test/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)     7285 2023-06-13 17:41:34.000000 devcycle-python-server-sdk-2.0.0/test/test_bucketing_client.py
--rw-r--r--   0 chris      (501) staff       (20)    11559 2023-06-13 17:41:34.000000 devcycle-python-server-sdk-2.0.0/test/test_dvc_cloud_client.py
--rw-r--r--   0 chris      (501) staff       (20)      368 2023-06-13 17:42:32.000000 devcycle-python-server-sdk-2.0.0/test/test_version.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-06-20 18:48:38.098317 devcycle-python-server-sdk-2.0.1/
+-rw-r--r--   0 chris      (501) staff       (20)     1071 2023-06-01 17:48:25.000000 devcycle-python-server-sdk-2.0.1/LICENSE
+-rw-r--r--   0 chris      (501) staff       (20)      277 2023-06-20 18:48:38.098387 devcycle-python-server-sdk-2.0.1/PKG-INFO
+-rw-r--r--   0 chris      (501) staff       (20)     2013 2023-06-20 18:40:44.000000 devcycle-python-server-sdk-2.0.1/README.md
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-06-20 18:48:38.093218 devcycle-python-server-sdk-2.0.1/devcycle_python_sdk/
+-rw-r--r--   0 chris      (501) staff       (20)        5 2023-06-20 18:46:37.000000 devcycle-python-server-sdk-2.0.1/devcycle_python_sdk/VERSION.txt
+-rw-r--r--   0 chris      (501) staff       (20)      277 2023-06-15 17:15:50.000000 devcycle-python-server-sdk-2.0.1/devcycle_python_sdk/__init__.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-06-20 18:48:38.093779 devcycle-python-server-sdk-2.0.1/devcycle_python_sdk/api/
+-rw-r--r--   0 chris      (501) staff       (20)        1 2023-06-13 17:41:34.000000 devcycle-python-server-sdk-2.0.1/devcycle_python_sdk/api/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)     5186 2023-06-13 17:41:34.000000 devcycle-python-server-sdk-2.0.1/devcycle_python_sdk/api/bucketing_client.py
+-rw-r--r--   0 chris      (501) staff       (20)      115 2023-06-20 18:40:44.000000 devcycle-python-server-sdk-2.0.1/devcycle_python_sdk/api/local_bucketing.py
+-rw-r--r--   0 chris      (501) staff       (20)     5637 2023-06-13 17:41:34.000000 devcycle-python-server-sdk-2.0.1/devcycle_python_sdk/dvc_cloud_client.py
+-rw-r--r--   0 chris      (501) staff       (20)     5357 2023-06-20 18:40:44.000000 devcycle-python-server-sdk-2.0.1/devcycle_python_sdk/dvc_local_client.py
+-rw-r--r--   0 chris      (501) staff       (20)     2028 2023-06-20 18:40:44.000000 devcycle-python-server-sdk-2.0.1/devcycle_python_sdk/dvc_options.py
+-rw-r--r--   0 chris      (501) staff       (20)      522 2023-06-13 17:41:34.000000 devcycle-python-server-sdk-2.0.1/devcycle_python_sdk/exceptions.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-06-20 18:48:38.094282 devcycle-python-server-sdk-2.0.1/devcycle_python_sdk/managers/
+-rw-r--r--   0 chris      (501) staff       (20)        0 2023-06-15 17:15:50.000000 devcycle-python-server-sdk-2.0.1/devcycle_python_sdk/managers/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)      720 2023-06-16 18:06:24.000000 devcycle-python-server-sdk-2.0.1/devcycle_python_sdk/managers/config_manager.py
+-rw-r--r--   0 chris      (501) staff       (20)      495 2023-06-15 17:15:50.000000 devcycle-python-server-sdk-2.0.1/devcycle_python_sdk/managers/event_queue_manager.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-06-20 18:48:38.095247 devcycle-python-server-sdk-2.0.1/devcycle_python_sdk/models/
+-rw-r--r--   0 chris      (501) staff       (20)        0 2023-06-13 17:41:34.000000 devcycle-python-server-sdk-2.0.1/devcycle_python_sdk/models/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)      442 2023-06-13 17:41:34.000000 devcycle-python-server-sdk-2.0.1/devcycle_python_sdk/models/error_response.py
+-rw-r--r--   0 chris      (501) staff       (20)      551 2023-06-13 17:41:34.000000 devcycle-python-server-sdk-2.0.1/devcycle_python_sdk/models/event.py
+-rw-r--r--   0 chris      (501) staff       (20)      480 2023-06-13 17:41:34.000000 devcycle-python-server-sdk-2.0.1/devcycle_python_sdk/models/feature.py
+-rw-r--r--   0 chris      (501) staff       (20)     1002 2023-06-20 18:40:44.000000 devcycle-python-server-sdk-2.0.1/devcycle_python_sdk/models/user.py
+-rw-r--r--   0 chris      (501) staff       (20)     1380 2023-06-13 17:41:34.000000 devcycle-python-server-sdk-2.0.1/devcycle_python_sdk/models/variable.py
+-rw-r--r--   0 chris      (501) staff       (20)        0 2023-06-20 17:48:34.000000 devcycle-python-server-sdk-2.0.1/devcycle_python_sdk/py.typed
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-06-20 18:48:38.095514 devcycle-python-server-sdk-2.0.1/devcycle_python_sdk/util/
+-rw-r--r--   0 chris      (501) staff       (20)        1 2023-06-13 17:41:34.000000 devcycle-python-server-sdk-2.0.1/devcycle_python_sdk/util/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)      253 2023-06-13 17:41:34.000000 devcycle-python-server-sdk-2.0.1/devcycle_python_sdk/util/version.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-06-20 18:48:38.096095 devcycle-python-server-sdk-2.0.1/devcycle_python_server_sdk.egg-info/
+-rw-r--r--   0 chris      (501) staff       (20)      277 2023-06-20 18:48:38.000000 devcycle-python-server-sdk-2.0.1/devcycle_python_server_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 chris      (501) staff       (20)     1452 2023-06-20 18:48:38.000000 devcycle-python-server-sdk-2.0.1/devcycle_python_server_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 chris      (501) staff       (20)        1 2023-06-20 18:48:38.000000 devcycle-python-server-sdk-2.0.1/devcycle_python_server_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 chris      (501) staff       (20)       52 2023-06-20 18:48:38.000000 devcycle-python-server-sdk-2.0.1/devcycle_python_server_sdk.egg-info/requires.txt
+-rw-r--r--   0 chris      (501) staff       (20)       33 2023-06-20 18:48:38.000000 devcycle-python-server-sdk-2.0.1/devcycle_python_server_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-06-20 18:48:38.096290 devcycle-python-server-sdk-2.0.1/example/
+-rw-r--r--   0 chris      (501) staff       (20)        0 2023-06-01 17:48:25.000000 devcycle-python-server-sdk-2.0.1/example/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)     2289 2023-06-13 17:41:34.000000 devcycle-python-server-sdk-2.0.1/example/example.py
+-rw-r--r--   0 chris      (501) staff       (20)       79 2023-06-20 18:48:38.098597 devcycle-python-server-sdk-2.0.1/setup.cfg
+-rw-r--r--   0 chris      (501) staff       (20)      890 2023-06-20 17:48:34.000000 devcycle-python-server-sdk-2.0.1/setup.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-06-20 18:48:38.096656 devcycle-python-server-sdk-2.0.1/test/
+-rw-r--r--   0 chris      (501) staff       (20)        0 2023-06-01 17:48:25.000000 devcycle-python-server-sdk-2.0.1/test/__init__.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-06-20 18:48:38.097155 devcycle-python-server-sdk-2.0.1/test/api/
+-rw-r--r--   0 chris      (501) staff       (20)        0 2023-06-15 17:15:50.000000 devcycle-python-server-sdk-2.0.1/test/api/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)     7285 2023-06-15 17:15:50.000000 devcycle-python-server-sdk-2.0.1/test/api/test_bucketing_client.py
+-rw-r--r--   0 chris      (501) staff       (20)      348 2023-06-15 17:15:50.000000 devcycle-python-server-sdk-2.0.1/test/api/test_local_bucketing.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-06-20 18:48:38.097780 devcycle-python-server-sdk-2.0.1/test/managers/
+-rw-r--r--   0 chris      (501) staff       (20)        0 2023-06-15 17:15:50.000000 devcycle-python-server-sdk-2.0.1/test/managers/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)      396 2023-06-16 18:06:24.000000 devcycle-python-server-sdk-2.0.1/test/managers/test_config_manager.py
+-rw-r--r--   0 chris      (501) staff       (20)      372 2023-06-15 17:15:50.000000 devcycle-python-server-sdk-2.0.1/test/managers/test_event_queue_manager.py
+-rw-r--r--   0 chris      (501) staff       (20)    11559 2023-06-13 17:41:34.000000 devcycle-python-server-sdk-2.0.1/test/test_dvc_cloud_client.py
+-rw-r--r--   0 chris      (501) staff       (20)     4806 2023-06-16 18:06:24.000000 devcycle-python-server-sdk-2.0.1/test/test_dvc_local_client.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-06-20 18:48:38.098078 devcycle-python-server-sdk-2.0.1/test/util/
+-rw-r--r--   0 chris      (501) staff       (20)        0 2023-06-15 17:15:50.000000 devcycle-python-server-sdk-2.0.1/test/util/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)      368 2023-06-20 18:46:37.000000 devcycle-python-server-sdk-2.0.1/test/util/test_version.py
```

### Comparing `devcycle-python-server-sdk-2.0.0/LICENSE` & `devcycle-python-server-sdk-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-2.0.0/README.md` & `devcycle-python-server-sdk-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-2.0.0/devcycle_python_sdk/api/bucketing_client.py` & `devcycle-python-server-sdk-2.0.1/devcycle_python_sdk/api/bucketing_client.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-2.0.0/devcycle_python_sdk/dvc_cloud_client.py` & `devcycle-python-server-sdk-2.0.1/devcycle_python_sdk/dvc_cloud_client.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-2.0.0/devcycle_python_sdk/exceptions.py` & `devcycle-python-server-sdk-2.0.1/devcycle_python_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-2.0.0/devcycle_python_sdk/models/event.py` & `devcycle-python-server-sdk-2.0.1/devcycle_python_sdk/models/event.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-2.0.0/devcycle_python_sdk/models/user.py` & `devcycle-python-server-sdk-2.0.1/devcycle_python_sdk/models/user.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-2.0.0/devcycle_python_sdk/models/variable.py` & `devcycle-python-server-sdk-2.0.1/devcycle_python_sdk/models/variable.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-2.0.0/example/example.py` & `devcycle-python-server-sdk-2.0.1/example/example.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-2.0.0/setup.py` & `devcycle-python-server-sdk-2.0.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,13 +21,13 @@
     version=VERSION,
     description="DevCycle Python SDK",
     author_email="",
     url="https://github.com/devcycleHQ/python-server-sdk",
     keywords=["DevCycle"],
     install_requires=REQUIRES,
     packages=find_packages(),
-    package_data={"": ["VERSION.txt"]},
+    package_data={"": ["VERSION.txt"], "devcycle_python_sdk": ["py.typed"]},
     include_package_data=True,
     long_description="""\
     The DevCycle Python SDK used for feature management.
     """,
 )
```

### Comparing `devcycle-python-server-sdk-2.0.0/test/test_bucketing_client.py` & `devcycle-python-server-sdk-2.0.1/test/api/test_bucketing_client.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-2.0.0/test/test_dvc_cloud_client.py` & `devcycle-python-server-sdk-2.0.1/test/test_dvc_cloud_client.py`

 * *Files identical despite different names*

