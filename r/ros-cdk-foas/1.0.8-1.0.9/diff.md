# Comparing `tmp/ros-cdk-foas-1.0.8.tar.gz` & `tmp/ros-cdk-foas-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-foas-1.0.8.tar", last modified: Thu Jul 14 02:35:20 2022, max compression
+gzip compressed data, was "dist/ros-cdk-foas-1.0.9.tar", last modified: Fri Sep 23 11:35:48 2022, max compression
```

## Comparing `ros-cdk-foas-1.0.8.tar` & `ros-cdk-foas-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:35:20.000000 ros-cdk-foas-1.0.8/
--rw-r--r--   0 root         (0) root         (0)    10279 2022-07-14 02:35:20.000000 ros-cdk-foas-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2022-07-14 02:35:20.000000 ros-cdk-foas-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2022-07-14 02:35:20.000000 ros-cdk-foas-1.0.8/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1244 2022-07-14 02:35:20.000000 ros-cdk-foas-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      182 2022-07-14 02:35:20.000000 ros-cdk-foas-1.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)      106 2022-07-14 02:35:20.000000 ros-cdk-foas-1.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-07-14 02:35:20.000000 ros-cdk-foas-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1800 2022-07-14 02:35:20.000000 ros-cdk-foas-1.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:35:20.000000 ros-cdk-foas-1.0.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:35:20.000000 ros-cdk-foas-1.0.8/src/ros_cdk_foas/
--rw-r--r--   0 root         (0) root         (0)    43407 2022-07-14 02:35:20.000000 ros-cdk-foas-1.0.8/src/ros_cdk_foas/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:35:20.000000 ros-cdk-foas-1.0.8/src/ros_cdk_foas/_jsii/
--rw-r--r--   0 root         (0) root         (0)      372 2022-07-14 02:35:20.000000 ros-cdk-foas-1.0.8/src/ros_cdk_foas/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    41739 2022-07-14 02:35:20.000000 ros-cdk-foas-1.0.8/src/ros_cdk_foas/_jsii/ros-cdk-foas@1.0.8.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:35:20.000000 ros-cdk-foas-1.0.8/src/ros_cdk_foas/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:35:20.000000 ros-cdk-foas-1.0.8/src/ros_cdk_foas.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1244 2022-07-14 02:35:20.000000 ros-cdk-foas-1.0.8/src/ros_cdk_foas.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      410 2022-07-14 02:35:20.000000 ros-cdk-foas-1.0.8/src/ros_cdk_foas.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:35:20.000000 ros-cdk-foas-1.0.8/src/ros_cdk_foas.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2022-07-14 02:35:20.000000 ros-cdk-foas-1.0.8/src/ros_cdk_foas.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2022-07-14 02:35:20.000000 ros-cdk-foas-1.0.8/src/ros_cdk_foas.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:35:48.000000 ros-cdk-foas-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)    10279 2022-09-23 11:35:48.000000 ros-cdk-foas-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-09-23 11:35:48.000000 ros-cdk-foas-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2022-09-23 11:35:48.000000 ros-cdk-foas-1.0.9/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1244 2022-09-23 11:35:48.000000 ros-cdk-foas-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      182 2022-09-23 11:35:48.000000 ros-cdk-foas-1.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      236 2022-09-23 11:35:48.000000 ros-cdk-foas-1.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-09-23 11:35:48.000000 ros-cdk-foas-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1829 2022-09-23 11:35:48.000000 ros-cdk-foas-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:35:48.000000 ros-cdk-foas-1.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:35:48.000000 ros-cdk-foas-1.0.9/src/ros_cdk_foas/
+-rw-r--r--   0 root         (0) root         (0)    52324 2022-09-23 11:35:48.000000 ros-cdk-foas-1.0.9/src/ros_cdk_foas/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:35:48.000000 ros-cdk-foas-1.0.9/src/ros_cdk_foas/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      406 2022-09-23 11:35:48.000000 ros-cdk-foas-1.0.9/src/ros_cdk_foas/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    41811 2022-09-23 11:35:48.000000 ros-cdk-foas-1.0.9/src/ros_cdk_foas/_jsii/ros-cdk-foas@1.0.9.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 11:35:48.000000 ros-cdk-foas-1.0.9/src/ros_cdk_foas/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:35:48.000000 ros-cdk-foas-1.0.9/src/ros_cdk_foas.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1244 2022-09-23 11:35:48.000000 ros-cdk-foas-1.0.9/src/ros_cdk_foas.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      410 2022-09-23 11:35:48.000000 ros-cdk-foas-1.0.9/src/ros_cdk_foas.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 11:35:48.000000 ros-cdk-foas-1.0.9/src/ros_cdk_foas.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2022-09-23 11:35:48.000000 ros-cdk-foas-1.0.9/src/ros_cdk_foas.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2022-09-23 11:35:48.000000 ros-cdk-foas-1.0.9/src/ros_cdk_foas.egg-info/top_level.txt
```

### Comparing `ros-cdk-foas-1.0.8/LICENSE` & `ros-cdk-foas-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-foas-1.0.8/PKG-INFO` & `ros-cdk-foas-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-foas
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS FOAS Construct Library
```

### Comparing `ros-cdk-foas-1.0.8/setup.py` & `ros-cdk-foas-1.0.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-foas",
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
         "ros_cdk_foas",
         "ros_cdk_foas._jsii"
     ],
     "package_data": {
         "ros_cdk_foas._jsii": [
-            "ros-cdk-foas@1.0.8.jsii.tgz"
+            "ros-cdk-foas@1.0.9.jsii.tgz"
         ],
         "ros_cdk_foas": [
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

### Comparing `ros-cdk-foas-1.0.8/src/ros_cdk_foas/__init__.py` & `ros-cdk-foas-1.0.9/src/ros_cdk_foas/__init__.py`

 * *Files 23% similar despite different names*

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
 
 
 class Cluster(
     ros_cdk_core.Resource,
@@ -29,73 +31,79 @@
 ):
     '''A ROS resource type:  ``ALIYUN::FOAS::Cluster``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "ClusterProps",
+        props: typing.Union["ClusterProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::FOAS::Cluster``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(Cluster.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrClusterId")
     def attr_cluster_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute ClusterId: Cluster ID.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrClusterId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrEngineVersions")
     def attr_engine_versions(self) -> ros_cdk_core.IResolvable:
         '''Attribute EngineVersions: Engine Versions.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrEngineVersions"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrMasterInstanceInfos")
     def attr_master_instance_infos(self) -> ros_cdk_core.IResolvable:
         '''Attribute MasterInstanceInfos: Master instance infos.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrMasterInstanceInfos"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrOrderId")
     def attr_order_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute OrderId: Order ID.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrOrderId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrSecurityGroupId")
     def attr_security_group_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute SecurityGroupId: Security group Id.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrSecurityGroupId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrSlaveInstanceInfos")
     def attr_slave_instance_infos(self) -> ros_cdk_core.IResolvable:
         '''Attribute SlaveInstanceInfos: Slave instance infos.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrSlaveInstanceInfos"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrState")
     def attr_state(self) -> ros_cdk_core.IResolvable:
         '''Attribute State: Cluster status.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrState"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVSwitchIds")
     def attr_v_switch_ids(self) -> ros_cdk_core.IResolvable:
         '''Attribute VSwitchIds: VSwitch Ids.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVSwitchIds"))
 
 
 @jsii.data_type(
@@ -114,26 +122,34 @@
     def __init__(
         self,
         *,
         cluster_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         description: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         oss_bucket: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         v_switch_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
-        order: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosCluster.OrderProperty"]] = None,
+        order: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosCluster.OrderProperty", typing.Dict[str, typing.Any]]]] = None,
         order_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::FOAS::Cluster``.
 
         :param cluster_name: Property clusterName: Cluster name. It begins with a letter, and contains only lowercase English letters, numbers, underscores (_), and is limited to 3-64 characters.
         :param description: Property description: Cluster description.
         :param oss_bucket: Property ossBucket: Bucket name in your OSS.
         :param v_switch_id: Property vSwitchId: VSwitch ID.
         :param order: Property order: Order detail. Only one of property Order or OrderId can be specified. Order is not suggested. Policy AliyunBSSFullAccess must be granted to StreamDefaultRole in RAM console. The order can not be cancelled.
         :param order_id: Property orderId: Order Id. Only one of property Order or OrderId can be specified. OrderId is suggested.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(ClusterProps.__init__)
+            check_type(argname="argument cluster_name", value=cluster_name, expected_type=type_hints["cluster_name"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument oss_bucket", value=oss_bucket, expected_type=type_hints["oss_bucket"])
+            check_type(argname="argument v_switch_id", value=v_switch_id, expected_type=type_hints["v_switch_id"])
+            check_type(argname="argument order", value=order, expected_type=type_hints["order"])
+            check_type(argname="argument order_id", value=order_id, expected_type=type_hints["order_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "cluster_name": cluster_name,
             "description": description,
             "oss_bucket": oss_bucket,
             "v_switch_id": v_switch_id,
         }
         if order is not None:
@@ -217,31 +233,37 @@
 ):
     '''A ROS resource type:  ``ALIYUN::FOAS::Project``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "ProjectProps",
+        props: typing.Union["ProjectProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::FOAS::Project``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(Project.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrState")
     def attr_state(self) -> ros_cdk_core.IResolvable:
         '''Attribute State: Project state.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrState"))
 
 
 @jsii.data_type(
@@ -272,14 +294,22 @@
         :param deploy_type: Property deployType: Cluster type: Exclusive cluster: cell Shared cluster: public.
         :param manager_ids: Property managerIds: Comma delimited account Id list of managers.
         :param name: Property name: Project name. It begins with a letter, and contains only lowercase English letters, numbers, underscores (_), and is limited to 3-64 characters.
         :param cluster_id: Property clusterId: Cluster ID.
         :param description: Property description: Project description.
         :param order_id: Property orderId: Order Id of Shared cluster.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(ProjectProps.__init__)
+            check_type(argname="argument deploy_type", value=deploy_type, expected_type=type_hints["deploy_type"])
+            check_type(argname="argument manager_ids", value=manager_ids, expected_type=type_hints["manager_ids"])
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+            check_type(argname="argument cluster_id", value=cluster_id, expected_type=type_hints["cluster_id"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument order_id", value=order_id, expected_type=type_hints["order_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "deploy_type": deploy_type,
             "manager_ids": manager_ids,
             "name": name,
         }
         if cluster_id is not None:
             self._values["cluster_id"] = cluster_id
@@ -355,181 +385,205 @@
 ):
     '''A ROS template type:  ``ALIYUN::FOAS::Cluster``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosClusterProps",
+        props: typing.Union["RosClusterProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::FOAS::Cluster``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosCluster.__init__)
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
+            type_hints = typing.get_type_hints(RosCluster._render_properties)
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
     @jsii.member(jsii_name="attrClusterId")
     def attr_cluster_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ClusterId: Cluster ID.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrClusterId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrEngineVersions")
     def attr_engine_versions(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: EngineVersions: Engine Versions.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrEngineVersions"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrMasterInstanceInfos")
     def attr_master_instance_infos(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: MasterInstanceInfos: Master instance infos.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrMasterInstanceInfos"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrOrderId")
     def attr_order_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: OrderId: Order ID.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrOrderId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrSecurityGroupId")
     def attr_security_group_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: SecurityGroupId: Security group Id.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrSecurityGroupId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrSlaveInstanceInfos")
     def attr_slave_instance_infos(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: SlaveInstanceInfos: Slave instance infos.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrSlaveInstanceInfos"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrState")
     def attr_state(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: State: Cluster status.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrState"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVSwitchIds")
     def attr_v_switch_ids(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: VSwitchIds: VSwitch Ids.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVSwitchIds"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="clusterName")
     def cluster_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: clusterName: Cluster name. It begins with a letter, and contains only lowercase English letters, numbers, underscores (_), and is limited to 3-64 characters.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "clusterName"))
 
     @cluster_name.setter
     def cluster_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "cluster_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "clusterName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="description")
     def description(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: description: Cluster description.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "description"))
 
     @description.setter
     def description(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "description").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "description", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="ossBucket")
     def oss_bucket(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: ossBucket: Bucket name in your OSS.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "ossBucket"))
 
     @oss_bucket.setter
     def oss_bucket(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "oss_bucket").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "ossBucket", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vSwitchId")
     def v_switch_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: vSwitchId: VSwitch ID.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "vSwitchId"))
 
     @v_switch_id.setter
     def v_switch_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "v_switch_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "vSwitchId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="order")
     def order(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosCluster.OrderProperty"]]:
         '''
         :Property:
 
@@ -541,17 +595,20 @@
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosCluster.OrderProperty"]], jsii.get(self, "order"))
 
     @order.setter
     def order(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosCluster.OrderProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "order").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "order", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="orderId")
     def order_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -561,14 +618,17 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "orderId"))
 
     @order_id.setter
     def order_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "order_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "orderId", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-foas.RosCluster.OrderProperty",
         jsii_struct_bases=[],
         name_mapping={
             "master_spec": "masterSpec",
@@ -594,14 +654,22 @@
             :param master_spec: 
             :param slave_spec: 
             :param master_number: 
             :param pay_model: 
             :param period: 
             :param slave_number: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosCluster.OrderProperty.__init__)
+                check_type(argname="argument master_spec", value=master_spec, expected_type=type_hints["master_spec"])
+                check_type(argname="argument slave_spec", value=slave_spec, expected_type=type_hints["slave_spec"])
+                check_type(argname="argument master_number", value=master_number, expected_type=type_hints["master_number"])
+                check_type(argname="argument pay_model", value=pay_model, expected_type=type_hints["pay_model"])
+                check_type(argname="argument period", value=period, expected_type=type_hints["period"])
+                check_type(argname="argument slave_number", value=slave_number, expected_type=type_hints["slave_number"])
             self._values: typing.Dict[str, typing.Any] = {
                 "master_spec": master_spec,
                 "slave_spec": slave_spec,
             }
             if master_number is not None:
                 self._values["master_number"] = master_number
             if pay_model is not None:
@@ -697,26 +765,34 @@
     def __init__(
         self,
         *,
         cluster_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         description: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         oss_bucket: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         v_switch_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
-        order: typing.Optional[typing.Union[ros_cdk_core.IResolvable, RosCluster.OrderProperty]] = None,
+        order: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosCluster.OrderProperty, typing.Dict[str, typing.Any]]]] = None,
         order_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::FOAS::Cluster``.
 
         :param cluster_name: 
         :param description: 
         :param oss_bucket: 
         :param v_switch_id: 
         :param order: 
         :param order_id: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosClusterProps.__init__)
+            check_type(argname="argument cluster_name", value=cluster_name, expected_type=type_hints["cluster_name"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument oss_bucket", value=oss_bucket, expected_type=type_hints["oss_bucket"])
+            check_type(argname="argument v_switch_id", value=v_switch_id, expected_type=type_hints["v_switch_id"])
+            check_type(argname="argument order", value=order, expected_type=type_hints["order"])
+            check_type(argname="argument order_id", value=order_id, expected_type=type_hints["order_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "cluster_name": cluster_name,
             "description": description,
             "oss_bucket": oss_bucket,
             "v_switch_id": v_switch_id,
         }
         if order is not None:
@@ -807,56 +883,65 @@
 ):
     '''A ROS template type:  ``ALIYUN::FOAS::Project``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosProjectProps",
+        props: typing.Union["RosProjectProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::FOAS::Project``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosProject.__init__)
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
+            type_hints = typing.get_type_hints(RosProject._render_properties)
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
     @jsii.member(jsii_name="attrState")
     def attr_state(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: State: Project state.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrState"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="deployType")
     def deploy_type(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         deployType: Cluster type:
         Exclusive cluster: cell
@@ -865,101 +950,122 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "deployType"))
 
     @deploy_type.setter
     def deploy_type(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosProject, "deploy_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "deployType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosProject, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="managerIds")
     def manager_ids(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: managerIds: Comma delimited account Id list of managers.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "managerIds"))
 
     @manager_ids.setter
     def manager_ids(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosProject, "manager_ids").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "managerIds", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="name")
     def name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: name: Project name. It begins with a letter, and contains only lowercase English letters, numbers, underscores (_), and is limited to 3-64 characters.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "name"))
 
     @name.setter
     def name(self, value: typing.Union[builtins.str, ros_cdk_core.IResolvable]) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosProject, "name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "name", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="clusterId")
     def cluster_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: clusterId: Cluster ID.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "clusterId"))
 
     @cluster_id.setter
     def cluster_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosProject, "cluster_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "clusterId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="description")
     def description(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: description: Project description.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "description"))
 
     @description.setter
     def description(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosProject, "description").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "description", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="orderId")
     def order_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: orderId: Order Id of Shared cluster.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "orderId"))
 
     @order_id.setter
     def order_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosProject, "order_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "orderId", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-foas.RosProjectProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -987,14 +1093,22 @@
         :param deploy_type: 
         :param manager_ids: 
         :param name: 
         :param cluster_id: 
         :param description: 
         :param order_id: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosProjectProps.__init__)
+            check_type(argname="argument deploy_type", value=deploy_type, expected_type=type_hints["deploy_type"])
+            check_type(argname="argument manager_ids", value=manager_ids, expected_type=type_hints["manager_ids"])
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+            check_type(argname="argument cluster_id", value=cluster_id, expected_type=type_hints["cluster_id"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument order_id", value=order_id, expected_type=type_hints["order_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "deploy_type": deploy_type,
             "manager_ids": manager_ids,
             "name": name,
         }
         if cluster_id is not None:
             self._values["cluster_id"] = cluster_id
```

### Comparing `ros-cdk-foas-1.0.8/src/ros_cdk_foas.egg-info/PKG-INFO` & `ros-cdk-foas-1.0.9/src/ros_cdk_foas.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-foas
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS FOAS Construct Library
```

