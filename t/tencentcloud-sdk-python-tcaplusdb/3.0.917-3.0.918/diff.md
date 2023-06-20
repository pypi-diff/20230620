# Comparing `tmp/tencentcloud-sdk-python-tcaplusdb-3.0.917.tar.gz` & `tmp/tencentcloud-sdk-python-tcaplusdb-3.0.918.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tcaplusdb-3.0.917.tar", last modified: Mon Jun 19 00:33:31 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tcaplusdb-3.0.918.tar", last modified: Tue Jun 20 02:48:42 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tcaplusdb-3.0.917.tar` & `tencentcloud-sdk-python-tcaplusdb-3.0.918.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:33:31.000000 tencentcloud-sdk-python-tcaplusdb-3.0.917/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:33:31.000000 tencentcloud-sdk-python-tcaplusdb-3.0.917/tencentcloud_sdk_python_tcaplusdb.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-19 00:33:31.000000 tencentcloud-sdk-python-tcaplusdb-3.0.917/tencentcloud_sdk_python_tcaplusdb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      505 2023-06-19 00:33:31.000000 tencentcloud-sdk-python-tcaplusdb-3.0.917/tencentcloud_sdk_python_tcaplusdb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1689 2023-06-19 00:33:31.000000 tencentcloud-sdk-python-tcaplusdb-3.0.917/tencentcloud_sdk_python_tcaplusdb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-19 00:33:31.000000 tencentcloud-sdk-python-tcaplusdb-3.0.917/tencentcloud_sdk_python_tcaplusdb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-19 00:33:31.000000 tencentcloud-sdk-python-tcaplusdb-3.0.917/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:33:31.000000 tencentcloud-sdk-python-tcaplusdb-3.0.917/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-19 00:33:31.000000 tencentcloud-sdk-python-tcaplusdb-3.0.917/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:33:31.000000 tencentcloud-sdk-python-tcaplusdb-3.0.917/tencentcloud/tcaplusdb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:33:31.000000 tencentcloud-sdk-python-tcaplusdb-3.0.917/tencentcloud/tcaplusdb/v20190823/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 00:33:31.000000 tencentcloud-sdk-python-tcaplusdb-3.0.917/tencentcloud/tcaplusdb/v20190823/__init__.py
--rw-r--r--   0 root         (0) root         (0)   195509 2023-06-19 00:33:31.000000 tencentcloud-sdk-python-tcaplusdb-3.0.917/tencentcloud/tcaplusdb/v20190823/models.py
--rw-r--r--   0 root         (0) root         (0)    48988 2023-06-19 00:33:31.000000 tencentcloud-sdk-python-tcaplusdb-3.0.917/tencentcloud/tcaplusdb/v20190823/tcaplusdb_client.py
--rw-r--r--   0 root         (0) root         (0)     3614 2023-06-19 00:33:31.000000 tencentcloud-sdk-python-tcaplusdb-3.0.917/tencentcloud/tcaplusdb/v20190823/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 00:33:31.000000 tencentcloud-sdk-python-tcaplusdb-3.0.917/tencentcloud/tcaplusdb/__init__.py
--rw-r--r--   0 root         (0) root         (0)      755 2023-06-19 00:33:31.000000 tencentcloud-sdk-python-tcaplusdb-3.0.917/README.rst
--rw-r--r--   0 root         (0) root         (0)     1689 2023-06-19 00:33:31.000000 tencentcloud-sdk-python-tcaplusdb-3.0.917/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1018 2023-06-19 00:33:31.000000 tencentcloud-sdk-python-tcaplusdb-3.0.917/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:48:42.000000 tencentcloud-sdk-python-tcaplusdb-3.0.918/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:48:42.000000 tencentcloud-sdk-python-tcaplusdb-3.0.918/tencentcloud_sdk_python_tcaplusdb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 02:48:42.000000 tencentcloud-sdk-python-tcaplusdb-3.0.918/tencentcloud_sdk_python_tcaplusdb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      505 2023-06-20 02:48:42.000000 tencentcloud-sdk-python-tcaplusdb-3.0.918/tencentcloud_sdk_python_tcaplusdb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1689 2023-06-20 02:48:42.000000 tencentcloud-sdk-python-tcaplusdb-3.0.918/tencentcloud_sdk_python_tcaplusdb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-20 02:48:42.000000 tencentcloud-sdk-python-tcaplusdb-3.0.918/tencentcloud_sdk_python_tcaplusdb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-20 02:48:42.000000 tencentcloud-sdk-python-tcaplusdb-3.0.918/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:48:42.000000 tencentcloud-sdk-python-tcaplusdb-3.0.918/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-20 02:48:42.000000 tencentcloud-sdk-python-tcaplusdb-3.0.918/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:48:42.000000 tencentcloud-sdk-python-tcaplusdb-3.0.918/tencentcloud/tcaplusdb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:48:42.000000 tencentcloud-sdk-python-tcaplusdb-3.0.918/tencentcloud/tcaplusdb/v20190823/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 02:48:42.000000 tencentcloud-sdk-python-tcaplusdb-3.0.918/tencentcloud/tcaplusdb/v20190823/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   195859 2023-06-20 02:48:42.000000 tencentcloud-sdk-python-tcaplusdb-3.0.918/tencentcloud/tcaplusdb/v20190823/models.py
+-rw-r--r--   0 root         (0) root         (0)    48988 2023-06-20 02:48:42.000000 tencentcloud-sdk-python-tcaplusdb-3.0.918/tencentcloud/tcaplusdb/v20190823/tcaplusdb_client.py
+-rw-r--r--   0 root         (0) root         (0)     3614 2023-06-20 02:48:42.000000 tencentcloud-sdk-python-tcaplusdb-3.0.918/tencentcloud/tcaplusdb/v20190823/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 02:48:42.000000 tencentcloud-sdk-python-tcaplusdb-3.0.918/tencentcloud/tcaplusdb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      755 2023-06-20 02:48:42.000000 tencentcloud-sdk-python-tcaplusdb-3.0.918/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1689 2023-06-20 02:48:42.000000 tencentcloud-sdk-python-tcaplusdb-3.0.918/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1018 2023-06-20 02:48:42.000000 tencentcloud-sdk-python-tcaplusdb-3.0.918/setup.py
```

### Comparing `tencentcloud-sdk-python-tcaplusdb-3.0.917/tencentcloud_sdk_python_tcaplusdb.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tcaplusdb-3.0.918/tencentcloud_sdk_python_tcaplusdb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tcaplusdb
-Version: 3.0.917
+Version: 3.0.918
 Summary: Tencent Cloud Tcaplusdb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tcaplusdb-3.0.917/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tcaplusdb-3.0.918/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tcaplusdb-3.0.917/tencentcloud/tcaplusdb/v20190823/models.py` & `tencentcloud-sdk-python-tcaplusdb-3.0.918/tencentcloud/tcaplusdb/v20190823/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -2304,15 +2304,15 @@
 
     def __init__(self):
         r"""
         :param ClusterId: 待查询表格所属集群ID
         :type ClusterId: str
         :param TableGroupIds: 待查询表格所属表格组ID列表
         :type TableGroupIds: list of str
-        :param SelectedTables: 待查询表格信息列表
+        :param SelectedTables: 待查询表格信息列表，用户不用关注，过滤请使用filter
         :type SelectedTables: list of SelectedTableInfoNew
         :param Filters: 过滤条件，本接口支持：TableName，TableInstanceId
         :type Filters: list of Filter
         :param Offset: 查询结果偏移量
         :type Offset: int
         :param Limit: 查询结果返回记录数量
         :type Limit: int
@@ -2833,23 +2833,28 @@
     """
 
     def __init__(self):
         r"""
         :param TaskId: TaskId由 AppInstanceId-taskId 组成，以区分不同集群的任务
 注意：此字段可能返回 null，表示取不到有效值。
         :type TaskId: str
+        :param ApplicationId: ApplicationId由 AppInstanceId-applicationId 组成，以区分不同集群的申请
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ApplicationId: str
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.TaskId = None
+        self.ApplicationId = None
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.TaskId = params.get("TaskId")
+        self.ApplicationId = params.get("ApplicationId")
         self.RequestId = params.get("RequestId")
 
 
 class KafkaInfo(AbstractModel):
     """ckafka地址信息
 
     """
```

### Comparing `tencentcloud-sdk-python-tcaplusdb-3.0.917/tencentcloud/tcaplusdb/v20190823/tcaplusdb_client.py` & `tencentcloud-sdk-python-tcaplusdb-3.0.918/tencentcloud/tcaplusdb/v20190823/tcaplusdb_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tcaplusdb-3.0.917/tencentcloud/tcaplusdb/v20190823/errorcodes.py` & `tencentcloud-sdk-python-tcaplusdb-3.0.918/tencentcloud/tcaplusdb/v20190823/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tcaplusdb-3.0.917/README.rst` & `tencentcloud-sdk-python-tcaplusdb-3.0.918/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tcaplusdb-3.0.917/PKG-INFO` & `tencentcloud-sdk-python-tcaplusdb-3.0.918/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tcaplusdb
-Version: 3.0.917
+Version: 3.0.918
 Summary: Tencent Cloud Tcaplusdb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tcaplusdb-3.0.917/setup.py` & `tencentcloud-sdk-python-tcaplusdb-3.0.918/setup.py`

 * *Files identical despite different names*

