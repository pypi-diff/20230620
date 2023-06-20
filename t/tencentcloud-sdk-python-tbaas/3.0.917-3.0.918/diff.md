# Comparing `tmp/tencentcloud-sdk-python-tbaas-3.0.917.tar.gz` & `tmp/tencentcloud-sdk-python-tbaas-3.0.918.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tbaas-3.0.917.tar", last modified: Mon Jun 19 00:33:14 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tbaas-3.0.918.tar", last modified: Tue Jun 20 02:48:27 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tbaas-3.0.917.tar` & `tencentcloud-sdk-python-tbaas-3.0.918.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:33:14.000000 tencentcloud-sdk-python-tbaas-3.0.917/
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-19 00:33:14.000000 tencentcloud-sdk-python-tbaas-3.0.917/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:33:14.000000 tencentcloud-sdk-python-tbaas-3.0.917/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-19 00:33:14.000000 tencentcloud-sdk-python-tbaas-3.0.917/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:33:14.000000 tencentcloud-sdk-python-tbaas-3.0.917/tencentcloud/tbaas/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 00:33:14.000000 tencentcloud-sdk-python-tbaas-3.0.917/tencentcloud/tbaas/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:33:14.000000 tencentcloud-sdk-python-tbaas-3.0.917/tencentcloud/tbaas/v20180416/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 00:33:14.000000 tencentcloud-sdk-python-tbaas-3.0.917/tencentcloud/tbaas/v20180416/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32021 2023-06-19 00:33:14.000000 tencentcloud-sdk-python-tbaas-3.0.917/tencentcloud/tbaas/v20180416/tbaas_client.py
--rw-r--r--   0 root         (0) root         (0)   108598 2023-06-19 00:33:14.000000 tencentcloud-sdk-python-tbaas-3.0.917/tencentcloud/tbaas/v20180416/models.py
--rw-r--r--   0 root         (0) root         (0)    11811 2023-06-19 00:33:14.000000 tencentcloud-sdk-python-tbaas-3.0.917/tencentcloud/tbaas/v20180416/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)      743 2023-06-19 00:33:14.000000 tencentcloud-sdk-python-tbaas-3.0.917/README.rst
--rw-r--r--   0 root         (0) root         (0)     1669 2023-06-19 00:33:14.000000 tencentcloud-sdk-python-tbaas-3.0.917/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:33:14.000000 tencentcloud-sdk-python-tbaas-3.0.917/tencentcloud_sdk_python_tbaas.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-19 00:33:14.000000 tencentcloud-sdk-python-tbaas-3.0.917/tencentcloud_sdk_python_tbaas.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      465 2023-06-19 00:33:14.000000 tencentcloud-sdk-python-tbaas-3.0.917/tencentcloud_sdk_python_tbaas.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1669 2023-06-19 00:33:14.000000 tencentcloud-sdk-python-tbaas-3.0.917/tencentcloud_sdk_python_tbaas.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-19 00:33:14.000000 tencentcloud-sdk-python-tbaas-3.0.917/tencentcloud_sdk_python_tbaas.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1010 2023-06-19 00:33:14.000000 tencentcloud-sdk-python-tbaas-3.0.917/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:48:27.000000 tencentcloud-sdk-python-tbaas-3.0.918/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-20 02:48:27.000000 tencentcloud-sdk-python-tbaas-3.0.918/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:48:27.000000 tencentcloud-sdk-python-tbaas-3.0.918/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-20 02:48:26.000000 tencentcloud-sdk-python-tbaas-3.0.918/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:48:27.000000 tencentcloud-sdk-python-tbaas-3.0.918/tencentcloud/tbaas/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 02:48:26.000000 tencentcloud-sdk-python-tbaas-3.0.918/tencentcloud/tbaas/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:48:27.000000 tencentcloud-sdk-python-tbaas-3.0.918/tencentcloud/tbaas/v20180416/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 02:48:26.000000 tencentcloud-sdk-python-tbaas-3.0.918/tencentcloud/tbaas/v20180416/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    33385 2023-06-20 02:48:26.000000 tencentcloud-sdk-python-tbaas-3.0.918/tencentcloud/tbaas/v20180416/tbaas_client.py
+-rw-r--r--   0 root         (0) root         (0)   111915 2023-06-20 02:48:26.000000 tencentcloud-sdk-python-tbaas-3.0.918/tencentcloud/tbaas/v20180416/models.py
+-rw-r--r--   0 root         (0) root         (0)    11811 2023-06-20 02:48:26.000000 tencentcloud-sdk-python-tbaas-3.0.918/tencentcloud/tbaas/v20180416/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)      743 2023-06-20 02:48:26.000000 tencentcloud-sdk-python-tbaas-3.0.918/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-06-20 02:48:27.000000 tencentcloud-sdk-python-tbaas-3.0.918/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:48:27.000000 tencentcloud-sdk-python-tbaas-3.0.918/tencentcloud_sdk_python_tbaas.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 02:48:26.000000 tencentcloud-sdk-python-tbaas-3.0.918/tencentcloud_sdk_python_tbaas.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      465 2023-06-20 02:48:27.000000 tencentcloud-sdk-python-tbaas-3.0.918/tencentcloud_sdk_python_tbaas.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-06-20 02:48:26.000000 tencentcloud-sdk-python-tbaas-3.0.918/tencentcloud_sdk_python_tbaas.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-20 02:48:26.000000 tencentcloud-sdk-python-tbaas-3.0.918/tencentcloud_sdk_python_tbaas.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-06-20 02:48:26.000000 tencentcloud-sdk-python-tbaas-3.0.918/setup.py
```

### Comparing `tencentcloud-sdk-python-tbaas-3.0.917/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tbaas-3.0.918/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tbaas-3.0.917/tencentcloud/tbaas/v20180416/tbaas_client.py` & `tencentcloud-sdk-python-tbaas-3.0.918/tencentcloud/tbaas/v20180416/tbaas_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,15 +92,17 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DeployDynamicBcosContract(self, request):
-        """动态部署并发布Bcos合约
+        """Bcos区块链引擎已下线，请选用其他区块链引擎
+
+        动态部署并发布Bcos合约
 
         :param request: Request instance for DeployDynamicBcosContract.
         :type request: :class:`tencentcloud.tbaas.v20180416.models.DeployDynamicBcosContractRequest`
         :rtype: :class:`tencentcloud.tbaas.v20180416.models.DeployDynamicBcosContractResponse`
 
         """
         try:
@@ -138,15 +140,17 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def GetBcosBlockByNumber(self, request):
-        """使用块高查询Bcos区块信息
+        """Bcos区块链引擎已下线，请选用其他区块链引擎
+
+        使用块高查询Bcos区块信息
 
         :param request: Request instance for GetBcosBlockByNumber.
         :type request: :class:`tencentcloud.tbaas.v20180416.models.GetBcosBlockByNumberRequest`
         :rtype: :class:`tencentcloud.tbaas.v20180416.models.GetBcosBlockByNumberResponse`
 
         """
         try:
@@ -161,15 +165,17 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def GetBcosBlockList(self, request):
-        """Bcos分页查询当前群组下的区块列表
+        """Bcos区块链引擎已下线，请选用其他区块链引擎
+
+        Bcos分页查询当前群组下的区块列表
 
         :param request: Request instance for GetBcosBlockList.
         :type request: :class:`tencentcloud.tbaas.v20180416.models.GetBcosBlockListRequest`
         :rtype: :class:`tencentcloud.tbaas.v20180416.models.GetBcosBlockListResponse`
 
         """
         try:
@@ -184,15 +190,17 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def GetBcosTransByHash(self, request):
-        """Bcos根据交易哈希查看交易详细信息
+        """Bcos区块链引擎已下线，请选用其他区块链引擎
+
+        Bcos根据交易哈希查看交易详细信息
 
         :param request: Request instance for GetBcosTransByHash.
         :type request: :class:`tencentcloud.tbaas.v20180416.models.GetBcosTransByHashRequest`
         :rtype: :class:`tencentcloud.tbaas.v20180416.models.GetBcosTransByHashResponse`
 
         """
         try:
@@ -207,15 +215,17 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def GetBcosTransList(self, request):
-        """Bcos分页查询当前群组的交易信息列表
+        """Bcos区块链引擎已下线，请选用其他区块链引擎
+
+        Bcos分页查询当前群组的交易信息列表
 
         :param request: Request instance for GetBcosTransList.
         :type request: :class:`tencentcloud.tbaas.v20180416.models.GetBcosTransListRequest`
         :rtype: :class:`tencentcloud.tbaas.v20180416.models.GetBcosTransListResponse`
 
         """
         try:
@@ -437,15 +447,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def GetLatesdTransactionList(self, request):
-        """获取最新交易列表
+        """获取最新交易列表（已废弃）
 
         :param request: Request instance for GetLatesdTransactionList.
         :type request: :class:`tencentcloud.tbaas.v20180416.models.GetLatesdTransactionListRequest`
         :rtype: :class:`tencentcloud.tbaas.v20180416.models.GetLatesdTransactionListResponse`
 
         """
         try:
@@ -459,14 +469,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def GetLatestTransactionList(self, request):
+        """获取fabric最新交易列表
+
+        :param request: Request instance for GetLatestTransactionList.
+        :type request: :class:`tencentcloud.tbaas.v20180416.models.GetLatestTransactionListRequest`
+        :rtype: :class:`tencentcloud.tbaas.v20180416.models.GetLatestTransactionListResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("GetLatestTransactionList", params, headers=headers)
+            response = json.loads(body)
+            model = models.GetLatestTransactionListResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def GetPeerLogForUser(self, request):
         """获取节点日志
 
         :param request: Request instance for GetPeerLogForUser.
         :type request: :class:`tencentcloud.tbaas.v20180416.models.GetPeerLogForUserRequest`
         :rtype: :class:`tencentcloud.tbaas.v20180416.models.GetPeerLogForUserResponse`
 
@@ -552,15 +585,17 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def InvokeBcosTrans(self, request):
-        """执行Bcos交易，支持动态部署的合约
+        """Bcos区块链引擎已下线，请选用其他区块链引擎
+
+        执行Bcos交易，支持动态部署的合约
 
         :param request: Request instance for InvokeBcosTrans.
         :type request: :class:`tencentcloud.tbaas.v20180416.models.InvokeBcosTransRequest`
         :rtype: :class:`tencentcloud.tbaas.v20180416.models.InvokeBcosTransResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-tbaas-3.0.917/tencentcloud/tbaas/v20180416/models.py` & `tencentcloud-sdk-python-tbaas-3.0.918/tencentcloud/tbaas/v20180416/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1806,14 +1806,104 @@
             for item in params.get("TransactionList"):
                 obj = TransactionItem()
                 obj._deserialize(item)
                 self.TransactionList.append(obj)
         self.RequestId = params.get("RequestId")
 
 
+class GetLatestTransactionListRequest(AbstractModel):
+    """GetLatestTransactionList请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Module: 模块名称，固定字段：transaction
+        :type Module: str
+        :param Operation: 操作名称，固定字段：latest_transaction_list
+        :type Operation: str
+        :param GroupId: 组织ID，固定字段：0
+        :type GroupId: int
+        :param ChannelId: 通道ID，固定字段：0
+        :type ChannelId: int
+        :param LatestBlockNumber: 获取的最新交易的区块数量，取值范围1~5
+        :type LatestBlockNumber: int
+        :param GroupName: 调用接口的组织名称，可以在组织管理列表中获取当前组织的名称
+        :type GroupName: str
+        :param ChannelName: 需要查询的通道名称，可在通道详情或列表中获取
+        :type ChannelName: str
+        :param ClusterId: 区块链网络ID，可在区块链网络详情或列表中获取
+        :type ClusterId: str
+        :param Offset: 需要获取的起始交易偏移
+        :type Offset: int
+        :param Limit: 需要获取的交易数量
+        :type Limit: int
+        """
+        self.Module = None
+        self.Operation = None
+        self.GroupId = None
+        self.ChannelId = None
+        self.LatestBlockNumber = None
+        self.GroupName = None
+        self.ChannelName = None
+        self.ClusterId = None
+        self.Offset = None
+        self.Limit = None
+
+
+    def _deserialize(self, params):
+        self.Module = params.get("Module")
+        self.Operation = params.get("Operation")
+        self.GroupId = params.get("GroupId")
+        self.ChannelId = params.get("ChannelId")
+        self.LatestBlockNumber = params.get("LatestBlockNumber")
+        self.GroupName = params.get("GroupName")
+        self.ChannelName = params.get("ChannelName")
+        self.ClusterId = params.get("ClusterId")
+        self.Offset = params.get("Offset")
+        self.Limit = params.get("Limit")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class GetLatestTransactionListResponse(AbstractModel):
+    """GetLatestTransactionList返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param TotalCount: 交易总数量
+        :type TotalCount: int
+        :param TransactionList: 交易列表
+        :type TransactionList: list of TransactionItem
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.TotalCount = None
+        self.TransactionList = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.TotalCount = params.get("TotalCount")
+        if params.get("TransactionList") is not None:
+            self.TransactionList = []
+            for item in params.get("TransactionList"):
+                obj = TransactionItem()
+                obj._deserialize(item)
+                self.TransactionList.append(obj)
+        self.RequestId = params.get("RequestId")
+
+
 class GetPeerLogForUserRequest(AbstractModel):
     """GetPeerLogForUser请求参数结构体
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-tbaas-3.0.917/tencentcloud/tbaas/v20180416/errorcodes.py` & `tencentcloud-sdk-python-tbaas-3.0.918/tencentcloud/tbaas/v20180416/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tbaas-3.0.917/README.rst` & `tencentcloud-sdk-python-tbaas-3.0.918/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tbaas-3.0.917/PKG-INFO` & `tencentcloud-sdk-python-tbaas-3.0.918/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tbaas
-Version: 3.0.917
+Version: 3.0.918
 Summary: Tencent Cloud Tbaas SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tbaas-3.0.917/tencentcloud_sdk_python_tbaas.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tbaas-3.0.918/tencentcloud_sdk_python_tbaas.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tbaas
-Version: 3.0.917
+Version: 3.0.918
 Summary: Tencent Cloud Tbaas SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tbaas-3.0.917/setup.py` & `tencentcloud-sdk-python-tbaas-3.0.918/setup.py`

 * *Files identical despite different names*

