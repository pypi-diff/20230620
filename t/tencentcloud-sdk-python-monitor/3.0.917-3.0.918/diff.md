# Comparing `tmp/tencentcloud-sdk-python-monitor-3.0.917.tar.gz` & `tmp/tencentcloud-sdk-python-monitor-3.0.918.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-monitor-3.0.917.tar", last modified: Mon Jun 19 00:29:28 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-monitor-3.0.918.tar", last modified: Tue Jun 20 02:44:32 2023, max compression
```

## Comparing `tencentcloud-sdk-python-monitor-3.0.917.tar` & `tencentcloud-sdk-python-monitor-3.0.918.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:29:28.000000 tencentcloud-sdk-python-monitor-3.0.917/
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-19 00:29:28.000000 tencentcloud-sdk-python-monitor-3.0.917/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:29:28.000000 tencentcloud-sdk-python-monitor-3.0.917/tencentcloud_sdk_python_monitor.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-19 00:29:28.000000 tencentcloud-sdk-python-monitor-3.0.917/tencentcloud_sdk_python_monitor.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      485 2023-06-19 00:29:28.000000 tencentcloud-sdk-python-monitor-3.0.917/tencentcloud_sdk_python_monitor.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-06-19 00:29:28.000000 tencentcloud-sdk-python-monitor-3.0.917/tencentcloud_sdk_python_monitor.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-19 00:29:28.000000 tencentcloud-sdk-python-monitor-3.0.917/tencentcloud_sdk_python_monitor.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:29:28.000000 tencentcloud-sdk-python-monitor-3.0.917/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-19 00:29:27.000000 tencentcloud-sdk-python-monitor-3.0.917/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:29:28.000000 tencentcloud-sdk-python-monitor-3.0.917/tencentcloud/monitor/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 00:29:27.000000 tencentcloud-sdk-python-monitor-3.0.917/tencentcloud/monitor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:29:28.000000 tencentcloud-sdk-python-monitor-3.0.917/tencentcloud/monitor/v20180724/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 00:29:27.000000 tencentcloud-sdk-python-monitor-3.0.917/tencentcloud/monitor/v20180724/__init__.py
--rw-r--r--   0 root         (0) root         (0)   554161 2023-06-19 00:29:27.000000 tencentcloud-sdk-python-monitor-3.0.917/tencentcloud/monitor/v20180724/models.py
--rw-r--r--   0 root         (0) root         (0)    10348 2023-06-19 00:29:27.000000 tencentcloud-sdk-python-monitor-3.0.917/tencentcloud/monitor/v20180724/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   144629 2023-06-19 00:29:27.000000 tencentcloud-sdk-python-monitor-3.0.917/tencentcloud/monitor/v20180724/monitor_client.py
--rw-r--r--   0 root         (0) root         (0)      749 2023-06-19 00:29:27.000000 tencentcloud-sdk-python-monitor-3.0.917/README.rst
--rw-r--r--   0 root         (0) root         (0)     1679 2023-06-19 00:29:28.000000 tencentcloud-sdk-python-monitor-3.0.917/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1014 2023-06-19 00:29:27.000000 tencentcloud-sdk-python-monitor-3.0.917/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:44:32.000000 tencentcloud-sdk-python-monitor-3.0.918/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-20 02:44:32.000000 tencentcloud-sdk-python-monitor-3.0.918/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:44:32.000000 tencentcloud-sdk-python-monitor-3.0.918/tencentcloud_sdk_python_monitor.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 02:44:32.000000 tencentcloud-sdk-python-monitor-3.0.918/tencentcloud_sdk_python_monitor.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      485 2023-06-20 02:44:32.000000 tencentcloud-sdk-python-monitor-3.0.918/tencentcloud_sdk_python_monitor.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-06-20 02:44:32.000000 tencentcloud-sdk-python-monitor-3.0.918/tencentcloud_sdk_python_monitor.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-20 02:44:32.000000 tencentcloud-sdk-python-monitor-3.0.918/tencentcloud_sdk_python_monitor.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:44:32.000000 tencentcloud-sdk-python-monitor-3.0.918/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-20 02:44:32.000000 tencentcloud-sdk-python-monitor-3.0.918/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:44:32.000000 tencentcloud-sdk-python-monitor-3.0.918/tencentcloud/monitor/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 02:44:32.000000 tencentcloud-sdk-python-monitor-3.0.918/tencentcloud/monitor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:44:32.000000 tencentcloud-sdk-python-monitor-3.0.918/tencentcloud/monitor/v20180724/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 02:44:32.000000 tencentcloud-sdk-python-monitor-3.0.918/tencentcloud/monitor/v20180724/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   554161 2023-06-20 02:44:32.000000 tencentcloud-sdk-python-monitor-3.0.918/tencentcloud/monitor/v20180724/models.py
+-rw-r--r--   0 root         (0) root         (0)    10348 2023-06-20 02:44:32.000000 tencentcloud-sdk-python-monitor-3.0.918/tencentcloud/monitor/v20180724/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   145047 2023-06-20 02:44:32.000000 tencentcloud-sdk-python-monitor-3.0.918/tencentcloud/monitor/v20180724/monitor_client.py
+-rw-r--r--   0 root         (0) root         (0)      749 2023-06-20 02:44:32.000000 tencentcloud-sdk-python-monitor-3.0.918/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-06-20 02:44:32.000000 tencentcloud-sdk-python-monitor-3.0.918/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-06-20 02:44:32.000000 tencentcloud-sdk-python-monitor-3.0.918/setup.py
```

### Comparing `tencentcloud-sdk-python-monitor-3.0.917/tencentcloud_sdk_python_monitor.egg-info/PKG-INFO` & `tencentcloud-sdk-python-monitor-3.0.918/tencentcloud_sdk_python_monitor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-monitor
-Version: 3.0.917
+Version: 3.0.918
 Summary: Tencent Cloud Monitor SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-monitor-3.0.917/tencentcloud/__init__.py` & `tencentcloud-sdk-python-monitor-3.0.918/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-monitor-3.0.917/tencentcloud/monitor/v20180724/models.py` & `tencentcloud-sdk-python-monitor-3.0.918/tencentcloud/monitor/v20180724/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-monitor-3.0.917/tencentcloud/monitor/v20180724/errorcodes.py` & `tencentcloud-sdk-python-monitor-3.0.918/tencentcloud/monitor/v20180724/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-monitor-3.0.917/tencentcloud/monitor/v20180724/monitor_client.py` & `tencentcloud-sdk-python-monitor-3.0.918/tencentcloud/monitor/v20180724/monitor_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -232,15 +232,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def CreateGrafanaInstance(self, request):
-        """创建 Grafana 实例
+        """本接口（CreateGrafanaInstance）用于创建 Grafana 包年包月实例，默认基础版、到期自动续费、不可使用代金券。
 
         :param request: Request instance for CreateGrafanaInstance.
         :type request: :class:`tencentcloud.monitor.v20180724.models.CreateGrafanaInstanceRequest`
         :rtype: :class:`tencentcloud.monitor.v20180724.models.CreateGrafanaInstanceResponse`
 
         """
         try:
@@ -694,15 +694,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DeleteGrafanaInstance(self, request):
-        """删除 Grafana 实例
+        """本接口（DeleteGrafanaInstance）用于 Grafana 包年包月实例的退费，调用后实例处于停服状态，不可使用，7天后自动销毁。
 
         :param request: Request instance for DeleteGrafanaInstance.
         :type request: :class:`tencentcloud.monitor.v20180724.models.DeleteGrafanaInstanceRequest`
         :rtype: :class:`tencentcloud.monitor.v20180724.models.DeleteGrafanaInstanceResponse`
 
         """
         try:
@@ -2880,15 +2880,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def ResumeGrafanaInstance(self, request):
-        """恢复 Grafana 实例
+        """本接口（ResumeGrafanaInstance）用于 Grafana 包年包月实例的停服续费，调用后按原版本续费一个月。仍在运行中的实例无法使用该接口进行续费。
 
         :param request: Request instance for ResumeGrafanaInstance.
         :type request: :class:`tencentcloud.monitor.v20180724.models.ResumeGrafanaInstanceRequest`
         :rtype: :class:`tencentcloud.monitor.v20180724.models.ResumeGrafanaInstanceResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-monitor-3.0.917/README.rst` & `tencentcloud-sdk-python-monitor-3.0.918/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-monitor-3.0.917/PKG-INFO` & `tencentcloud-sdk-python-monitor-3.0.918/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-monitor
-Version: 3.0.917
+Version: 3.0.918
 Summary: Tencent Cloud Monitor SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-monitor-3.0.917/setup.py` & `tencentcloud-sdk-python-monitor-3.0.918/setup.py`

 * *Files identical despite different names*

