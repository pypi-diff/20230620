# Comparing `tmp/ros-cdk-adb-1.0.8.tar.gz` & `tmp/ros-cdk-adb-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-adb-1.0.8.tar", last modified: Thu Jul 14 02:27:47 2022, max compression
+gzip compressed data, was "dist/ros-cdk-adb-1.0.9.tar", last modified: Fri Sep 23 12:11:17 2022, max compression
```

## Comparing `ros-cdk-adb-1.0.8.tar` & `ros-cdk-adb-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:27:47.000000 ros-cdk-adb-1.0.8/
--rw-r--r--   0 root         (0) root         (0)    10279 2022-07-14 02:27:47.000000 ros-cdk-adb-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2022-07-14 02:27:47.000000 ros-cdk-adb-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2022-07-14 02:27:47.000000 ros-cdk-adb-1.0.8/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1240 2022-07-14 02:27:47.000000 ros-cdk-adb-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      179 2022-07-14 02:27:47.000000 ros-cdk-adb-1.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)      106 2022-07-14 02:27:47.000000 ros-cdk-adb-1.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-07-14 02:27:47.000000 ros-cdk-adb-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1794 2022-07-14 02:27:47.000000 ros-cdk-adb-1.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:27:47.000000 ros-cdk-adb-1.0.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:27:47.000000 ros-cdk-adb-1.0.8/src/ros_cdk_adb/
--rw-r--r--   0 root         (0) root         (0)    67066 2022-07-14 02:27:47.000000 ros-cdk-adb-1.0.8/src/ros_cdk_adb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:27:47.000000 ros-cdk-adb-1.0.8/src/ros_cdk_adb/_jsii/
--rw-r--r--   0 root         (0) root         (0)      370 2022-07-14 02:27:47.000000 ros-cdk-adb-1.0.8/src/ros_cdk_adb/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    45650 2022-07-14 02:27:47.000000 ros-cdk-adb-1.0.8/src/ros_cdk_adb/_jsii/ros-cdk-adb@1.0.8.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:27:47.000000 ros-cdk-adb-1.0.8/src/ros_cdk_adb/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:27:47.000000 ros-cdk-adb-1.0.8/src/ros_cdk_adb.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1240 2022-07-14 02:27:47.000000 ros-cdk-adb-1.0.8/src/ros_cdk_adb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      400 2022-07-14 02:27:47.000000 ros-cdk-adb-1.0.8/src/ros_cdk_adb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:27:47.000000 ros-cdk-adb-1.0.8/src/ros_cdk_adb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2022-07-14 02:27:47.000000 ros-cdk-adb-1.0.8/src/ros_cdk_adb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2022-07-14 02:27:47.000000 ros-cdk-adb-1.0.8/src/ros_cdk_adb.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:11:17.000000 ros-cdk-adb-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)    10279 2022-09-23 12:11:17.000000 ros-cdk-adb-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-09-23 12:11:17.000000 ros-cdk-adb-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2022-09-23 12:11:17.000000 ros-cdk-adb-1.0.9/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1240 2022-09-23 12:11:17.000000 ros-cdk-adb-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      179 2022-09-23 12:11:17.000000 ros-cdk-adb-1.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      236 2022-09-23 12:11:17.000000 ros-cdk-adb-1.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-09-23 12:11:17.000000 ros-cdk-adb-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1823 2022-09-23 12:11:17.000000 ros-cdk-adb-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:11:17.000000 ros-cdk-adb-1.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:11:17.000000 ros-cdk-adb-1.0.9/src/ros_cdk_adb/
+-rw-r--r--   0 root         (0) root         (0)    80728 2022-09-23 12:11:17.000000 ros-cdk-adb-1.0.9/src/ros_cdk_adb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:11:17.000000 ros-cdk-adb-1.0.9/src/ros_cdk_adb/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      404 2022-09-23 12:11:17.000000 ros-cdk-adb-1.0.9/src/ros_cdk_adb/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    45563 2022-09-23 12:11:17.000000 ros-cdk-adb-1.0.9/src/ros_cdk_adb/_jsii/ros-cdk-adb@1.0.9.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 12:11:17.000000 ros-cdk-adb-1.0.9/src/ros_cdk_adb/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:11:17.000000 ros-cdk-adb-1.0.9/src/ros_cdk_adb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1240 2022-09-23 12:11:17.000000 ros-cdk-adb-1.0.9/src/ros_cdk_adb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      400 2022-09-23 12:11:17.000000 ros-cdk-adb-1.0.9/src/ros_cdk_adb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 12:11:17.000000 ros-cdk-adb-1.0.9/src/ros_cdk_adb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2022-09-23 12:11:17.000000 ros-cdk-adb-1.0.9/src/ros_cdk_adb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2022-09-23 12:11:17.000000 ros-cdk-adb-1.0.9/src/ros_cdk_adb.egg-info/top_level.txt
```

### Comparing `ros-cdk-adb-1.0.8/LICENSE` & `ros-cdk-adb-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-adb-1.0.8/PKG-INFO` & `ros-cdk-adb-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-adb
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS ADB Construct Library
```

### Comparing `ros-cdk-adb-1.0.8/setup.py` & `ros-cdk-adb-1.0.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-adb",
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
         "ros_cdk_adb",
         "ros_cdk_adb._jsii"
     ],
     "package_data": {
         "ros_cdk_adb._jsii": [
-            "ros-cdk-adb@1.0.8.jsii.tgz"
+            "ros-cdk-adb@1.0.9.jsii.tgz"
         ],
         "ros_cdk_adb": [
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

### Comparing `ros-cdk-adb-1.0.8/src/ros_cdk_adb/__init__.py` & `ros-cdk-adb-1.0.9/src/ros_cdk_adb/__init__.py`

 * *Files 15% similar despite different names*

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
 
 
 class Account(
     ros_cdk_core.Resource,
@@ -29,43 +31,49 @@
 ):
     '''A ROS resource type:  ``ALIYUN::ADB::Account``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "AccountProps",
+        props: typing.Union["AccountProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::ADB::Account``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(Account.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrAccountName")
     def attr_account_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute AccountName: The name of the account.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAccountName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrAccountType")
     def attr_account_type(self) -> ros_cdk_core.IResolvable:
         '''Attribute AccountType: The type of the account.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAccountType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDbClusterId")
     def attr_db_cluster_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute DBClusterId: The ID of the cluster.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDbClusterId"))
 
 
 @jsii.data_type(
@@ -93,14 +101,21 @@
 
         :param account_name: Property accountName: The name of the account.
         :param account_password: Property accountPassword: The password of the account. The password must contain uppercase letters, lowercase letters, digits, and special characters. Special characters include ! @ # $ % ^ & * () _ + - and = The password must be 8 to 32 characters in length.
         :param db_cluster_id: Property dbClusterId: The ID of the cluster.
         :param account_description: Property accountDescription: The description of the account. The description cannot start with http://or https://. The description can be up to 256 characters in length.
         :param account_type: Property accountType: Normal: standard account Super: privileged account.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(AccountProps.__init__)
+            check_type(argname="argument account_name", value=account_name, expected_type=type_hints["account_name"])
+            check_type(argname="argument account_password", value=account_password, expected_type=type_hints["account_password"])
+            check_type(argname="argument db_cluster_id", value=db_cluster_id, expected_type=type_hints["db_cluster_id"])
+            check_type(argname="argument account_description", value=account_description, expected_type=type_hints["account_description"])
+            check_type(argname="argument account_type", value=account_type, expected_type=type_hints["account_type"])
         self._values: typing.Dict[str, typing.Any] = {
             "account_name": account_name,
             "account_password": account_password,
             "db_cluster_id": db_cluster_id,
         }
         if account_description is not None:
             self._values["account_description"] = account_description
@@ -173,43 +188,49 @@
 ):
     '''A ROS resource type:  ``ALIYUN::ADB::DBCluster``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "DBClusterProps",
+        props: typing.Union["DBClusterProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::ADB::DBCluster``.
 
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
     @jsii.member(jsii_name="attrConnectionString")
     def attr_connection_string(self) -> ros_cdk_core.IResolvable:
         '''Attribute ConnectionString: Vpc connection string.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrConnectionString"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDbClusterId")
     def attr_db_cluster_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute DBClusterId: The ID of the cluster.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDbClusterId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrOrderId")
     def attr_order_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute OrderId: The ID of the order.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrOrderId"))
 
 
 @jsii.data_type(
@@ -252,15 +273,15 @@
         db_node_group_count: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         db_node_storage: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         elastic_io_resource: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         executor_count: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         period: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         period_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         resource_group_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        tags: typing.Optional[typing.Sequence["RosDBCluster.TagsProperty"]] = None,
+        tags: typing.Optional[typing.Sequence[typing.Union["RosDBCluster.TagsProperty", typing.Dict[str, typing.Any]]]] = None,
         zone_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::ADB::DBCluster``.
 
         :param db_cluster_category: Property dbClusterCategory: The edition of the cluster. Valid values when the cluster is in reserved mode: Basic Cluster When the cluster is in elastic mode, set the value to MixedStorage.
         :param db_cluster_version: Property dbClusterVersion: The version of the cluster. Set the value to 3.0.
         :param mode: Property mode: The mode of the cluster. Valid values: Reserver: the reserved mode Flexible: the elastic mode
@@ -276,14 +297,34 @@
         :param executor_count: Property executorCount: ExecutorCount.
         :param period: Property period: Valid values when the Period parameter is set to Month: 1, 2, 3, 4, 5, 6, 7, 8, and 9. Valid values when the Period parameter is set to Year: 1, 2, and 3.
         :param period_type: Property periodType: The subscription period for the cluster. This parameter is required if the PayType parameter is set to Prepaid. Valid values: Year: subscription on a yearly basis Month: subscription on a monthly basis
         :param resource_group_id: Property resourceGroupId: The ID of the resource group.
         :param tags: Property tags: Tags to attach to instance. Max support 20 tags to add during create instance. Each tag with two properties Key and Value, and Key is required.
         :param zone_id: Property zoneId: The zone ID of the cluster. You can call the DescribeRegions operation to query the most recent zone list.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(DBClusterProps.__init__)
+            check_type(argname="argument db_cluster_category", value=db_cluster_category, expected_type=type_hints["db_cluster_category"])
+            check_type(argname="argument db_cluster_version", value=db_cluster_version, expected_type=type_hints["db_cluster_version"])
+            check_type(argname="argument mode", value=mode, expected_type=type_hints["mode"])
+            check_type(argname="argument pay_type", value=pay_type, expected_type=type_hints["pay_type"])
+            check_type(argname="argument vpc_id", value=vpc_id, expected_type=type_hints["vpc_id"])
+            check_type(argname="argument v_switch_id", value=v_switch_id, expected_type=type_hints["v_switch_id"])
+            check_type(argname="argument compute_resource", value=compute_resource, expected_type=type_hints["compute_resource"])
+            check_type(argname="argument db_cluster_class", value=db_cluster_class, expected_type=type_hints["db_cluster_class"])
+            check_type(argname="argument db_cluster_description", value=db_cluster_description, expected_type=type_hints["db_cluster_description"])
+            check_type(argname="argument db_node_group_count", value=db_node_group_count, expected_type=type_hints["db_node_group_count"])
+            check_type(argname="argument db_node_storage", value=db_node_storage, expected_type=type_hints["db_node_storage"])
+            check_type(argname="argument elastic_io_resource", value=elastic_io_resource, expected_type=type_hints["elastic_io_resource"])
+            check_type(argname="argument executor_count", value=executor_count, expected_type=type_hints["executor_count"])
+            check_type(argname="argument period", value=period, expected_type=type_hints["period"])
+            check_type(argname="argument period_type", value=period_type, expected_type=type_hints["period_type"])
+            check_type(argname="argument resource_group_id", value=resource_group_id, expected_type=type_hints["resource_group_id"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
+            check_type(argname="argument zone_id", value=zone_id, expected_type=type_hints["zone_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "db_cluster_category": db_cluster_category,
             "db_cluster_version": db_cluster_version,
             "mode": mode,
             "pay_type": pay_type,
             "vpc_id": vpc_id,
             "v_switch_id": v_switch_id,
@@ -527,87 +568,99 @@
 ):
     '''A ROS template type:  ``ALIYUN::ADB::Account``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosAccountProps",
+        props: typing.Union["RosAccountProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::ADB::Account``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosAccount.__init__)
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
+            type_hints = typing.get_type_hints(RosAccount._render_properties)
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
     @jsii.member(jsii_name="attrAccountName")
     def attr_account_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: AccountName: The name of the account.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAccountName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrAccountType")
     def attr_account_type(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: AccountType: The type of the account.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAccountType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDbClusterId")
     def attr_db_cluster_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: DBClusterId: The ID of the cluster.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDbClusterId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="accountName")
     def account_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: accountName: The name of the account.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "accountName"))
 
     @account_name.setter
     def account_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAccount, "account_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "accountName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="accountPassword")
     def account_password(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         ::
 
 
 
@@ -624,41 +677,50 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "accountPassword"))
 
     @account_password.setter
     def account_password(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAccount, "account_password").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "accountPassword", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dbClusterId")
     def db_cluster_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: dbClusterId: The ID of the cluster.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "dbClusterId"))
 
     @db_cluster_id.setter
     def db_cluster_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAccount, "db_cluster_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dbClusterId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAccount, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="accountDescription")
     def account_description(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -669,17 +731,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "accountDescription"))
 
     @account_description.setter
     def account_description(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAccount, "account_description").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "accountDescription", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="accountType")
     def account_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -689,14 +754,17 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "accountType"))
 
     @account_type.setter
     def account_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAccount, "account_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "accountType", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-adb.RosAccountProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -721,14 +789,21 @@
 
         :param account_name: 
         :param account_password: 
         :param db_cluster_id: 
         :param account_description: 
         :param account_type: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosAccountProps.__init__)
+            check_type(argname="argument account_name", value=account_name, expected_type=type_hints["account_name"])
+            check_type(argname="argument account_password", value=account_password, expected_type=type_hints["account_password"])
+            check_type(argname="argument db_cluster_id", value=db_cluster_id, expected_type=type_hints["db_cluster_id"])
+            check_type(argname="argument account_description", value=account_description, expected_type=type_hints["account_description"])
+            check_type(argname="argument account_type", value=account_type, expected_type=type_hints["account_type"])
         self._values: typing.Dict[str, typing.Any] = {
             "account_name": account_name,
             "account_password": account_password,
             "db_cluster_id": db_cluster_id,
         }
         if account_description is not None:
             self._values["account_description"] = account_description
@@ -820,72 +895,81 @@
 ):
     '''A ROS template type:  ``ALIYUN::ADB::DBCluster``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosDBClusterProps",
+        props: typing.Union["RosDBClusterProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::ADB::DBCluster``.
 
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
     @jsii.member(jsii_name="attrConnectionString")
     def attr_connection_string(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ConnectionString: Vpc connection string.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrConnectionString"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDbClusterId")
     def attr_db_cluster_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: DBClusterId: The ID of the cluster.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDbClusterId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrOrderId")
     def attr_order_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: OrderId: The ID of the order.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrOrderId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dbClusterCategory")
     def db_cluster_category(
         self,
     ) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
@@ -898,59 +982,71 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "dbClusterCategory"))
 
     @db_cluster_category.setter
     def db_cluster_category(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBCluster, "db_cluster_category").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dbClusterCategory", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dbClusterVersion")
     def db_cluster_version(
         self,
     ) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: dbClusterVersion: The version of the cluster. Set the value to 3.0.
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
     @jsii.member(jsii_name="mode")
     def mode(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         mode: The mode of the cluster. Valid values:
         Reserver: the reserved mode
         Flexible: the elastic mode
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "mode"))
 
     @mode.setter
     def mode(self, value: typing.Union[builtins.str, ros_cdk_core.IResolvable]) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBCluster, "mode").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "mode", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="payType")
     def pay_type(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         payType: The billing method of the cluster. Valid values:
         Postpaid: pay-as-you-go
@@ -959,64 +1055,76 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "payType"))
 
     @pay_type.setter
     def pay_type(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBCluster, "pay_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "payType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vpcId")
     def vpc_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: vpcId: The ID of the VPC.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "vpcId"))
 
     @vpc_id.setter
     def vpc_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBCluster, "vpc_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "vpcId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vSwitchId")
     def v_switch_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: vSwitchId: The ID of the vSwitch.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "vSwitchId"))
 
     @v_switch_id.setter
     def v_switch_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBCluster, "v_switch_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "vSwitchId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="computeResource")
     def compute_resource(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: computeResource: The computing resource of the cluster. This parameter is required in elastic mode.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "computeResource"))
 
     @compute_resource.setter
     def compute_resource(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBCluster, "compute_resource").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "computeResource", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dbClusterClass")
     def db_cluster_class(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -1027,34 +1135,40 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "dbClusterClass"))
 
     @db_cluster_class.setter
     def db_cluster_class(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBCluster, "db_cluster_class").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dbClusterClass", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dbClusterDescription")
     def db_cluster_description(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: dbClusterDescription: The description of the cluster.
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
     @jsii.member(jsii_name="dbNodeGroupCount")
     def db_node_group_count(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -1065,17 +1179,20 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "dbNodeGroupCount"))
 
     @db_node_group_count.setter
     def db_node_group_count(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBCluster, "db_node_group_count").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dbNodeGroupCount", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dbNodeStorage")
     def db_node_storage(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -1090,17 +1207,20 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "dbNodeStorage"))
 
     @db_node_storage.setter
     def db_node_storage(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBCluster, "db_node_storage").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dbNodeStorage", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="elasticIoResource")
     def elastic_io_resource(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -1110,34 +1230,40 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "elasticIoResource"))
 
     @elastic_io_resource.setter
     def elastic_io_resource(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBCluster, "elastic_io_resource").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "elasticIoResource", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="executorCount")
     def executor_count(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: executorCount: ExecutorCount
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "executorCount"))
 
     @executor_count.setter
     def executor_count(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBCluster, "executor_count").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "executorCount", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="period")
     def period(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -1147,17 +1273,20 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "period"))
 
     @period.setter
     def period(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBCluster, "period").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "period", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="periodType")
     def period_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -1168,63 +1297,75 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "periodType"))
 
     @period_type.setter
     def period_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBCluster, "period_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "periodType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="resourceGroupId")
     def resource_group_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: resourceGroupId: The ID of the resource group.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "resourceGroupId"))
 
     @resource_group_id.setter
     def resource_group_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBCluster, "resource_group_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "resourceGroupId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="tags")
     def tags(self) -> typing.Optional[typing.List["RosDBCluster.TagsProperty"]]:
         '''
         :Property: tags: Tags to attach to instance. Max support 20 tags to add during create instance. Each tag with two properties Key and Value, and Key is required.
         '''
         return typing.cast(typing.Optional[typing.List["RosDBCluster.TagsProperty"]], jsii.get(self, "tags"))
 
     @tags.setter
     def tags(
         self,
         value: typing.Optional[typing.List["RosDBCluster.TagsProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBCluster, "tags").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "tags", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="zoneId")
     def zone_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: zoneId: The zone ID of the cluster. You can call the DescribeRegions operation to query the most recent zone list.
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
         jsii_type="@alicloud/ros-cdk-adb.RosDBCluster.TagsProperty",
         jsii_struct_bases=[],
         name_mapping={"key": "key", "value": "value"},
     )
@@ -1235,14 +1376,18 @@
             key: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param key: 
             :param value: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosDBCluster.TagsProperty.__init__)
+                check_type(argname="argument key", value=key, expected_type=type_hints["key"])
+                check_type(argname="argument value", value=value, expected_type=type_hints["value"])
             self._values: typing.Dict[str, typing.Any] = {
                 "key": key,
             }
             if value is not None:
                 self._values["value"] = value
 
         @builtins.property
@@ -1316,15 +1461,15 @@
         db_node_group_count: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         db_node_storage: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         elastic_io_resource: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         executor_count: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         period: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         period_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         resource_group_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        tags: typing.Optional[typing.Sequence[RosDBCluster.TagsProperty]] = None,
+        tags: typing.Optional[typing.Sequence[typing.Union[RosDBCluster.TagsProperty, typing.Dict[str, typing.Any]]]] = None,
         zone_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::ADB::DBCluster``.
 
         :param db_cluster_category: 
         :param db_cluster_version: 
         :param mode: 
@@ -1340,14 +1485,34 @@
         :param executor_count: 
         :param period: 
         :param period_type: 
         :param resource_group_id: 
         :param tags: 
         :param zone_id: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosDBClusterProps.__init__)
+            check_type(argname="argument db_cluster_category", value=db_cluster_category, expected_type=type_hints["db_cluster_category"])
+            check_type(argname="argument db_cluster_version", value=db_cluster_version, expected_type=type_hints["db_cluster_version"])
+            check_type(argname="argument mode", value=mode, expected_type=type_hints["mode"])
+            check_type(argname="argument pay_type", value=pay_type, expected_type=type_hints["pay_type"])
+            check_type(argname="argument vpc_id", value=vpc_id, expected_type=type_hints["vpc_id"])
+            check_type(argname="argument v_switch_id", value=v_switch_id, expected_type=type_hints["v_switch_id"])
+            check_type(argname="argument compute_resource", value=compute_resource, expected_type=type_hints["compute_resource"])
+            check_type(argname="argument db_cluster_class", value=db_cluster_class, expected_type=type_hints["db_cluster_class"])
+            check_type(argname="argument db_cluster_description", value=db_cluster_description, expected_type=type_hints["db_cluster_description"])
+            check_type(argname="argument db_node_group_count", value=db_node_group_count, expected_type=type_hints["db_node_group_count"])
+            check_type(argname="argument db_node_storage", value=db_node_storage, expected_type=type_hints["db_node_storage"])
+            check_type(argname="argument elastic_io_resource", value=elastic_io_resource, expected_type=type_hints["elastic_io_resource"])
+            check_type(argname="argument executor_count", value=executor_count, expected_type=type_hints["executor_count"])
+            check_type(argname="argument period", value=period, expected_type=type_hints["period"])
+            check_type(argname="argument period_type", value=period_type, expected_type=type_hints["period_type"])
+            check_type(argname="argument resource_group_id", value=resource_group_id, expected_type=type_hints["resource_group_id"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
+            check_type(argname="argument zone_id", value=zone_id, expected_type=type_hints["zone_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "db_cluster_category": db_cluster_category,
             "db_cluster_version": db_cluster_version,
             "mode": mode,
             "pay_type": pay_type,
             "vpc_id": vpc_id,
             "v_switch_id": v_switch_id,
```

### Comparing `ros-cdk-adb-1.0.8/src/ros_cdk_adb.egg-info/PKG-INFO` & `ros-cdk-adb-1.0.9/src/ros_cdk_adb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-adb
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS ADB Construct Library
```

