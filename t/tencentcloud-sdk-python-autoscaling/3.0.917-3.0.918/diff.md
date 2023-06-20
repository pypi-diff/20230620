# Comparing `tmp/tencentcloud-sdk-python-autoscaling-3.0.917.tar.gz` & `tmp/tencentcloud-sdk-python-autoscaling-3.0.918.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-autoscaling-3.0.917.tar", last modified: Mon Jun 19 00:18:00 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-autoscaling-3.0.918.tar", last modified: Tue Jun 20 02:33:07 2023, max compression
```

## Comparing `tencentcloud-sdk-python-autoscaling-3.0.917.tar` & `tencentcloud-sdk-python-autoscaling-3.0.918.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:18:00.000000 tencentcloud-sdk-python-autoscaling-3.0.917/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:18:00.000000 tencentcloud-sdk-python-autoscaling-3.0.917/tencentcloud_sdk_python_autoscaling.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-19 00:18:00.000000 tencentcloud-sdk-python-autoscaling-3.0.917/tencentcloud_sdk_python_autoscaling.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      525 2023-06-19 00:18:00.000000 tencentcloud-sdk-python-autoscaling-3.0.917/tencentcloud_sdk_python_autoscaling.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1699 2023-06-19 00:18:00.000000 tencentcloud-sdk-python-autoscaling-3.0.917/tencentcloud_sdk_python_autoscaling.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-19 00:18:00.000000 tencentcloud-sdk-python-autoscaling-3.0.917/tencentcloud_sdk_python_autoscaling.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-19 00:18:00.000000 tencentcloud-sdk-python-autoscaling-3.0.917/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:18:00.000000 tencentcloud-sdk-python-autoscaling-3.0.917/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-19 00:18:00.000000 tencentcloud-sdk-python-autoscaling-3.0.917/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:18:00.000000 tencentcloud-sdk-python-autoscaling-3.0.917/tencentcloud/autoscaling/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 00:18:00.000000 tencentcloud-sdk-python-autoscaling-3.0.917/tencentcloud/autoscaling/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:18:00.000000 tencentcloud-sdk-python-autoscaling-3.0.917/tencentcloud/autoscaling/v20180419/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 00:18:00.000000 tencentcloud-sdk-python-autoscaling-3.0.917/tencentcloud/autoscaling/v20180419/__init__.py
--rw-r--r--   0 root         (0) root         (0)   258716 2023-06-19 00:18:00.000000 tencentcloud-sdk-python-autoscaling-3.0.917/tencentcloud/autoscaling/v20180419/models.py
--rw-r--r--   0 root         (0) root         (0)    19836 2023-06-19 00:18:00.000000 tencentcloud-sdk-python-autoscaling-3.0.917/tencentcloud/autoscaling/v20180419/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    60526 2023-06-19 00:18:00.000000 tencentcloud-sdk-python-autoscaling-3.0.917/tencentcloud/autoscaling/v20180419/autoscaling_client.py
--rw-r--r--   0 root         (0) root         (0)      761 2023-06-19 00:18:00.000000 tencentcloud-sdk-python-autoscaling-3.0.917/README.rst
--rw-r--r--   0 root         (0) root         (0)     1699 2023-06-19 00:18:00.000000 tencentcloud-sdk-python-autoscaling-3.0.917/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1022 2023-06-19 00:18:00.000000 tencentcloud-sdk-python-autoscaling-3.0.917/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:33:07.000000 tencentcloud-sdk-python-autoscaling-3.0.918/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:33:07.000000 tencentcloud-sdk-python-autoscaling-3.0.918/tencentcloud_sdk_python_autoscaling.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 02:33:07.000000 tencentcloud-sdk-python-autoscaling-3.0.918/tencentcloud_sdk_python_autoscaling.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      525 2023-06-20 02:33:07.000000 tencentcloud-sdk-python-autoscaling-3.0.918/tencentcloud_sdk_python_autoscaling.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1699 2023-06-20 02:33:07.000000 tencentcloud-sdk-python-autoscaling-3.0.918/tencentcloud_sdk_python_autoscaling.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-20 02:33:07.000000 tencentcloud-sdk-python-autoscaling-3.0.918/tencentcloud_sdk_python_autoscaling.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-20 02:33:07.000000 tencentcloud-sdk-python-autoscaling-3.0.918/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:33:07.000000 tencentcloud-sdk-python-autoscaling-3.0.918/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-20 02:33:07.000000 tencentcloud-sdk-python-autoscaling-3.0.918/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:33:07.000000 tencentcloud-sdk-python-autoscaling-3.0.918/tencentcloud/autoscaling/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 02:33:07.000000 tencentcloud-sdk-python-autoscaling-3.0.918/tencentcloud/autoscaling/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:33:07.000000 tencentcloud-sdk-python-autoscaling-3.0.918/tencentcloud/autoscaling/v20180419/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 02:33:07.000000 tencentcloud-sdk-python-autoscaling-3.0.918/tencentcloud/autoscaling/v20180419/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   258716 2023-06-20 02:33:07.000000 tencentcloud-sdk-python-autoscaling-3.0.918/tencentcloud/autoscaling/v20180419/models.py
+-rw-r--r--   0 root         (0) root         (0)    19989 2023-06-20 02:33:07.000000 tencentcloud-sdk-python-autoscaling-3.0.918/tencentcloud/autoscaling/v20180419/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    60526 2023-06-20 02:33:07.000000 tencentcloud-sdk-python-autoscaling-3.0.918/tencentcloud/autoscaling/v20180419/autoscaling_client.py
+-rw-r--r--   0 root         (0) root         (0)      761 2023-06-20 02:33:07.000000 tencentcloud-sdk-python-autoscaling-3.0.918/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1699 2023-06-20 02:33:07.000000 tencentcloud-sdk-python-autoscaling-3.0.918/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1022 2023-06-20 02:33:07.000000 tencentcloud-sdk-python-autoscaling-3.0.918/setup.py
```

### Comparing `tencentcloud-sdk-python-autoscaling-3.0.917/tencentcloud_sdk_python_autoscaling.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-autoscaling-3.0.918/tencentcloud_sdk_python_autoscaling.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-autoscaling-3.0.917/tencentcloud_sdk_python_autoscaling.egg-info/PKG-INFO` & `tencentcloud-sdk-python-autoscaling-3.0.918/tencentcloud_sdk_python_autoscaling.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-autoscaling
-Version: 3.0.917
+Version: 3.0.918
 Summary: Tencent Cloud Autoscaling SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-autoscaling-3.0.917/tencentcloud/__init__.py` & `tencentcloud-sdk-python-autoscaling-3.0.918/tencentcloud/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.917'
+__version__ = '3.0.918'
```

### Comparing `tencentcloud-sdk-python-autoscaling-3.0.917/tencentcloud/autoscaling/v20180419/models.py` & `tencentcloud-sdk-python-autoscaling-3.0.918/tencentcloud/autoscaling/v20180419/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-autoscaling-3.0.917/tencentcloud/autoscaling/v20180419/errorcodes.py` & `tencentcloud-sdk-python-autoscaling-3.0.918/tencentcloud/autoscaling/v20180419/errorcodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -232,14 +232,17 @@
 
 # 生命周期挂钩名称重复。
 INVALIDPARAMETERVALUE_LIFECYCLEHOOKNAMEDUPLICATED = 'InvalidParameterValue.LifecycleHookNameDuplicated'
 
 # 取值超出限制。
 INVALIDPARAMETERVALUE_LIMITEXCEEDED = 'InvalidParameterValue.LimitExceeded'
 
+# 不支持目标组类型的监听器。
+INVALIDPARAMETERVALUE_LISTENERTARGETTYPENOTSUPPORTED = 'InvalidParameterValue.ListenerTargetTypeNotSupported'
+
 # 当前账户在带宽包模式中必须填写带宽包ID参数。
 INVALIDPARAMETERVALUE_MISSINGBANDWIDTHPACKAGEID = 'InvalidParameterValue.MissingBandwidthPackageId'
 
 # 无资源权限。
 INVALIDPARAMETERVALUE_NORESOURCEPERMISSION = 'InvalidParameterValue.NoResourcePermission'
 
 # 提供的值不是浮点字符串格式。
```

### Comparing `tencentcloud-sdk-python-autoscaling-3.0.917/tencentcloud/autoscaling/v20180419/autoscaling_client.py` & `tencentcloud-sdk-python-autoscaling-3.0.918/tencentcloud/autoscaling/v20180419/autoscaling_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-autoscaling-3.0.917/README.rst` & `tencentcloud-sdk-python-autoscaling-3.0.918/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-autoscaling-3.0.917/PKG-INFO` & `tencentcloud-sdk-python-autoscaling-3.0.918/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-autoscaling
-Version: 3.0.917
+Version: 3.0.918
 Summary: Tencent Cloud Autoscaling SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-autoscaling-3.0.917/setup.py` & `tencentcloud-sdk-python-autoscaling-3.0.918/setup.py`

 * *Files identical despite different names*

