# Comparing `tmp/aliyun-python-sdk-bpstudio-1.0.2.tar.gz` & `tmp/aliyun-python-sdk-bpstudio-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-bpstudio-1.0.2.tar", last modified: Mon May 22 09:05:24 2023, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-bpstudio-1.0.3.tar", last modified: Tue Jun 20 03:07:41 2023, max compression
```

## Comparing `aliyun-python-sdk-bpstudio-1.0.2.tar` & `aliyun-python-sdk-bpstudio-1.0.3.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 09:05:24.000000 aliyun-python-sdk-bpstudio-1.0.2/
--rw-r--r--   0 root         (0) root         (0)      575 2023-05-22 09:05:24.000000 aliyun-python-sdk-bpstudio-1.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       40 2023-05-22 09:05:24.000000 aliyun-python-sdk-bpstudio-1.0.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1562 2023-05-22 09:05:24.000000 aliyun-python-sdk-bpstudio-1.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      537 2023-05-22 09:05:24.000000 aliyun-python-sdk-bpstudio-1.0.2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 09:05:24.000000 aliyun-python-sdk-bpstudio-1.0.2/aliyun_python_sdk_bpstudio.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1562 2023-05-22 09:05:24.000000 aliyun-python-sdk-bpstudio-1.0.2/aliyun_python_sdk_bpstudio.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1366 2023-05-22 09:05:24.000000 aliyun-python-sdk-bpstudio-1.0.2/aliyun_python_sdk_bpstudio.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 09:05:24.000000 aliyun-python-sdk-bpstudio-1.0.2/aliyun_python_sdk_bpstudio.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-05-22 09:05:24.000000 aliyun-python-sdk-bpstudio-1.0.2/aliyun_python_sdk_bpstudio.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-05-22 09:05:24.000000 aliyun-python-sdk-bpstudio-1.0.2/aliyun_python_sdk_bpstudio.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 09:05:24.000000 aliyun-python-sdk-bpstudio-1.0.2/aliyunsdkbpstudio/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-22 09:05:24.000000 aliyun-python-sdk-bpstudio-1.0.2/aliyunsdkbpstudio/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 09:05:24.000000 aliyun-python-sdk-bpstudio-1.0.2/aliyunsdkbpstudio/request/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-22 09:05:24.000000 aliyun-python-sdk-bpstudio-1.0.2/aliyunsdkbpstudio/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 09:05:24.000000 aliyun-python-sdk-bpstudio-1.0.2/aliyunsdkbpstudio/request/v20210931/
--rw-r--r--   0 root         (0) root         (0)     1654 2023-05-22 09:05:24.000000 aliyun-python-sdk-bpstudio-1.0.2/aliyunsdkbpstudio/request/v20210931/ChangeResourceGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     2556 2023-05-22 09:05:24.000000 aliyun-python-sdk-bpstudio-1.0.2/aliyunsdkbpstudio/request/v20210931/CreateApplicationRequest.py
--rw-r--r--   0 root         (0) root         (0)     1448 2023-05-22 09:05:24.000000 aliyun-python-sdk-bpstudio-1.0.2/aliyunsdkbpstudio/request/v20210931/DeleteApplicationRequest.py
--rw-r--r--   0 root         (0) root         (0)     1449 2023-05-22 09:05:24.000000 aliyun-python-sdk-bpstudio-1.0.2/aliyunsdkbpstudio/request/v20210931/DeployApplicationRequest.py
--rw-r--r--   0 root         (0) root         (0)     1818 2023-05-22 09:05:24.000000 aliyun-python-sdk-bpstudio-1.0.2/aliyunsdkbpstudio/request/v20210931/ExecuteOperationASyncRequest.py
--rw-r--r--   0 root         (0) root         (0)     1442 2023-05-22 09:05:24.000000 aliyun-python-sdk-bpstudio-1.0.2/aliyunsdkbpstudio/request/v20210931/GetApplicationRequest.py
--rw-r--r--   0 root         (0) root         (0)     1452 2023-05-22 09:05:24.000000 aliyun-python-sdk-bpstudio-1.0.2/aliyunsdkbpstudio/request/v20210931/GetExecuteOperationResultRequest.py
--rw-r--r--   0 root         (0) root         (0)     1584 2023-05-22 09:05:24.000000 aliyun-python-sdk-bpstudio-1.0.2/aliyunsdkbpstudio/request/v20210931/GetTemplateRequest.py
--rw-r--r--   0 root         (0) root         (0)     1222 2023-05-22 09:05:24.000000 aliyun-python-sdk-bpstudio-1.0.2/aliyunsdkbpstudio/request/v20210931/GetTokenRequest.py
--rw-r--r--   0 root         (0) root         (0)     2132 2023-05-22 09:05:24.000000 aliyun-python-sdk-bpstudio-1.0.2/aliyunsdkbpstudio/request/v20210931/ListApplicationRequest.py
--rw-r--r--   0 root         (0) root         (0)     2245 2023-05-22 09:05:24.000000 aliyun-python-sdk-bpstudio-1.0.2/aliyunsdkbpstudio/request/v20210931/ListTagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2288 2023-05-22 09:05:24.000000 aliyun-python-sdk-bpstudio-1.0.2/aliyunsdkbpstudio/request/v20210931/ListTemplateRequest.py
--rw-r--r--   0 root         (0) root         (0)     1450 2023-05-22 09:05:24.000000 aliyun-python-sdk-bpstudio-1.0.2/aliyunsdkbpstudio/request/v20210931/ReleaseApplicationRequest.py
--rw-r--r--   0 root         (0) root         (0)     1453 2023-05-22 09:05:24.000000 aliyun-python-sdk-bpstudio-1.0.2/aliyunsdkbpstudio/request/v20210931/ValidateApplicationRequest.py
--rw-r--r--   0 root         (0) root         (0)     1450 2023-05-22 09:05:24.000000 aliyun-python-sdk-bpstudio-1.0.2/aliyunsdkbpstudio/request/v20210931/ValuateApplicationRequest.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-22 09:05:24.000000 aliyun-python-sdk-bpstudio-1.0.2/aliyunsdkbpstudio/request/v20210931/__init__.py
--rw-r--r--   0 root         (0) root         (0)      102 2023-05-22 09:05:24.000000 aliyun-python-sdk-bpstudio-1.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2477 2023-05-22 09:05:24.000000 aliyun-python-sdk-bpstudio-1.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 03:07:41.000000 aliyun-python-sdk-bpstudio-1.0.3/
+-rw-r--r--   0 root         (0) root         (0)      575 2023-06-20 03:07:40.000000 aliyun-python-sdk-bpstudio-1.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       40 2023-06-20 03:07:40.000000 aliyun-python-sdk-bpstudio-1.0.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1562 2023-06-20 03:07:41.000000 aliyun-python-sdk-bpstudio-1.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      537 2023-06-20 03:07:40.000000 aliyun-python-sdk-bpstudio-1.0.3/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 03:07:41.000000 aliyun-python-sdk-bpstudio-1.0.3/aliyun_python_sdk_bpstudio.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1562 2023-06-20 03:07:41.000000 aliyun-python-sdk-bpstudio-1.0.3/aliyun_python_sdk_bpstudio.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1428 2023-06-20 03:07:41.000000 aliyun-python-sdk-bpstudio-1.0.3/aliyun_python_sdk_bpstudio.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 03:07:41.000000 aliyun-python-sdk-bpstudio-1.0.3/aliyun_python_sdk_bpstudio.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-06-20 03:07:41.000000 aliyun-python-sdk-bpstudio-1.0.3/aliyun_python_sdk_bpstudio.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-06-20 03:07:41.000000 aliyun-python-sdk-bpstudio-1.0.3/aliyun_python_sdk_bpstudio.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 03:07:41.000000 aliyun-python-sdk-bpstudio-1.0.3/aliyunsdkbpstudio/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-20 03:07:40.000000 aliyun-python-sdk-bpstudio-1.0.3/aliyunsdkbpstudio/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 03:07:41.000000 aliyun-python-sdk-bpstudio-1.0.3/aliyunsdkbpstudio/request/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 03:07:40.000000 aliyun-python-sdk-bpstudio-1.0.3/aliyunsdkbpstudio/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 03:07:41.000000 aliyun-python-sdk-bpstudio-1.0.3/aliyunsdkbpstudio/request/v20210931/
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-06-20 03:07:40.000000 aliyun-python-sdk-bpstudio-1.0.3/aliyunsdkbpstudio/request/v20210931/ChangeResourceGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2556 2023-06-20 03:07:40.000000 aliyun-python-sdk-bpstudio-1.0.3/aliyunsdkbpstudio/request/v20210931/CreateApplicationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1448 2023-06-20 03:07:40.000000 aliyun-python-sdk-bpstudio-1.0.3/aliyunsdkbpstudio/request/v20210931/DeleteApplicationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1449 2023-06-20 03:07:40.000000 aliyun-python-sdk-bpstudio-1.0.3/aliyunsdkbpstudio/request/v20210931/DeployApplicationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1818 2023-06-20 03:07:40.000000 aliyun-python-sdk-bpstudio-1.0.3/aliyunsdkbpstudio/request/v20210931/ExecuteOperationASyncRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1442 2023-06-20 03:07:40.000000 aliyun-python-sdk-bpstudio-1.0.3/aliyunsdkbpstudio/request/v20210931/GetApplicationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1452 2023-06-20 03:07:40.000000 aliyun-python-sdk-bpstudio-1.0.3/aliyunsdkbpstudio/request/v20210931/GetExecuteOperationResultRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1584 2023-06-20 03:07:40.000000 aliyun-python-sdk-bpstudio-1.0.3/aliyunsdkbpstudio/request/v20210931/GetTemplateRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1222 2023-06-20 03:07:40.000000 aliyun-python-sdk-bpstudio-1.0.3/aliyunsdkbpstudio/request/v20210931/GetTokenRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2132 2023-06-20 03:07:40.000000 aliyun-python-sdk-bpstudio-1.0.3/aliyunsdkbpstudio/request/v20210931/ListApplicationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2245 2023-06-20 03:07:40.000000 aliyun-python-sdk-bpstudio-1.0.3/aliyunsdkbpstudio/request/v20210931/ListTagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2288 2023-06-20 03:07:40.000000 aliyun-python-sdk-bpstudio-1.0.3/aliyunsdkbpstudio/request/v20210931/ListTemplateRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1450 2023-06-20 03:07:40.000000 aliyun-python-sdk-bpstudio-1.0.3/aliyunsdkbpstudio/request/v20210931/ReleaseApplicationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1453 2023-06-20 03:07:40.000000 aliyun-python-sdk-bpstudio-1.0.3/aliyunsdkbpstudio/request/v20210931/ValidateApplicationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1450 2023-06-20 03:07:40.000000 aliyun-python-sdk-bpstudio-1.0.3/aliyunsdkbpstudio/request/v20210931/ValuateApplicationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2184 2023-06-20 03:07:40.000000 aliyun-python-sdk-bpstudio-1.0.3/aliyunsdkbpstudio/request/v20210931/ValuateTemplateRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 03:07:40.000000 aliyun-python-sdk-bpstudio-1.0.3/aliyunsdkbpstudio/request/v20210931/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      102 2023-06-20 03:07:41.000000 aliyun-python-sdk-bpstudio-1.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2477 2023-06-20 03:07:40.000000 aliyun-python-sdk-bpstudio-1.0.3/setup.py
```

### Comparing `aliyun-python-sdk-bpstudio-1.0.2/LICENSE` & `aliyun-python-sdk-bpstudio-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bpstudio-1.0.2/PKG-INFO` & `aliyun-python-sdk-bpstudio-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-bpstudio
-Version: 1.0.2
+Version: 1.0.3
 Summary: The bpstudio module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-bpstudio
```

### Comparing `aliyun-python-sdk-bpstudio-1.0.2/README.rst` & `aliyun-python-sdk-bpstudio-1.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bpstudio-1.0.2/aliyun_python_sdk_bpstudio.egg-info/PKG-INFO` & `aliyun-python-sdk-bpstudio-1.0.3/aliyun_python_sdk_bpstudio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-bpstudio
-Version: 1.0.2
+Version: 1.0.3
 Summary: The bpstudio module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-bpstudio
```

### Comparing `aliyun-python-sdk-bpstudio-1.0.2/aliyun_python_sdk_bpstudio.egg-info/SOURCES.txt` & `aliyun-python-sdk-bpstudio-1.0.3/aliyun_python_sdk_bpstudio.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -21,8 +21,9 @@
 aliyunsdkbpstudio/request/v20210931/GetTokenRequest.py
 aliyunsdkbpstudio/request/v20210931/ListApplicationRequest.py
 aliyunsdkbpstudio/request/v20210931/ListTagResourcesRequest.py
 aliyunsdkbpstudio/request/v20210931/ListTemplateRequest.py
 aliyunsdkbpstudio/request/v20210931/ReleaseApplicationRequest.py
 aliyunsdkbpstudio/request/v20210931/ValidateApplicationRequest.py
 aliyunsdkbpstudio/request/v20210931/ValuateApplicationRequest.py
+aliyunsdkbpstudio/request/v20210931/ValuateTemplateRequest.py
 aliyunsdkbpstudio/request/v20210931/__init__.py
```

### Comparing `aliyun-python-sdk-bpstudio-1.0.2/aliyunsdkbpstudio/request/v20210931/ChangeResourceGroupRequest.py` & `aliyun-python-sdk-bpstudio-1.0.3/aliyunsdkbpstudio/request/v20210931/ChangeResourceGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bpstudio-1.0.2/aliyunsdkbpstudio/request/v20210931/CreateApplicationRequest.py` & `aliyun-python-sdk-bpstudio-1.0.3/aliyunsdkbpstudio/request/v20210931/CreateApplicationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bpstudio-1.0.2/aliyunsdkbpstudio/request/v20210931/DeleteApplicationRequest.py` & `aliyun-python-sdk-bpstudio-1.0.3/aliyunsdkbpstudio/request/v20210931/DeleteApplicationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bpstudio-1.0.2/aliyunsdkbpstudio/request/v20210931/DeployApplicationRequest.py` & `aliyun-python-sdk-bpstudio-1.0.3/aliyunsdkbpstudio/request/v20210931/DeployApplicationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bpstudio-1.0.2/aliyunsdkbpstudio/request/v20210931/ExecuteOperationASyncRequest.py` & `aliyun-python-sdk-bpstudio-1.0.3/aliyunsdkbpstudio/request/v20210931/ExecuteOperationASyncRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bpstudio-1.0.2/aliyunsdkbpstudio/request/v20210931/GetApplicationRequest.py` & `aliyun-python-sdk-bpstudio-1.0.3/aliyunsdkbpstudio/request/v20210931/GetApplicationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bpstudio-1.0.2/aliyunsdkbpstudio/request/v20210931/GetExecuteOperationResultRequest.py` & `aliyun-python-sdk-bpstudio-1.0.3/aliyunsdkbpstudio/request/v20210931/GetExecuteOperationResultRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bpstudio-1.0.2/aliyunsdkbpstudio/request/v20210931/GetTemplateRequest.py` & `aliyun-python-sdk-bpstudio-1.0.3/aliyunsdkbpstudio/request/v20210931/GetTemplateRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bpstudio-1.0.2/aliyunsdkbpstudio/request/v20210931/GetTokenRequest.py` & `aliyun-python-sdk-bpstudio-1.0.3/aliyunsdkbpstudio/request/v20210931/GetTokenRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bpstudio-1.0.2/aliyunsdkbpstudio/request/v20210931/ListApplicationRequest.py` & `aliyun-python-sdk-bpstudio-1.0.3/aliyunsdkbpstudio/request/v20210931/ListApplicationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bpstudio-1.0.2/aliyunsdkbpstudio/request/v20210931/ListTagResourcesRequest.py` & `aliyun-python-sdk-bpstudio-1.0.3/aliyunsdkbpstudio/request/v20210931/ListTagResourcesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bpstudio-1.0.2/aliyunsdkbpstudio/request/v20210931/ListTemplateRequest.py` & `aliyun-python-sdk-bpstudio-1.0.3/aliyunsdkbpstudio/request/v20210931/ListTemplateRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bpstudio-1.0.2/aliyunsdkbpstudio/request/v20210931/ReleaseApplicationRequest.py` & `aliyun-python-sdk-bpstudio-1.0.3/aliyunsdkbpstudio/request/v20210931/ReleaseApplicationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bpstudio-1.0.2/aliyunsdkbpstudio/request/v20210931/ValidateApplicationRequest.py` & `aliyun-python-sdk-bpstudio-1.0.3/aliyunsdkbpstudio/request/v20210931/ValidateApplicationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bpstudio-1.0.2/aliyunsdkbpstudio/request/v20210931/ValuateApplicationRequest.py` & `aliyun-python-sdk-bpstudio-1.0.3/aliyunsdkbpstudio/request/v20210931/ValuateApplicationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-bpstudio-1.0.2/setup.py` & `aliyun-python-sdk-bpstudio-1.0.3/setup.py`

 * *Files identical despite different names*

