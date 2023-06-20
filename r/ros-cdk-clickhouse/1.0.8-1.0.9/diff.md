# Comparing `tmp/ros-cdk-clickhouse-1.0.8.tar.gz` & `tmp/ros-cdk-clickhouse-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-clickhouse-1.0.8.tar", last modified: Thu Jul 14 02:23:12 2022, max compression
+gzip compressed data, was "dist/ros-cdk-clickhouse-1.0.9.tar", last modified: Fri Sep 23 11:19:28 2022, max compression
```

## Comparing `ros-cdk-clickhouse-1.0.8.tar` & `ros-cdk-clickhouse-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:23:12.000000 ros-cdk-clickhouse-1.0.8/
--rw-r--r--   0 root         (0) root         (0)    10279 2022-07-14 02:23:12.000000 ros-cdk-clickhouse-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2022-07-14 02:23:12.000000 ros-cdk-clickhouse-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2022-07-14 02:23:12.000000 ros-cdk-clickhouse-1.0.8/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1268 2022-07-14 02:23:12.000000 ros-cdk-clickhouse-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      200 2022-07-14 02:23:12.000000 ros-cdk-clickhouse-1.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)      106 2022-07-14 02:23:12.000000 ros-cdk-clickhouse-1.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-07-14 02:23:12.000000 ros-cdk-clickhouse-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1836 2022-07-14 02:23:12.000000 ros-cdk-clickhouse-1.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:23:12.000000 ros-cdk-clickhouse-1.0.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:23:12.000000 ros-cdk-clickhouse-1.0.8/src/ros_cdk_clickhouse/
--rw-r--r--   0 root         (0) root         (0)    56551 2022-07-14 02:23:12.000000 ros-cdk-clickhouse-1.0.8/src/ros_cdk_clickhouse/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:23:12.000000 ros-cdk-clickhouse-1.0.8/src/ros_cdk_clickhouse/_jsii/
--rw-r--r--   0 root         (0) root         (0)      397 2022-07-14 02:23:12.000000 ros-cdk-clickhouse-1.0.8/src/ros_cdk_clickhouse/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    39229 2022-07-14 02:23:12.000000 ros-cdk-clickhouse-1.0.8/src/ros_cdk_clickhouse/_jsii/ros-cdk-clickhouse@1.0.8.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:23:12.000000 ros-cdk-clickhouse-1.0.8/src/ros_cdk_clickhouse/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:23:12.000000 ros-cdk-clickhouse-1.0.8/src/ros_cdk_clickhouse.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1268 2022-07-14 02:23:12.000000 ros-cdk-clickhouse-1.0.8/src/ros_cdk_clickhouse.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      470 2022-07-14 02:23:12.000000 ros-cdk-clickhouse-1.0.8/src/ros_cdk_clickhouse.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:23:12.000000 ros-cdk-clickhouse-1.0.8/src/ros_cdk_clickhouse.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2022-07-14 02:23:12.000000 ros-cdk-clickhouse-1.0.8/src/ros_cdk_clickhouse.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2022-07-14 02:23:12.000000 ros-cdk-clickhouse-1.0.8/src/ros_cdk_clickhouse.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:19:28.000000 ros-cdk-clickhouse-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)    10279 2022-09-23 11:19:28.000000 ros-cdk-clickhouse-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-09-23 11:19:28.000000 ros-cdk-clickhouse-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2022-09-23 11:19:28.000000 ros-cdk-clickhouse-1.0.9/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1268 2022-09-23 11:19:28.000000 ros-cdk-clickhouse-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      200 2022-09-23 11:19:28.000000 ros-cdk-clickhouse-1.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      236 2022-09-23 11:19:28.000000 ros-cdk-clickhouse-1.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-09-23 11:19:28.000000 ros-cdk-clickhouse-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1865 2022-09-23 11:19:28.000000 ros-cdk-clickhouse-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:19:28.000000 ros-cdk-clickhouse-1.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:19:28.000000 ros-cdk-clickhouse-1.0.9/src/ros_cdk_clickhouse/
+-rw-r--r--   0 root         (0) root         (0)    64004 2022-09-23 11:19:28.000000 ros-cdk-clickhouse-1.0.9/src/ros_cdk_clickhouse/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:19:28.000000 ros-cdk-clickhouse-1.0.9/src/ros_cdk_clickhouse/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      431 2022-09-23 11:19:28.000000 ros-cdk-clickhouse-1.0.9/src/ros_cdk_clickhouse/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    39294 2022-09-23 11:19:28.000000 ros-cdk-clickhouse-1.0.9/src/ros_cdk_clickhouse/_jsii/ros-cdk-clickhouse@1.0.9.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 11:19:28.000000 ros-cdk-clickhouse-1.0.9/src/ros_cdk_clickhouse/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:19:28.000000 ros-cdk-clickhouse-1.0.9/src/ros_cdk_clickhouse.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1268 2022-09-23 11:19:28.000000 ros-cdk-clickhouse-1.0.9/src/ros_cdk_clickhouse.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      470 2022-09-23 11:19:28.000000 ros-cdk-clickhouse-1.0.9/src/ros_cdk_clickhouse.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 11:19:28.000000 ros-cdk-clickhouse-1.0.9/src/ros_cdk_clickhouse.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2022-09-23 11:19:28.000000 ros-cdk-clickhouse-1.0.9/src/ros_cdk_clickhouse.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2022-09-23 11:19:28.000000 ros-cdk-clickhouse-1.0.9/src/ros_cdk_clickhouse.egg-info/top_level.txt
```

### Comparing `ros-cdk-clickhouse-1.0.8/LICENSE` & `ros-cdk-clickhouse-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-clickhouse-1.0.8/PKG-INFO` & `ros-cdk-clickhouse-1.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-clickhouse
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS CLICKHOUSE Construct Library
```

### Comparing `ros-cdk-clickhouse-1.0.8/setup.py` & `ros-cdk-clickhouse-1.0.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-clickhouse",
-    "version": "1.0.8",
+    "version": "1.0.9",
     "description": "Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com",
     "license": "Apache-2.0",
     "url": "https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git",
     "long_description_content_type": "text/markdown",
     "author": "ROS Development Team",
     "bdist_wheel": {
         "universal": true
@@ -22,26 +22,27 @@
     },
     "packages": [
         "ros_cdk_clickhouse",
         "ros_cdk_clickhouse._jsii"
     ],
     "package_data": {
         "ros_cdk_clickhouse._jsii": [
-            "ros-cdk-clickhouse@1.0.8.jsii.tgz"
+            "ros-cdk-clickhouse@1.0.9.jsii.tgz"
         ],
         "ros_cdk_clickhouse": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
         "constructs>=3.0.4, <4.0.0",
-        "jsii>=1.62.0, <2.0.0",
+        "jsii>=1.68.0, <2.0.0",
         "publication>=0.0.3",
-        "ros-cdk-core>=1.0.6, <2.0.0"
+        "ros-cdk-core>=1.0.6, <2.0.0",
+        "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.7",
```

### Comparing `ros-cdk-clickhouse-1.0.8/src/ros_cdk_clickhouse/__init__.py` & `ros-cdk-clickhouse-1.0.9/src/ros_cdk_clickhouse/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 import enum
 import typing
 
 import jsii
 import publication
 import typing_extensions
 
+from typeguard import check_type
+
 from ._jsii import *
 
 import ros_cdk_core
 
 
 class DBCluster(
     ros_cdk_core.Resource,
@@ -29,217 +31,223 @@
 ):
     '''A ROS resource type:  ``ALIYUN::ClickHouse::DBCluster``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "DBClusterProps",
+        props: typing.Union["DBClusterProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::ClickHouse::DBCluster``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(DBCluster.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrAliUid")
     def attr_ali_uid(self) -> ros_cdk_core.IResolvable:
         '''Attribute AliUid: AliUid.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAliUid"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrBid")
     def attr_bid(self) -> ros_cdk_core.IResolvable:
         '''Attribute Bid: BusinessID.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrBid"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrCategory")
     def attr_category(self) -> ros_cdk_core.IResolvable:
         '''Attribute Category: Series, value: Basic: Basic version.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrCategory"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrCommodityCode")
     def attr_commodity_code(self) -> ros_cdk_core.IResolvable:
         '''Attribute CommodityCode: Product Code.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrCommodityCode"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrConnectionString")
     def attr_connection_string(self) -> ros_cdk_core.IResolvable:
         '''Attribute ConnectionString: ConnectionString.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrConnectionString"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDbClusterDescription")
     def attr_db_cluster_description(self) -> ros_cdk_core.IResolvable:
         '''Attribute DBClusterDescription: DBClusterDescription.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDbClusterDescription"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDbClusterId")
     def attr_db_cluster_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute DBClusterId: The id of DBCluster.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDbClusterId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDbClusterNetworkType")
     def attr_db_cluster_network_type(self) -> ros_cdk_core.IResolvable:
         '''Attribute DBClusterNetworkType: Network type of the cluster instance, value: VPC.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDbClusterNetworkType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDbClusterType")
     def attr_db_cluster_type(self) -> ros_cdk_core.IResolvable:
         '''Attribute DBClusterType: Cluster instance type, value:  Common: normal instance;
 
         Readonly: read-only instance; Guard: disaster recovery instance
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDbClusterType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDbClusterVersion")
     def attr_db_cluster_version(self) -> ros_cdk_core.IResolvable:
         '''Attribute DBClusterVersion: Version, value:  19.15.2.2.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDbClusterVersion"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDbNodeClass")
     def attr_db_node_class(self) -> ros_cdk_core.IResolvable:
         '''Attribute DBNodeClass: DBNodeClass.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDbNodeClass"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDbNodeCount")
     def attr_db_node_count(self) -> ros_cdk_core.IResolvable:
         '''Attribute DBNodeCount: Number of node groups.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDbNodeCount"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDbNodeStorage")
     def attr_db_node_storage(self) -> ros_cdk_core.IResolvable:
         '''Attribute DBNodeStorage: DBNodeStorage.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDbNodeStorage"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDbNodeStorageType")
     def attr_db_node_storage_type(self) -> ros_cdk_core.IResolvable:
         '''Attribute DbNodeStorageType: Instance node storage type.
 
         Valid values:  cloud_essd, cloud_efficiency.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDbNodeStorageType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrEncryptionKey")
     def attr_encryption_key(self) -> ros_cdk_core.IResolvable:
         '''Attribute EncryptionKey: KMS key ID.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrEncryptionKey"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrEncryptionType")
     def attr_encryption_type(self) -> ros_cdk_core.IResolvable:
         '''Attribute EncryptionType: Kms key type, only cloud disk encryption is supported and the value is CloudDisk.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrEncryptionType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrEngine")
     def attr_engine(self) -> ros_cdk_core.IResolvable:
         '''Attribute Engine: Engine.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrEngine"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrEngineVersion")
     def attr_engine_version(self) -> ros_cdk_core.IResolvable:
         '''Attribute EngineVersion: EngineVersion.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrEngineVersion"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrIsExpired")
     def attr_is_expired(self) -> ros_cdk_core.IResolvable:
         '''Attribute IsExpired: IsExpired.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrIsExpired"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrLockMode")
     def attr_lock_mode(self) -> ros_cdk_core.IResolvable:
         '''Attribute LockMode: LockMode.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrLockMode"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrLockReason")
     def attr_lock_reason(self) -> ros_cdk_core.IResolvable:
         '''Attribute LockReason: Reason for lock.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrLockReason"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPaymentType")
     def attr_payment_type(self) -> ros_cdk_core.IResolvable:
         '''Attribute PaymentType: PayType.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPaymentType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPeriod")
     def attr_period(self) -> ros_cdk_core.IResolvable:
         '''Attribute Period: Prepaid time period.If the payment type is Prepaid, this parameter is mandatory. Specify the prepaid cluster as a yearly or monthly type. Valid values:  Year, Month.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPeriod"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPort")
     def attr_port(self) -> ros_cdk_core.IResolvable:
         '''Attribute Port: Connection port.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPort"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPublicConnectionString")
     def attr_public_connection_string(self) -> ros_cdk_core.IResolvable:
         '''Attribute PublicConnectionString: Internet connection address.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPublicConnectionString"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPublicPort")
     def attr_public_port(self) -> ros_cdk_core.IResolvable:
         '''Attribute PublicPort: PublicPort.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPublicPort"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrStorageType")
     def attr_storage_type(self) -> ros_cdk_core.IResolvable:
         '''Attribute StorageType: StorageType.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrStorageType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVpcCloudInstanceId")
     def attr_vpc_cloud_instance_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute VpcCloudInstanceId: VpcCloudInstanceId.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVpcCloudInstanceId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVpcId")
     def attr_vpc_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute VpcId: VpcId.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVpcId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVSwitchId")
     def attr_v_switch_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute VSwitchId: VSwitchId.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVSwitchId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrZoneId")
     def attr_zone_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute ZoneId: ZoneId.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrZoneId"))
 
 
 @jsii.data_type(
@@ -300,14 +308,32 @@
         :param encryption_type: Property encryptionType: Kms key type, only cloud disk encryption is supported and the value is CloudDisk.
         :param period: Property period: Prepaid time period.If the payment type is Prepaid, this parameter is mandatory. Specify the prepaid cluster as a yearly or monthly type. Valid values: Year, Month.
         :param used_time: Property usedTime: When Period is Month, the value of UsedTime is [1-9]. When Period is Year, the value of UsedTime is [1-3]
         :param vpc_id: Property vpcId: VpcId.
         :param v_switch_id: Property vSwitchId: VSwitchId.
         :param zone_id: Property zoneId: ZoneId.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(DBClusterProps.__init__)
+            check_type(argname="argument category", value=category, expected_type=type_hints["category"])
+            check_type(argname="argument db_cluster_network_type", value=db_cluster_network_type, expected_type=type_hints["db_cluster_network_type"])
+            check_type(argname="argument db_cluster_type", value=db_cluster_type, expected_type=type_hints["db_cluster_type"])
+            check_type(argname="argument db_cluster_version", value=db_cluster_version, expected_type=type_hints["db_cluster_version"])
+            check_type(argname="argument db_node_count", value=db_node_count, expected_type=type_hints["db_node_count"])
+            check_type(argname="argument db_node_storage", value=db_node_storage, expected_type=type_hints["db_node_storage"])
+            check_type(argname="argument db_node_storage_type", value=db_node_storage_type, expected_type=type_hints["db_node_storage_type"])
+            check_type(argname="argument payment_type", value=payment_type, expected_type=type_hints["payment_type"])
+            check_type(argname="argument db_cluster_description", value=db_cluster_description, expected_type=type_hints["db_cluster_description"])
+            check_type(argname="argument encryption_key", value=encryption_key, expected_type=type_hints["encryption_key"])
+            check_type(argname="argument encryption_type", value=encryption_type, expected_type=type_hints["encryption_type"])
+            check_type(argname="argument period", value=period, expected_type=type_hints["period"])
+            check_type(argname="argument used_time", value=used_time, expected_type=type_hints["used_time"])
+            check_type(argname="argument vpc_id", value=vpc_id, expected_type=type_hints["vpc_id"])
+            check_type(argname="argument v_switch_id", value=v_switch_id, expected_type=type_hints["v_switch_id"])
+            check_type(argname="argument zone_id", value=zone_id, expected_type=type_hints["zone_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "category": category,
             "db_cluster_network_type": db_cluster_network_type,
             "db_cluster_type": db_cluster_type,
             "db_cluster_version": db_cluster_version,
             "db_node_count": db_node_count,
             "db_node_storage": db_node_storage,
@@ -485,564 +511,624 @@
 ):
     '''A ROS template type:  ``ALIYUN::ClickHouse::DBCluster``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosDBClusterProps",
+        props: typing.Union["RosDBClusterProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::ClickHouse::DBCluster``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosDBCluster.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
     @jsii.member(jsii_name="renderProperties")
     def _render_properties(
         self,
         props: typing.Mapping[builtins.str, typing.Any],
     ) -> typing.Mapping[builtins.str, typing.Any]:
         '''
         :param props: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosDBCluster._render_properties)
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.invoke(self, "renderProperties", [props]))
 
-    @jsii.python.classproperty # type: ignore[misc]
+    @jsii.python.classproperty
     @jsii.member(jsii_name="ROS_RESOURCE_TYPE_NAME")
     def ROS_RESOURCE_TYPE_NAME(cls) -> builtins.str:
         '''The resource type name for this resource class.'''
         return typing.cast(builtins.str, jsii.sget(cls, "ROS_RESOURCE_TYPE_NAME"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrAliUid")
     def attr_ali_uid(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: AliUid: AliUid
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAliUid"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrBid")
     def attr_bid(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Bid: BusinessID
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrBid"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrCategory")
     def attr_category(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Category: Series, value: Basic: Basic version
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrCategory"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrCommodityCode")
     def attr_commodity_code(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: CommodityCode: Product Code
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrCommodityCode"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrConnectionString")
     def attr_connection_string(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ConnectionString: ConnectionString
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrConnectionString"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDbClusterDescription")
     def attr_db_cluster_description(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: DBClusterDescription: DBClusterDescription
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDbClusterDescription"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDbClusterId")
     def attr_db_cluster_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: DBClusterId: The id of DBCluster
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDbClusterId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDbClusterNetworkType")
     def attr_db_cluster_network_type(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: DBClusterNetworkType: Network type of the cluster instance, value: VPC
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDbClusterNetworkType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDbClusterType")
     def attr_db_cluster_type(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: DBClusterType: Cluster instance type, value:  Common: normal instance;  Readonly: read-only instance; Guard: disaster recovery instance
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDbClusterType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDbClusterVersion")
     def attr_db_cluster_version(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: DBClusterVersion: Version, value:  19.15.2.2
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDbClusterVersion"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDbNodeClass")
     def attr_db_node_class(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: DBNodeClass: DBNodeClass
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDbNodeClass"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDbNodeCount")
     def attr_db_node_count(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: DBNodeCount: Number of node groups
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDbNodeCount"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDbNodeStorage")
     def attr_db_node_storage(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: DBNodeStorage: DBNodeStorage
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDbNodeStorage"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDbNodeStorageType")
     def attr_db_node_storage_type(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: DbNodeStorageType: Instance node storage type. Valid values:  cloud_essd, cloud_efficiency.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDbNodeStorageType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrEncryptionKey")
     def attr_encryption_key(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: EncryptionKey: KMS key ID
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrEncryptionKey"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrEncryptionType")
     def attr_encryption_type(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: EncryptionType: Kms key type, only cloud disk encryption is supported and the value is CloudDisk.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrEncryptionType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrEngine")
     def attr_engine(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Engine: Engine
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrEngine"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrEngineVersion")
     def attr_engine_version(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: EngineVersion: EngineVersion
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrEngineVersion"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrIsExpired")
     def attr_is_expired(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: IsExpired: IsExpired
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrIsExpired"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrLockMode")
     def attr_lock_mode(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: LockMode: LockMode
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrLockMode"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrLockReason")
     def attr_lock_reason(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: LockReason: Reason for lock
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrLockReason"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPaymentType")
     def attr_payment_type(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: PaymentType: PayType
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPaymentType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPeriod")
     def attr_period(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Period: Prepaid time period.If the payment type is Prepaid, this parameter is mandatory. Specify the prepaid cluster as a yearly or monthly type. Valid values:  Year, Month.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPeriod"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPort")
     def attr_port(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Port: Connection port
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPort"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPublicConnectionString")
     def attr_public_connection_string(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: PublicConnectionString: Internet connection address
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPublicConnectionString"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPublicPort")
     def attr_public_port(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: PublicPort: PublicPort
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPublicPort"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrStorageType")
     def attr_storage_type(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: StorageType: StorageType
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrStorageType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVpcCloudInstanceId")
     def attr_vpc_cloud_instance_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: VpcCloudInstanceId: VpcCloudInstanceId
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVpcCloudInstanceId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVpcId")
     def attr_vpc_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: VpcId: VpcId
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVpcId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVSwitchId")
     def attr_v_switch_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: VSwitchId: VSwitchId
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVSwitchId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrZoneId")
     def attr_zone_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ZoneId: ZoneId
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrZoneId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="category")
     def category(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: category: Series, value: Basic: Basic version
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "category"))
 
     @category.setter
     def category(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBCluster, "category").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "category", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dbClusterNetworkType")
     def db_cluster_network_type(
         self,
     ) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: dbClusterNetworkType: Network type of the cluster instance, value: VPC
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "dbClusterNetworkType"))
 
     @db_cluster_network_type.setter
     def db_cluster_network_type(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBCluster, "db_cluster_network_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dbClusterNetworkType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dbClusterType")
     def db_cluster_type(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: dbClusterType: Cluster instance type, value:  Common: normal instance;  Readonly: read-only instance; Guard: disaster recovery instance
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "dbClusterType"))
 
     @db_cluster_type.setter
     def db_cluster_type(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBCluster, "db_cluster_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dbClusterType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dbClusterVersion")
     def db_cluster_version(
         self,
     ) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: dbClusterVersion: Version, value:  19.15.2.2
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "dbClusterVersion"))
 
     @db_cluster_version.setter
     def db_cluster_version(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBCluster, "db_cluster_version").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dbClusterVersion", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dbNodeCount")
     def db_node_count(self) -> typing.Union[jsii.Number, ros_cdk_core.IResolvable]:
         '''
         :Property: dbNodeCount: Number of node groups
         '''
         return typing.cast(typing.Union[jsii.Number, ros_cdk_core.IResolvable], jsii.get(self, "dbNodeCount"))
 
     @db_node_count.setter
     def db_node_count(
         self,
         value: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBCluster, "db_node_count").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dbNodeCount", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dbNodeStorage")
     def db_node_storage(self) -> typing.Union[jsii.Number, ros_cdk_core.IResolvable]:
         '''
         :Property: dbNodeStorage: DBNodeStorage
         '''
         return typing.cast(typing.Union[jsii.Number, ros_cdk_core.IResolvable], jsii.get(self, "dbNodeStorage"))
 
     @db_node_storage.setter
     def db_node_storage(
         self,
         value: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBCluster, "db_node_storage").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dbNodeStorage", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dbNodeStorageType")
     def db_node_storage_type(
         self,
     ) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: dbNodeStorageType: Instance node storage type. Valid values:  cloud_essd, cloud_efficiency.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "dbNodeStorageType"))
 
     @db_node_storage_type.setter
     def db_node_storage_type(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBCluster, "db_node_storage_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dbNodeStorageType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBCluster, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="paymentType")
     def payment_type(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: paymentType: PayType
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "paymentType"))
 
     @payment_type.setter
     def payment_type(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBCluster, "payment_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "paymentType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dbClusterDescription")
     def db_cluster_description(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: dbClusterDescription: DBClusterDescription
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "dbClusterDescription"))
 
     @db_cluster_description.setter
     def db_cluster_description(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBCluster, "db_cluster_description").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dbClusterDescription", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="encryptionKey")
     def encryption_key(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: encryptionKey: KMS key ID
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "encryptionKey"))
 
     @encryption_key.setter
     def encryption_key(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBCluster, "encryption_key").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "encryptionKey", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="encryptionType")
     def encryption_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: encryptionType: Kms key type, only cloud disk encryption is supported and the value is CloudDisk.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "encryptionType"))
 
     @encryption_type.setter
     def encryption_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBCluster, "encryption_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "encryptionType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="period")
     def period(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: period: Prepaid time period.If the payment type is Prepaid, this parameter is mandatory. Specify the prepaid cluster as a yearly or monthly type. Valid values:  Year, Month.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "period"))
 
     @period.setter
     def period(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBCluster, "period").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "period", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="usedTime")
     def used_time(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: usedTime: When Period is Month, the value of UsedTime is [1-9].  When Period is Year, the value of UsedTime is [1-3]
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "usedTime"))
 
     @used_time.setter
     def used_time(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBCluster, "used_time").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "usedTime", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vpcId")
     def vpc_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: vpcId: VpcId
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "vpcId"))
 
     @vpc_id.setter
     def vpc_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBCluster, "vpc_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "vpcId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vSwitchId")
     def v_switch_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: vSwitchId: VSwitchId
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "vSwitchId"))
 
     @v_switch_id.setter
     def v_switch_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBCluster, "v_switch_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "vSwitchId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="zoneId")
     def zone_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: zoneId: ZoneId
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "zoneId"))
 
     @zone_id.setter
     def zone_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBCluster, "zone_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "zoneId", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-clickhouse.RosDBClusterProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -1100,14 +1186,32 @@
         :param encryption_type: 
         :param period: 
         :param used_time: 
         :param vpc_id: 
         :param v_switch_id: 
         :param zone_id: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosDBClusterProps.__init__)
+            check_type(argname="argument category", value=category, expected_type=type_hints["category"])
+            check_type(argname="argument db_cluster_network_type", value=db_cluster_network_type, expected_type=type_hints["db_cluster_network_type"])
+            check_type(argname="argument db_cluster_type", value=db_cluster_type, expected_type=type_hints["db_cluster_type"])
+            check_type(argname="argument db_cluster_version", value=db_cluster_version, expected_type=type_hints["db_cluster_version"])
+            check_type(argname="argument db_node_count", value=db_node_count, expected_type=type_hints["db_node_count"])
+            check_type(argname="argument db_node_storage", value=db_node_storage, expected_type=type_hints["db_node_storage"])
+            check_type(argname="argument db_node_storage_type", value=db_node_storage_type, expected_type=type_hints["db_node_storage_type"])
+            check_type(argname="argument payment_type", value=payment_type, expected_type=type_hints["payment_type"])
+            check_type(argname="argument db_cluster_description", value=db_cluster_description, expected_type=type_hints["db_cluster_description"])
+            check_type(argname="argument encryption_key", value=encryption_key, expected_type=type_hints["encryption_key"])
+            check_type(argname="argument encryption_type", value=encryption_type, expected_type=type_hints["encryption_type"])
+            check_type(argname="argument period", value=period, expected_type=type_hints["period"])
+            check_type(argname="argument used_time", value=used_time, expected_type=type_hints["used_time"])
+            check_type(argname="argument vpc_id", value=vpc_id, expected_type=type_hints["vpc_id"])
+            check_type(argname="argument v_switch_id", value=v_switch_id, expected_type=type_hints["v_switch_id"])
+            check_type(argname="argument zone_id", value=zone_id, expected_type=type_hints["zone_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "category": category,
             "db_cluster_network_type": db_cluster_network_type,
             "db_cluster_type": db_cluster_type,
             "db_cluster_version": db_cluster_version,
             "db_node_count": db_node_count,
             "db_node_storage": db_node_storage,
```

### Comparing `ros-cdk-clickhouse-1.0.8/src/ros_cdk_clickhouse.egg-info/PKG-INFO` & `ros-cdk-clickhouse-1.0.9/src/ros_cdk_clickhouse.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-clickhouse
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS CLICKHOUSE Construct Library
```

