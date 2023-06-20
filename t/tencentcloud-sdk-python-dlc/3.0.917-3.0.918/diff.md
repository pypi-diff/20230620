# Comparing `tmp/tencentcloud-sdk-python-dlc-3.0.917.tar.gz` & `tmp/tencentcloud-sdk-python-dlc-3.0.918.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-dlc-3.0.917.tar", last modified: Mon Jun 19 00:23:52 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-dlc-3.0.918.tar", last modified: Tue Jun 20 02:39:06 2023, max compression
```

## Comparing `tencentcloud-sdk-python-dlc-3.0.917.tar` & `tencentcloud-sdk-python-dlc-3.0.918.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:23:52.000000 tencentcloud-sdk-python-dlc-3.0.917/
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-19 00:23:52.000000 tencentcloud-sdk-python-dlc-3.0.917/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:23:52.000000 tencentcloud-sdk-python-dlc-3.0.917/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-19 00:23:52.000000 tencentcloud-sdk-python-dlc-3.0.917/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:23:52.000000 tencentcloud-sdk-python-dlc-3.0.917/tencentcloud/dlc/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 00:23:52.000000 tencentcloud-sdk-python-dlc-3.0.917/tencentcloud/dlc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:23:52.000000 tencentcloud-sdk-python-dlc-3.0.917/tencentcloud/dlc/v20210125/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 00:23:52.000000 tencentcloud-sdk-python-dlc-3.0.917/tencentcloud/dlc/v20210125/__init__.py
--rw-r--r--   0 root         (0) root         (0)   342962 2023-06-19 00:23:52.000000 tencentcloud-sdk-python-dlc-3.0.917/tencentcloud/dlc/v20210125/models.py
--rw-r--r--   0 root         (0) root         (0)    11538 2023-06-19 00:23:52.000000 tencentcloud-sdk-python-dlc-3.0.917/tencentcloud/dlc/v20210125/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    82270 2023-06-19 00:23:52.000000 tencentcloud-sdk-python-dlc-3.0.917/tencentcloud/dlc/v20210125/dlc_client.py
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-19 00:23:52.000000 tencentcloud-sdk-python-dlc-3.0.917/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 00:23:52.000000 tencentcloud-sdk-python-dlc-3.0.917/tencentcloud_sdk_python_dlc.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-19 00:23:52.000000 tencentcloud-sdk-python-dlc-3.0.917/tencentcloud_sdk_python_dlc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-19 00:23:52.000000 tencentcloud-sdk-python-dlc-3.0.917/tencentcloud_sdk_python_dlc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-19 00:23:52.000000 tencentcloud-sdk-python-dlc-3.0.917/tencentcloud_sdk_python_dlc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-19 00:23:52.000000 tencentcloud-sdk-python-dlc-3.0.917/tencentcloud_sdk_python_dlc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-19 00:23:52.000000 tencentcloud-sdk-python-dlc-3.0.917/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-19 00:23:52.000000 tencentcloud-sdk-python-dlc-3.0.917/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:39:06.000000 tencentcloud-sdk-python-dlc-3.0.918/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-20 02:39:06.000000 tencentcloud-sdk-python-dlc-3.0.918/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:39:06.000000 tencentcloud-sdk-python-dlc-3.0.918/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-20 02:39:06.000000 tencentcloud-sdk-python-dlc-3.0.918/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:39:06.000000 tencentcloud-sdk-python-dlc-3.0.918/tencentcloud/dlc/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 02:39:06.000000 tencentcloud-sdk-python-dlc-3.0.918/tencentcloud/dlc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:39:06.000000 tencentcloud-sdk-python-dlc-3.0.918/tencentcloud/dlc/v20210125/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 02:39:06.000000 tencentcloud-sdk-python-dlc-3.0.918/tencentcloud/dlc/v20210125/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   351937 2023-06-20 02:39:06.000000 tencentcloud-sdk-python-dlc-3.0.918/tencentcloud/dlc/v20210125/models.py
+-rw-r--r--   0 root         (0) root         (0)    11538 2023-06-20 02:39:06.000000 tencentcloud-sdk-python-dlc-3.0.918/tencentcloud/dlc/v20210125/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    82316 2023-06-20 02:39:06.000000 tencentcloud-sdk-python-dlc-3.0.918/tencentcloud/dlc/v20210125/dlc_client.py
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-20 02:39:06.000000 tencentcloud-sdk-python-dlc-3.0.918/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:39:06.000000 tencentcloud-sdk-python-dlc-3.0.918/tencentcloud_sdk_python_dlc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 02:39:06.000000 tencentcloud-sdk-python-dlc-3.0.918/tencentcloud_sdk_python_dlc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-20 02:39:06.000000 tencentcloud-sdk-python-dlc-3.0.918/tencentcloud_sdk_python_dlc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-20 02:39:06.000000 tencentcloud-sdk-python-dlc-3.0.918/tencentcloud_sdk_python_dlc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-20 02:39:06.000000 tencentcloud-sdk-python-dlc-3.0.918/tencentcloud_sdk_python_dlc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-20 02:39:06.000000 tencentcloud-sdk-python-dlc-3.0.918/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-20 02:39:06.000000 tencentcloud-sdk-python-dlc-3.0.918/setup.py
```

### Comparing `tencentcloud-sdk-python-dlc-3.0.917/tencentcloud/__init__.py` & `tencentcloud-sdk-python-dlc-3.0.918/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-dlc-3.0.917/tencentcloud/dlc/v20210125/models.py` & `tencentcloud-sdk-python-dlc-3.0.918/tencentcloud/dlc/v20210125/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -964,14 +964,89 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class CommonMetrics(AbstractModel):
+    """任务公共指标
+
+    """
+
+    def __init__(self):
+        r"""
+        :param CreateTaskTime: 创建任务时长，单位：ms
+注意：此字段可能返回 null，表示取不到有效值。
+        :type CreateTaskTime: float
+        :param ProcessTime: 预处理总时长，单位：ms
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ProcessTime: float
+        :param QueueTime: 排队时长，单位：ms
+注意：此字段可能返回 null，表示取不到有效值。
+        :type QueueTime: float
+        :param ExecutionTime: 执行时长，单位：ms
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ExecutionTime: float
+        :param IsResultCacheHit: 是否命中结果缓存
+注意：此字段可能返回 null，表示取不到有效值。
+        :type IsResultCacheHit: bool
+        :param MatchedMVBytes: 匹配物化视图数据量
+注意：此字段可能返回 null，表示取不到有效值。
+        :type MatchedMVBytes: int
+        :param MatchedMVs: 匹配物化视图列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type MatchedMVs: str
+        :param AffectedBytes: 结果数据量，单位：byte
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AffectedBytes: str
+        :param AffectedRows: 	结果行数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AffectedRows: int
+        :param ProcessedBytes: 扫描数据量，单位：byte
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ProcessedBytes: int
+        :param ProcessedRows: 	扫描行数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ProcessedRows: int
+        """
+        self.CreateTaskTime = None
+        self.ProcessTime = None
+        self.QueueTime = None
+        self.ExecutionTime = None
+        self.IsResultCacheHit = None
+        self.MatchedMVBytes = None
+        self.MatchedMVs = None
+        self.AffectedBytes = None
+        self.AffectedRows = None
+        self.ProcessedBytes = None
+        self.ProcessedRows = None
+
+
+    def _deserialize(self, params):
+        self.CreateTaskTime = params.get("CreateTaskTime")
+        self.ProcessTime = params.get("ProcessTime")
+        self.QueueTime = params.get("QueueTime")
+        self.ExecutionTime = params.get("ExecutionTime")
+        self.IsResultCacheHit = params.get("IsResultCacheHit")
+        self.MatchedMVBytes = params.get("MatchedMVBytes")
+        self.MatchedMVs = params.get("MatchedMVs")
+        self.AffectedBytes = params.get("AffectedBytes")
+        self.AffectedRows = params.get("AffectedRows")
+        self.ProcessedBytes = params.get("ProcessedBytes")
+        self.ProcessedRows = params.get("ProcessedRows")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class CreateDMSDatabaseRequest(AbstractModel):
     """CreateDMSDatabase请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -1184,15 +1259,15 @@
         :type Tags: list of TagInfo
         :param AutoSuspend: 是否自定挂起集群：false（默认）：不自动挂起、true：自动挂起
         :type AutoSuspend: bool
         :param CrontabResumeSuspend: 定时启停集群策略：0（默认）：关闭定时策略、1：开启定时策略（注：定时启停策略与自动挂起策略互斥）
         :type CrontabResumeSuspend: int
         :param CrontabResumeSuspendStrategy: 定时启停策略，复杂类型：包含启停时间、挂起集群策略
         :type CrontabResumeSuspendStrategy: :class:`tencentcloud.dlc.v20210125.models.CrontabResumeSuspendStrategy`
-        :param EngineExecType: 引擎执行任务类型，默认为SQL
+        :param EngineExecType: 引擎执行任务类型，有效值：SQL/BATCH，默认为SQL
         :type EngineExecType: str
         :param MaxConcurrency: 单个集群最大并发任务数，默认5
         :type MaxConcurrency: int
         :param TolerableQueueTime: 可容忍的排队时间，默认0。当任务排队的时间超过可容忍的时间时可能会触发扩容。如果该参数为0，则表示一旦有任务排队就可能立即触发扩容。
         :type TolerableQueueTime: int
         :param AutoSuspendTime: 集群自动挂起时间，默认10分钟
         :type AutoSuspendTime: int
@@ -1752,15 +1827,15 @@
 
     def __init__(self):
         r"""
         :param SessionId: Session唯一标识
         :type SessionId: str
         :param Code: 执行的代码
         :type Code: str
-        :param Kind: 类型，当前支持：spark、pyspark、sparkr、sql
+        :param Kind: 类型，当前支持：sql
         :type Kind: str
         :param SaveResult: 是否保存运行结果
         :type SaveResult: bool
         """
         self.SessionId = None
         self.Code = None
         self.Kind = None
@@ -1913,61 +1988,61 @@
 class CreateSparkAppRequest(AbstractModel):
     """CreateSparkApp请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param AppName: spark应用名
+        :param AppName: spark作业名
         :type AppName: str
-        :param AppType: 1代表spark jar应用，2代表spark streaming应用
+        :param AppType: spark作业类型，1代表spark jar作业，2代表spark streaming作业
         :type AppType: int
-        :param DataEngine: 执行spark作业的数据引擎
+        :param DataEngine: 执行spark作业的数据引擎名称
         :type DataEngine: str
-        :param AppFile: spark应用的执行入口
+        :param AppFile: spark作业程序包文件路径
         :type AppFile: str
-        :param RoleArn: 执行spark作业的角色ID
+        :param RoleArn: 数据访问策略，CAM Role arn
         :type RoleArn: int
-        :param AppDriverSize: spark作业driver资源规格大小, 可取small,medium,large,xlarge
+        :param AppDriverSize: 指定的Driver规格，当前支持：small（默认，1cu）、medium（2cu）、large（4cu）、xlarge（8cu）
         :type AppDriverSize: str
-        :param AppExecutorSize: spark作业executor资源规格大小, 可取small,medium,large,xlarge
+        :param AppExecutorSize: 指定的Executor规格，当前支持：small（默认，1cu）、medium（2cu）、large（4cu）、xlarge（8cu）
         :type AppExecutorSize: str
         :param AppExecutorNums: spark作业executor个数
         :type AppExecutorNums: int
         :param Eni: 该字段已下线，请使用字段Datasource
         :type Eni: str
-        :param IsLocal: 是否本地上传，可去cos,lakefs
+        :param IsLocal: spark作业程序包是否本地上传，cos：存放与cos，lakefs：本地上传（控制台使用，该方式不支持直接接口调用）
         :type IsLocal: str
-        :param MainClass: spark jar作业时的主类
+        :param MainClass: spark作业主类
         :type MainClass: str
         :param AppConf: spark配置，以换行符分隔
         :type AppConf: str
-        :param IsLocalJars: 是否本地上传，包含cos,lakefs
+        :param IsLocalJars: spark 作业依赖jar包是否本地上传，cos：存放与cos，lakefs：本地上传（控制台使用，该方式不支持直接接口调用）
         :type IsLocalJars: str
-        :param AppJars: spark jar作业依赖jars，以逗号分隔
+        :param AppJars: spark 作业依赖jar包（--jars），以逗号分隔
         :type AppJars: str
-        :param IsLocalFiles: 是否本地上传，包含cos,lakefs
+        :param IsLocalFiles: spark作业依赖文件资源是否本地上传，cos：存放与cos，lakefs：本地上传（控制台使用，该方式不支持直接接口调用）
         :type IsLocalFiles: str
-        :param AppFiles: spark作业依赖资源，以逗号分隔
+        :param AppFiles: spark作业依赖文件资源（--files）（非jar、zip），以逗号分隔
         :type AppFiles: str
-        :param CmdArgs: spark作业命令行参数
+        :param CmdArgs: spark作业程序入参，空格分割
         :type CmdArgs: str
-        :param MaxRetries: 只对spark流任务生效
+        :param MaxRetries: 最大重试次数，只对spark流任务生效
         :type MaxRetries: int
-        :param DataSource: 数据源名
+        :param DataSource: 数据源名称
         :type DataSource: str
-        :param IsLocalPythonFiles: pyspark：依赖上传方式，1、cos；2、lakefs（控制台使用，该方式不支持直接接口调用）
+        :param IsLocalPythonFiles: pyspark：依赖上传方式，cos：存放与cos，lakefs：本地上传（控制台使用，该方式不支持直接接口调用）
         :type IsLocalPythonFiles: str
-        :param AppPythonFiles: pyspark：python依赖, 除py文件外，还支持zip/egg等归档格式，多文件以逗号分隔
+        :param AppPythonFiles: pyspark作业依赖python资源（--py-files），支持py/zip/egg等归档格式，多文件以逗号分隔
         :type AppPythonFiles: str
-        :param IsLocalArchives: archives：依赖上传方式，1、cos；2、lakefs（控制台使用，该方式不支持直接接口调用）
+        :param IsLocalArchives: spark作业依赖archives资源是否本地上传，cos：存放与cos，lakefs：本地上传（控制台使用，该方式不支持直接接口调用）
         :type IsLocalArchives: str
-        :param AppArchives: archives：依赖资源
+        :param AppArchives: spark作业依赖archives资源（--archives），支持tar.gz/tgz/tar等归档格式，以逗号分隔
         :type AppArchives: str
-        :param SparkImage: Spark Image 版本
+        :param SparkImage: Spark Image 版本号
         :type SparkImage: str
         :param SparkImageVersion: Spark Image 版本名称
         :type SparkImageVersion: str
         :param AppExecutorMaxNumbers: 指定的Executor数量（最大值），默认为1，当开启动态分配有效，若未开启，则该值等于AppExecutorNums
         :type AppExecutorMaxNumbers: int
         :param SessionId: 关联dlc查询脚本id
         :type SessionId: str
@@ -2069,15 +2144,15 @@
 
     """
 
     def __init__(self):
         r"""
         :param JobName: spark作业名
         :type JobName: str
-        :param CmdArgs: spark作业的命令行参数，以空格分隔；一般用于周期性调用使用
+        :param CmdArgs: spark作业程序入参，以空格分隔；一般用于周期性调用使用
         :type CmdArgs: str
         """
         self.JobName = None
         self.CmdArgs = None
 
 
     def _deserialize(self, params):
@@ -3633,15 +3708,15 @@
 class DeleteSparkAppRequest(AbstractModel):
     """DeleteSparkApp请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param AppName: spark应用名
+        :param AppName: spark作业名
         :type AppName: str
         """
         self.AppName = None
 
 
     def _deserialize(self, params):
         self.AppName = params.get("AppName")
@@ -4248,35 +4323,29 @@
 
     """
 
     def __init__(self):
         r"""
         :param Offset: 偏移量，默认为0。
         :type Offset: int
-        :param Filters: 滤类型，传参Name应为以下其中一个,
-data-engine-name - String 
-engine-type - String
-state - String 
-mode - String 
-create-time - String 
-message - String
+        :param Filters: 过滤类型，支持如下的过滤类型，传参Name应为以下其中一个, data-engine-name - String（数据引擎名称）：engine-type - String（引擎类型：spark：spark 引擎，presto：presto引擎），state - String (数据引擎状态 -2已删除 -1失败 0初始化中 1挂起 2运行中 3准备删除 4删除中) ， mode - String（计费模式 0共享模式 1按量计费 2包年包月） ， create-time - String（创建时间，10位时间戳） message - String （描述信息），cluster-type - String (集群资源类型 spark_private/presto_private/presto_cu/spark_cu)，engine-id - String（数据引擎ID），key-word - String（数据引擎名称或集群资源类型或描述信息模糊搜索），engine-exec-type - String（引擎执行任务类型，SQL/BATCH）
         :type Filters: list of Filter
         :param SortBy: 排序字段，支持如下字段类型，create-time
         :type SortBy: str
         :param Sorting: 排序方式，desc表示正序，asc表示反序， 默认为asc。
         :type Sorting: str
         :param Limit: 返回数量，默认为10，最大值为100。
         :type Limit: int
         :param DatasourceConnectionName: 已废弃，请使用DatasourceConnectionNameSet
         :type DatasourceConnectionName: str
         :param ExcludePublicEngine: 是否不返回共享引擎，true不返回共享引擎，false可以返回共享引擎
         :type ExcludePublicEngine: bool
         :param AccessTypes: 参数应该为引擎权限类型，有效类型："USE", "MODIFY", "OPERATE", "MONITOR", "DELETE"
         :type AccessTypes: list of str
-        :param EngineExecType: 引擎执行任务类型，有效值：SQL/BATCH
+        :param EngineExecType: 引擎执行任务类型，有效值：SQL/BATCH，默认为SQL
         :type EngineExecType: str
         :param EngineType: 引擎类型，有效值：spark/presto
         :type EngineType: str
         :param DatasourceConnectionNameSet: 网络配置列表，若传入该参数，则返回网络配置关联的计算引擎
         :type DatasourceConnectionNameSet: list of str
         """
         self.Offset = None
@@ -4361,15 +4430,15 @@
         :type Limit: int
         :param Offset: 数据偏移量，从0开始，默认为0。
         :type Offset: int
         :param KeyWord: 模糊匹配，库名关键字。
         :type KeyWord: str
         :param DatasourceConnectionName: 数据源唯名称，该名称可以通过DescribeDatasourceConnection接口查询到。默认为DataLakeCatalog
         :type DatasourceConnectionName: str
-        :param Sort: 排序字段，当前版本仅支持按库名排序
+        :param Sort: 排序字段，CreateTime：创建时间，Name：数据库名称
         :type Sort: str
         :param Asc: 排序类型：false：降序（默认）、true：升序
         :type Asc: bool
         """
         self.Limit = None
         self.Offset = None
         self.KeyWord = None
@@ -4427,15 +4496,15 @@
 class DescribeEngineUsageInfoRequest(AbstractModel):
     """DescribeEngineUsageInfo请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param DataEngineId: House Id
+        :param DataEngineId: 数据引擎ID
         :type DataEngineId: str
         """
         self.DataEngineId = None
 
 
     def _deserialize(self, params):
         self.DataEngineId = params.get("DataEngineId")
@@ -4847,17 +4916,17 @@
         :type DataEngineName: str
         :param State: Session状态，包含：not_started（未启动）、starting（已启动）、idle（等待输入）、busy(正在运行statement)、shutting_down（停止）、error（异常）、dead（已退出）、killed（被杀死）、success（正常停止）
         :type State: list of str
         :param SortFields: 排序字段（默认按创建时间）
         :type SortFields: list of str
         :param Asc: 排序字段：true：升序、false：降序（默认）
         :type Asc: bool
-        :param Limit: 分页字段
+        :param Limit: 分页参数，默认10
         :type Limit: int
-        :param Offset: 分页字段
+        :param Offset: 分页参数，默认0
         :type Offset: int
         """
         self.DataEngineName = None
         self.State = None
         self.SortFields = None
         self.Asc = None
         self.Limit = None
@@ -5073,15 +5142,15 @@
 class DescribeSparkAppJobRequest(AbstractModel):
     """DescribeSparkAppJob请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param JobId: spark作业Id，与JobName同时存在时，JobName无效
+        :param JobId: spark作业Id，与JobName同时存在时，JobName无效，JobId与JobName至少存在一个
         :type JobId: str
         :param JobName: spark作业名
         :type JobName: str
         """
         self.JobId = None
         self.JobName = None
 
@@ -5133,15 +5202,15 @@
 
     def __init__(self):
         r"""
         :param SortBy: 返回结果按照该字段排序
         :type SortBy: str
         :param Sorting: 正序或者倒序，例如：desc
         :type Sorting: str
-        :param Filters: 按照该参数过滤,支持spark-job-name
+        :param Filters: 过滤条件，如下支持的过滤类型，传参Name应为其一:spark-job-name（作业名称），spark-job-id（作业id），spark-app-type（作业类型，1：批任务，2：流任务，4：SQL作业），user-name（创建人），key-word（作业名称或ID关键词模糊搜索）
         :type Filters: list of Filter
         :param StartTime: 更新时间起始点，支持格式：yyyy-MM-dd HH:mm:ss
         :type StartTime: str
         :param EndTime: 更新时间截止点，支持格式：yyyy-MM-dd HH:mm:ss
         :type EndTime: str
         :param Offset: 查询列表偏移量, 默认值0
         :type Offset: int
@@ -5220,17 +5289,17 @@
         :type JobId: str
         :param Offset: 分页查询偏移量
         :type Offset: int
         :param Limit: 分页查询Limit
         :type Limit: int
         :param TaskId: 执行实例id
         :type TaskId: str
-        :param StartTime: 更新时间起始点
+        :param StartTime: 更新时间起始点，支持格式：yyyy-MM-dd HH:mm:ss
         :type StartTime: str
-        :param EndTime: 更新时间截止点
+        :param EndTime: 更新时间截止点，支持格式：yyyy-MM-dd HH:mm:ss
         :type EndTime: str
         :param Filters: 按照该参数过滤,支持task-state
         :type Filters: list of Filter
         """
         self.JobId = None
         self.Offset = None
         self.Limit = None
@@ -5453,19 +5522,19 @@
         :type Offset: int
         :param Filters: 过滤条件，如下支持的过滤类型，传参Name应为其一
 table-name - String - （过滤条件）数据表名称,形如：table-001。
 table-id - String - （过滤条件）table id形如：12342。
         :type Filters: list of Filter
         :param DatasourceConnectionName: 指定查询的数据源名称，默认为DataLakeCatalog
         :type DatasourceConnectionName: str
-        :param StartTime: 起始时间：用于对更新时间的筛选
+        :param StartTime: 起始时间：用于对更新时间的筛选，格式为yyyy-mm-dd HH:MM:SS
         :type StartTime: str
-        :param EndTime: 终止时间：用于对更新时间的筛选
+        :param EndTime: 终止时间：用于对更新时间的筛选，格式为yyyy-mm-dd HH:MM:SS
         :type EndTime: str
-        :param Sort: 排序字段，支持：CreateTime、UpdateTime、StorageSize、RecordCount、Name（不传则默认按name升序）
+        :param Sort: 排序字段，支持：CreateTime（创建时间）、UpdateTime（更新时间）、StorageSize（存储空间）、RecordCount（行数）、Name（表名称）（不传则默认按name升序）
         :type Sort: str
         :param Asc: 排序字段，false：降序（默认）；true：升序
         :type Asc: bool
         :param TableType: table type，表类型查询,可用值:EXTERNAL_TABLE,INDEX_TABLE,MANAGED_TABLE,MATERIALIZED_VIEW,TABLE,VIEW,VIRTUAL_VIEW
         :type TableType: str
         :param TableFormat: 筛选字段-表格式：不传（默认）为查全部；LAKEFS：托管表；ICEBERG：非托管iceberg表；HIVE：非托管hive表；OTHER：非托管其它；
         :type TableFormat: str
@@ -5617,15 +5686,15 @@
         :type SortBy: str
         :param Sorting: 排序方式，desc表示正序，asc表示反序， 默认为asc。
         :type Sorting: str
         :param StartTime: 起始时间点，格式为yyyy-mm-dd HH:MM:SS。默认为45天前的当前时刻
         :type StartTime: str
         :param EndTime: 结束时间点，格式为yyyy-mm-dd HH:MM:SS时间跨度在(0,30天]，支持最近45天数据查询。默认为当前时刻
         :type EndTime: str
-        :param DataEngineName: 支持计算资源名字筛选
+        :param DataEngineName: 数据引擎名称，用于筛选
         :type DataEngineName: str
         """
         self.Limit = None
         self.Offset = None
         self.Filters = None
         self.SortBy = None
         self.Sorting = None
@@ -6733,63 +6802,63 @@
 class ModifySparkAppRequest(AbstractModel):
     """ModifySparkApp请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param AppName: spark应用名
+        :param AppName: spark作业名
         :type AppName: str
-        :param AppType: 1代表spark jar应用，2代表spark streaming应用
+        :param AppType: spark作业类型，1代表spark jar作业，2代表spark streaming作业
         :type AppType: int
-        :param DataEngine: 执行spark作业的数据引擎
+        :param DataEngine: 执行spark作业的数据引擎名称
         :type DataEngine: str
-        :param AppFile: spark应用的执行入口
+        :param AppFile: spark作业程序包文件路径
         :type AppFile: str
-        :param RoleArn: 执行spark作业的角色ID
+        :param RoleArn: 数据访问策略，CAM Role arn
         :type RoleArn: int
-        :param AppDriverSize: spark作业driver资源规格大小, 可取small,medium,large,xlarge
+        :param AppDriverSize: 指定的Driver规格，当前支持：small（默认，1cu）、medium（2cu）、large（4cu）、xlarge（8cu）
         :type AppDriverSize: str
-        :param AppExecutorSize: spark作业executor资源规格大小, 可取small,medium,large,xlarge
+        :param AppExecutorSize: 指定的Executor规格，当前支持：small（默认，1cu）、medium（2cu）、large（4cu）、xlarge（8cu）
         :type AppExecutorSize: str
         :param AppExecutorNums: spark作业executor个数
         :type AppExecutorNums: int
-        :param SparkAppId: spark应用Id
+        :param SparkAppId: spark作业Id
         :type SparkAppId: str
         :param Eni: 该字段已下线，请使用字段Datasource
         :type Eni: str
-        :param IsLocal: 是否本地上传，可取cos,lakefs
+        :param IsLocal: spark作业程序包是否本地上传，cos：存放与cos，lakefs：本地上传（控制台使用，该方式不支持直接接口调用）
         :type IsLocal: str
-        :param MainClass: spark jar作业时的主类
+        :param MainClass: spark作业主类
         :type MainClass: str
         :param AppConf: spark配置，以换行符分隔
         :type AppConf: str
-        :param IsLocalJars: jar资源依赖上传方式，1、cos；2、lakefs（控制台使用，该方式不支持直接接口调用）
+        :param IsLocalJars: spark 作业依赖jar包是否本地上传，cos：存放与cos，lakefs：本地上传（控制台使用，该方式不支持直接接口调用）
         :type IsLocalJars: str
-        :param AppJars: spark jar作业依赖jars，以逗号分隔
+        :param AppJars: spark 作业依赖jar包（--jars），以逗号分隔
         :type AppJars: str
-        :param IsLocalFiles: file资源依赖上传方式，1、cos；2、lakefs（控制台使用，该方式不支持直接接口调用）
+        :param IsLocalFiles: spark作业依赖文件资源是否本地上传，cos：存放与cos，lakefs：本地上传（控制台使用，该方式不支持直接接口调用）
         :type IsLocalFiles: str
-        :param AppFiles: spark作业依赖资源，以逗号分隔
+        :param AppFiles: spark作业依赖文件资源（--files）（非jar、zip），以逗号分隔
         :type AppFiles: str
-        :param IsLocalPythonFiles: pyspark：依赖上传方式，1、cos；2、lakefs（控制台使用，该方式不支持直接接口调用）
+        :param IsLocalPythonFiles: pyspark：依赖上传方式，cos：存放与cos，lakefs：本地上传（控制台使用，该方式不支持直接接口调用）
         :type IsLocalPythonFiles: str
-        :param AppPythonFiles: pyspark：python依赖, 除py文件外，还支持zip/egg等归档格式，多文件以逗号分隔
+        :param AppPythonFiles: pyspark作业依赖python资源（--py-files），支持py/zip/egg等归档格式，多文件以逗号分隔
         :type AppPythonFiles: str
-        :param CmdArgs: spark作业命令行参数
+        :param CmdArgs: spark作业程序入参
         :type CmdArgs: str
-        :param MaxRetries: 只对spark流任务生效
+        :param MaxRetries: 最大重试次数，只对spark流任务生效
         :type MaxRetries: int
         :param DataSource: 数据源名
         :type DataSource: str
-        :param IsLocalArchives: archives：依赖上传方式，1、cos；2、lakefs（控制台使用，该方式不支持直接接口调用）
+        :param IsLocalArchives: spark作业依赖archives资源是否本地上传，cos：存放与cos，lakefs：本地上传（控制台使用，该方式不支持直接接口调用）
         :type IsLocalArchives: str
-        :param AppArchives: archives：依赖资源
+        :param AppArchives: spark作业依赖archives资源（--archives），支持tar.gz/tgz/tar等归档格式，以逗号分隔
         :type AppArchives: str
-        :param SparkImage: Spark Image 版本
+        :param SparkImage: Spark Image 版本号
         :type SparkImage: str
         :param SparkImageVersion: Spark Image 版本名称
         :type SparkImageVersion: str
         :param AppExecutorMaxNumbers: 指定的Executor数量（最大值），默认为1，当开启动态分配有效，若未开启，则该值等于AppExecutorNums
         :type AppExecutorMaxNumbers: int
         :param SessionId: 关联dlc查询脚本
         :type SessionId: str
@@ -7552,14 +7621,44 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class PrestoMonitorMetrics(AbstractModel):
+    """Presto监控指标
+
+    """
+
+    def __init__(self):
+        r"""
+        :param LocalCacheHitRate: 	Alluxio本地缓存命中率
+注意：此字段可能返回 null，表示取不到有效值。
+        :type LocalCacheHitRate: float
+        :param FragmentCacheHitRate: Fragment缓存命中率
+注意：此字段可能返回 null，表示取不到有效值。
+        :type FragmentCacheHitRate: float
+        """
+        self.LocalCacheHitRate = None
+        self.FragmentCacheHitRate = None
+
+
+    def _deserialize(self, params):
+        self.LocalCacheHitRate = params.get("LocalCacheHitRate")
+        self.FragmentCacheHitRate = params.get("FragmentCacheHitRate")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class Property(AbstractModel):
     """数据库和数据表属性信息
 
     """
 
     def __init__(self):
         r"""
@@ -7950,14 +8049,44 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class SparkMonitorMetrics(AbstractModel):
+    """Spark监控数据
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ShuffleWriteBytesCos: shuffle写溢出到COS数据量，单位：byte
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ShuffleWriteBytesCos: int
+        :param ShuffleWriteBytesTotal: shuffle写数据量，单位：byte
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ShuffleWriteBytesTotal: int
+        """
+        self.ShuffleWriteBytesCos = None
+        self.ShuffleWriteBytesTotal = None
+
+
+    def _deserialize(self, params):
+        self.ShuffleWriteBytesCos = params.get("ShuffleWriteBytesCos")
+        self.ShuffleWriteBytesTotal = params.get("ShuffleWriteBytesTotal")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class SparkSessionBatchLog(AbstractModel):
     """SparkSQL批任务运行日志
 
     """
 
     def __init__(self):
         r"""
@@ -8725,14 +8854,23 @@
         :type ExecutorSize: str
         :param ExecutorNums: 指定executor数量，最小值为1，最大值小于集群规格
 注意：此字段可能返回 null，表示取不到有效值。
         :type ExecutorNums: int
         :param ExecutorMaxNumbers: 指定executor max数量（动态配置场景下），最小值为1，最大值小于集群规格（当ExecutorMaxNumbers小于ExecutorNums时，改值设定为ExecutorNums）
 注意：此字段可能返回 null，表示取不到有效值。
         :type ExecutorMaxNumbers: int
+        :param CommonMetrics: 任务公共指标数据
+注意：此字段可能返回 null，表示取不到有效值。
+        :type CommonMetrics: :class:`tencentcloud.dlc.v20210125.models.CommonMetrics`
+        :param SparkMonitorMetrics: spark任务指标数据
+注意：此字段可能返回 null，表示取不到有效值。
+        :type SparkMonitorMetrics: :class:`tencentcloud.dlc.v20210125.models.SparkMonitorMetrics`
+        :param PrestoMonitorMetrics: presto任务指标数据
+注意：此字段可能返回 null，表示取不到有效值。
+        :type PrestoMonitorMetrics: :class:`tencentcloud.dlc.v20210125.models.PrestoMonitorMetrics`
         """
         self.DatabaseName = None
         self.DataAmount = None
         self.Id = None
         self.UsedTime = None
         self.OutputPath = None
         self.CreateTime = None
@@ -8763,14 +8901,17 @@
         self.TotalTime = None
         self.CmdArgs = None
         self.ImageVersion = None
         self.DriverSize = None
         self.ExecutorSize = None
         self.ExecutorNums = None
         self.ExecutorMaxNumbers = None
+        self.CommonMetrics = None
+        self.SparkMonitorMetrics = None
+        self.PrestoMonitorMetrics = None
 
 
     def _deserialize(self, params):
         self.DatabaseName = params.get("DatabaseName")
         self.DataAmount = params.get("DataAmount")
         self.Id = params.get("Id")
         self.UsedTime = params.get("UsedTime")
@@ -8803,14 +8944,23 @@
         self.TotalTime = params.get("TotalTime")
         self.CmdArgs = params.get("CmdArgs")
         self.ImageVersion = params.get("ImageVersion")
         self.DriverSize = params.get("DriverSize")
         self.ExecutorSize = params.get("ExecutorSize")
         self.ExecutorNums = params.get("ExecutorNums")
         self.ExecutorMaxNumbers = params.get("ExecutorMaxNumbers")
+        if params.get("CommonMetrics") is not None:
+            self.CommonMetrics = CommonMetrics()
+            self.CommonMetrics._deserialize(params.get("CommonMetrics"))
+        if params.get("SparkMonitorMetrics") is not None:
+            self.SparkMonitorMetrics = SparkMonitorMetrics()
+            self.SparkMonitorMetrics._deserialize(params.get("SparkMonitorMetrics"))
+        if params.get("PrestoMonitorMetrics") is not None:
+            self.PrestoMonitorMetrics = PrestoMonitorMetrics()
+            self.PrestoMonitorMetrics._deserialize(params.get("PrestoMonitorMetrics"))
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-dlc-3.0.917/tencentcloud/dlc/v20210125/errorcodes.py` & `tencentcloud-sdk-python-dlc-3.0.918/tencentcloud/dlc/v20210125/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dlc-3.0.917/tencentcloud/dlc/v20210125/dlc_client.py` & `tencentcloud-sdk-python-dlc-3.0.918/tencentcloud/dlc/v20210125/dlc_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -207,15 +207,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def CancelNotebookSessionStatement(self, request):
-        """本接口（CancelNotebookSessionStatement）用于取消session statement
+        """本接口（CancelNotebookSessionStatement）用于取消session中执行的任务
 
         :param request: Request instance for CancelNotebookSessionStatement.
         :type request: :class:`tencentcloud.dlc.v20210125.models.CancelNotebookSessionStatementRequest`
         :rtype: :class:`tencentcloud.dlc.v20210125.models.CancelNotebookSessionStatementResponse`
 
         """
         try:
@@ -230,15 +230,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def CancelNotebookSessionStatementBatch(self, request):
-        """本接口（CancelNotebookSessionStatementBatch）用于按批取消Session statement。
+        """本接口（CancelNotebookSessionStatementBatch）用于批量取消Session 中执行的任务
 
         :param request: Request instance for CancelNotebookSessionStatementBatch.
         :type request: :class:`tencentcloud.dlc.v20210125.models.CancelNotebookSessionStatementBatchRequest`
         :rtype: :class:`tencentcloud.dlc.v20210125.models.CancelNotebookSessionStatementBatchResponse`
 
         """
         try:
@@ -276,15 +276,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def CancelTask(self, request):
-        """本接口（CancelTask），用于取消任务执行
+        """本接口（CancelTask），用于取消任务
 
         :param request: Request instance for CancelTask.
         :type request: :class:`tencentcloud.dlc.v20210125.models.CancelTaskRequest`
         :rtype: :class:`tencentcloud.dlc.v20210125.models.CancelTaskResponse`
 
         """
         try:
@@ -483,15 +483,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def CreateNotebookSession(self, request):
-        """本接口（CreateNotebookSession）用于创建notebook livy session
+        """本接口（CreateNotebookSession）用于创建交互式session（notebook）
 
         :param request: Request instance for CreateNotebookSession.
         :type request: :class:`tencentcloud.dlc.v20210125.models.CreateNotebookSessionRequest`
         :rtype: :class:`tencentcloud.dlc.v20210125.models.CreateNotebookSessionResponse`
 
         """
         try:
@@ -506,15 +506,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def CreateNotebookSessionStatement(self, request):
-        """本接口（CreateNotebookSessionStatement）用于创建session statement
+        """本接口（CreateNotebookSessionStatement）用于在session中执行代码片段
 
         :param request: Request instance for CreateNotebookSessionStatement.
         :type request: :class:`tencentcloud.dlc.v20210125.models.CreateNotebookSessionStatementRequest`
         :rtype: :class:`tencentcloud.dlc.v20210125.models.CreateNotebookSessionStatementResponse`
 
         """
         try:
@@ -529,15 +529,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def CreateNotebookSessionStatementSupportBatchSQL(self, request):
-        """本接口（CreateNotebookSessionStatementSupportBatchSQL）用于创建Statement批量运行SQL任务。
+        """本接口（CreateNotebookSessionStatementSupportBatchSQL）用于创建交互式session并执行SQL任务
 
         :param request: Request instance for CreateNotebookSessionStatementSupportBatchSQL.
         :type request: :class:`tencentcloud.dlc.v20210125.models.CreateNotebookSessionStatementSupportBatchSQLRequest`
         :rtype: :class:`tencentcloud.dlc.v20210125.models.CreateNotebookSessionStatementSupportBatchSQLResponse`
 
         """
         try:
@@ -598,15 +598,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def CreateSparkApp(self, request):
-        """创建spark应用
+        """创建spark作业
 
         :param request: Request instance for CreateSparkApp.
         :type request: :class:`tencentcloud.dlc.v20210125.models.CreateSparkAppRequest`
         :rtype: :class:`tencentcloud.dlc.v20210125.models.CreateSparkAppResponse`
 
         """
         try:
@@ -621,15 +621,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def CreateSparkAppTask(self, request):
-        """创建spark任务
+        """启动Spark作业
 
         :param request: Request instance for CreateSparkAppTask.
         :type request: :class:`tencentcloud.dlc.v20210125.models.CreateSparkAppTaskRequest`
         :rtype: :class:`tencentcloud.dlc.v20210125.models.CreateSparkAppTaskResponse`
 
         """
         try:
@@ -713,15 +713,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def CreateTask(self, request):
-        """本接口（CreateTask）用于创建sql查询任务。（推荐使用CreateTasks接口）
+        """本接口（CreateTask）用于创建并执行SQL任务。（推荐使用CreateTasks接口）
 
         :param request: Request instance for CreateTask.
         :type request: :class:`tencentcloud.dlc.v20210125.models.CreateTaskRequest`
         :rtype: :class:`tencentcloud.dlc.v20210125.models.CreateTaskResponse`
 
         """
         try:
@@ -736,15 +736,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def CreateTasks(self, request):
-        """本接口（CreateTasks），用于批量创建任务
+        """本接口（CreateTasks），用于批量创建并执行SQL任务
 
         :param request: Request instance for CreateTasks.
         :type request: :class:`tencentcloud.dlc.v20210125.models.CreateTasksRequest`
         :rtype: :class:`tencentcloud.dlc.v20210125.models.CreateTasksResponse`
 
         """
         try:
@@ -874,15 +874,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DeleteSparkApp(self, request):
-        """删除spark应用
+        """删除spark作业
 
         :param request: Request instance for DeleteSparkApp.
         :type request: :class:`tencentcloud.dlc.v20210125.models.DeleteSparkAppRequest`
         :rtype: :class:`tencentcloud.dlc.v20210125.models.DeleteSparkAppResponse`
 
         """
         try:
@@ -1058,15 +1058,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeDataEngines(self, request):
-        """本接口（DescribeDataEngines）用于获取DataEngines信息列表
+        """本接口（DescribeDataEngines）用于查询DataEngines信息列表
 
         :param request: Request instance for DescribeDataEngines.
         :type request: :class:`tencentcloud.dlc.v20210125.models.DescribeDataEnginesRequest`
         :rtype: :class:`tencentcloud.dlc.v20210125.models.DescribeDataEnginesResponse`
 
         """
         try:
@@ -1104,15 +1104,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeEngineUsageInfo(self, request):
-        """本接口根据引擎ID获取数据引擎资源使用情况
+        """本接口根据引擎ID查询数据引擎资源使用情况
 
         :param request: Request instance for DescribeEngineUsageInfo.
         :type request: :class:`tencentcloud.dlc.v20210125.models.DescribeEngineUsageInfoRequest`
         :rtype: :class:`tencentcloud.dlc.v20210125.models.DescribeEngineUsageInfoResponse`
 
         """
         try:
@@ -1127,15 +1127,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeForbiddenTablePro(self, request):
-        """本接口（DescribeForbiddenTablePro）用于获取被禁用的表属性列表
+        """本接口（DescribeForbiddenTablePro）用于查询被禁用的表属性列表（新）
 
         :param request: Request instance for DescribeForbiddenTablePro.
         :type request: :class:`tencentcloud.dlc.v20210125.models.DescribeForbiddenTableProRequest`
         :rtype: :class:`tencentcloud.dlc.v20210125.models.DescribeForbiddenTableProResponse`
 
         """
         try:
@@ -1196,15 +1196,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeNotebookSession(self, request):
-        """本接口（DescribeNotebookSession）用于获取notebook livy session详情信息
+        """本接口（DescribeNotebookSession）用于查询交互式 session详情信息
 
         :param request: Request instance for DescribeNotebookSession.
         :type request: :class:`tencentcloud.dlc.v20210125.models.DescribeNotebookSessionRequest`
         :rtype: :class:`tencentcloud.dlc.v20210125.models.DescribeNotebookSessionResponse`
 
         """
         try:
@@ -1219,15 +1219,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeNotebookSessionLog(self, request):
-        """本接口（DescribeNotebookSessionLog）用于获取notebook livy session日志
+        """本接口（DescribeNotebookSessionLog）用于查询交互式 session日志
 
         :param request: Request instance for DescribeNotebookSessionLog.
         :type request: :class:`tencentcloud.dlc.v20210125.models.DescribeNotebookSessionLogRequest`
         :rtype: :class:`tencentcloud.dlc.v20210125.models.DescribeNotebookSessionLogResponse`
 
         """
         try:
@@ -1242,15 +1242,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeNotebookSessionStatement(self, request):
-        """本接口（DescribeNotebookSessionStatement）用于获取session statement信息
+        """本接口（DescribeNotebookSessionStatement）用于查询session 中执行任务的详情
 
         :param request: Request instance for DescribeNotebookSessionStatement.
         :type request: :class:`tencentcloud.dlc.v20210125.models.DescribeNotebookSessionStatementRequest`
         :rtype: :class:`tencentcloud.dlc.v20210125.models.DescribeNotebookSessionStatementResponse`
 
         """
         try:
@@ -1288,15 +1288,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeNotebookSessionStatements(self, request):
-        """本接口（DescribeNotebookSessionStatements）用于获取Session Statement列表。
+        """本接口（DescribeNotebookSessionStatements）用于查询Session中执行的任务列表
 
         :param request: Request instance for DescribeNotebookSessionStatements.
         :type request: :class:`tencentcloud.dlc.v20210125.models.DescribeNotebookSessionStatementsRequest`
         :rtype: :class:`tencentcloud.dlc.v20210125.models.DescribeNotebookSessionStatementsResponse`
 
         """
         try:
@@ -1311,15 +1311,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeNotebookSessions(self, request):
-        """本接口（DescribeNotebookSessions）用于获取notebook livy session列表
+        """本接口（DescribeNotebookSessions）用于查询交互式 session列表
 
         :param request: Request instance for DescribeNotebookSessions.
         :type request: :class:`tencentcloud.dlc.v20210125.models.DescribeNotebookSessionsRequest`
         :rtype: :class:`tencentcloud.dlc.v20210125.models.DescribeNotebookSessionsResponse`
 
         """
         try:
@@ -1357,15 +1357,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeScripts(self, request):
-        """该接口（DescribeScripts）用于获取所有SQL查询。
+        """该接口（DescribeScripts）用于查询SQL脚本列表
 
         :param request: Request instance for DescribeScripts.
         :type request: :class:`tencentcloud.dlc.v20210125.models.DescribeScriptsRequest`
         :rtype: :class:`tencentcloud.dlc.v20210125.models.DescribeScriptsResponse`
 
         """
         try:
@@ -1380,15 +1380,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeSparkAppJob(self, request):
-        """查询具体的spark应用
+        """查询spark作业信息
 
         :param request: Request instance for DescribeSparkAppJob.
         :type request: :class:`tencentcloud.dlc.v20210125.models.DescribeSparkAppJobRequest`
         :rtype: :class:`tencentcloud.dlc.v20210125.models.DescribeSparkAppJobResponse`
 
         """
         try:
@@ -1403,15 +1403,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeSparkAppJobs(self, request):
-        """获取spark应用列表。
+        """查询spark作业列表
 
         :param request: Request instance for DescribeSparkAppJobs.
         :type request: :class:`tencentcloud.dlc.v20210125.models.DescribeSparkAppJobsRequest`
         :rtype: :class:`tencentcloud.dlc.v20210125.models.DescribeSparkAppJobsResponse`
 
         """
         try:
@@ -1426,15 +1426,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeSparkAppTasks(self, request):
-        """查询spark应用的运行任务实例列表
+        """查询Spark作业的运行任务列表
 
         :param request: Request instance for DescribeSparkAppTasks.
         :type request: :class:`tencentcloud.dlc.v20210125.models.DescribeSparkAppTasksRequest`
         :rtype: :class:`tencentcloud.dlc.v20210125.models.DescribeSparkAppTasksResponse`
 
         """
         try:
@@ -1794,15 +1794,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def ListTaskJobLogDetail(self, request):
-        """本接口（ListTaskJobLogDetail）用于获取spark-jar日志列表
+        """本接口（ListTaskJobLogDetail）用于获取spark 作业任务日志详情
 
         :param request: Request instance for ListTaskJobLogDetail.
         :type request: :class:`tencentcloud.dlc.v20210125.models.ListTaskJobLogDetailRequest`
         :rtype: :class:`tencentcloud.dlc.v20210125.models.ListTaskJobLogDetailResponse`
 
         """
         try:
@@ -1863,15 +1863,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def ModifySparkApp(self, request):
-        """更新spark应用
+        """更新spark作业
 
         :param request: Request instance for ModifySparkApp.
         :type request: :class:`tencentcloud.dlc.v20210125.models.ModifySparkAppRequest`
         :rtype: :class:`tencentcloud.dlc.v20210125.models.ModifySparkAppResponse`
 
         """
         try:
@@ -1978,15 +1978,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def SuspendResumeDataEngine(self, request):
-        """本接口用于控制暂停或恢复数据引擎
+        """本接口用于控制挂起或启动数据引擎
 
         :param request: Request instance for SuspendResumeDataEngine.
         :type request: :class:`tencentcloud.dlc.v20210125.models.SuspendResumeDataEngineRequest`
         :rtype: :class:`tencentcloud.dlc.v20210125.models.SuspendResumeDataEngineResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-dlc-3.0.917/README.rst` & `tencentcloud-sdk-python-dlc-3.0.918/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dlc-3.0.917/tencentcloud_sdk_python_dlc.egg-info/PKG-INFO` & `tencentcloud-sdk-python-dlc-3.0.918/tencentcloud_sdk_python_dlc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dlc
-Version: 3.0.917
+Version: 3.0.918
 Summary: Tencent Cloud Dlc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dlc-3.0.917/PKG-INFO` & `tencentcloud-sdk-python-dlc-3.0.918/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dlc
-Version: 3.0.917
+Version: 3.0.918
 Summary: Tencent Cloud Dlc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dlc-3.0.917/setup.py` & `tencentcloud-sdk-python-dlc-3.0.918/setup.py`

 * *Files identical despite different names*

