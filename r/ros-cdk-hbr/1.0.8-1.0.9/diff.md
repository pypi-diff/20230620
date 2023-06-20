# Comparing `tmp/ros-cdk-hbr-1.0.8.tar.gz` & `tmp/ros-cdk-hbr-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-hbr-1.0.8.tar", last modified: Thu Jul 14 02:39:05 2022, max compression
+gzip compressed data, was "dist/ros-cdk-hbr-1.0.9.tar", last modified: Fri Sep 23 11:49:17 2022, max compression
```

## Comparing `ros-cdk-hbr-1.0.8.tar` & `ros-cdk-hbr-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:39:05.000000 ros-cdk-hbr-1.0.8/
--rw-r--r--   0 root         (0) root         (0)    10279 2022-07-14 02:39:05.000000 ros-cdk-hbr-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2022-07-14 02:39:05.000000 ros-cdk-hbr-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2022-07-14 02:39:05.000000 ros-cdk-hbr-1.0.8/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1240 2022-07-14 02:39:05.000000 ros-cdk-hbr-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      179 2022-07-14 02:39:05.000000 ros-cdk-hbr-1.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)      106 2022-07-14 02:39:05.000000 ros-cdk-hbr-1.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-07-14 02:39:05.000000 ros-cdk-hbr-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1794 2022-07-14 02:39:05.000000 ros-cdk-hbr-1.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:39:05.000000 ros-cdk-hbr-1.0.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:39:05.000000 ros-cdk-hbr-1.0.8/src/ros_cdk_hbr/
--rw-r--r--   0 root         (0) root         (0)   122587 2022-07-14 02:39:05.000000 ros-cdk-hbr-1.0.8/src/ros_cdk_hbr/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:39:05.000000 ros-cdk-hbr-1.0.8/src/ros_cdk_hbr/_jsii/
--rw-r--r--   0 root         (0) root         (0)      370 2022-07-14 02:39:05.000000 ros-cdk-hbr-1.0.8/src/ros_cdk_hbr/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    65784 2022-07-14 02:39:05.000000 ros-cdk-hbr-1.0.8/src/ros_cdk_hbr/_jsii/ros-cdk-hbr@1.0.8.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:39:05.000000 ros-cdk-hbr-1.0.8/src/ros_cdk_hbr/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:39:05.000000 ros-cdk-hbr-1.0.8/src/ros_cdk_hbr.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1240 2022-07-14 02:39:05.000000 ros-cdk-hbr-1.0.8/src/ros_cdk_hbr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      400 2022-07-14 02:39:05.000000 ros-cdk-hbr-1.0.8/src/ros_cdk_hbr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:39:05.000000 ros-cdk-hbr-1.0.8/src/ros_cdk_hbr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2022-07-14 02:39:05.000000 ros-cdk-hbr-1.0.8/src/ros_cdk_hbr.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2022-07-14 02:39:05.000000 ros-cdk-hbr-1.0.8/src/ros_cdk_hbr.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:49:17.000000 ros-cdk-hbr-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)    10279 2022-09-23 11:49:17.000000 ros-cdk-hbr-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-09-23 11:49:17.000000 ros-cdk-hbr-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2022-09-23 11:49:17.000000 ros-cdk-hbr-1.0.9/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1240 2022-09-23 11:49:17.000000 ros-cdk-hbr-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      179 2022-09-23 11:49:17.000000 ros-cdk-hbr-1.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      236 2022-09-23 11:49:17.000000 ros-cdk-hbr-1.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-09-23 11:49:17.000000 ros-cdk-hbr-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1823 2022-09-23 11:49:17.000000 ros-cdk-hbr-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:49:17.000000 ros-cdk-hbr-1.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:49:17.000000 ros-cdk-hbr-1.0.9/src/ros_cdk_hbr/
+-rw-r--r--   0 root         (0) root         (0)   144872 2022-09-23 11:49:17.000000 ros-cdk-hbr-1.0.9/src/ros_cdk_hbr/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:49:17.000000 ros-cdk-hbr-1.0.9/src/ros_cdk_hbr/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      404 2022-09-23 11:49:17.000000 ros-cdk-hbr-1.0.9/src/ros_cdk_hbr/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    65854 2022-09-23 11:49:17.000000 ros-cdk-hbr-1.0.9/src/ros_cdk_hbr/_jsii/ros-cdk-hbr@1.0.9.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 11:49:17.000000 ros-cdk-hbr-1.0.9/src/ros_cdk_hbr/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:49:17.000000 ros-cdk-hbr-1.0.9/src/ros_cdk_hbr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1240 2022-09-23 11:49:17.000000 ros-cdk-hbr-1.0.9/src/ros_cdk_hbr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      400 2022-09-23 11:49:17.000000 ros-cdk-hbr-1.0.9/src/ros_cdk_hbr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 11:49:17.000000 ros-cdk-hbr-1.0.9/src/ros_cdk_hbr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2022-09-23 11:49:17.000000 ros-cdk-hbr-1.0.9/src/ros_cdk_hbr.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2022-09-23 11:49:17.000000 ros-cdk-hbr-1.0.9/src/ros_cdk_hbr.egg-info/top_level.txt
```

### Comparing `ros-cdk-hbr-1.0.8/LICENSE` & `ros-cdk-hbr-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-hbr-1.0.8/PKG-INFO` & `ros-cdk-hbr-1.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-hbr
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS HBR Construct Library
```

### Comparing `ros-cdk-hbr-1.0.8/setup.py` & `ros-cdk-hbr-1.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-hbr",
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
         "ros_cdk_hbr",
         "ros_cdk_hbr._jsii"
     ],
     "package_data": {
         "ros_cdk_hbr._jsii": [
-            "ros-cdk-hbr@1.0.8.jsii.tgz"
+            "ros-cdk-hbr@1.0.9.jsii.tgz"
         ],
         "ros_cdk_hbr": [
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

### Comparing `ros-cdk-hbr-1.0.8/src/ros_cdk_hbr/__init__.py` & `ros-cdk-hbr-1.0.9/src/ros_cdk_hbr/__init__.py`

 * *Files 17% similar despite different names*

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
 
 
 class BackupClients(
     ros_cdk_core.Resource,
@@ -29,37 +31,43 @@
 ):
     '''A ROS resource type:  ``ALIYUN::HBR::BackupClients``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "BackupClientsProps",
+        props: typing.Union["BackupClientsProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::HBR::BackupClients``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(BackupClients.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrClientIds")
     def attr_client_ids(self) -> ros_cdk_core.IResolvable:
         '''Attribute ClientIds: ID list of clients installed in instances.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrClientIds"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInstanceIds")
     def attr_instance_ids(self) -> ros_cdk_core.IResolvable:
         '''Attribute InstanceIds: ID list of instances to install backup client.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInstanceIds"))
 
 
 @jsii.data_type(
@@ -68,21 +76,25 @@
     name_mapping={"instance_ids": "instanceIds", "tags": "tags"},
 )
 class BackupClientsProps:
     def __init__(
         self,
         *,
         instance_ids: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]],
-        tags: typing.Optional[typing.Sequence["RosBackupClients.TagsProperty"]] = None,
+        tags: typing.Optional[typing.Sequence[typing.Union["RosBackupClients.TagsProperty", typing.Dict[str, typing.Any]]]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::HBR::BackupClients``.
 
         :param instance_ids: Property instanceIds: ID list of instances to install backup client.
         :param tags: Property tags: Tags to attach to instance. Max support 20 tags to add during create instance. Each tag with two properties Key and Value, and Key is required.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(BackupClientsProps.__init__)
+            check_type(argname="argument instance_ids", value=instance_ids, expected_type=type_hints["instance_ids"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
         self._values: typing.Dict[str, typing.Any] = {
             "instance_ids": instance_ids,
         }
         if tags is not None:
             self._values["tags"] = tags
 
     @builtins.property
@@ -122,49 +134,55 @@
 ):
     '''A ROS resource type:  ``ALIYUN::HBR::DbAgent``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "DbAgentProps",
+        props: typing.Union["DbAgentProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::HBR::DbAgent``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(DbAgent.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInstanceIds")
     def attr_instance_ids(self) -> ros_cdk_core.IResolvable:
         '''Attribute InstanceIds: Uni backup agent instance ids.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInstanceIds"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTaskId")
     def attr_task_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute TaskId: Uni backup agent install task id.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTaskId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrUniBackupInstanceDetails")
     def attr_uni_backup_instance_details(self) -> ros_cdk_core.IResolvable:
         '''Attribute UniBackupInstanceDetails: Uni backup agent instance info details.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrUniBackupInstanceDetails"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrUniBackupInstances")
     def attr_uni_backup_instances(self) -> ros_cdk_core.IResolvable:
         '''Attribute UniBackupInstances: Uni backup agent instance info.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrUniBackupInstances"))
 
 
 @jsii.data_type(
@@ -172,20 +190,23 @@
     jsii_struct_bases=[],
     name_mapping={"instance_info": "instanceInfo"},
 )
 class DbAgentProps:
     def __init__(
         self,
         *,
-        instance_info: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosDbAgent.InstanceInfoProperty"]]],
+        instance_info: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosDbAgent.InstanceInfoProperty", typing.Dict[str, typing.Any]]]]],
     ) -> None:
         '''Properties for defining a ``ALIYUN::HBR::DbAgent``.
 
         :param instance_info: Property instanceInfo: Instance infos.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(DbAgentProps.__init__)
+            check_type(argname="argument instance_info", value=instance_info, expected_type=type_hints["instance_info"])
         self._values: typing.Dict[str, typing.Any] = {
             "instance_info": instance_info,
         }
 
     @builtins.property
     def instance_info(
         self,
@@ -214,160 +235,166 @@
 ):
     '''A ROS resource type:  ``ALIYUN::HBR::DbPlan``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "DbPlanProps",
+        props: typing.Union["DbPlanProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::HBR::DbPlan``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(DbPlan.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrContinuousPlan")
     def attr_continuous_plan(self) -> ros_cdk_core.IResolvable:
         '''Attribute ContinuousPlan: Continuous backup plan schedule.
 
         Use {   "type": "continuous" }.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrContinuousPlan"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrContinuousUuid")
     def attr_continuous_uuid(self) -> ros_cdk_core.IResolvable:
         '''Attribute ContinuousUuid: Uuid of continuous backup plan.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrContinuousUuid"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrCumulativePlan")
     def attr_cumulative_plan(self) -> ros_cdk_core.IResolvable:
         '''Attribute CumulativePlan: Cumulative plan schedule, only for mssql.
 
         More details see FullPlan.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrCumulativePlan"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrCumulativeUuid")
     def attr_cumulative_uuid(self) -> ros_cdk_core.IResolvable:
         '''Attribute CumulativeUuid: Uuid of cumulative plan.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrCumulativeUuid"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDbPlanName")
     def attr_db_plan_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute DbPlanName: Display name of the backup plan.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDbPlanName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrFullPlan")
     def attr_full_plan(self) -> ros_cdk_core.IResolvable:
         '''Attribute FullPlan: Full backup plan schedule.
 
         daily: {"type": "daily", "start": "00:00:00", "interval": 3}, weekly {"type":"weekly","start": "03:00:00","days": [1,2,3,4,5],"interval": 1}, days can be 0 - 6, 0 means Sunday, and interval can be 1 - 52.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrFullPlan"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrFullUuid")
     def attr_full_uuid(self) -> ros_cdk_core.IResolvable:
         '''Attribute FullUuid: Uuid of full backup plan.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrFullUuid"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrHostUuid")
     def attr_host_uuid(self) -> ros_cdk_core.IResolvable:
         '''Attribute HostUuid: Uuid of the host of the database instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrHostUuid"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrIncPlan")
     def attr_inc_plan(self) -> ros_cdk_core.IResolvable:
         '''Attribute IncPlan: Incremental backup plan schedule.
 
         Only for mysql and oracle. More details see FullPlan.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrIncPlan"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrIncUuid")
     def attr_inc_uuid(self) -> ros_cdk_core.IResolvable:
         '''Attribute IncUuid: Uuid of the incremental bakcup plan.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrIncUuid"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInstanceUuid")
     def attr_instance_uuid(self) -> ros_cdk_core.IResolvable:
         '''Attribute InstanceUuid: Uuid of database instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInstanceUuid"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrLogPlan")
     def attr_log_plan(self) -> ros_cdk_core.IResolvable:
         '''Attribute LogPlan: Log backup plan schedule.More details see FullPlan.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrLogPlan"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrLogUuid")
     def attr_log_uuid(self) -> ros_cdk_core.IResolvable:
         '''Attribute LogUuid: Uuid of the log backup plan.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrLogUuid"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrMaxRateLimit")
     def attr_max_rate_limit(self) -> ros_cdk_core.IResolvable:
         '''Attribute MaxRateLimit: Max rate limit for backup job,.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrMaxRateLimit"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrMaxRetrySeconds")
     def attr_max_retry_seconds(self) -> ros_cdk_core.IResolvable:
         '''Attribute MaxRetrySeconds: Max retry seconds on network failure.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrMaxRetrySeconds"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrOptions")
     def attr_options(self) -> ros_cdk_core.IResolvable:
         '''Attribute Options: Backup options in json format, different for each type of database.
 
         For Oracle, use {"channels":4,"compression":"lzop","offline_backup":false,"archivelog_reserve_hours":24,"custom_commands":""}, "channels" means numbers of concurrent theads, "archivelog_reserve_hours" means how long before the archive log will be deleted after backup job completed, other paramters should use the default vaule. For Mysql, use {"channels":4,"compression":"lzop","del_binlog":false}, "del_binlog" means whether the binlog will be deleted after backup completed, only take effect for log or continuous backup. For SQL Server, use {"channels":4,"verify":false,"compression":"lzop","backup_new_databases":false}.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrOptions"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPlanId")
     def attr_plan_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute PlanId: Id of the backup plan.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPlanId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrSourceType")
     def attr_source_type(self) -> ros_cdk_core.IResolvable:
         '''Attribute SourceType: Database type, allowed value: MYSQL, ORACLE, MSSQL.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrSourceType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTarget")
     def attr_target(self) -> ros_cdk_core.IResolvable:
         '''Attribute Target: Target vault to backup.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTarget"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVaultId")
     def attr_vault_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute VaultId: Vault ID to create backup plan, the backup data will be stored to the vault.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVaultId"))
 
 
 @jsii.data_type(
@@ -403,15 +430,15 @@
         full_plan: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         inc_plan: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         instance_uuid: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         log_plan: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         max_rate_limit: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         max_retry_seconds: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         options: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        source: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosDbPlan.SourceProperty"]] = None,
+        source: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosDbPlan.SourceProperty", typing.Dict[str, typing.Any]]]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::HBR::DbPlan``.
 
         :param db_plan_name: Property dbPlanName: Display name of the backup plan.
         :param host_uuid: Property hostUuid: Uuid of the host of the database instance.
         :param source_type: Property sourceType: Database type, allowed value: MYSQL, ORACLE, MSSQL.
         :param vault_id: Property vaultId: Vault ID to create backup plan, the backup data will be stored to the vault.
@@ -422,14 +449,30 @@
         :param instance_uuid: Property instanceUuid: Uuid of database instance.
         :param log_plan: Property logPlan: Log backup plan schedule.More details see FullPlan.
         :param max_rate_limit: Property maxRateLimit: Max rate limit for backup job,.
         :param max_retry_seconds: Property maxRetrySeconds: Max retry seconds on network failure.
         :param options: Property options: Backup options in json format, different for each type of database. For Oracle, use {"channels":4,"compression":"lzop","offline_backup":false,"archivelog_reserve_hours":24,"custom_commands":""}, "channels" means numbers of concurrent theads, "archivelog_reserve_hours" means how long before the archive log will be deleted after backup job completed, other paramters should use the default vaule. For Mysql, use {"channels":4,"compression":"lzop","del_binlog":false}, "del_binlog" means whether the binlog will be deleted after backup completed, only take effect for log or continuous backup. For SQL Server, use {"channels":4,"verify":false,"compression":"lzop","backup_new_databases":false}.
         :param source: Property source: Which database instance or database will be backup.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(DbPlanProps.__init__)
+            check_type(argname="argument db_plan_name", value=db_plan_name, expected_type=type_hints["db_plan_name"])
+            check_type(argname="argument host_uuid", value=host_uuid, expected_type=type_hints["host_uuid"])
+            check_type(argname="argument source_type", value=source_type, expected_type=type_hints["source_type"])
+            check_type(argname="argument vault_id", value=vault_id, expected_type=type_hints["vault_id"])
+            check_type(argname="argument continuous_plan", value=continuous_plan, expected_type=type_hints["continuous_plan"])
+            check_type(argname="argument cumulative_plan", value=cumulative_plan, expected_type=type_hints["cumulative_plan"])
+            check_type(argname="argument full_plan", value=full_plan, expected_type=type_hints["full_plan"])
+            check_type(argname="argument inc_plan", value=inc_plan, expected_type=type_hints["inc_plan"])
+            check_type(argname="argument instance_uuid", value=instance_uuid, expected_type=type_hints["instance_uuid"])
+            check_type(argname="argument log_plan", value=log_plan, expected_type=type_hints["log_plan"])
+            check_type(argname="argument max_rate_limit", value=max_rate_limit, expected_type=type_hints["max_rate_limit"])
+            check_type(argname="argument max_retry_seconds", value=max_retry_seconds, expected_type=type_hints["max_retry_seconds"])
+            check_type(argname="argument options", value=options, expected_type=type_hints["options"])
+            check_type(argname="argument source", value=source, expected_type=type_hints["source"])
         self._values: typing.Dict[str, typing.Any] = {
             "db_plan_name": db_plan_name,
             "host_uuid": host_uuid,
             "source_type": source_type,
             "vault_id": vault_id,
         }
         if continuous_plan is not None:
@@ -595,58 +638,64 @@
 ):
     '''A ROS resource type:  ``ALIYUN::HBR::DbVault``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "DbVaultProps",
+        props: typing.Union["DbVaultProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::HBR::DbVault``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(DbVault.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDescription")
     def attr_description(self) -> ros_cdk_core.IResolvable:
         '''Attribute Description: Description of the vault.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDescription"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrRetentionDays")
     def attr_retention_days(self) -> ros_cdk_core.IResolvable:
         '''Attribute RetentionDays: Data retention days of the vault.
 
         Data will be deleted when it's older than this time.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrRetentionDays"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVaultId")
     def attr_vault_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute VaultId: Vault ID.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVaultId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVaultName")
     def attr_vault_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute VaultName: Display name of the vault.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVaultName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVaultRegionId")
     def attr_vault_region_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute VaultRegionId: The region ID to create the vault.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVaultRegionId"))
 
 
 @jsii.data_type(
@@ -664,24 +713,31 @@
     def __init__(
         self,
         *,
         retention_days: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
         vault_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         vault_region_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         description: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        tags: typing.Optional[typing.Sequence["RosDbVault.TagsProperty"]] = None,
+        tags: typing.Optional[typing.Sequence[typing.Union["RosDbVault.TagsProperty", typing.Dict[str, typing.Any]]]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::HBR::DbVault``.
 
         :param retention_days: Property retentionDays: Data retention days of the vault. Data will be deleted when it's older than this time.
         :param vault_name: Property vaultName: Display name of the vault.
         :param vault_region_id: Property vaultRegionId: The region ID to create the vault.
         :param description: Property description: Description of the vault.
         :param tags: Property tags: Tags to attach to instance. Max support 20 tags to add during create instance. Each tag with two properties Key and Value, and Key is required.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(DbVaultProps.__init__)
+            check_type(argname="argument retention_days", value=retention_days, expected_type=type_hints["retention_days"])
+            check_type(argname="argument vault_name", value=vault_name, expected_type=type_hints["vault_name"])
+            check_type(argname="argument vault_region_id", value=vault_region_id, expected_type=type_hints["vault_region_id"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
         self._values: typing.Dict[str, typing.Any] = {
             "retention_days": retention_days,
             "vault_name": vault_name,
             "vault_region_id": vault_region_id,
         }
         if description is not None:
             self._values["description"] = description
@@ -748,55 +804,61 @@
 ):
     '''A ROS resource type:  ``ALIYUN::HBR::RestoreJob``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RestoreJobProps",
+        props: typing.Union["RestoreJobProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::HBR::RestoreJob``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RestoreJob.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrErrorMessage")
     def attr_error_message(self) -> ros_cdk_core.IResolvable:
         '''Attribute ErrorMessage: Error message of restore job.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrErrorMessage"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrRestoreId")
     def attr_restore_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute RestoreId: Restore job ID.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrRestoreId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrRestoreType")
     def attr_restore_type(self) -> ros_cdk_core.IResolvable:
         '''Attribute RestoreType: Restore type.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrRestoreType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrSourceType")
     def attr_source_type(self) -> ros_cdk_core.IResolvable:
         '''Attribute SourceType: Source type.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrSourceType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrStatus")
     def attr_status(self) -> ros_cdk_core.IResolvable:
         '''Attribute Status: Restore job status.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrStatus"))
 
 
 @jsii.data_type(
@@ -836,14 +898,25 @@
         :param source_instance_id: Property sourceInstanceId: Source instance ID. It should be provided when SourceType=ECS_FILE.
         :param source_type: Property sourceType: Source type.
         :param target_client_id: Property targetClientId: Target client ID. It should be provided when RestoreType=FILE.
         :param target_instance_id: Property targetInstanceId: Target instance ID. It should be provided when RestoreType=ECS_FILE.
         :param target_path: Property targetPath: Target path. For instance, "/".
         :param vault_id: Property vaultId: Vault ID.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RestoreJobProps.__init__)
+            check_type(argname="argument restore_type", value=restore_type, expected_type=type_hints["restore_type"])
+            check_type(argname="argument snapshot_id", value=snapshot_id, expected_type=type_hints["snapshot_id"])
+            check_type(argname="argument source_client_id", value=source_client_id, expected_type=type_hints["source_client_id"])
+            check_type(argname="argument source_instance_id", value=source_instance_id, expected_type=type_hints["source_instance_id"])
+            check_type(argname="argument source_type", value=source_type, expected_type=type_hints["source_type"])
+            check_type(argname="argument target_client_id", value=target_client_id, expected_type=type_hints["target_client_id"])
+            check_type(argname="argument target_instance_id", value=target_instance_id, expected_type=type_hints["target_instance_id"])
+            check_type(argname="argument target_path", value=target_path, expected_type=type_hints["target_path"])
+            check_type(argname="argument vault_id", value=vault_id, expected_type=type_hints["vault_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "restore_type": restore_type,
             "snapshot_id": snapshot_id,
             "source_client_id": source_client_id,
             "source_instance_id": source_instance_id,
             "source_type": source_type,
             "target_client_id": target_client_id,
@@ -953,102 +1026,120 @@
 ):
     '''A ROS template type:  ``ALIYUN::HBR::BackupClients``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosBackupClientsProps",
+        props: typing.Union["RosBackupClientsProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::HBR::BackupClients``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosBackupClients.__init__)
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
+            type_hints = typing.get_type_hints(RosBackupClients._render_properties)
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
     @jsii.member(jsii_name="attrClientIds")
     def attr_client_ids(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ClientIds: ID list of clients installed in instances
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrClientIds"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInstanceIds")
     def attr_instance_ids(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: InstanceIds: ID list of instances to install backup client
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInstanceIds"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosBackupClients, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="instanceIds")
     def instance_ids(
         self,
     ) -> typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]:
         '''
         :Property: instanceIds: ID list of instances to install backup client
         '''
         return typing.cast(typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]], jsii.get(self, "instanceIds"))
 
     @instance_ids.setter
     def instance_ids(
         self,
         value: typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosBackupClients, "instance_ids").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "instanceIds", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="tags")
     def tags(self) -> typing.Optional[typing.List["RosBackupClients.TagsProperty"]]:
         '''
         :Property: tags: Tags to attach to instance. Max support 20 tags to add during create instance. Each tag with two properties Key and Value, and Key is required.
         '''
         return typing.cast(typing.Optional[typing.List["RosBackupClients.TagsProperty"]], jsii.get(self, "tags"))
 
     @tags.setter
     def tags(
         self,
         value: typing.Optional[typing.List["RosBackupClients.TagsProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosBackupClients, "tags").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "tags", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-hbr.RosBackupClients.TagsProperty",
         jsii_struct_bases=[],
         name_mapping={"key": "key", "value": "value"},
     )
@@ -1059,14 +1150,18 @@
             key: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param key: 
             :param value: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosBackupClients.TagsProperty.__init__)
+                check_type(argname="argument key", value=key, expected_type=type_hints["key"])
+                check_type(argname="argument value", value=value, expected_type=type_hints["value"])
             self._values: typing.Dict[str, typing.Any] = {
                 "key": key,
             }
             if value is not None:
                 self._values["value"] = value
 
         @builtins.property
@@ -1106,21 +1201,25 @@
     name_mapping={"instance_ids": "instanceIds", "tags": "tags"},
 )
 class RosBackupClientsProps:
     def __init__(
         self,
         *,
         instance_ids: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]],
-        tags: typing.Optional[typing.Sequence[RosBackupClients.TagsProperty]] = None,
+        tags: typing.Optional[typing.Sequence[typing.Union[RosBackupClients.TagsProperty, typing.Dict[str, typing.Any]]]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::HBR::BackupClients``.
 
         :param instance_ids: 
         :param tags: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosBackupClientsProps.__init__)
+            check_type(argname="argument instance_ids", value=instance_ids, expected_type=type_hints["instance_ids"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
         self._values: typing.Dict[str, typing.Any] = {
             "instance_ids": instance_ids,
         }
         if tags is not None:
             self._values["tags"] = tags
 
     @builtins.property
@@ -1161,103 +1260,118 @@
 ):
     '''A ROS template type:  ``ALIYUN::HBR::DbAgent``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosDbAgentProps",
+        props: typing.Union["RosDbAgentProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::HBR::DbAgent``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosDbAgent.__init__)
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
+            type_hints = typing.get_type_hints(RosDbAgent._render_properties)
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
     @jsii.member(jsii_name="attrInstanceIds")
     def attr_instance_ids(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: InstanceIds: Uni backup agent instance ids
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInstanceIds"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTaskId")
     def attr_task_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: TaskId: Uni backup agent install task id.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTaskId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrUniBackupInstanceDetails")
     def attr_uni_backup_instance_details(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: UniBackupInstanceDetails: Uni backup agent instance info details
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrUniBackupInstanceDetails"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrUniBackupInstances")
     def attr_uni_backup_instances(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: UniBackupInstances: Uni backup agent instance info
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrUniBackupInstances"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDbAgent, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="instanceInfo")
     def instance_info(
         self,
     ) -> typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosDbAgent.InstanceInfoProperty"]]]:
         '''
         :Property: instanceInfo: Instance infos
         '''
         return typing.cast(typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosDbAgent.InstanceInfoProperty"]]], jsii.get(self, "instanceInfo"))
 
     @instance_info.setter
     def instance_info(
         self,
         value: typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosDbAgent.InstanceInfoProperty"]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDbAgent, "instance_info").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "instanceInfo", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-hbr.RosDbAgent.InstanceInfoProperty",
         jsii_struct_bases=[],
         name_mapping={
             "instance_id": "instanceId",
@@ -1280,14 +1394,21 @@
             '''
             :param instance_id: 
             :param source_type: 
             :param authentication_type: 
             :param password: 
             :param user_name: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosDbAgent.InstanceInfoProperty.__init__)
+                check_type(argname="argument instance_id", value=instance_id, expected_type=type_hints["instance_id"])
+                check_type(argname="argument source_type", value=source_type, expected_type=type_hints["source_type"])
+                check_type(argname="argument authentication_type", value=authentication_type, expected_type=type_hints["authentication_type"])
+                check_type(argname="argument password", value=password, expected_type=type_hints["password"])
+                check_type(argname="argument user_name", value=user_name, expected_type=type_hints["user_name"])
             self._values: typing.Dict[str, typing.Any] = {
                 "instance_id": instance_id,
                 "source_type": source_type,
             }
             if authentication_type is not None:
                 self._values["authentication_type"] = authentication_type
             if password is not None:
@@ -1360,20 +1481,23 @@
     jsii_struct_bases=[],
     name_mapping={"instance_info": "instanceInfo"},
 )
 class RosDbAgentProps:
     def __init__(
         self,
         *,
-        instance_info: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosDbAgent.InstanceInfoProperty]]],
+        instance_info: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosDbAgent.InstanceInfoProperty, typing.Dict[str, typing.Any]]]]],
     ) -> None:
         '''Properties for defining a ``ALIYUN::HBR::DbAgent``.
 
         :param instance_info: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosDbAgentProps.__init__)
+            check_type(argname="argument instance_info", value=instance_info, expected_type=type_hints["instance_info"])
         self._values: typing.Dict[str, typing.Any] = {
             "instance_info": instance_info,
         }
 
     @builtins.property
     def instance_info(
         self,
@@ -1404,444 +1528,498 @@
 ):
     '''A ROS template type:  ``ALIYUN::HBR::DbPlan``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosDbPlanProps",
+        props: typing.Union["RosDbPlanProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::HBR::DbPlan``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosDbPlan.__init__)
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
+            type_hints = typing.get_type_hints(RosDbPlan._render_properties)
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
     @jsii.member(jsii_name="attrContinuousPlan")
     def attr_continuous_plan(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ContinuousPlan: Continuous backup plan schedule. Use {   "type": "continuous" }.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrContinuousPlan"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrContinuousUuid")
     def attr_continuous_uuid(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ContinuousUuid: Uuid of continuous backup plan.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrContinuousUuid"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrCumulativePlan")
     def attr_cumulative_plan(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: CumulativePlan: Cumulative plan schedule, only for mssql. More details see FullPlan.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrCumulativePlan"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrCumulativeUuid")
     def attr_cumulative_uuid(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: CumulativeUuid: Uuid of cumulative plan.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrCumulativeUuid"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDbPlanName")
     def attr_db_plan_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: DbPlanName: Display name of the backup plan.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDbPlanName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrFullPlan")
     def attr_full_plan(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: FullPlan: Full backup plan schedule. daily: {"type": "daily", "start": "00:00:00", "interval": 3}, weekly {"type":"weekly","start": "03:00:00","days": [1,2,3,4,5],"interval": 1}, days can be 0 - 6, 0 means Sunday, and interval can be 1 - 52.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrFullPlan"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrFullUuid")
     def attr_full_uuid(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: FullUuid: Uuid of full backup plan.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrFullUuid"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrHostUuid")
     def attr_host_uuid(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: HostUuid: Uuid of the host of the database instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrHostUuid"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrIncPlan")
     def attr_inc_plan(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: IncPlan: Incremental backup plan schedule. Only for mysql and oracle. More details see FullPlan.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrIncPlan"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrIncUuid")
     def attr_inc_uuid(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: IncUuid: Uuid of the incremental bakcup plan.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrIncUuid"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInstanceUuid")
     def attr_instance_uuid(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: InstanceUuid: Uuid of database instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInstanceUuid"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrLogPlan")
     def attr_log_plan(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: LogPlan: Log backup plan schedule.More details see FullPlan.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrLogPlan"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrLogUuid")
     def attr_log_uuid(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: LogUuid: Uuid of the log backup plan.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrLogUuid"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrMaxRateLimit")
     def attr_max_rate_limit(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: MaxRateLimit: Max rate limit for backup job,
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrMaxRateLimit"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrMaxRetrySeconds")
     def attr_max_retry_seconds(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: MaxRetrySeconds: Max retry seconds on network failure.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrMaxRetrySeconds"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrOptions")
     def attr_options(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Options: Backup options in json format, different for each type of database. For Oracle, use {"channels":4,"compression":"lzop","offline_backup":false,"archivelog_reserve_hours":24,"custom_commands":""}, "channels" means numbers of concurrent theads, "archivelog_reserve_hours" means how long before the archive log will be deleted after backup job completed, other paramters should use the default vaule. For Mysql, use {"channels":4,"compression":"lzop","del_binlog":false}, "del_binlog" means whether the binlog will be deleted after backup completed, only take effect for log or continuous backup. For SQL Server, use {"channels":4,"verify":false,"compression":"lzop","backup_new_databases":false}.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrOptions"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPlanId")
     def attr_plan_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: PlanId: Id of the backup plan.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPlanId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrSourceType")
     def attr_source_type(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: SourceType: Database type, allowed value: MYSQL, ORACLE, MSSQL
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrSourceType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTarget")
     def attr_target(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Target: Target vault to backup.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTarget"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVaultId")
     def attr_vault_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: VaultId: Vault ID to create backup plan, the backup data will be stored to the vault.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVaultId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dbPlanName")
     def db_plan_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: dbPlanName: Display name of the backup plan.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "dbPlanName"))
 
     @db_plan_name.setter
     def db_plan_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDbPlan, "db_plan_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dbPlanName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDbPlan, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="hostUuid")
     def host_uuid(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: hostUuid: Uuid of the host of the database instance.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "hostUuid"))
 
     @host_uuid.setter
     def host_uuid(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDbPlan, "host_uuid").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "hostUuid", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="sourceType")
     def source_type(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: sourceType: Database type, allowed value: MYSQL, ORACLE, MSSQL
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "sourceType"))
 
     @source_type.setter
     def source_type(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDbPlan, "source_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "sourceType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vaultId")
     def vault_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: vaultId: Vault ID to create backup plan, the backup data will be stored to the vault.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "vaultId"))
 
     @vault_id.setter
     def vault_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDbPlan, "vault_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "vaultId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="continuousPlan")
     def continuous_plan(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: continuousPlan: Continuous backup plan schedule. Use {   "type": "continuous" }.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "continuousPlan"))
 
     @continuous_plan.setter
     def continuous_plan(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDbPlan, "continuous_plan").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "continuousPlan", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="cumulativePlan")
     def cumulative_plan(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: cumulativePlan: Cumulative plan schedule, only for mssql. More details see FullPlan.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "cumulativePlan"))
 
     @cumulative_plan.setter
     def cumulative_plan(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDbPlan, "cumulative_plan").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "cumulativePlan", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="fullPlan")
     def full_plan(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: fullPlan: Full backup plan schedule. daily: {"type": "daily", "start": "00:00:00", "interval": 3}, weekly {"type":"weekly","start": "03:00:00","days": [1,2,3,4,5],"interval": 1}, days can be 0 - 6, 0 means Sunday, and interval can be 1 - 52.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "fullPlan"))
 
     @full_plan.setter
     def full_plan(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDbPlan, "full_plan").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "fullPlan", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="incPlan")
     def inc_plan(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: incPlan: Incremental backup plan schedule. Only for mysql and oracle. More details see FullPlan.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "incPlan"))
 
     @inc_plan.setter
     def inc_plan(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDbPlan, "inc_plan").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "incPlan", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="instanceUuid")
     def instance_uuid(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: instanceUuid: Uuid of database instance.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "instanceUuid"))
 
     @instance_uuid.setter
     def instance_uuid(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDbPlan, "instance_uuid").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "instanceUuid", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="logPlan")
     def log_plan(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: logPlan: Log backup plan schedule.More details see FullPlan.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "logPlan"))
 
     @log_plan.setter
     def log_plan(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDbPlan, "log_plan").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "logPlan", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="maxRateLimit")
     def max_rate_limit(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: maxRateLimit: Max rate limit for backup job,
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "maxRateLimit"))
 
     @max_rate_limit.setter
     def max_rate_limit(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDbPlan, "max_rate_limit").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "maxRateLimit", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="maxRetrySeconds")
     def max_retry_seconds(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: maxRetrySeconds: Max retry seconds on network failure.
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "maxRetrySeconds"))
 
     @max_retry_seconds.setter
     def max_retry_seconds(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDbPlan, "max_retry_seconds").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "maxRetrySeconds", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="options")
     def options(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: options: Backup options in json format, different for each type of database. For Oracle, use {"channels":4,"compression":"lzop","offline_backup":false,"archivelog_reserve_hours":24,"custom_commands":""}, "channels" means numbers of concurrent theads, "archivelog_reserve_hours" means how long before the archive log will be deleted after backup job completed, other paramters should use the default vaule. For Mysql, use {"channels":4,"compression":"lzop","del_binlog":false}, "del_binlog" means whether the binlog will be deleted after backup completed, only take effect for log or continuous backup. For SQL Server, use {"channels":4,"verify":false,"compression":"lzop","backup_new_databases":false}.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "options"))
 
     @options.setter
     def options(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDbPlan, "options").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "options", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="source")
     def source(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosDbPlan.SourceProperty"]]:
         '''
         :Property: source: Which database instance or database will be backup.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosDbPlan.SourceProperty"]], jsii.get(self, "source"))
 
     @source.setter
     def source(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosDbPlan.SourceProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDbPlan, "source").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "source", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-hbr.RosDbPlan.SourceProperty",
         jsii_struct_bases=[],
         name_mapping={"entries": "entries"},
     )
@@ -1850,14 +2028,17 @@
             self,
             *,
             entries: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]] = None,
         ) -> None:
             '''
             :param entries: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosDbPlan.SourceProperty.__init__)
+                check_type(argname="argument entries", value=entries, expected_type=type_hints["entries"])
             self._values: typing.Dict[str, typing.Any] = {}
             if entries is not None:
                 self._values["entries"] = entries
 
         @builtins.property
         def entries(
             self,
@@ -1913,15 +2094,15 @@
         full_plan: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         inc_plan: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         instance_uuid: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         log_plan: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         max_rate_limit: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         max_retry_seconds: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         options: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        source: typing.Optional[typing.Union[ros_cdk_core.IResolvable, RosDbPlan.SourceProperty]] = None,
+        source: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosDbPlan.SourceProperty, typing.Dict[str, typing.Any]]]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::HBR::DbPlan``.
 
         :param db_plan_name: 
         :param host_uuid: 
         :param source_type: 
         :param vault_id: 
@@ -1932,14 +2113,30 @@
         :param instance_uuid: 
         :param log_plan: 
         :param max_rate_limit: 
         :param max_retry_seconds: 
         :param options: 
         :param source: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosDbPlanProps.__init__)
+            check_type(argname="argument db_plan_name", value=db_plan_name, expected_type=type_hints["db_plan_name"])
+            check_type(argname="argument host_uuid", value=host_uuid, expected_type=type_hints["host_uuid"])
+            check_type(argname="argument source_type", value=source_type, expected_type=type_hints["source_type"])
+            check_type(argname="argument vault_id", value=vault_id, expected_type=type_hints["vault_id"])
+            check_type(argname="argument continuous_plan", value=continuous_plan, expected_type=type_hints["continuous_plan"])
+            check_type(argname="argument cumulative_plan", value=cumulative_plan, expected_type=type_hints["cumulative_plan"])
+            check_type(argname="argument full_plan", value=full_plan, expected_type=type_hints["full_plan"])
+            check_type(argname="argument inc_plan", value=inc_plan, expected_type=type_hints["inc_plan"])
+            check_type(argname="argument instance_uuid", value=instance_uuid, expected_type=type_hints["instance_uuid"])
+            check_type(argname="argument log_plan", value=log_plan, expected_type=type_hints["log_plan"])
+            check_type(argname="argument max_rate_limit", value=max_rate_limit, expected_type=type_hints["max_rate_limit"])
+            check_type(argname="argument max_retry_seconds", value=max_retry_seconds, expected_type=type_hints["max_retry_seconds"])
+            check_type(argname="argument options", value=options, expected_type=type_hints["options"])
+            check_type(argname="argument source", value=source, expected_type=type_hints["source"])
         self._values: typing.Dict[str, typing.Any] = {
             "db_plan_name": db_plan_name,
             "host_uuid": host_uuid,
             "source_type": source_type,
             "vault_id": vault_id,
         }
         if continuous_plan is not None:
@@ -2118,171 +2315,198 @@
 ):
     '''A ROS template type:  ``ALIYUN::HBR::DbVault``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosDbVaultProps",
+        props: typing.Union["RosDbVaultProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::HBR::DbVault``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosDbVault.__init__)
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
+            type_hints = typing.get_type_hints(RosDbVault._render_properties)
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
     @jsii.member(jsii_name="attrDescription")
     def attr_description(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Description: Description of the vault.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDescription"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrRetentionDays")
     def attr_retention_days(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: RetentionDays: Data retention days of the vault. Data will be deleted when it's older than this time.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrRetentionDays"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVaultId")
     def attr_vault_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: VaultId: Vault ID.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVaultId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVaultName")
     def attr_vault_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: VaultName: Display name of the vault.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVaultName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVaultRegionId")
     def attr_vault_region_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: VaultRegionId: The region ID to create the vault.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVaultRegionId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDbVault, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="retentionDays")
     def retention_days(self) -> typing.Union[jsii.Number, ros_cdk_core.IResolvable]:
         '''
         :Property: retentionDays: Data retention days of the vault. Data will be deleted when it's older than this time.
         '''
         return typing.cast(typing.Union[jsii.Number, ros_cdk_core.IResolvable], jsii.get(self, "retentionDays"))
 
     @retention_days.setter
     def retention_days(
         self,
         value: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDbVault, "retention_days").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "retentionDays", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vaultName")
     def vault_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: vaultName: Display name of the vault.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "vaultName"))
 
     @vault_name.setter
     def vault_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDbVault, "vault_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "vaultName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vaultRegionId")
     def vault_region_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: vaultRegionId: The region ID to create the vault.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "vaultRegionId"))
 
     @vault_region_id.setter
     def vault_region_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDbVault, "vault_region_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "vaultRegionId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="description")
     def description(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: description: Description of the vault.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "description"))
 
     @description.setter
     def description(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDbVault, "description").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "description", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="tags")
     def tags(self) -> typing.Optional[typing.List["RosDbVault.TagsProperty"]]:
         '''
         :Property: tags: Tags to attach to instance. Max support 20 tags to add during create instance. Each tag with two properties Key and Value, and Key is required.
         '''
         return typing.cast(typing.Optional[typing.List["RosDbVault.TagsProperty"]], jsii.get(self, "tags"))
 
     @tags.setter
     def tags(
         self,
         value: typing.Optional[typing.List["RosDbVault.TagsProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDbVault, "tags").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "tags", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-hbr.RosDbVault.TagsProperty",
         jsii_struct_bases=[],
         name_mapping={"key": "key", "value": "value"},
     )
@@ -2293,14 +2517,18 @@
             key: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param key: 
             :param value: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosDbVault.TagsProperty.__init__)
+                check_type(argname="argument key", value=key, expected_type=type_hints["key"])
+                check_type(argname="argument value", value=value, expected_type=type_hints["value"])
             self._values: typing.Dict[str, typing.Any] = {
                 "key": key,
             }
             if value is not None:
                 self._values["value"] = value
 
         @builtins.property
@@ -2349,24 +2577,31 @@
     def __init__(
         self,
         *,
         retention_days: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
         vault_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         vault_region_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         description: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        tags: typing.Optional[typing.Sequence[RosDbVault.TagsProperty]] = None,
+        tags: typing.Optional[typing.Sequence[typing.Union[RosDbVault.TagsProperty, typing.Dict[str, typing.Any]]]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::HBR::DbVault``.
 
         :param retention_days: 
         :param vault_name: 
         :param vault_region_id: 
         :param description: 
         :param tags: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosDbVaultProps.__init__)
+            check_type(argname="argument retention_days", value=retention_days, expected_type=type_hints["retention_days"])
+            check_type(argname="argument vault_name", value=vault_name, expected_type=type_hints["vault_name"])
+            check_type(argname="argument vault_region_id", value=vault_region_id, expected_type=type_hints["vault_region_id"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
         self._values: typing.Dict[str, typing.Any] = {
             "retention_days": retention_days,
             "vault_name": vault_name,
             "vault_region_id": vault_region_id,
         }
         if description is not None:
             self._values["description"] = description
@@ -2437,233 +2672,272 @@
 ):
     '''A ROS template type:  ``ALIYUN::HBR::RestoreJob``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosRestoreJobProps",
+        props: typing.Union["RosRestoreJobProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::HBR::RestoreJob``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosRestoreJob.__init__)
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
+            type_hints = typing.get_type_hints(RosRestoreJob._render_properties)
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
     @jsii.member(jsii_name="attrErrorMessage")
     def attr_error_message(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ErrorMessage: Error message of restore job
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrErrorMessage"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrRestoreId")
     def attr_restore_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: RestoreId: Restore job ID
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrRestoreId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrRestoreType")
     def attr_restore_type(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: RestoreType: Restore type
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrRestoreType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrSourceType")
     def attr_source_type(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: SourceType: Source type
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrSourceType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrStatus")
     def attr_status(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Status: Restore job status
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrStatus"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosRestoreJob, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="restoreType")
     def restore_type(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: restoreType: Restore type
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "restoreType"))
 
     @restore_type.setter
     def restore_type(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosRestoreJob, "restore_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "restoreType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="snapshotId")
     def snapshot_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: snapshotId: Snapshot ID
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "snapshotId"))
 
     @snapshot_id.setter
     def snapshot_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosRestoreJob, "snapshot_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "snapshotId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="sourceClientId")
     def source_client_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: sourceClientId: Source client ID. It should be provided when SourceType=FILE.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "sourceClientId"))
 
     @source_client_id.setter
     def source_client_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosRestoreJob, "source_client_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "sourceClientId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="sourceInstanceId")
     def source_instance_id(
         self,
     ) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: sourceInstanceId: Source instance ID. It should be provided when SourceType=ECS_FILE.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "sourceInstanceId"))
 
     @source_instance_id.setter
     def source_instance_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosRestoreJob, "source_instance_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "sourceInstanceId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="sourceType")
     def source_type(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: sourceType: Source type
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "sourceType"))
 
     @source_type.setter
     def source_type(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosRestoreJob, "source_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "sourceType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="targetClientId")
     def target_client_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: targetClientId: Target client ID. It should be provided when RestoreType=FILE.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "targetClientId"))
 
     @target_client_id.setter
     def target_client_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosRestoreJob, "target_client_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "targetClientId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="targetInstanceId")
     def target_instance_id(
         self,
     ) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: targetInstanceId: Target instance ID. It should be provided when RestoreType=ECS_FILE.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "targetInstanceId"))
 
     @target_instance_id.setter
     def target_instance_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosRestoreJob, "target_instance_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "targetInstanceId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="targetPath")
     def target_path(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: targetPath: Target path. For instance, "/".
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "targetPath"))
 
     @target_path.setter
     def target_path(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosRestoreJob, "target_path").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "targetPath", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vaultId")
     def vault_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: vaultId: Vault ID
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "vaultId"))
 
     @vault_id.setter
     def vault_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosRestoreJob, "vault_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "vaultId", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-hbr.RosRestoreJobProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -2700,14 +2974,25 @@
         :param source_instance_id: 
         :param source_type: 
         :param target_client_id: 
         :param target_instance_id: 
         :param target_path: 
         :param vault_id: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosRestoreJobProps.__init__)
+            check_type(argname="argument restore_type", value=restore_type, expected_type=type_hints["restore_type"])
+            check_type(argname="argument snapshot_id", value=snapshot_id, expected_type=type_hints["snapshot_id"])
+            check_type(argname="argument source_client_id", value=source_client_id, expected_type=type_hints["source_client_id"])
+            check_type(argname="argument source_instance_id", value=source_instance_id, expected_type=type_hints["source_instance_id"])
+            check_type(argname="argument source_type", value=source_type, expected_type=type_hints["source_type"])
+            check_type(argname="argument target_client_id", value=target_client_id, expected_type=type_hints["target_client_id"])
+            check_type(argname="argument target_instance_id", value=target_instance_id, expected_type=type_hints["target_instance_id"])
+            check_type(argname="argument target_path", value=target_path, expected_type=type_hints["target_path"])
+            check_type(argname="argument vault_id", value=vault_id, expected_type=type_hints["vault_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "restore_type": restore_type,
             "snapshot_id": snapshot_id,
             "source_client_id": source_client_id,
             "source_instance_id": source_instance_id,
             "source_type": source_type,
             "target_client_id": target_client_id,
```

### Comparing `ros-cdk-hbr-1.0.8/src/ros_cdk_hbr.egg-info/PKG-INFO` & `ros-cdk-hbr-1.0.9/src/ros_cdk_hbr.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-hbr
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS HBR Construct Library
```

