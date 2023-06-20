# Comparing `tmp/tencentcloud-sdk-python-tke-3.0.917.tar.gz` & `tmp/tencentcloud-sdk-python-tke-3.0.918.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tke-3.0.917.tar", last modified: Mon Jun 19 00:35:45 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tke-3.0.918.tar", last modified: Tue Jun 20 02:50:55 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tke-3.0.917.tar` & `tencentcloud-sdk-python-tke-3.0.918.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:35:45.000000 tencentcloud-sdk-python-tke-3.0.917/
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-19 00:35:45.000000 tencentcloud-sdk-python-tke-3.0.917/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:35:45.000000 tencentcloud-sdk-python-tke-3.0.917/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-19 00:35:45.000000 tencentcloud-sdk-python-tke-3.0.917/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:35:45.000000 tencentcloud-sdk-python-tke-3.0.917/tencentcloud/tke/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 00:35:45.000000 tencentcloud-sdk-python-tke-3.0.917/tencentcloud/tke/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:35:45.000000 tencentcloud-sdk-python-tke-3.0.917/tencentcloud/tke/v20180525/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 00:35:45.000000 tencentcloud-sdk-python-tke-3.0.917/tencentcloud/tke/v20180525/__init__.py
--rw-r--r--   0 root         (0) root         (0)   186106 2023-06-19 00:35:45.000000 tencentcloud-sdk-python-tke-3.0.917/tencentcloud/tke/v20180525/tke_client.py
--rw-r--r--   0 root         (0) root         (0)   673736 2023-06-19 00:35:45.000000 tencentcloud-sdk-python-tke-3.0.917/tencentcloud/tke/v20180525/models.py
--rw-r--r--   0 root         (0) root         (0)    19455 2023-06-19 00:35:45.000000 tencentcloud-sdk-python-tke-3.0.917/tencentcloud/tke/v20180525/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-19 00:35:45.000000 tencentcloud-sdk-python-tke-3.0.917/README.rst
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-19 00:35:45.000000 tencentcloud-sdk-python-tke-3.0.917/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-19 00:35:45.000000 tencentcloud-sdk-python-tke-3.0.917/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:35:45.000000 tencentcloud-sdk-python-tke-3.0.917/tencentcloud_sdk_python_tke.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-19 00:35:45.000000 tencentcloud-sdk-python-tke-3.0.917/tencentcloud_sdk_python_tke.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-19 00:35:45.000000 tencentcloud-sdk-python-tke-3.0.917/tencentcloud_sdk_python_tke.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-19 00:35:45.000000 tencentcloud-sdk-python-tke-3.0.917/tencentcloud_sdk_python_tke.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-19 00:35:45.000000 tencentcloud-sdk-python-tke-3.0.917/tencentcloud_sdk_python_tke.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:50:55.000000 tencentcloud-sdk-python-tke-3.0.918/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-20 02:50:55.000000 tencentcloud-sdk-python-tke-3.0.918/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:50:55.000000 tencentcloud-sdk-python-tke-3.0.918/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-20 02:50:55.000000 tencentcloud-sdk-python-tke-3.0.918/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:50:55.000000 tencentcloud-sdk-python-tke-3.0.918/tencentcloud/tke/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 02:50:55.000000 tencentcloud-sdk-python-tke-3.0.918/tencentcloud/tke/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:50:55.000000 tencentcloud-sdk-python-tke-3.0.918/tencentcloud/tke/v20180525/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 02:50:55.000000 tencentcloud-sdk-python-tke-3.0.918/tencentcloud/tke/v20180525/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   190354 2023-06-20 02:50:55.000000 tencentcloud-sdk-python-tke-3.0.918/tencentcloud/tke/v20180525/tke_client.py
+-rw-r--r--   0 root         (0) root         (0)   682751 2023-06-20 02:50:55.000000 tencentcloud-sdk-python-tke-3.0.918/tencentcloud/tke/v20180525/models.py
+-rw-r--r--   0 root         (0) root         (0)    19455 2023-06-20 02:50:55.000000 tencentcloud-sdk-python-tke-3.0.918/tencentcloud/tke/v20180525/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-20 02:50:55.000000 tencentcloud-sdk-python-tke-3.0.918/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-20 02:50:55.000000 tencentcloud-sdk-python-tke-3.0.918/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-20 02:50:55.000000 tencentcloud-sdk-python-tke-3.0.918/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:50:55.000000 tencentcloud-sdk-python-tke-3.0.918/tencentcloud_sdk_python_tke.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 02:50:55.000000 tencentcloud-sdk-python-tke-3.0.918/tencentcloud_sdk_python_tke.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-20 02:50:55.000000 tencentcloud-sdk-python-tke-3.0.918/tencentcloud_sdk_python_tke.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-20 02:50:55.000000 tencentcloud-sdk-python-tke-3.0.918/tencentcloud_sdk_python_tke.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-20 02:50:55.000000 tencentcloud-sdk-python-tke-3.0.918/tencentcloud_sdk_python_tke.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-tke-3.0.917/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tke-3.0.918/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tke-3.0.917/tencentcloud/tke/v20180525/tke_client.py` & `tencentcloud-sdk-python-tke-3.0.918/tencentcloud/tke/v20180525/tke_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -827,14 +827,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DeleteAddon(self, request):
+        """删除一个addon
+
+        :param request: Request instance for DeleteAddon.
+        :type request: :class:`tencentcloud.tke.v20180525.models.DeleteAddonRequest`
+        :rtype: :class:`tencentcloud.tke.v20180525.models.DeleteAddonResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DeleteAddon", params, headers=headers)
+            response = json.loads(body)
+            model = models.DeleteAddonResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DeleteBackupStorageLocation(self, request):
         """删除备份仓库
 
         :param request: Request instance for DeleteBackupStorageLocation.
         :type request: :class:`tencentcloud.tke.v20180525.models.DeleteBackupStorageLocationRequest`
         :rtype: :class:`tencentcloud.tke.v20180525.models.DeleteBackupStorageLocationResponse`
 
@@ -1448,14 +1471,60 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DescribeAddon(self, request):
+        """获取addon列表
+
+        :param request: Request instance for DescribeAddon.
+        :type request: :class:`tencentcloud.tke.v20180525.models.DescribeAddonRequest`
+        :rtype: :class:`tencentcloud.tke.v20180525.models.DescribeAddonResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeAddon", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeAddonResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def DescribeAddonValues(self, request):
+        """获取一个addon的参数
+
+        :param request: Request instance for DescribeAddonValues.
+        :type request: :class:`tencentcloud.tke.v20180525.models.DescribeAddonValuesRequest`
+        :rtype: :class:`tencentcloud.tke.v20180525.models.DescribeAddonValuesResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeAddonValues", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeAddonValuesResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DescribeAvailableClusterVersion(self, request):
         """获取集群可以升级的所有版本
 
         :param request: Request instance for DescribeAvailableClusterVersion.
         :type request: :class:`tencentcloud.tke.v20180525.models.DescribeAvailableClusterVersionRequest`
         :rtype: :class:`tencentcloud.tke.v20180525.models.DescribeAvailableClusterVersionResponse`
 
@@ -3610,14 +3679,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def InstallAddon(self, request):
+        """为目标集群安装一个addon
+
+        :param request: Request instance for InstallAddon.
+        :type request: :class:`tencentcloud.tke.v20180525.models.InstallAddonRequest`
+        :rtype: :class:`tencentcloud.tke.v20180525.models.InstallAddonResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("InstallAddon", params, headers=headers)
+            response = json.loads(body)
+            model = models.InstallAddonResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def InstallEdgeLogAgent(self, request):
         """在tke@edge集群的边缘节点上安装日志采集组件
 
         :param request: Request instance for InstallEdgeLogAgent.
         :type request: :class:`tencentcloud.tke.v20180525.models.InstallEdgeLogAgentRequest`
         :rtype: :class:`tencentcloud.tke.v20180525.models.InstallEdgeLogAgentResponse`
 
@@ -4367,14 +4459,37 @@
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
+
+
+    def UpdateAddon(self, request):
+        """更新一个addon的参数和版本
+
+        :param request: Request instance for UpdateAddon.
+        :type request: :class:`tencentcloud.tke.v20180525.models.UpdateAddonRequest`
+        :rtype: :class:`tencentcloud.tke.v20180525.models.UpdateAddonResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("UpdateAddon", params, headers=headers)
+            response = json.loads(body)
+            model = models.UpdateAddonResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
 
 
     def UpdateClusterKubeconfig(self, request):
         """对集群的Kubeconfig信息进行更新
 
         :param request: Request instance for UpdateClusterKubeconfig.
         :type request: :class:`tencentcloud.tke.v20180525.models.UpdateClusterKubeconfigRequest`
```

### Comparing `tencentcloud-sdk-python-tke-3.0.917/tencentcloud/tke/v20180525/models.py` & `tencentcloud-sdk-python-tke-3.0.918/tencentcloud/tke/v20180525/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -322,14 +322,57 @@
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.RequestId = params.get("RequestId")
 
 
+class Addon(AbstractModel):
+    """addon的具体描述
+
+    """
+
+    def __init__(self):
+        r"""
+        :param AddonName: addon名称
+        :type AddonName: str
+        :param AddonVersion: addon的版本
+        :type AddonVersion: str
+        :param RawValues: addon的参数，是一个json格式的base64转码后的字符串
+注意：此字段可能返回 null，表示取不到有效值。
+        :type RawValues: str
+        :param Phase: addon的状态
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Phase: str
+        :param Reason: addon失败的原因
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Reason: str
+        """
+        self.AddonName = None
+        self.AddonVersion = None
+        self.RawValues = None
+        self.Phase = None
+        self.Reason = None
+
+
+    def _deserialize(self, params):
+        self.AddonName = params.get("AddonName")
+        self.AddonVersion = params.get("AddonVersion")
+        self.RawValues = params.get("RawValues")
+        self.Phase = params.get("Phase")
+        self.Reason = params.get("Reason")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class AppChart(AbstractModel):
     """app所支持的chart
 
     """
 
     def __init__(self):
         r"""
@@ -4138,14 +4181,59 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class DeleteAddonRequest(AbstractModel):
+    """DeleteAddon请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ClusterId: 集群ID
+        :type ClusterId: str
+        :param AddonName: addon名称
+        :type AddonName: str
+        """
+        self.ClusterId = None
+        self.AddonName = None
+
+
+    def _deserialize(self, params):
+        self.ClusterId = params.get("ClusterId")
+        self.AddonName = params.get("AddonName")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DeleteAddonResponse(AbstractModel):
+    """DeleteAddon返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RequestId = params.get("RequestId")
+
+
 class DeleteBackupStorageLocationRequest(AbstractModel):
     """DeleteBackupStorageLocation请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -5408,14 +5496,121 @@
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.RequestId = params.get("RequestId")
 
 
+class DescribeAddonRequest(AbstractModel):
+    """DescribeAddon请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ClusterId: 集群ID
+        :type ClusterId: str
+        :param AddonName: addon名称（不传时会返回集群下全部的addon）
+        :type AddonName: str
+        """
+        self.ClusterId = None
+        self.AddonName = None
+
+
+    def _deserialize(self, params):
+        self.ClusterId = params.get("ClusterId")
+        self.AddonName = params.get("AddonName")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeAddonResponse(AbstractModel):
+    """DescribeAddon返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Addons: addon列表
+        :type Addons: list of Addon
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.Addons = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("Addons") is not None:
+            self.Addons = []
+            for item in params.get("Addons"):
+                obj = Addon()
+                obj._deserialize(item)
+                self.Addons.append(obj)
+        self.RequestId = params.get("RequestId")
+
+
+class DescribeAddonValuesRequest(AbstractModel):
+    """DescribeAddonValues请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ClusterId: 集群ID
+        :type ClusterId: str
+        :param AddonName: addon名称
+        :type AddonName: str
+        """
+        self.ClusterId = None
+        self.AddonName = None
+
+
+    def _deserialize(self, params):
+        self.ClusterId = params.get("ClusterId")
+        self.AddonName = params.get("AddonName")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeAddonValuesResponse(AbstractModel):
+    """DescribeAddonValues返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Values: 参数列表，如果addon已安装，会使用已设置的的参数做渲染，是一个json格式的字符串
+        :type Values: str
+        :param DefaultValues: addon支持的参数列表，使用默认值，是一个json格式的字符串
+        :type DefaultValues: str
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.Values = None
+        self.DefaultValues = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.Values = params.get("Values")
+        self.DefaultValues = params.get("DefaultValues")
+        self.RequestId = params.get("RequestId")
+
+
 class DescribeAvailableClusterVersionRequest(AbstractModel):
     """DescribeAvailableClusterVersion请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -12659,14 +12854,67 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class InstallAddonRequest(AbstractModel):
+    """InstallAddon请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ClusterId: 集群ID
+        :type ClusterId: str
+        :param AddonName: addon名称
+        :type AddonName: str
+        :param AddonVersion: addon版本（不传默认安装最新版本）
+        :type AddonVersion: str
+        :param RawValues: addon的参数，是一个json格式的base64转码后的字符串（addon参数由DescribeAddonValues获取）
+        :type RawValues: str
+        """
+        self.ClusterId = None
+        self.AddonName = None
+        self.AddonVersion = None
+        self.RawValues = None
+
+
+    def _deserialize(self, params):
+        self.ClusterId = params.get("ClusterId")
+        self.AddonName = params.get("AddonName")
+        self.AddonVersion = params.get("AddonVersion")
+        self.RawValues = params.get("RawValues")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class InstallAddonResponse(AbstractModel):
+    """InstallAddon返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RequestId = params.get("RequestId")
+
+
 class InstallEdgeLogAgentRequest(AbstractModel):
     """InstallEdgeLogAgent请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -18325,14 +18573,67 @@
 
     """
 
     def __init__(self):
         r"""
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
+        """
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RequestId = params.get("RequestId")
+
+
+class UpdateAddonRequest(AbstractModel):
+    """UpdateAddon请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ClusterId: 集群ID
+        :type ClusterId: str
+        :param AddonName: addon名称
+        :type AddonName: str
+        :param AddonVersion: addon版本（不传默认不更新）
+        :type AddonVersion: str
+        :param RawValues: addon的参数，是一个json格式的base64转码后的字符串（addon参数由DescribeAddonValues获取）
+        :type RawValues: str
+        """
+        self.ClusterId = None
+        self.AddonName = None
+        self.AddonVersion = None
+        self.RawValues = None
+
+
+    def _deserialize(self, params):
+        self.ClusterId = params.get("ClusterId")
+        self.AddonName = params.get("AddonName")
+        self.AddonVersion = params.get("AddonVersion")
+        self.RawValues = params.get("RawValues")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class UpdateAddonResponse(AbstractModel):
+    """UpdateAddon返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
         """
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.RequestId = params.get("RequestId")
```

### Comparing `tencentcloud-sdk-python-tke-3.0.917/tencentcloud/tke/v20180525/errorcodes.py` & `tencentcloud-sdk-python-tke-3.0.918/tencentcloud/tke/v20180525/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tke-3.0.917/README.rst` & `tencentcloud-sdk-python-tke-3.0.918/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tke-3.0.917/PKG-INFO` & `tencentcloud-sdk-python-tke-3.0.918/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tke
-Version: 3.0.917
+Version: 3.0.918
 Summary: Tencent Cloud Tke SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tke-3.0.917/setup.py` & `tencentcloud-sdk-python-tke-3.0.918/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tke-3.0.917/tencentcloud_sdk_python_tke.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tke-3.0.918/tencentcloud_sdk_python_tke.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tke
-Version: 3.0.917
+Version: 3.0.918
 Summary: Tencent Cloud Tke SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

