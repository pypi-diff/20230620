# Comparing `tmp/tencentcloud-sdk-python-cfs-3.0.917.tar.gz` & `tmp/tencentcloud-sdk-python-cfs-3.0.918.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cfs-3.0.917.tar", last modified: Mon Jun 19 00:20:33 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cfs-3.0.918.tar", last modified: Tue Jun 20 02:35:59 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cfs-3.0.917.tar` & `tencentcloud-sdk-python-cfs-3.0.918.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:20:33.000000 tencentcloud-sdk-python-cfs-3.0.917/
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-19 00:20:33.000000 tencentcloud-sdk-python-cfs-3.0.917/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:20:33.000000 tencentcloud-sdk-python-cfs-3.0.917/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-19 00:20:33.000000 tencentcloud-sdk-python-cfs-3.0.917/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:20:33.000000 tencentcloud-sdk-python-cfs-3.0.917/tencentcloud/cfs/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 00:20:33.000000 tencentcloud-sdk-python-cfs-3.0.917/tencentcloud/cfs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:20:33.000000 tencentcloud-sdk-python-cfs-3.0.917/tencentcloud/cfs/v20190719/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 00:20:33.000000 tencentcloud-sdk-python-cfs-3.0.917/tencentcloud/cfs/v20190719/__init__.py
--rw-r--r--   0 root         (0) root         (0)    39796 2023-06-19 00:20:33.000000 tencentcloud-sdk-python-cfs-3.0.917/tencentcloud/cfs/v20190719/cfs_client.py
--rw-r--r--   0 root         (0) root         (0)   117345 2023-06-19 00:20:33.000000 tencentcloud-sdk-python-cfs-3.0.917/tencentcloud/cfs/v20190719/models.py
--rw-r--r--   0 root         (0) root         (0)    14559 2023-06-19 00:20:33.000000 tencentcloud-sdk-python-cfs-3.0.917/tencentcloud/cfs/v20190719/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-19 00:20:33.000000 tencentcloud-sdk-python-cfs-3.0.917/README.rst
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-19 00:20:33.000000 tencentcloud-sdk-python-cfs-3.0.917/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-19 00:20:33.000000 tencentcloud-sdk-python-cfs-3.0.917/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:20:33.000000 tencentcloud-sdk-python-cfs-3.0.917/tencentcloud_sdk_python_cfs.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-19 00:20:33.000000 tencentcloud-sdk-python-cfs-3.0.917/tencentcloud_sdk_python_cfs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-19 00:20:33.000000 tencentcloud-sdk-python-cfs-3.0.917/tencentcloud_sdk_python_cfs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-19 00:20:33.000000 tencentcloud-sdk-python-cfs-3.0.917/tencentcloud_sdk_python_cfs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-19 00:20:33.000000 tencentcloud-sdk-python-cfs-3.0.917/tencentcloud_sdk_python_cfs.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:35:59.000000 tencentcloud-sdk-python-cfs-3.0.918/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-20 02:35:59.000000 tencentcloud-sdk-python-cfs-3.0.918/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:35:59.000000 tencentcloud-sdk-python-cfs-3.0.918/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-20 02:35:58.000000 tencentcloud-sdk-python-cfs-3.0.918/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:35:59.000000 tencentcloud-sdk-python-cfs-3.0.918/tencentcloud/cfs/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 02:35:58.000000 tencentcloud-sdk-python-cfs-3.0.918/tencentcloud/cfs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:35:59.000000 tencentcloud-sdk-python-cfs-3.0.918/tencentcloud/cfs/v20190719/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 02:35:58.000000 tencentcloud-sdk-python-cfs-3.0.918/tencentcloud/cfs/v20190719/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    39796 2023-06-20 02:35:58.000000 tencentcloud-sdk-python-cfs-3.0.918/tencentcloud/cfs/v20190719/cfs_client.py
+-rw-r--r--   0 root         (0) root         (0)   117576 2023-06-20 02:35:58.000000 tencentcloud-sdk-python-cfs-3.0.918/tencentcloud/cfs/v20190719/models.py
+-rw-r--r--   0 root         (0) root         (0)    15741 2023-06-20 02:35:58.000000 tencentcloud-sdk-python-cfs-3.0.918/tencentcloud/cfs/v20190719/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-20 02:35:58.000000 tencentcloud-sdk-python-cfs-3.0.918/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-20 02:35:59.000000 tencentcloud-sdk-python-cfs-3.0.918/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-20 02:35:58.000000 tencentcloud-sdk-python-cfs-3.0.918/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:35:59.000000 tencentcloud-sdk-python-cfs-3.0.918/tencentcloud_sdk_python_cfs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 02:35:59.000000 tencentcloud-sdk-python-cfs-3.0.918/tencentcloud_sdk_python_cfs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-20 02:35:59.000000 tencentcloud-sdk-python-cfs-3.0.918/tencentcloud_sdk_python_cfs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-20 02:35:59.000000 tencentcloud-sdk-python-cfs-3.0.918/tencentcloud_sdk_python_cfs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-20 02:35:59.000000 tencentcloud-sdk-python-cfs-3.0.918/tencentcloud_sdk_python_cfs.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-cfs-3.0.917/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cfs-3.0.918/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cfs-3.0.917/tencentcloud/cfs/v20190719/cfs_client.py` & `tencentcloud-sdk-python-cfs-3.0.918/tencentcloud/cfs/v20190719/cfs_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cfs-3.0.917/tencentcloud/cfs/v20190719/models.py` & `tencentcloud-sdk-python-cfs-3.0.918/tencentcloud/cfs/v20190719/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,14 +53,16 @@
         :type FileSystems: list of FileSystemByPolicy
         :param DayOfMonth: 快照定期备份在一个月的某个时间；该参数与DayOfWeek,IntervalDays互斥
 注意：此字段可能返回 null，表示取不到有效值。
         :type DayOfMonth: str
         :param IntervalDays: 快照定期间隔天数，1-365 天；该参数与DayOfMonth,DayOfWeek互斥
 注意：此字段可能返回 null，表示取不到有效值。
         :type IntervalDays: int
+        :param CrossRegionsAliveDays: 跨地域复制的快照保留时间
+        :type CrossRegionsAliveDays: int
         """
         self.AutoSnapshotPolicyId = None
         self.PolicyName = None
         self.CreationTime = None
         self.FileSystemNums = None
         self.DayOfWeek = None
         self.Hour = None
@@ -69,14 +71,15 @@
         self.Status = None
         self.AppId = None
         self.AliveDays = None
         self.RegionName = None
         self.FileSystems = None
         self.DayOfMonth = None
         self.IntervalDays = None
+        self.CrossRegionsAliveDays = None
 
 
     def _deserialize(self, params):
         self.AutoSnapshotPolicyId = params.get("AutoSnapshotPolicyId")
         self.PolicyName = params.get("PolicyName")
         self.CreationTime = params.get("CreationTime")
         self.FileSystemNums = params.get("FileSystemNums")
@@ -92,14 +95,15 @@
             self.FileSystems = []
             for item in params.get("FileSystems"):
                 obj = FileSystemByPolicy()
                 obj._deserialize(item)
                 self.FileSystems.append(obj)
         self.DayOfMonth = params.get("DayOfMonth")
         self.IntervalDays = params.get("IntervalDays")
+        self.CrossRegionsAliveDays = params.get("CrossRegionsAliveDays")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-cfs-3.0.917/tencentcloud/cfs/v20190719/errorcodes.py` & `tencentcloud-sdk-python-cfs-3.0.918/tencentcloud/cfs/v20190719/errorcodes.py`

 * *Files 3% similar despite different names*

```diff
@@ -88,14 +88,17 @@
 
 # 文件系统快照策略名称超过限制。
 INVALIDPARAMETER_SNAPSHOTPOLICYNAMELIMITEXCEEDED = 'InvalidParameter.SnapshotPolicyNameLimitExceeded'
 
 # 参数取值错误。
 INVALIDPARAMETERVALUE = 'InvalidParameterValue'
 
+# 自动扩容策略不存在
+INVALIDPARAMETERVALUE_AUTOPOLICYNOTFOUND = 'InvalidParameterValue.AutoPolicyNotFound'
+
 # 用于保证请求幂等性的字符串长度超过限制（不能超过64字节）。
 INVALIDPARAMETERVALUE_CLIENTTOKENLIMITEXCEEDED = 'InvalidParameterValue.ClientTokenLimitExceeded'
 
 # 权限组名称重复。
 INVALIDPARAMETERVALUE_DUPLICATEDPGROUPNAME = 'InvalidParameterValue.DuplicatedPgroupName'
 
 # 规则IP重复。
@@ -106,14 +109,17 @@
 
 # 用户自定义名称过长（超过64字节)。
 INVALIDPARAMETERVALUE_FSNAMELIMITEXCEEDED = 'InvalidParameterValue.FsNameLimitExceeded'
 
 # 文件系统配额设置超出上限。
 INVALIDPARAMETERVALUE_FSSIZELIMITEXCEEDED = 'InvalidParameterValue.FsSizeLimitExceeded'
 
+# 无效的AliveDays值错误
+INVALIDPARAMETERVALUE_INVALIDALIVEDAYS = 'InvalidParameterValue.InvalidAliveDays'
+
 # 规则IP错误。
 INVALIDPARAMETERVALUE_INVALIDAUTHCLIENTIP = 'InvalidParameterValue.InvalidAuthClientIp'
 
 # 扩容策略参数无效
 INVALIDPARAMETERVALUE_INVALIDAUTOSCALEUPPARAMS = 'InvalidParameterValue.InvalidAutoScaleUpParams'
 
 # 用于保证请求幂等性的字符串错误。
@@ -139,14 +145,17 @@
 
 # 无效的网络类型。
 INVALIDPARAMETERVALUE_INVALIDNETINTERFACE = 'InvalidParameterValue.InvalidNetInterface'
 
 # DayOfMonth 参数错误
 INVALIDPARAMETERVALUE_INVALIDPARAMDAYOFMONTH = 'InvalidParameterValue.InvalidParamDayOfMonth'
 
+# 无效的参数，DayOfWeek
+INVALIDPARAMETERVALUE_INVALIDPARAMDAYOFWEEK = 'InvalidParameterValue.InvalidParamDayOfWeek'
+
 # IntervalDays 参数值错误
 INVALIDPARAMETERVALUE_INVALIDPARAMINTERVALDAYS = 'InvalidParameterValue.InvalidParamIntervalDays'
 
 # 权限组不属于该用户。
 INVALIDPARAMETERVALUE_INVALIDPGROUP = 'InvalidParameterValue.InvalidPgroup'
 
 # 权限组ID无效。
@@ -169,14 +178,23 @@
 
 # 读写权限设置错误。
 INVALIDPARAMETERVALUE_INVALIDRWPERMISSION = 'InvalidParameterValue.InvalidRwPermission'
 
 # 扩容目标容量参数错误
 INVALIDPARAMETERVALUE_INVALIDSCALEUPTARGETCAPACITY = 'InvalidParameterValue.InvalidScaleupTargetCapacity'
 
+# 无效的快照策略状态
+INVALIDPARAMETERVALUE_INVALIDSNAPPOLICYSTATUS = 'InvalidParameterValue.InvalidSnapPolicyStatus'
+
+# 无效的快照名称
+INVALIDPARAMETERVALUE_INVALIDSNAPSHOTNAME = 'InvalidParameterValue.InvalidSnapshotName'
+
+# 无效的快照策略名称
+INVALIDPARAMETERVALUE_INVALIDSNAPSHOTPOLICYNAME = 'InvalidParameterValue.InvalidSnapshotPolicyName'
+
 # 无效的快照状态。
 INVALIDPARAMETERVALUE_INVALIDSNAPSHOTSTATUS = 'InvalidParameterValue.InvalidSnapshotStatus'
 
 # 资源包不存在或已绑定。
 INVALIDPARAMETERVALUE_INVALIDSTORAGERESOURCEPKG = 'InvalidParameterValue.InvalidStorageResourcePkg'
 
 # 存储类型参数错误。
@@ -229,14 +247,17 @@
 
 # 权限组名称不能为空。
 INVALIDPARAMETERVALUE_MISSINGPGROUPNAME = 'InvalidParameterValue.MissingPgroupName'
 
 # 缺少快照策略参数
 INVALIDPARAMETERVALUE_MISSINGPOLICYPARAM = 'InvalidParameterValue.MissingPolicyParam'
 
+# 缺少参数Snapshot Name，或者aliveDays
+INVALIDPARAMETERVALUE_MISSINGSNAPNAMEORALIVEDAY = 'InvalidParameterValue.MissingSnapNameOrAliveDay'
+
 # 未绑定存储包。
 INVALIDPARAMETERVALUE_MISSINGSTORAGERESOURCEPKG = 'InvalidParameterValue.MissingStorageResourcePkg'
 
 # SUBNETID和UNSUBNETID不能同时为空。
 INVALIDPARAMETERVALUE_MISSINGSUBNETIDORUNSUBNETID = 'InvalidParameterValue.MissingSubnetidOrUnsubnetid'
 
 # VPC相关参数缺失。
@@ -268,14 +289,20 @@
 
 # 配额类型错误。
 INVALIDPARAMETERVALUE_QUOTAUSERTYPEERROR = 'InvalidParameterValue.QuotaUserTypeError'
 
 # 权限组规则和权限组不匹配。
 INVALIDPARAMETERVALUE_RULENOTMATCHPGROUP = 'InvalidParameterValue.RuleNotMatchPgroup'
 
+# 快照名称超限制，名称长度不超过64位字符
+INVALIDPARAMETERVALUE_SNAPSHOTNAMELIMITEXCEEDED = 'InvalidParameterValue.SnapshotNameLimitExceeded'
+
+# 快照策略名称超过64位限制
+INVALIDPARAMETERVALUE_SNAPSHOTPOLICYNAMELIMITEXCEEDED = 'InvalidParameterValue.SnapshotPolicyNameLimitExceeded'
+
 # 参数值错误: 标签键个数超过上限（6个）。
 INVALIDPARAMETERVALUE_TAGKEYFILTERLIMITEXCEEDED = 'InvalidParameterValue.TagKeyFilterLimitExceeded'
 
 # 标签键长度超过限制（不能超过127字节）。
 INVALIDPARAMETERVALUE_TAGKEYLIMITEXCEEDED = 'InvalidParameterValue.TagKeyLimitExceeded'
 
 # 标签值个数超过上限（10个）。
```

### Comparing `tencentcloud-sdk-python-cfs-3.0.917/README.rst` & `tencentcloud-sdk-python-cfs-3.0.918/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cfs-3.0.917/PKG-INFO` & `tencentcloud-sdk-python-cfs-3.0.918/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cfs
-Version: 3.0.917
+Version: 3.0.918
 Summary: Tencent Cloud Cfs SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cfs-3.0.917/setup.py` & `tencentcloud-sdk-python-cfs-3.0.918/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cfs-3.0.917/tencentcloud_sdk_python_cfs.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cfs-3.0.918/tencentcloud_sdk_python_cfs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cfs
-Version: 3.0.917
+Version: 3.0.918
 Summary: Tencent Cloud Cfs SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

