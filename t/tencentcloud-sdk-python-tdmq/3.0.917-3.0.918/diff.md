# Comparing `tmp/tencentcloud-sdk-python-tdmq-3.0.917.tar.gz` & `tmp/tencentcloud-sdk-python-tdmq-3.0.918.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tdmq-3.0.917.tar", last modified: Mon Jun 19 00:34:26 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tdmq-3.0.918.tar", last modified: Tue Jun 20 02:49:40 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tdmq-3.0.917.tar` & `tencentcloud-sdk-python-tdmq-3.0.918.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:34:26.000000 tencentcloud-sdk-python-tdmq-3.0.917/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:34:26.000000 tencentcloud-sdk-python-tdmq-3.0.917/tencentcloud_sdk_python_tdmq.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-19 00:34:26.000000 tencentcloud-sdk-python-tdmq-3.0.917/tencentcloud_sdk_python_tdmq.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-06-19 00:34:26.000000 tencentcloud-sdk-python-tdmq-3.0.917/tencentcloud_sdk_python_tdmq.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-06-19 00:34:26.000000 tencentcloud-sdk-python-tdmq-3.0.917/tencentcloud_sdk_python_tdmq.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-19 00:34:26.000000 tencentcloud-sdk-python-tdmq-3.0.917/tencentcloud_sdk_python_tdmq.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-19 00:34:26.000000 tencentcloud-sdk-python-tdmq-3.0.917/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:34:26.000000 tencentcloud-sdk-python-tdmq-3.0.917/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-19 00:34:26.000000 tencentcloud-sdk-python-tdmq-3.0.917/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:34:26.000000 tencentcloud-sdk-python-tdmq-3.0.917/tencentcloud/tdmq/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 00:34:26.000000 tencentcloud-sdk-python-tdmq-3.0.917/tencentcloud/tdmq/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:34:26.000000 tencentcloud-sdk-python-tdmq-3.0.917/tencentcloud/tdmq/v20200217/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 00:34:26.000000 tencentcloud-sdk-python-tdmq-3.0.917/tencentcloud/tdmq/v20200217/__init__.py
--rw-r--r--   0 root         (0) root         (0)   403511 2023-06-19 00:34:26.000000 tencentcloud-sdk-python-tdmq-3.0.917/tencentcloud/tdmq/v20200217/models.py
--rw-r--r--   0 root         (0) root         (0)    10117 2023-06-19 00:34:26.000000 tencentcloud-sdk-python-tdmq-3.0.917/tencentcloud/tdmq/v20200217/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   109282 2023-06-19 00:34:26.000000 tencentcloud-sdk-python-tdmq-3.0.917/tencentcloud/tdmq/v20200217/tdmq_client.py
--rw-r--r--   0 root         (0) root         (0)      740 2023-06-19 00:34:26.000000 tencentcloud-sdk-python-tdmq-3.0.917/README.rst
--rw-r--r--   0 root         (0) root         (0)     1664 2023-06-19 00:34:26.000000 tencentcloud-sdk-python-tdmq-3.0.917/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1008 2023-06-19 00:34:26.000000 tencentcloud-sdk-python-tdmq-3.0.917/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:49:40.000000 tencentcloud-sdk-python-tdmq-3.0.918/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:49:40.000000 tencentcloud-sdk-python-tdmq-3.0.918/tencentcloud_sdk_python_tdmq.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 02:49:40.000000 tencentcloud-sdk-python-tdmq-3.0.918/tencentcloud_sdk_python_tdmq.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-06-20 02:49:40.000000 tencentcloud-sdk-python-tdmq-3.0.918/tencentcloud_sdk_python_tdmq.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-06-20 02:49:40.000000 tencentcloud-sdk-python-tdmq-3.0.918/tencentcloud_sdk_python_tdmq.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-20 02:49:40.000000 tencentcloud-sdk-python-tdmq-3.0.918/tencentcloud_sdk_python_tdmq.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-20 02:49:40.000000 tencentcloud-sdk-python-tdmq-3.0.918/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:49:40.000000 tencentcloud-sdk-python-tdmq-3.0.918/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-20 02:49:40.000000 tencentcloud-sdk-python-tdmq-3.0.918/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:49:40.000000 tencentcloud-sdk-python-tdmq-3.0.918/tencentcloud/tdmq/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 02:49:40.000000 tencentcloud-sdk-python-tdmq-3.0.918/tencentcloud/tdmq/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:49:40.000000 tencentcloud-sdk-python-tdmq-3.0.918/tencentcloud/tdmq/v20200217/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 02:49:40.000000 tencentcloud-sdk-python-tdmq-3.0.918/tencentcloud/tdmq/v20200217/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   405597 2023-06-20 02:49:40.000000 tencentcloud-sdk-python-tdmq-3.0.918/tencentcloud/tdmq/v20200217/models.py
+-rw-r--r--   0 root         (0) root         (0)    10117 2023-06-20 02:49:40.000000 tencentcloud-sdk-python-tdmq-3.0.918/tencentcloud/tdmq/v20200217/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   110163 2023-06-20 02:49:40.000000 tencentcloud-sdk-python-tdmq-3.0.918/tencentcloud/tdmq/v20200217/tdmq_client.py
+-rw-r--r--   0 root         (0) root         (0)      740 2023-06-20 02:49:40.000000 tencentcloud-sdk-python-tdmq-3.0.918/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-06-20 02:49:40.000000 tencentcloud-sdk-python-tdmq-3.0.918/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-06-20 02:49:40.000000 tencentcloud-sdk-python-tdmq-3.0.918/setup.py
```

### Comparing `tencentcloud-sdk-python-tdmq-3.0.917/tencentcloud_sdk_python_tdmq.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tdmq-3.0.918/tencentcloud_sdk_python_tdmq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tdmq
-Version: 3.0.917
+Version: 3.0.918
 Summary: Tencent Cloud Tdmq SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tdmq-3.0.917/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tdmq-3.0.918/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tdmq-3.0.917/tencentcloud/tdmq/v20200217/models.py` & `tencentcloud-sdk-python-tdmq-3.0.918/tencentcloud/tdmq/v20200217/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -10749,14 +10749,84 @@
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.RequestId = params.get("RequestId")
 
 
+class SendRocketMQMessageRequest(AbstractModel):
+    """SendRocketMQMessage请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ClusterId: 集群id
+        :type ClusterId: str
+        :param NamespaceId: 命名空间
+        :type NamespaceId: str
+        :param TopicName: topic名称
+        :type TopicName: str
+        :param MsgBody: 信息内容
+        :type MsgBody: str
+        :param MsgKey: 消息key信息
+        :type MsgKey: str
+        :param MsgTag: 消息tag信息
+        :type MsgTag: str
+        """
+        self.ClusterId = None
+        self.NamespaceId = None
+        self.TopicName = None
+        self.MsgBody = None
+        self.MsgKey = None
+        self.MsgTag = None
+
+
+    def _deserialize(self, params):
+        self.ClusterId = params.get("ClusterId")
+        self.NamespaceId = params.get("NamespaceId")
+        self.TopicName = params.get("TopicName")
+        self.MsgBody = params.get("MsgBody")
+        self.MsgKey = params.get("MsgKey")
+        self.MsgTag = params.get("MsgTag")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class SendRocketMQMessageResponse(AbstractModel):
+    """SendRocketMQMessage返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Result: 发送结果
+        :type Result: bool
+        :param MsgId: 消息ID
+注意：此字段可能返回 null，表示取不到有效值。
+        :type MsgId: str
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.Result = None
+        self.MsgId = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.Result = params.get("Result")
+        self.MsgId = params.get("MsgId")
+        self.RequestId = params.get("RequestId")
+
+
 class Sort(AbstractModel):
     """排序器
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-tdmq-3.0.917/tencentcloud/tdmq/v20200217/errorcodes.py` & `tencentcloud-sdk-python-tdmq-3.0.918/tencentcloud/tdmq/v20200217/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tdmq-3.0.917/tencentcloud/tdmq/v20200217/tdmq_client.py` & `tencentcloud-sdk-python-tdmq-3.0.918/tencentcloud/tdmq/v20200217/tdmq_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -2748,14 +2748,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def SendRocketMQMessage(self, request):
+        """发送RocketMQ消息
+
+        :param request: Request instance for SendRocketMQMessage.
+        :type request: :class:`tencentcloud.tdmq.v20200217.models.SendRocketMQMessageRequest`
+        :rtype: :class:`tencentcloud.tdmq.v20200217.models.SendRocketMQMessageResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("SendRocketMQMessage", params, headers=headers)
+            response = json.loads(body)
+            model = models.SendRocketMQMessageResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def UnbindCmqDeadLetter(self, request):
         """解绑cmq死信队列
 
         :param request: Request instance for UnbindCmqDeadLetter.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.UnbindCmqDeadLetterRequest`
         :rtype: :class:`tencentcloud.tdmq.v20200217.models.UnbindCmqDeadLetterResponse`
```

### Comparing `tencentcloud-sdk-python-tdmq-3.0.917/README.rst` & `tencentcloud-sdk-python-tdmq-3.0.918/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tdmq-3.0.917/PKG-INFO` & `tencentcloud-sdk-python-tdmq-3.0.918/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tdmq
-Version: 3.0.917
+Version: 3.0.918
 Summary: Tencent Cloud Tdmq SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tdmq-3.0.917/setup.py` & `tencentcloud-sdk-python-tdmq-3.0.918/setup.py`

 * *Files identical despite different names*

