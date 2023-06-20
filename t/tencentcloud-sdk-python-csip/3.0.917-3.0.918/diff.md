# Comparing `tmp/tencentcloud-sdk-python-csip-3.0.917.tar.gz` & `tmp/tencentcloud-sdk-python-csip-3.0.918.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-csip-3.0.917.tar", last modified: Mon Jun 19 00:22:35 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-csip-3.0.918.tar", last modified: Tue Jun 20 02:37:52 2023, max compression
```

## Comparing `tencentcloud-sdk-python-csip-3.0.917.tar` & `tencentcloud-sdk-python-csip-3.0.918.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:22:35.000000 tencentcloud-sdk-python-csip-3.0.917/
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-19 00:22:35.000000 tencentcloud-sdk-python-csip-3.0.917/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:22:35.000000 tencentcloud-sdk-python-csip-3.0.917/tencentcloud_sdk_python_csip.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-19 00:22:35.000000 tencentcloud-sdk-python-csip-3.0.917/tencentcloud_sdk_python_csip.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-06-19 00:22:35.000000 tencentcloud-sdk-python-csip-3.0.917/tencentcloud_sdk_python_csip.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-06-19 00:22:35.000000 tencentcloud-sdk-python-csip-3.0.917/tencentcloud_sdk_python_csip.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-19 00:22:35.000000 tencentcloud-sdk-python-csip-3.0.917/tencentcloud_sdk_python_csip.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:22:35.000000 tencentcloud-sdk-python-csip-3.0.917/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-19 00:22:35.000000 tencentcloud-sdk-python-csip-3.0.917/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:22:35.000000 tencentcloud-sdk-python-csip-3.0.917/tencentcloud/csip/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 00:22:35.000000 tencentcloud-sdk-python-csip-3.0.917/tencentcloud/csip/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:22:35.000000 tencentcloud-sdk-python-csip-3.0.917/tencentcloud/csip/v20221121/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 00:22:35.000000 tencentcloud-sdk-python-csip-3.0.917/tencentcloud/csip/v20221121/__init__.py
--rw-r--r--   0 root         (0) root         (0)   108427 2023-06-19 00:22:35.000000 tencentcloud-sdk-python-csip-3.0.917/tencentcloud/csip/v20221121/models.py
--rw-r--r--   0 root         (0) root         (0)    13590 2023-06-19 00:22:35.000000 tencentcloud-sdk-python-csip-3.0.917/tencentcloud/csip/v20221121/csip_client.py
--rw-r--r--   0 root         (0) root         (0)     1836 2023-06-19 00:22:35.000000 tencentcloud-sdk-python-csip-3.0.917/tencentcloud/csip/v20221121/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)      740 2023-06-19 00:22:35.000000 tencentcloud-sdk-python-csip-3.0.917/README.rst
--rw-r--r--   0 root         (0) root         (0)     1664 2023-06-19 00:22:35.000000 tencentcloud-sdk-python-csip-3.0.917/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1008 2023-06-19 00:22:35.000000 tencentcloud-sdk-python-csip-3.0.917/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:37:52.000000 tencentcloud-sdk-python-csip-3.0.918/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-20 02:37:52.000000 tencentcloud-sdk-python-csip-3.0.918/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:37:52.000000 tencentcloud-sdk-python-csip-3.0.918/tencentcloud_sdk_python_csip.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 02:37:52.000000 tencentcloud-sdk-python-csip-3.0.918/tencentcloud_sdk_python_csip.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-06-20 02:37:52.000000 tencentcloud-sdk-python-csip-3.0.918/tencentcloud_sdk_python_csip.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-06-20 02:37:52.000000 tencentcloud-sdk-python-csip-3.0.918/tencentcloud_sdk_python_csip.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-20 02:37:52.000000 tencentcloud-sdk-python-csip-3.0.918/tencentcloud_sdk_python_csip.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:37:52.000000 tencentcloud-sdk-python-csip-3.0.918/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-20 02:37:52.000000 tencentcloud-sdk-python-csip-3.0.918/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:37:52.000000 tencentcloud-sdk-python-csip-3.0.918/tencentcloud/csip/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 02:37:52.000000 tencentcloud-sdk-python-csip-3.0.918/tencentcloud/csip/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:37:52.000000 tencentcloud-sdk-python-csip-3.0.918/tencentcloud/csip/v20221121/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 02:37:52.000000 tencentcloud-sdk-python-csip-3.0.918/tencentcloud/csip/v20221121/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   117193 2023-06-20 02:37:52.000000 tencentcloud-sdk-python-csip-3.0.918/tencentcloud/csip/v20221121/models.py
+-rw-r--r--   0 root         (0) root         (0)    14511 2023-06-20 02:37:52.000000 tencentcloud-sdk-python-csip-3.0.918/tencentcloud/csip/v20221121/csip_client.py
+-rw-r--r--   0 root         (0) root         (0)     1836 2023-06-20 02:37:52.000000 tencentcloud-sdk-python-csip-3.0.918/tencentcloud/csip/v20221121/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)      740 2023-06-20 02:37:52.000000 tencentcloud-sdk-python-csip-3.0.918/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-06-20 02:37:52.000000 tencentcloud-sdk-python-csip-3.0.918/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-06-20 02:37:52.000000 tencentcloud-sdk-python-csip-3.0.918/setup.py
```

### Comparing `tencentcloud-sdk-python-csip-3.0.917/tencentcloud_sdk_python_csip.egg-info/PKG-INFO` & `tencentcloud-sdk-python-csip-3.0.918/tencentcloud_sdk_python_csip.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-csip
-Version: 3.0.917
+Version: 3.0.918
 Summary: Tencent Cloud Csip SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-csip-3.0.917/tencentcloud/__init__.py` & `tencentcloud-sdk-python-csip-3.0.918/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-csip-3.0.917/tencentcloud/csip/v20221121/models.py` & `tencentcloud-sdk-python-csip-3.0.918/tencentcloud/csip/v20221121/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -894,14 +894,98 @@
 
 
     def _deserialize(self, params):
         self.Data = params.get("Data")
         self.RequestId = params.get("RequestId")
 
 
+class CreateRiskCenterScanTaskRequest(AbstractModel):
+    """CreateRiskCenterScanTask请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param TaskName: 任务名称
+        :type TaskName: str
+        :param ScanAssetType: 0-全扫，1-指定资产扫，2-排除资产扫，3-手动填写扫；1和2则Assets字段必填，3则SelfDefiningAssets必填
+        :type ScanAssetType: int
+        :param ScanItem: 扫描项目；port/poc/weakpass/webcontent/configrisk
+        :type ScanItem: list of str
+        :param ScanPlanType: 0-周期任务,1-立即扫描,2-定时扫描,3-自定义；0,2,3则ScanPlanContent必填
+        :type ScanPlanType: int
+        :param Assets: 扫描资产信息列表
+        :type Assets: list of TaskAssetObject
+        :param ScanPlanContent: 扫描计划详情
+        :type ScanPlanContent: str
+        :param SelfDefiningAssets: ip/域名/url数组
+        :type SelfDefiningAssets: list of str
+        :param TaskAdvanceCFG: 高级配置
+        :type TaskAdvanceCFG: :class:`tencentcloud.csip.v20221121.models.TaskAdvanceCFG`
+        :param TaskMode: 体检模式，0-标准模式，1-快速模式，2-高级模式，默认标准模式
+        :type TaskMode: int
+        """
+        self.TaskName = None
+        self.ScanAssetType = None
+        self.ScanItem = None
+        self.ScanPlanType = None
+        self.Assets = None
+        self.ScanPlanContent = None
+        self.SelfDefiningAssets = None
+        self.TaskAdvanceCFG = None
+        self.TaskMode = None
+
+
+    def _deserialize(self, params):
+        self.TaskName = params.get("TaskName")
+        self.ScanAssetType = params.get("ScanAssetType")
+        self.ScanItem = params.get("ScanItem")
+        self.ScanPlanType = params.get("ScanPlanType")
+        if params.get("Assets") is not None:
+            self.Assets = []
+            for item in params.get("Assets"):
+                obj = TaskAssetObject()
+                obj._deserialize(item)
+                self.Assets.append(obj)
+        self.ScanPlanContent = params.get("ScanPlanContent")
+        self.SelfDefiningAssets = params.get("SelfDefiningAssets")
+        if params.get("TaskAdvanceCFG") is not None:
+            self.TaskAdvanceCFG = TaskAdvanceCFG()
+            self.TaskAdvanceCFG._deserialize(params.get("TaskAdvanceCFG"))
+        self.TaskMode = params.get("TaskMode")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class CreateRiskCenterScanTaskResponse(AbstractModel):
+    """CreateRiskCenterScanTask返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param TaskId: 任务id
+        :type TaskId: str
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.TaskId = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.TaskId = params.get("TaskId")
+        self.RequestId = params.get("RequestId")
+
+
 class DBAssetVO(AbstractModel):
     """db资产输出字段
 
     """
 
     def __init__(self):
         r"""
@@ -2863,14 +2947,193 @@
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
+
+
+class TaskAdvanceCFG(AbstractModel):
+    """任务高级配置
+
+    """
+
+    def __init__(self):
+        r"""
+        :param VulRisk: 漏洞风险高级配置
+        :type VulRisk: list of TaskCenterVulRiskInputParam
+        :param WeakPwdRisk: 弱口令风险高级配置
+        :type WeakPwdRisk: list of TaskCenterWeakPwdRiskInputParam
+        :param CFGRisk: 配置风险高级配置
+        :type CFGRisk: list of TaskCenterCFGRiskInputParam
+        """
+        self.VulRisk = None
+        self.WeakPwdRisk = None
+        self.CFGRisk = None
+
+
+    def _deserialize(self, params):
+        if params.get("VulRisk") is not None:
+            self.VulRisk = []
+            for item in params.get("VulRisk"):
+                obj = TaskCenterVulRiskInputParam()
+                obj._deserialize(item)
+                self.VulRisk.append(obj)
+        if params.get("WeakPwdRisk") is not None:
+            self.WeakPwdRisk = []
+            for item in params.get("WeakPwdRisk"):
+                obj = TaskCenterWeakPwdRiskInputParam()
+                obj._deserialize(item)
+                self.WeakPwdRisk.append(obj)
+        if params.get("CFGRisk") is not None:
+            self.CFGRisk = []
+            for item in params.get("CFGRisk"):
+                obj = TaskCenterCFGRiskInputParam()
+                obj._deserialize(item)
+                self.CFGRisk.append(obj)
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class TaskAssetObject(AbstractModel):
+    """任务资产项
+
+    """
+
+    def __init__(self):
+        r"""
+        :param AssetName: 资产名
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AssetName: str
+        :param InstanceType: 	资产类型
+注意：此字段可能返回 null，表示取不到有效值。
+        :type InstanceType: str
+        :param AssetType: 资产分类
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AssetType: str
+        :param Asset: ip/域名/资产id，数据库id等
+        :type Asset: str
+        :param Region: 地域
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Region: str
+        """
+        self.AssetName = None
+        self.InstanceType = None
+        self.AssetType = None
+        self.Asset = None
+        self.Region = None
+
+
+    def _deserialize(self, params):
+        self.AssetName = params.get("AssetName")
+        self.InstanceType = params.get("InstanceType")
+        self.AssetType = params.get("AssetType")
+        self.Asset = params.get("Asset")
+        self.Region = params.get("Region")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class TaskCenterCFGRiskInputParam(AbstractModel):
+    """配置风险高级配置
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ItemId: 检测项ID
+        :type ItemId: str
+        :param Enable: 是否开启，0-不开启，1-开启
+        :type Enable: int
+        :param ResourceType: 资源类型
+        :type ResourceType: str
+        """
+        self.ItemId = None
+        self.Enable = None
+        self.ResourceType = None
+
+
+    def _deserialize(self, params):
+        self.ItemId = params.get("ItemId")
+        self.Enable = params.get("Enable")
+        self.ResourceType = params.get("ResourceType")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class TaskCenterVulRiskInputParam(AbstractModel):
+    """漏洞风险高级配置
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RiskId: 风险ID
+        :type RiskId: str
+        :param Enable: 是否开启，0-不开启，1-开启
+        :type Enable: int
+        """
+        self.RiskId = None
+        self.Enable = None
+
+
+    def _deserialize(self, params):
+        self.RiskId = params.get("RiskId")
+        self.Enable = params.get("Enable")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class TaskCenterWeakPwdRiskInputParam(AbstractModel):
+    """弱口令风险高级配置
+
+    """
+
+    def __init__(self):
+        r"""
+        :param CheckItemId: 检测项ID
+        :type CheckItemId: int
+        :param Enable: 是否开启，0-不开启，1-开启
+        :type Enable: int
+        """
+        self.CheckItemId = None
+        self.Enable = None
+
+
+    def _deserialize(self, params):
+        self.CheckItemId = params.get("CheckItemId")
+        self.Enable = params.get("Enable")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
 
 
 class Vpc(AbstractModel):
     """vpc列表数据
 
     """
```

### Comparing `tencentcloud-sdk-python-csip-3.0.917/tencentcloud/csip/v20221121/csip_client.py` & `tencentcloud-sdk-python-csip-3.0.918/tencentcloud/csip/v20221121/csip_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,14 +68,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def CreateRiskCenterScanTask(self, request):
+        """创建风险中心扫描任务
+
+        :param request: Request instance for CreateRiskCenterScanTask.
+        :type request: :class:`tencentcloud.csip.v20221121.models.CreateRiskCenterScanTaskRequest`
+        :rtype: :class:`tencentcloud.csip.v20221121.models.CreateRiskCenterScanTaskResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("CreateRiskCenterScanTask", params, headers=headers)
+            response = json.loads(body)
+            model = models.CreateRiskCenterScanTaskResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DescribeCVMAssetInfo(self, request):
         """cvm详情
 
         :param request: Request instance for DescribeCVMAssetInfo.
         :type request: :class:`tencentcloud.csip.v20221121.models.DescribeCVMAssetInfoRequest`
         :rtype: :class:`tencentcloud.csip.v20221121.models.DescribeCVMAssetInfoResponse`
```

### Comparing `tencentcloud-sdk-python-csip-3.0.917/tencentcloud/csip/v20221121/errorcodes.py` & `tencentcloud-sdk-python-csip-3.0.918/tencentcloud/csip/v20221121/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-csip-3.0.917/README.rst` & `tencentcloud-sdk-python-csip-3.0.918/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-csip-3.0.917/PKG-INFO` & `tencentcloud-sdk-python-csip-3.0.918/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-csip
-Version: 3.0.917
+Version: 3.0.918
 Summary: Tencent Cloud Csip SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-csip-3.0.917/setup.py` & `tencentcloud-sdk-python-csip-3.0.918/setup.py`

 * *Files identical despite different names*

