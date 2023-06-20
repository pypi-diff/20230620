# Comparing `tmp/tencentcloud-sdk-python-sms-3.0.917.tar.gz` & `tmp/tencentcloud-sdk-python-sms-3.0.918.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-sms-3.0.917.tar", last modified: Mon Jun 19 00:31:58 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-sms-3.0.918.tar", last modified: Tue Jun 20 02:47:07 2023, max compression
```

## Comparing `tencentcloud-sdk-python-sms-3.0.917.tar` & `tencentcloud-sdk-python-sms-3.0.918.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:31:58.000000 tencentcloud-sdk-python-sms-3.0.917/
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-19 00:31:58.000000 tencentcloud-sdk-python-sms-3.0.917/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:31:58.000000 tencentcloud-sdk-python-sms-3.0.917/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-19 00:31:58.000000 tencentcloud-sdk-python-sms-3.0.917/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:31:58.000000 tencentcloud-sdk-python-sms-3.0.917/tencentcloud/sms/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 00:31:58.000000 tencentcloud-sdk-python-sms-3.0.917/tencentcloud/sms/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:31:58.000000 tencentcloud-sdk-python-sms-3.0.917/tencentcloud/sms/v20190711/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 00:31:58.000000 tencentcloud-sdk-python-sms-3.0.917/tencentcloud/sms/v20190711/__init__.py
--rw-r--r--   0 root         (0) root         (0)    60170 2023-06-19 00:31:58.000000 tencentcloud-sdk-python-sms-3.0.917/tencentcloud/sms/v20190711/models.py
--rw-r--r--   0 root         (0) root         (0)    26567 2023-06-19 00:31:58.000000 tencentcloud-sdk-python-sms-3.0.917/tencentcloud/sms/v20190711/sms_client.py
--rw-r--r--   0 root         (0) root         (0)    18520 2023-06-19 00:31:58.000000 tencentcloud-sdk-python-sms-3.0.917/tencentcloud/sms/v20190711/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:31:58.000000 tencentcloud-sdk-python-sms-3.0.917/tencentcloud/sms/v20210111/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 00:31:58.000000 tencentcloud-sdk-python-sms-3.0.917/tencentcloud/sms/v20210111/__init__.py
--rw-r--r--   0 root         (0) root         (0)    68482 2023-06-19 00:31:58.000000 tencentcloud-sdk-python-sms-3.0.917/tencentcloud/sms/v20210111/models.py
--rw-r--r--   0 root         (0) root         (0)    28333 2023-06-19 00:31:58.000000 tencentcloud-sdk-python-sms-3.0.917/tencentcloud/sms/v20210111/sms_client.py
--rw-r--r--   0 root         (0) root         (0)    19342 2023-06-19 00:31:58.000000 tencentcloud-sdk-python-sms-3.0.917/tencentcloud/sms/v20210111/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:31:58.000000 tencentcloud-sdk-python-sms-3.0.917/tencentcloud_sdk_python_sms.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-19 00:31:58.000000 tencentcloud-sdk-python-sms-3.0.917/tencentcloud_sdk_python_sms.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      603 2023-06-19 00:31:58.000000 tencentcloud-sdk-python-sms-3.0.917/tencentcloud_sdk_python_sms.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-19 00:31:58.000000 tencentcloud-sdk-python-sms-3.0.917/tencentcloud_sdk_python_sms.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-19 00:31:58.000000 tencentcloud-sdk-python-sms-3.0.917/tencentcloud_sdk_python_sms.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-19 00:31:58.000000 tencentcloud-sdk-python-sms-3.0.917/README.rst
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-19 00:31:58.000000 tencentcloud-sdk-python-sms-3.0.917/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-19 00:31:58.000000 tencentcloud-sdk-python-sms-3.0.917/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:47:07.000000 tencentcloud-sdk-python-sms-3.0.918/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-20 02:47:07.000000 tencentcloud-sdk-python-sms-3.0.918/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:47:07.000000 tencentcloud-sdk-python-sms-3.0.918/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-20 02:47:07.000000 tencentcloud-sdk-python-sms-3.0.918/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:47:07.000000 tencentcloud-sdk-python-sms-3.0.918/tencentcloud/sms/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 02:47:07.000000 tencentcloud-sdk-python-sms-3.0.918/tencentcloud/sms/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:47:07.000000 tencentcloud-sdk-python-sms-3.0.918/tencentcloud/sms/v20190711/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 02:47:07.000000 tencentcloud-sdk-python-sms-3.0.918/tencentcloud/sms/v20190711/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    60203 2023-06-20 02:47:07.000000 tencentcloud-sdk-python-sms-3.0.918/tencentcloud/sms/v20190711/models.py
+-rw-r--r--   0 root         (0) root         (0)    26567 2023-06-20 02:47:07.000000 tencentcloud-sdk-python-sms-3.0.918/tencentcloud/sms/v20190711/sms_client.py
+-rw-r--r--   0 root         (0) root         (0)    18520 2023-06-20 02:47:07.000000 tencentcloud-sdk-python-sms-3.0.918/tencentcloud/sms/v20190711/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:47:07.000000 tencentcloud-sdk-python-sms-3.0.918/tencentcloud/sms/v20210111/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 02:47:07.000000 tencentcloud-sdk-python-sms-3.0.918/tencentcloud/sms/v20210111/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    68515 2023-06-20 02:47:07.000000 tencentcloud-sdk-python-sms-3.0.918/tencentcloud/sms/v20210111/models.py
+-rw-r--r--   0 root         (0) root         (0)    28333 2023-06-20 02:47:07.000000 tencentcloud-sdk-python-sms-3.0.918/tencentcloud/sms/v20210111/sms_client.py
+-rw-r--r--   0 root         (0) root         (0)    19342 2023-06-20 02:47:07.000000 tencentcloud-sdk-python-sms-3.0.918/tencentcloud/sms/v20210111/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:47:07.000000 tencentcloud-sdk-python-sms-3.0.918/tencentcloud_sdk_python_sms.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 02:47:07.000000 tencentcloud-sdk-python-sms-3.0.918/tencentcloud_sdk_python_sms.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      603 2023-06-20 02:47:07.000000 tencentcloud-sdk-python-sms-3.0.918/tencentcloud_sdk_python_sms.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-20 02:47:07.000000 tencentcloud-sdk-python-sms-3.0.918/tencentcloud_sdk_python_sms.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-20 02:47:07.000000 tencentcloud-sdk-python-sms-3.0.918/tencentcloud_sdk_python_sms.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-20 02:47:07.000000 tencentcloud-sdk-python-sms-3.0.918/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-20 02:47:07.000000 tencentcloud-sdk-python-sms-3.0.918/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-20 02:47:07.000000 tencentcloud-sdk-python-sms-3.0.918/setup.py
```

### Comparing `tencentcloud-sdk-python-sms-3.0.917/tencentcloud/__init__.py` & `tencentcloud-sdk-python-sms-3.0.918/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-sms-3.0.917/tencentcloud/sms/v20190711/models.py` & `tencentcloud-sdk-python-sms-3.0.918/tencentcloud/sms/v20190711/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1305,15 +1305,15 @@
         :type SmsSdkAppid: str
         :param Sign: 短信签名内容，使用 UTF-8 编码，必须填写已审核通过的签名，签名信息可登录 [短信控制台](https://console.cloud.tencent.com/smsv2)  查看。注：国内短信为必填参数。
         :type Sign: str
         :param TemplateParamSet: 模板参数，若无模板参数，则设置为空。
         :type TemplateParamSet: list of str
         :param ExtendCode: 短信码号扩展号，默认未开通，如需开通请联系 [sms helper](https://cloud.tencent.com/document/product/382/3773)。
         :type ExtendCode: str
-        :param SessionContext: 用户的 session 内容，可以携带用户侧 ID 等上下文信息，server 会原样返回。
+        :param SessionContext: 用户的 session 内容，可以携带用户侧 ID 等上下文信息，server 会原样返回。注意长度需小于512字节。
         :type SessionContext: str
         :param SenderId: 国内短信无senderid，无需填写该项；若需开通国际/港澳台短信senderid，请联系smshelper。
         :type SenderId: str
         """
         self.PhoneNumberSet = None
         self.TemplateID = None
         self.SmsSdkAppid = None
```

### Comparing `tencentcloud-sdk-python-sms-3.0.917/tencentcloud/sms/v20190711/sms_client.py` & `tencentcloud-sdk-python-sms-3.0.918/tencentcloud/sms/v20190711/sms_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-sms-3.0.917/tencentcloud/sms/v20190711/errorcodes.py` & `tencentcloud-sdk-python-sms-3.0.918/tencentcloud/sms/v20190711/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-sms-3.0.917/tencentcloud/sms/v20210111/models.py` & `tencentcloud-sdk-python-sms-3.0.918/tencentcloud/sms/v20210111/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1493,15 +1493,15 @@
 <dx-alert infotype="notice" title="注意">发送国内短信该参数必填。</dx-alert>
         :type SignName: str
         :param TemplateParamSet: 模板参数，若无模板参数，则设置为空。
 <dx-alert infotype="notice" title="注意">模板参数的个数需要与 TemplateId 对应模板的变量个数保持一致。</dx-alert>
         :type TemplateParamSet: list of str
         :param ExtendCode: 短信码号扩展号，默认未开通，如需开通请联系 [腾讯云短信小助手](https://cloud.tencent.com/document/product/382/3773#.E6.8A.80.E6.9C.AF.E4.BA.A4.E6.B5.81)。
         :type ExtendCode: str
-        :param SessionContext: 用户的 session 内容，可以携带用户侧 ID 等上下文信息，server 会原样返回。
+        :param SessionContext: 用户的 session 内容，可以携带用户侧 ID 等上下文信息，server 会原样返回。注意长度需小于512字节。
         :type SessionContext: str
         :param SenderId: 国内短信无需填写该项；国际/港澳台短信已申请独立 SenderId 需要填写该字段，默认使用公共 SenderId，无需填写该字段。
 注：月度使用量达到指定量级可申请独立 SenderId 使用，详情请联系 [腾讯云短信小助手](https://cloud.tencent.com/document/product/382/3773#.E6.8A.80.E6.9C.AF.E4.BA.A4.E6.B5.81)。
         :type SenderId: str
         """
         self.PhoneNumberSet = None
         self.SmsSdkAppId = None
```

### Comparing `tencentcloud-sdk-python-sms-3.0.917/tencentcloud/sms/v20210111/sms_client.py` & `tencentcloud-sdk-python-sms-3.0.918/tencentcloud/sms/v20210111/sms_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-sms-3.0.917/tencentcloud/sms/v20210111/errorcodes.py` & `tencentcloud-sdk-python-sms-3.0.918/tencentcloud/sms/v20210111/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-sms-3.0.917/tencentcloud_sdk_python_sms.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-sms-3.0.918/tencentcloud_sdk_python_sms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-sms-3.0.917/tencentcloud_sdk_python_sms.egg-info/PKG-INFO` & `tencentcloud-sdk-python-sms-3.0.918/tencentcloud_sdk_python_sms.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-sms
-Version: 3.0.917
+Version: 3.0.918
 Summary: Tencent Cloud Sms SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-sms-3.0.917/README.rst` & `tencentcloud-sdk-python-sms-3.0.918/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-sms-3.0.917/PKG-INFO` & `tencentcloud-sdk-python-sms-3.0.918/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-sms
-Version: 3.0.917
+Version: 3.0.918
 Summary: Tencent Cloud Sms SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-sms-3.0.917/setup.py` & `tencentcloud-sdk-python-sms-3.0.918/setup.py`

 * *Files identical despite different names*

