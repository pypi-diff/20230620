# Comparing `tmp/ros-cdk-edas-1.0.8.tar.gz` & `tmp/ros-cdk-edas-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-edas-1.0.8.tar", last modified: Thu Jul 14 02:18:17 2022, max compression
+gzip compressed data, was "dist/ros-cdk-edas-1.0.9.tar", last modified: Fri Sep 23 11:32:49 2022, max compression
```

## Comparing `ros-cdk-edas-1.0.8.tar` & `ros-cdk-edas-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:18:17.000000 ros-cdk-edas-1.0.8/
--rw-r--r--   0 root         (0) root         (0)    10279 2022-07-14 02:18:16.000000 ros-cdk-edas-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2022-07-14 02:18:16.000000 ros-cdk-edas-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2022-07-14 02:18:16.000000 ros-cdk-edas-1.0.8/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1244 2022-07-14 02:18:17.000000 ros-cdk-edas-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      182 2022-07-14 02:18:16.000000 ros-cdk-edas-1.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)      106 2022-07-14 02:18:16.000000 ros-cdk-edas-1.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-07-14 02:18:17.000000 ros-cdk-edas-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1800 2022-07-14 02:18:16.000000 ros-cdk-edas-1.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:18:17.000000 ros-cdk-edas-1.0.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:18:17.000000 ros-cdk-edas-1.0.8/src/ros_cdk_edas/
--rw-r--r--   0 root         (0) root         (0)   407338 2022-07-14 02:18:16.000000 ros-cdk-edas-1.0.8/src/ros_cdk_edas/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:18:17.000000 ros-cdk-edas-1.0.8/src/ros_cdk_edas/_jsii/
--rw-r--r--   0 root         (0) root         (0)      372 2022-07-14 02:18:16.000000 ros-cdk-edas-1.0.8/src/ros_cdk_edas/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)   140767 2022-07-14 02:18:16.000000 ros-cdk-edas-1.0.8/src/ros_cdk_edas/_jsii/ros-cdk-edas@1.0.8.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:18:16.000000 ros-cdk-edas-1.0.8/src/ros_cdk_edas/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:18:17.000000 ros-cdk-edas-1.0.8/src/ros_cdk_edas.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1244 2022-07-14 02:18:16.000000 ros-cdk-edas-1.0.8/src/ros_cdk_edas.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      410 2022-07-14 02:18:16.000000 ros-cdk-edas-1.0.8/src/ros_cdk_edas.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:18:16.000000 ros-cdk-edas-1.0.8/src/ros_cdk_edas.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2022-07-14 02:18:16.000000 ros-cdk-edas-1.0.8/src/ros_cdk_edas.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2022-07-14 02:18:16.000000 ros-cdk-edas-1.0.8/src/ros_cdk_edas.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:32:49.000000 ros-cdk-edas-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)    10279 2022-09-23 11:32:49.000000 ros-cdk-edas-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-09-23 11:32:49.000000 ros-cdk-edas-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2022-09-23 11:32:49.000000 ros-cdk-edas-1.0.9/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1244 2022-09-23 11:32:49.000000 ros-cdk-edas-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      182 2022-09-23 11:32:49.000000 ros-cdk-edas-1.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      236 2022-09-23 11:32:49.000000 ros-cdk-edas-1.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-09-23 11:32:49.000000 ros-cdk-edas-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1829 2022-09-23 11:32:49.000000 ros-cdk-edas-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:32:49.000000 ros-cdk-edas-1.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:32:49.000000 ros-cdk-edas-1.0.9/src/ros_cdk_edas/
+-rw-r--r--   0 root         (0) root         (0)   483589 2022-09-23 11:32:49.000000 ros-cdk-edas-1.0.9/src/ros_cdk_edas/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:32:49.000000 ros-cdk-edas-1.0.9/src/ros_cdk_edas/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      406 2022-09-23 11:32:49.000000 ros-cdk-edas-1.0.9/src/ros_cdk_edas/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   140813 2022-09-23 11:32:49.000000 ros-cdk-edas-1.0.9/src/ros_cdk_edas/_jsii/ros-cdk-edas@1.0.9.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 11:32:49.000000 ros-cdk-edas-1.0.9/src/ros_cdk_edas/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:32:49.000000 ros-cdk-edas-1.0.9/src/ros_cdk_edas.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1244 2022-09-23 11:32:49.000000 ros-cdk-edas-1.0.9/src/ros_cdk_edas.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      410 2022-09-23 11:32:49.000000 ros-cdk-edas-1.0.9/src/ros_cdk_edas.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 11:32:49.000000 ros-cdk-edas-1.0.9/src/ros_cdk_edas.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2022-09-23 11:32:49.000000 ros-cdk-edas-1.0.9/src/ros_cdk_edas.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2022-09-23 11:32:49.000000 ros-cdk-edas-1.0.9/src/ros_cdk_edas.egg-info/top_level.txt
```

### Comparing `ros-cdk-edas-1.0.8/LICENSE` & `ros-cdk-edas-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-edas-1.0.8/PKG-INFO` & `ros-cdk-edas-1.0.9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-edas
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS EDAS Construct Library
```

### Comparing `ros-cdk-edas-1.0.8/setup.py` & `ros-cdk-edas-1.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-edas",
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
         "ros_cdk_edas",
         "ros_cdk_edas._jsii"
     ],
     "package_data": {
         "ros_cdk_edas._jsii": [
-            "ros-cdk-edas@1.0.8.jsii.tgz"
+            "ros-cdk-edas@1.0.9.jsii.tgz"
         ],
         "ros_cdk_edas": [
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

### Comparing `ros-cdk-edas-1.0.8/src/ros_cdk_edas/__init__.py` & `ros-cdk-edas-1.0.9/src/ros_cdk_edas/__init__.py`

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
 
 
 class Application(
     ros_cdk_core.Resource,
@@ -29,37 +31,43 @@
 ):
     '''A ROS resource type:  ``ALIYUN::EDAS::Application``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "ApplicationProps",
+        props: typing.Union["ApplicationProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::EDAS::Application``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(Application.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrAppId")
     def attr_app_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute AppId: Application Id, a unique identifier EDAS application.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAppId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPort")
     def attr_port(self) -> ros_cdk_core.IResolvable:
         '''Attribute Port: Application port.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPort"))
 
 
 @jsii.data_type(
@@ -102,14 +110,26 @@
         :param description: Property description: Descriptive information.
         :param ecu_info: Property ecuInfo: Machine capacity is needed ecu_id (ECS Examples introducing another unique identity EDAS EDAS), the plurality of "," separated (by querying ListScaleOutEcu wherein ecu_id Interface to obtain).
         :param health_check_url: Property healthCheckUrl: Application Health Check URL.
         :param logical_region_id: Property logicalRegionId: Namespace ID.
         :param package_type: Property packageType: Application packet format, possible values: war or jar.
         :param resource_group_id: Property resourceGroupId: Resource group id.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(ApplicationProps.__init__)
+            check_type(argname="argument application_name", value=application_name, expected_type=type_hints["application_name"])
+            check_type(argname="argument cluster_id", value=cluster_id, expected_type=type_hints["cluster_id"])
+            check_type(argname="argument build_pack_id", value=build_pack_id, expected_type=type_hints["build_pack_id"])
+            check_type(argname="argument component_ids", value=component_ids, expected_type=type_hints["component_ids"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument ecu_info", value=ecu_info, expected_type=type_hints["ecu_info"])
+            check_type(argname="argument health_check_url", value=health_check_url, expected_type=type_hints["health_check_url"])
+            check_type(argname="argument logical_region_id", value=logical_region_id, expected_type=type_hints["logical_region_id"])
+            check_type(argname="argument package_type", value=package_type, expected_type=type_hints["package_type"])
+            check_type(argname="argument resource_group_id", value=resource_group_id, expected_type=type_hints["resource_group_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "application_name": application_name,
             "cluster_id": cluster_id,
         }
         if build_pack_id is not None:
             self._values["build_pack_id"] = build_pack_id
         if component_ids is not None:
@@ -232,49 +252,55 @@
 ):
     '''A ROS resource type:  ``ALIYUN::EDAS::Cluster``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "ClusterProps",
+        props: typing.Union["ClusterProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::EDAS::Cluster``.
 
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
     @jsii.member(jsii_name="attrClusterName")
     def attr_cluster_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute ClusterName: Cluster name.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrClusterName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrClusterType")
     def attr_cluster_type(self) -> ros_cdk_core.IResolvable:
         '''Attribute ClusterType: Cluster type.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrClusterType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrIaasProvider")
     def attr_iaas_provider(self) -> ros_cdk_core.IResolvable:
         '''Attribute IaasProvider: Provider.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrIaasProvider"))
 
 
 class ClusterMember(
@@ -284,43 +310,49 @@
 ):
     '''A ROS resource type:  ``ALIYUN::EDAS::ClusterMember``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "ClusterMemberProps",
+        props: typing.Union["ClusterMemberProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::EDAS::ClusterMember``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(ClusterMember.__init__)
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
     @jsii.member(jsii_name="attrClusterMemberIds")
     def attr_cluster_member_ids(self) -> ros_cdk_core.IResolvable:
         '''Attribute ClusterMemberIds: Cluster member IDs corresponding to the ECS instance IDs.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrClusterMemberIds"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInstanceIds")
     def attr_instance_ids(self) -> ros_cdk_core.IResolvable:
         '''Attribute InstanceIds: ECS instance IDs.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInstanceIds"))
 
 
 @jsii.data_type(
@@ -342,14 +374,19 @@
     ) -> None:
         '''Properties for defining a ``ALIYUN::EDAS::ClusterMember``.
 
         :param cluster_id: Property clusterId: Cluster ID to import ECS instance.
         :param instance_ids: Property instanceIds: ECS instance ID list to import.
         :param password: Property password: Password ECS hosts need to import (ECS settings can continue to use purchased).
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(ClusterMemberProps.__init__)
+            check_type(argname="argument cluster_id", value=cluster_id, expected_type=type_hints["cluster_id"])
+            check_type(argname="argument instance_ids", value=instance_ids, expected_type=type_hints["instance_ids"])
+            check_type(argname="argument password", value=password, expected_type=type_hints["password"])
         self._values: typing.Dict[str, typing.Any] = {
             "cluster_id": cluster_id,
             "instance_ids": instance_ids,
             "password": password,
         }
 
     @builtins.property
@@ -418,14 +455,23 @@
         :param cluster_type: Property clusterType: Cluster type. 1-Swarm cluster, 2-ECS cluster, 3-Kubernetes Cluster
         :param network_mode: Property networkMode: Network Type. 1- classic network, 2-VPC
         :param logical_region_id: Property logicalRegionId: Custom namespace RegionId (format: Physical Region: custom namespace identifier).
         :param oversold_factor: Property oversoldFactor: Docker CPU cluster oversold. Support 2 (1: 2 ratio) / 4 (1: 4) / 8 (1: 8 ratio)
         :param resource_group_id: Property resourceGroupId: Resource group id.
         :param vpc_id: Property vpcId: VPC network ID. If network selection VPC, this parameter Required
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(ClusterProps.__init__)
+            check_type(argname="argument cluster_name", value=cluster_name, expected_type=type_hints["cluster_name"])
+            check_type(argname="argument cluster_type", value=cluster_type, expected_type=type_hints["cluster_type"])
+            check_type(argname="argument network_mode", value=network_mode, expected_type=type_hints["network_mode"])
+            check_type(argname="argument logical_region_id", value=logical_region_id, expected_type=type_hints["logical_region_id"])
+            check_type(argname="argument oversold_factor", value=oversold_factor, expected_type=type_hints["oversold_factor"])
+            check_type(argname="argument resource_group_id", value=resource_group_id, expected_type=type_hints["resource_group_id"])
+            check_type(argname="argument vpc_id", value=vpc_id, expected_type=type_hints["vpc_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "cluster_name": cluster_name,
             "cluster_type": cluster_type,
             "network_mode": network_mode,
         }
         if logical_region_id is not None:
             self._values["logical_region_id"] = logical_region_id
@@ -520,43 +566,49 @@
 ):
     '''A ROS resource type:  ``ALIYUN::EDAS::DeployGroup``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "DeployGroupProps",
+        props: typing.Union["DeployGroupProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::EDAS::DeployGroup``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(DeployGroup.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrAppId")
     def attr_app_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute AppId: Application ID.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAppId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrGroupName")
     def attr_group_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute GroupName: Deploy group name.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrGroupName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrId")
     def attr_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute Id: Deploy group ID.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrId"))
 
 
 @jsii.data_type(
@@ -572,14 +624,18 @@
         group_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
         '''Properties for defining a ``ALIYUN::EDAS::DeployGroup``.
 
         :param app_id: Property appId: Application ID.
         :param group_name: Property groupName: Group name, maximum length of 64.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(DeployGroupProps.__init__)
+            check_type(argname="argument app_id", value=app_id, expected_type=type_hints["app_id"])
+            check_type(argname="argument group_name", value=group_name, expected_type=type_hints["group_name"])
         self._values: typing.Dict[str, typing.Any] = {
             "app_id": app_id,
             "group_name": group_name,
         }
 
     @builtins.property
     def app_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
@@ -614,55 +670,61 @@
 ):
     '''A ROS resource type:  ``ALIYUN::EDAS::K8sApplication``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "K8sApplicationProps",
+        props: typing.Union["K8sApplicationProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::EDAS::K8sApplication``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(K8sApplication.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrAppId")
     def attr_app_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute AppId: The ID of the application.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAppId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrAppName")
     def attr_app_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute AppName: The name of the application.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAppName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrChangeOrderId")
     def attr_change_order_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute ChangeOrderId: The ID of the change process.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrChangeOrderId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrClusterId")
     def attr_cluster_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute ClusterId: The cluster ID of the application.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrClusterId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrCsClusterId")
     def attr_cs_cluster_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute CsClusterId: The K8s cluster ID of the application.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrCsClusterId"))
 
 
 @jsii.data_type(
@@ -723,58 +785,58 @@
     def __init__(
         self,
         *,
         app_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         cluster_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         application_description: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         command: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        command_args: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosK8sApplication.CommandArgsProperty"]]]] = None,
+        command_args: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosK8sApplication.CommandArgsProperty", typing.Dict[str, typing.Any]]]]]] = None,
         deploy_across_nodes: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         deploy_across_zones: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         edas_container_version: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         enable_ahas: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
-        envs: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosK8sApplication.EnvsProperty"]]]] = None,
+        envs: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosK8sApplication.EnvsProperty", typing.Dict[str, typing.Any]]]]]] = None,
         image_url: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         internet_slb_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         internet_slb_port: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         internet_slb_protocol: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         internet_target_port: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         intranet_slb_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         intranet_slb_port: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         intranet_slb_protocol: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         intranet_target_port: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         is_multilingual_app: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
-        java_start_up_config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosK8sApplication.JavaStartUpConfigProperty"]] = None,
+        java_start_up_config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosK8sApplication.JavaStartUpConfigProperty", typing.Dict[str, typing.Any]]]] = None,
         jdk: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         limit_cpu: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         limit_mem: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
-        liveness: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosK8sApplication.LivenessProperty"]] = None,
-        local_volume: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosK8sApplication.LocalVolumeProperty"]]]] = None,
+        liveness: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosK8sApplication.LivenessProperty", typing.Dict[str, typing.Any]]]] = None,
+        local_volume: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosK8sApplication.LocalVolumeProperty", typing.Dict[str, typing.Any]]]]]] = None,
         logical_region_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        mount_descs: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosK8sApplication.MountDescsProperty"]]]] = None,
+        mount_descs: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosK8sApplication.MountDescsProperty", typing.Dict[str, typing.Any]]]]]] = None,
         namespace: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         nas_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         package_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         package_url: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         package_version: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        post_start: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosK8sApplication.PostStartProperty"]] = None,
-        pre_stop: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosK8sApplication.PreStopProperty"]] = None,
-        readiness: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosK8sApplication.ReadinessProperty"]] = None,
+        post_start: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosK8sApplication.PostStartProperty", typing.Dict[str, typing.Any]]]] = None,
+        pre_stop: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosK8sApplication.PreStopProperty", typing.Dict[str, typing.Any]]]] = None,
+        readiness: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosK8sApplication.ReadinessProperty", typing.Dict[str, typing.Any]]]] = None,
         replicas: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         repo_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         requests_cpu: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         requests_mem: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         runtime_class_name: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        sls_configs: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosK8sApplication.SlsConfigsProperty"]]]] = None,
+        sls_configs: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosK8sApplication.SlsConfigsProperty", typing.Dict[str, typing.Any]]]]]] = None,
         storage_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         timeout: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         uri_encoding: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         use_body_encoding: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         web_container: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        web_container_config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosK8sApplication.WebContainerConfigProperty"]] = None,
+        web_container_config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosK8sApplication.WebContainerConfigProperty", typing.Dict[str, typing.Any]]]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::EDAS::K8sApplication``.
 
         :param app_name: Property appName: The name of the application. The name must start with a letter and can contain digits, letters, and hyphens (-). It can be up to 36 characters in length.
         :param cluster_id: Property clusterId: The cluster ID. You can query the cluster ID by calling the ListCluster operation. For more information, see ListCluster.
         :param application_description: Property applicationDescription: The description of the application.
         :param command: Property command: The command that is specified. If it is specified, it replaces the startup command in the image when the image is started.
@@ -819,14 +881,64 @@
         :param storage_type: Property storageType: Only SSD is supported.
         :param timeout: Property timeout: The timeout interval of the change process. Unit: seconds.
         :param uri_encoding: Property uriEncoding: The uniform resource identifier (URI) encoding scheme. Valid values: ISO-8859-1, GBK, GB2312, and UTF-8. Note If this parameter is not specified in application configuration, the default URI encoding scheme in the Tomcat container is applied.
         :param use_body_encoding: Property useBodyEncoding: Specifies whether useBodyEncodingForURI is enabled. Note If this parameter is not specified in application configuration, the default value false is applied.
         :param web_container: Property webContainer: The version of the Tomcat container on which the deployment package of the application depends. This parameter is applicable to Spring Cloud and Apache Dubbo applications that are deployed by using WAR packages. This parameter is not supported when you deploy an application by using images.
         :param web_container_config: Property webContainerConfig: The Tomcat container configuration.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(K8sApplicationProps.__init__)
+            check_type(argname="argument app_name", value=app_name, expected_type=type_hints["app_name"])
+            check_type(argname="argument cluster_id", value=cluster_id, expected_type=type_hints["cluster_id"])
+            check_type(argname="argument application_description", value=application_description, expected_type=type_hints["application_description"])
+            check_type(argname="argument command", value=command, expected_type=type_hints["command"])
+            check_type(argname="argument command_args", value=command_args, expected_type=type_hints["command_args"])
+            check_type(argname="argument deploy_across_nodes", value=deploy_across_nodes, expected_type=type_hints["deploy_across_nodes"])
+            check_type(argname="argument deploy_across_zones", value=deploy_across_zones, expected_type=type_hints["deploy_across_zones"])
+            check_type(argname="argument edas_container_version", value=edas_container_version, expected_type=type_hints["edas_container_version"])
+            check_type(argname="argument enable_ahas", value=enable_ahas, expected_type=type_hints["enable_ahas"])
+            check_type(argname="argument envs", value=envs, expected_type=type_hints["envs"])
+            check_type(argname="argument image_url", value=image_url, expected_type=type_hints["image_url"])
+            check_type(argname="argument internet_slb_id", value=internet_slb_id, expected_type=type_hints["internet_slb_id"])
+            check_type(argname="argument internet_slb_port", value=internet_slb_port, expected_type=type_hints["internet_slb_port"])
+            check_type(argname="argument internet_slb_protocol", value=internet_slb_protocol, expected_type=type_hints["internet_slb_protocol"])
+            check_type(argname="argument internet_target_port", value=internet_target_port, expected_type=type_hints["internet_target_port"])
+            check_type(argname="argument intranet_slb_id", value=intranet_slb_id, expected_type=type_hints["intranet_slb_id"])
+            check_type(argname="argument intranet_slb_port", value=intranet_slb_port, expected_type=type_hints["intranet_slb_port"])
+            check_type(argname="argument intranet_slb_protocol", value=intranet_slb_protocol, expected_type=type_hints["intranet_slb_protocol"])
+            check_type(argname="argument intranet_target_port", value=intranet_target_port, expected_type=type_hints["intranet_target_port"])
+            check_type(argname="argument is_multilingual_app", value=is_multilingual_app, expected_type=type_hints["is_multilingual_app"])
+            check_type(argname="argument java_start_up_config", value=java_start_up_config, expected_type=type_hints["java_start_up_config"])
+            check_type(argname="argument jdk", value=jdk, expected_type=type_hints["jdk"])
+            check_type(argname="argument limit_cpu", value=limit_cpu, expected_type=type_hints["limit_cpu"])
+            check_type(argname="argument limit_mem", value=limit_mem, expected_type=type_hints["limit_mem"])
+            check_type(argname="argument liveness", value=liveness, expected_type=type_hints["liveness"])
+            check_type(argname="argument local_volume", value=local_volume, expected_type=type_hints["local_volume"])
+            check_type(argname="argument logical_region_id", value=logical_region_id, expected_type=type_hints["logical_region_id"])
+            check_type(argname="argument mount_descs", value=mount_descs, expected_type=type_hints["mount_descs"])
+            check_type(argname="argument namespace", value=namespace, expected_type=type_hints["namespace"])
+            check_type(argname="argument nas_id", value=nas_id, expected_type=type_hints["nas_id"])
+            check_type(argname="argument package_type", value=package_type, expected_type=type_hints["package_type"])
+            check_type(argname="argument package_url", value=package_url, expected_type=type_hints["package_url"])
+            check_type(argname="argument package_version", value=package_version, expected_type=type_hints["package_version"])
+            check_type(argname="argument post_start", value=post_start, expected_type=type_hints["post_start"])
+            check_type(argname="argument pre_stop", value=pre_stop, expected_type=type_hints["pre_stop"])
+            check_type(argname="argument readiness", value=readiness, expected_type=type_hints["readiness"])
+            check_type(argname="argument replicas", value=replicas, expected_type=type_hints["replicas"])
+            check_type(argname="argument repo_id", value=repo_id, expected_type=type_hints["repo_id"])
+            check_type(argname="argument requests_cpu", value=requests_cpu, expected_type=type_hints["requests_cpu"])
+            check_type(argname="argument requests_mem", value=requests_mem, expected_type=type_hints["requests_mem"])
+            check_type(argname="argument runtime_class_name", value=runtime_class_name, expected_type=type_hints["runtime_class_name"])
+            check_type(argname="argument sls_configs", value=sls_configs, expected_type=type_hints["sls_configs"])
+            check_type(argname="argument storage_type", value=storage_type, expected_type=type_hints["storage_type"])
+            check_type(argname="argument timeout", value=timeout, expected_type=type_hints["timeout"])
+            check_type(argname="argument uri_encoding", value=uri_encoding, expected_type=type_hints["uri_encoding"])
+            check_type(argname="argument use_body_encoding", value=use_body_encoding, expected_type=type_hints["use_body_encoding"])
+            check_type(argname="argument web_container", value=web_container, expected_type=type_hints["web_container"])
+            check_type(argname="argument web_container_config", value=web_container_config, expected_type=type_hints["web_container_config"])
         self._values: typing.Dict[str, typing.Any] = {
             "app_name": app_name,
             "cluster_id": cluster_id,
         }
         if application_description is not None:
             self._values["application_description"] = application_description
         if command is not None:
@@ -1448,79 +1560,85 @@
 ):
     '''A ROS resource type:  ``ALIYUN::EDAS::K8sCluster``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "K8sClusterProps",
+        props: typing.Union["K8sClusterProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::EDAS::K8sCluster``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(K8sCluster.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrClusterId")
     def attr_cluster_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute ClusterId: The ID of the cluster.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrClusterId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrClusterName")
     def attr_cluster_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute ClusterName: The name of the cluster.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrClusterName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrClusterType")
     def attr_cluster_type(self) -> ros_cdk_core.IResolvable:
         '''Attribute ClusterType: The type of the cluster: 2: ECS cluster 5: Container Service K8s cluster or Serverless K8s cluster.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrClusterType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrCsClusterId")
     def attr_cs_cluster_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute CsClusterId: The ID of the K8s cluster.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrCsClusterId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrNetworkMode")
     def attr_network_mode(self) -> ros_cdk_core.IResolvable:
         '''Attribute NetworkMode: Network node: 1: Classic network 2: VPC.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrNetworkMode"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrNodeNum")
     def attr_node_num(self) -> ros_cdk_core.IResolvable:
         '''Attribute NodeNum: Number of nodes.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrNodeNum"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrSubNetCidr")
     def attr_sub_net_cidr(self) -> ros_cdk_core.IResolvable:
         '''Attribute SubNetCidr: Sub net CIDR.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrSubNetCidr"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVpcId")
     def attr_vpc_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute VpcId: The ID of the cluster.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVpcId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVswitchId")
     def attr_vswitch_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute VswitchId: The ID of the cluster.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVswitchId"))
 
 
 @jsii.data_type(
@@ -1542,14 +1660,19 @@
     ) -> None:
         '''Properties for defining a ``ALIYUN::EDAS::K8sCluster``.
 
         :param cs_cluster_id: Property csClusterId: The ID of the CS cluster.
         :param enable_asm: Property enableAsm: Whether enable ASM.
         :param namespace_id: Property namespaceId: The ID of the namespace to which the cluster that you want to import belongs.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(K8sClusterProps.__init__)
+            check_type(argname="argument cs_cluster_id", value=cs_cluster_id, expected_type=type_hints["cs_cluster_id"])
+            check_type(argname="argument enable_asm", value=enable_asm, expected_type=type_hints["enable_asm"])
+            check_type(argname="argument namespace_id", value=namespace_id, expected_type=type_hints["namespace_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "cs_cluster_id": cs_cluster_id,
         }
         if enable_asm is not None:
             self._values["enable_asm"] = enable_asm
         if namespace_id is not None:
             self._values["namespace_id"] = namespace_id
@@ -1596,55 +1719,61 @@
 ):
     '''A ROS resource type:  ``ALIYUN::EDAS::K8sSlbBinding``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "K8sSlbBindingProps",
+        props: typing.Union["K8sSlbBindingProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::EDAS::K8sSlbBinding``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(K8sSlbBinding.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrAddress")
     def attr_address(self) -> ros_cdk_core.IResolvable:
         '''Attribute Address: The address of load balancer instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAddress"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrAppId")
     def attr_app_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute AppId: The ID of the application.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAppId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrChangeOrderId")
     def attr_change_order_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute ChangeOrderId: The ID of the change process.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrChangeOrderId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrLoadBalancerId")
     def attr_load_balancer_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute LoadBalancerId: The ID of load balancer instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrLoadBalancerId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrLoadBalancerName")
     def attr_load_balancer_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute LoadBalancerName: The name of load balancer instance defined in EDAS.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrLoadBalancerName"))
 
 
 @jsii.data_type(
@@ -1662,15 +1791,15 @@
 )
 class K8sSlbBindingProps:
     def __init__(
         self,
         *,
         app_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         cluster_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
-        service_port_infos: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosK8sSlbBinding.ServicePortInfosProperty"]]],
+        service_port_infos: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosK8sSlbBinding.ServicePortInfosProperty", typing.Dict[str, typing.Any]]]]],
         type: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         load_balancer_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         scheduler: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         specification: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::EDAS::K8sSlbBinding``.
 
@@ -1678,14 +1807,23 @@
         :param cluster_id: Property clusterId: The ID of the cluster.
         :param service_port_infos: Property servicePortInfos: The information about the ports.
         :param type: Property type: The type of the SLB instance. Valid values: internet and intranet.
         :param load_balancer_id: Property loadBalancerId: The ID of the load balancer instance. If you leave this parameter empty, Enterprise Distributed Application Service (EDAS) automatically purchases an SLB instance.
         :param scheduler: Property scheduler: The scheduling algorithm. Valid values: wrr: Backend servers that have higher weights receive more requests than those that have lower weights. rr: Requests are distributed to backend servers in sequence. Default value: rr
         :param specification: Property specification: The specification of the load balancer instance.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(K8sSlbBindingProps.__init__)
+            check_type(argname="argument app_id", value=app_id, expected_type=type_hints["app_id"])
+            check_type(argname="argument cluster_id", value=cluster_id, expected_type=type_hints["cluster_id"])
+            check_type(argname="argument service_port_infos", value=service_port_infos, expected_type=type_hints["service_port_infos"])
+            check_type(argname="argument type", value=type, expected_type=type_hints["type"])
+            check_type(argname="argument load_balancer_id", value=load_balancer_id, expected_type=type_hints["load_balancer_id"])
+            check_type(argname="argument scheduler", value=scheduler, expected_type=type_hints["scheduler"])
+            check_type(argname="argument specification", value=specification, expected_type=type_hints["specification"])
         self._values: typing.Dict[str, typing.Any] = {
             "app_id": app_id,
             "cluster_id": cluster_id,
             "service_port_infos": service_port_infos,
             "type": type,
         }
         if load_balancer_id is not None:
@@ -1780,120 +1918,141 @@
 ):
     '''A ROS template type:  ``ALIYUN::EDAS::Application``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosApplicationProps",
+        props: typing.Union["RosApplicationProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::EDAS::Application``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosApplication.__init__)
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
+            type_hints = typing.get_type_hints(RosApplication._render_properties)
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
     @jsii.member(jsii_name="attrAppId")
     def attr_app_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: AppId: Application Id, a unique identifier EDAS application
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAppId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPort")
     def attr_port(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Port: Application port
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPort"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="applicationName")
     def application_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: applicationName: The application name (only allow the use of numbers, letters, -, _, up to 36 characters)
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "applicationName"))
 
     @application_name.setter
     def application_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosApplication, "application_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "applicationName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="clusterId")
     def cluster_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: clusterId: Cluster ID of ECS application
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "clusterId"))
 
     @cluster_id.setter
     def cluster_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosApplication, "cluster_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "clusterId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosApplication, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="buildPackId")
     def build_pack_id(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: buildPackId: EDAS-Container construct a packet number (available version list acquired through the ListBuildPack API (ConfigId of response) or "container version" table "Building packet number" column acquisition). When creating HSF application, this parameter must be specified
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "buildPackId"))
 
     @build_pack_id.setter
     def build_pack_id(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosApplication, "build_pack_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "buildPackId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="componentIds")
     def component_ids(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -1905,34 +2064,40 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "componentIds"))
 
     @component_ids.setter
     def component_ids(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosApplication, "component_ids").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "componentIds", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="description")
     def description(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: description: Descriptive information
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "description"))
 
     @description.setter
     def description(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosApplication, "description").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "description", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="ecuInfo")
     def ecu_info(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -1942,82 +2107,97 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "ecuInfo"))
 
     @ecu_info.setter
     def ecu_info(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosApplication, "ecu_info").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "ecuInfo", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="healthCheckUrl")
     def health_check_url(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: healthCheckUrl: Application Health Check URL
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "healthCheckUrl"))
 
     @health_check_url.setter
     def health_check_url(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosApplication, "health_check_url").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "healthCheckUrl", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="logicalRegionId")
     def logical_region_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: logicalRegionId: Namespace ID
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "logicalRegionId"))
 
     @logical_region_id.setter
     def logical_region_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosApplication, "logical_region_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "logicalRegionId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="packageType")
     def package_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: packageType: Application packet format, possible values: war or jar
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "packageType"))
 
     @package_type.setter
     def package_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosApplication, "package_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "packageType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="resourceGroupId")
     def resource_group_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: resourceGroupId: Resource group id.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "resourceGroupId"))
 
     @resource_group_id.setter
     def resource_group_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosApplication, "resource_group_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "resourceGroupId", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-edas.RosApplicationProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -2057,14 +2237,26 @@
         :param description: 
         :param ecu_info: 
         :param health_check_url: 
         :param logical_region_id: 
         :param package_type: 
         :param resource_group_id: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosApplicationProps.__init__)
+            check_type(argname="argument application_name", value=application_name, expected_type=type_hints["application_name"])
+            check_type(argname="argument cluster_id", value=cluster_id, expected_type=type_hints["cluster_id"])
+            check_type(argname="argument build_pack_id", value=build_pack_id, expected_type=type_hints["build_pack_id"])
+            check_type(argname="argument component_ids", value=component_ids, expected_type=type_hints["component_ids"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument ecu_info", value=ecu_info, expected_type=type_hints["ecu_info"])
+            check_type(argname="argument health_check_url", value=health_check_url, expected_type=type_hints["health_check_url"])
+            check_type(argname="argument logical_region_id", value=logical_region_id, expected_type=type_hints["logical_region_id"])
+            check_type(argname="argument package_type", value=package_type, expected_type=type_hints["package_type"])
+            check_type(argname="argument resource_group_id", value=resource_group_id, expected_type=type_hints["resource_group_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "application_name": application_name,
             "cluster_id": cluster_id,
         }
         if build_pack_id is not None:
             self._values["build_pack_id"] = build_pack_id
         if component_ids is not None:
@@ -2207,324 +2399,378 @@
 ):
     '''A ROS template type:  ``ALIYUN::EDAS::Cluster``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosClusterProps",
+        props: typing.Union["RosClusterProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::EDAS::Cluster``.
 
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
         :Attribute: ClusterId: Cluster ID
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrClusterId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrClusterName")
     def attr_cluster_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ClusterName: Cluster name
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrClusterName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrClusterType")
     def attr_cluster_type(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ClusterType: Cluster type
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrClusterType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrIaasProvider")
     def attr_iaas_provider(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: IaasProvider: Provider
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrIaasProvider"))
 
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
         :Property: clusterName: Cluster name
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
     @jsii.member(jsii_name="clusterType")
     def cluster_type(self) -> typing.Union[jsii.Number, ros_cdk_core.IResolvable]:
         '''
         :Property: clusterType: Cluster type. 1-Swarm cluster, 2-ECS cluster, 3-Kubernetes Cluster
         '''
         return typing.cast(typing.Union[jsii.Number, ros_cdk_core.IResolvable], jsii.get(self, "clusterType"))
 
     @cluster_type.setter
     def cluster_type(
         self,
         value: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "cluster_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "clusterType", value)
 
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
     @jsii.member(jsii_name="networkMode")
     def network_mode(self) -> typing.Union[jsii.Number, ros_cdk_core.IResolvable]:
         '''
         :Property: networkMode: Network Type. 1- classic network, 2-VPC
         '''
         return typing.cast(typing.Union[jsii.Number, ros_cdk_core.IResolvable], jsii.get(self, "networkMode"))
 
     @network_mode.setter
     def network_mode(
         self,
         value: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "network_mode").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "networkMode", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="logicalRegionId")
     def logical_region_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: logicalRegionId: Custom namespace RegionId (format: Physical Region: custom namespace identifier)
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "logicalRegionId"))
 
     @logical_region_id.setter
     def logical_region_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "logical_region_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "logicalRegionId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="oversoldFactor")
     def oversold_factor(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: oversoldFactor: Docker CPU cluster oversold. Support 2 (1: 2 ratio) / 4 (1: 4) / 8 (1: 8 ratio)
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "oversoldFactor"))
 
     @oversold_factor.setter
     def oversold_factor(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "oversold_factor").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "oversoldFactor", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="resourceGroupId")
     def resource_group_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: resourceGroupId: Resource group id.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "resourceGroupId"))
 
     @resource_group_id.setter
     def resource_group_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "resource_group_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "resourceGroupId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vpcId")
     def vpc_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: vpcId: VPC network ID. If network selection VPC, this parameter Required
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "vpcId"))
 
     @vpc_id.setter
     def vpc_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "vpc_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "vpcId", value)
 
 
 class RosClusterMember(
     ros_cdk_core.RosResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@alicloud/ros-cdk-edas.RosClusterMember",
 ):
     '''A ROS template type:  ``ALIYUN::EDAS::ClusterMember``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosClusterMemberProps",
+        props: typing.Union["RosClusterMemberProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::EDAS::ClusterMember``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosClusterMember.__init__)
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
+            type_hints = typing.get_type_hints(RosClusterMember._render_properties)
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
     @jsii.member(jsii_name="attrClusterMemberIds")
     def attr_cluster_member_ids(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ClusterMemberIds: Cluster member IDs corresponding to the ECS instance IDs.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrClusterMemberIds"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInstanceIds")
     def attr_instance_ids(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: InstanceIds: ECS instance IDs.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInstanceIds"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="clusterId")
     def cluster_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: clusterId: Cluster ID to import ECS instance
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "clusterId"))
 
     @cluster_id.setter
     def cluster_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosClusterMember, "cluster_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "clusterId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosClusterMember, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="instanceIds")
     def instance_ids(
         self,
     ) -> typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]:
         '''
         :Property: instanceIds: ECS instance ID list to import.
         '''
         return typing.cast(typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]], jsii.get(self, "instanceIds"))
 
     @instance_ids.setter
     def instance_ids(
         self,
         value: typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosClusterMember, "instance_ids").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "instanceIds", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="password")
     def password(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: password: Password ECS hosts need to import (ECS settings can continue to use purchased)
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "password"))
 
     @password.setter
     def password(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosClusterMember, "password").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "password", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-edas.RosClusterMemberProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -2543,14 +2789,19 @@
     ) -> None:
         '''Properties for defining a ``ALIYUN::EDAS::ClusterMember``.
 
         :param cluster_id: 
         :param instance_ids: 
         :param password: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosClusterMemberProps.__init__)
+            check_type(argname="argument cluster_id", value=cluster_id, expected_type=type_hints["cluster_id"])
+            check_type(argname="argument instance_ids", value=instance_ids, expected_type=type_hints["instance_ids"])
+            check_type(argname="argument password", value=password, expected_type=type_hints["password"])
         self._values: typing.Dict[str, typing.Any] = {
             "cluster_id": cluster_id,
             "instance_ids": instance_ids,
             "password": password,
         }
 
     @builtins.property
@@ -2625,14 +2876,23 @@
         :param cluster_type: 
         :param network_mode: 
         :param logical_region_id: 
         :param oversold_factor: 
         :param resource_group_id: 
         :param vpc_id: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosClusterProps.__init__)
+            check_type(argname="argument cluster_name", value=cluster_name, expected_type=type_hints["cluster_name"])
+            check_type(argname="argument cluster_type", value=cluster_type, expected_type=type_hints["cluster_type"])
+            check_type(argname="argument network_mode", value=network_mode, expected_type=type_hints["network_mode"])
+            check_type(argname="argument logical_region_id", value=logical_region_id, expected_type=type_hints["logical_region_id"])
+            check_type(argname="argument oversold_factor", value=oversold_factor, expected_type=type_hints["oversold_factor"])
+            check_type(argname="argument resource_group_id", value=resource_group_id, expected_type=type_hints["resource_group_id"])
+            check_type(argname="argument vpc_id", value=vpc_id, expected_type=type_hints["vpc_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "cluster_name": cluster_name,
             "cluster_type": cluster_type,
             "network_mode": network_mode,
         }
         if logical_region_id is not None:
             self._values["logical_region_id"] = logical_region_id
@@ -2729,108 +2989,126 @@
 ):
     '''A ROS template type:  ``ALIYUN::EDAS::DeployGroup``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosDeployGroupProps",
+        props: typing.Union["RosDeployGroupProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::EDAS::DeployGroup``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosDeployGroup.__init__)
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
+            type_hints = typing.get_type_hints(RosDeployGroup._render_properties)
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
     @jsii.member(jsii_name="attrAppId")
     def attr_app_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: AppId: Application ID
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAppId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrGroupName")
     def attr_group_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: GroupName: Deploy group name
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrGroupName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrId")
     def attr_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Id: Deploy group ID
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="appId")
     def app_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: appId: Application ID
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "appId"))
 
     @app_id.setter
     def app_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDeployGroup, "app_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "appId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDeployGroup, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="groupName")
     def group_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: groupName: Group name, maximum length of 64.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "groupName"))
 
     @group_name.setter
     def group_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDeployGroup, "group_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "groupName", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-edas.RosDeployGroupProps",
     jsii_struct_bases=[],
     name_mapping={"app_id": "appId", "group_name": "groupName"},
@@ -2843,14 +3121,18 @@
         group_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
         '''Properties for defining a ``ALIYUN::EDAS::DeployGroup``.
 
         :param app_id: 
         :param group_name: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosDeployGroupProps.__init__)
+            check_type(argname="argument app_id", value=app_id, expected_type=type_hints["app_id"])
+            check_type(argname="argument group_name", value=group_name, expected_type=type_hints["group_name"])
         self._values: typing.Dict[str, typing.Any] = {
             "app_id": app_id,
             "group_name": group_name,
         }
 
     @builtins.property
     def app_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
@@ -2889,88 +3171,97 @@
 ):
     '''A ROS template type:  ``ALIYUN::EDAS::K8sApplication``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosK8sApplicationProps",
+        props: typing.Union["RosK8sApplicationProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::EDAS::K8sApplication``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosK8sApplication.__init__)
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
+            type_hints = typing.get_type_hints(RosK8sApplication._render_properties)
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
     @jsii.member(jsii_name="attrAppId")
     def attr_app_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: AppId: The ID of the application.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAppId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrAppName")
     def attr_app_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: AppName: The name of the application.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAppName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrChangeOrderId")
     def attr_change_order_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ChangeOrderId: The ID of the change process.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrChangeOrderId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrClusterId")
     def attr_cluster_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ClusterId: The cluster ID of the application.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrClusterId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrCsClusterId")
     def attr_cs_cluster_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: CsClusterId: The K8s cluster ID of the application.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrCsClusterId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="appName")
     def app_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         appName: The name of the application. The name must start with a letter and can contain digits,
         letters, and hyphens (-). It can be up to 36 characters in length.
@@ -2978,17 +3269,20 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "appName"))
 
     @app_name.setter
     def app_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosK8sApplication, "app_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "appName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="clusterId")
     def cluster_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         clusterId: The cluster ID. You can query the cluster ID by calling the ListCluster operation.
         For more information, see ListCluster.
@@ -2996,111 +3290,132 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "clusterId"))
 
     @cluster_id.setter
     def cluster_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosK8sApplication, "cluster_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "clusterId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosK8sApplication, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="applicationDescription")
     def application_description(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: applicationDescription: The description of the application.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "applicationDescription"))
 
     @application_description.setter
     def application_description(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosK8sApplication, "application_description").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "applicationDescription", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="command")
     def command(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: command: The command that is specified. If it is specified, it replaces the startup command in the image when the image is started.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "command"))
 
     @command.setter
     def command(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosK8sApplication, "command").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "command", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="commandArgs")
     def command_args(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosK8sApplication.CommandArgsProperty"]]]]:
         '''
         :Property: commandArgs: The collection of commands. For example, [{"argument":"-c"},{"argument":"test"}], where -c and test are two parameters that can be set.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosK8sApplication.CommandArgsProperty"]]]], jsii.get(self, "commandArgs"))
 
     @command_args.setter
     def command_args(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosK8sApplication.CommandArgsProperty"]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosK8sApplication, "command_args").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "commandArgs", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="deployAcrossNodes")
     def deploy_across_nodes(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property: deployAcrossNodes: Specifies whether to distribute application instances to multiple nodes. The value true indicates yes, whereas other values indicate no.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "deployAcrossNodes"))
 
     @deploy_across_nodes.setter
     def deploy_across_nodes(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosK8sApplication, "deploy_across_nodes").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "deployAcrossNodes", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="deployAcrossZones")
     def deploy_across_zones(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property: deployAcrossZones: Specifies whether to distribute application instances to multiple zones. The value true indicates yes, whereas other values indicate no.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "deployAcrossZones"))
 
     @deploy_across_zones.setter
     def deploy_across_zones(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosK8sApplication, "deploy_across_zones").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "deployAcrossZones", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="edasContainerVersion")
     def edas_container_version(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -3110,119 +3425,140 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "edasContainerVersion"))
 
     @edas_container_version.setter
     def edas_container_version(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosK8sApplication, "edas_container_version").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "edasContainerVersion", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableAhas")
     def enable_ahas(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property: enableAhas: Specifies whether to enable access to Application High Availability Service (AHAS).
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "enableAhas"))
 
     @enable_ahas.setter
     def enable_ahas(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosK8sApplication, "enable_ahas").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableAhas", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="envs")
     def envs(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosK8sApplication.EnvsProperty"]]]]:
         '''
         :Property: envs: The collection of deployment environment variables. For example, [{"Name":"x","Value":"y"},{"Name":"x2","Value":"y2"}].
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosK8sApplication.EnvsProperty"]]]], jsii.get(self, "envs"))
 
     @envs.setter
     def envs(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosK8sApplication.EnvsProperty"]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosK8sApplication, "envs").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "envs", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="imageUrl")
     def image_url(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: imageUrl: The image URL. When PackageType is set to Image, this parameter is required.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "imageUrl"))
 
     @image_url.setter
     def image_url(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosK8sApplication, "image_url").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "imageUrl", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="internetSlbId")
     def internet_slb_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: internetSlbId: The ID of the Internet-facing SLB instance. If this parameter is not specified, EDAS automatically purchases a new SLB instance for you.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "internetSlbId"))
 
     @internet_slb_id.setter
     def internet_slb_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosK8sApplication, "internet_slb_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "internetSlbId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="internetSlbPort")
     def internet_slb_port(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: internetSlbPort: The frontend port of the Internet-facing SLB instance. Valid values: 1 to 65535.
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "internetSlbPort"))
 
     @internet_slb_port.setter
     def internet_slb_port(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosK8sApplication, "internet_slb_port").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "internetSlbPort", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="internetSlbProtocol")
     def internet_slb_protocol(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: internetSlbProtocol: The protocol of the Internet-facing SLB instance. Valid values: TCP, HTTP, and HTTPS.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "internetSlbProtocol"))
 
     @internet_slb_protocol.setter
     def internet_slb_protocol(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosK8sApplication, "internet_slb_protocol").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "internetSlbProtocol", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="internetTargetPort")
     def internet_target_port(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -3232,102 +3568,120 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "internetTargetPort"))
 
     @internet_target_port.setter
     def internet_target_port(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosK8sApplication, "internet_target_port").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "internetTargetPort", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="intranetSlbId")
     def intranet_slb_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: intranetSlbId: The ID of the internal-facing SLB instance. If this parameter is not specified, Enterprise Distributed Application Service (EDAS) automatically purchases a new SLB instance for you.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "intranetSlbId"))
 
     @intranet_slb_id.setter
     def intranet_slb_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosK8sApplication, "intranet_slb_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "intranetSlbId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="intranetSlbPort")
     def intranet_slb_port(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: intranetSlbPort: The frontend port of the internal-facing SLB instance. Valid values: 1 to 65535.
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "intranetSlbPort"))
 
     @intranet_slb_port.setter
     def intranet_slb_port(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosK8sApplication, "intranet_slb_port").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "intranetSlbPort", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="intranetSlbProtocol")
     def intranet_slb_protocol(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: intranetSlbProtocol: The protocol of the internal-facing SLB instance. Valid values: TCP, HTTP, and HTTPS.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "intranetSlbProtocol"))
 
     @intranet_slb_protocol.setter
     def intranet_slb_protocol(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosK8sApplication, "intranet_slb_protocol").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "intranetSlbProtocol", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="intranetTargetPort")
     def intranet_target_port(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: intranetTargetPort: The backend port of the internal-facing Server Load Balancer (SLB) instance, which is also the service port of the application. Valid values: 1 to 65535.
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "intranetTargetPort"))
 
     @intranet_target_port.setter
     def intranet_target_port(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosK8sApplication, "intranet_target_port").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "intranetTargetPort", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="isMultilingualApp")
     def is_multilingual_app(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property: isMultilingualApp: Specifies whether the application is a multi-language application.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "isMultilingualApp"))
 
     @is_multilingual_app.setter
     def is_multilingual_app(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosK8sApplication, "is_multilingual_app").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "isMultilingualApp", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="javaStartUpConfig")
     def java_start_up_config(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosK8sApplication.JavaStartUpConfigProperty"]]:
         '''
         :Property:
 
@@ -3337,17 +3691,20 @@
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosK8sApplication.JavaStartUpConfigProperty"]], jsii.get(self, "javaStartUpConfig"))
 
     @java_start_up_config.setter
     def java_start_up_config(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosK8sApplication.JavaStartUpConfigProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosK8sApplication, "java_start_up_config").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "javaStartUpConfig", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="jdk")
     def jdk(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -3357,17 +3714,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "jdk"))
 
     @jdk.setter
     def jdk(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosK8sApplication, "jdk").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "jdk", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="limitCpu")
     def limit_cpu(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -3377,119 +3737,140 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "limitCpu"))
 
     @limit_cpu.setter
     def limit_cpu(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosK8sApplication, "limit_cpu").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "limitCpu", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="limitMem")
     def limit_mem(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: limitMem: The maximum amount of memory allowed for each application instance when the application is running. Unit: MB.
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "limitMem"))
 
     @limit_mem.setter
     def limit_mem(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosK8sApplication, "limit_mem").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "limitMem", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="liveness")
     def liveness(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosK8sApplication.LivenessProperty"]]:
         '''
         :Property: liveness: The liveness check on the container.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosK8sApplication.LivenessProperty"]], jsii.get(self, "liveness"))
 
     @liveness.setter
     def liveness(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosK8sApplication.LivenessProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosK8sApplication, "liveness").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "liveness", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="localVolume")
     def local_volume(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosK8sApplication.LocalVolumeProperty"]]]]:
         '''
         :Property: localVolume: The configuration for mounting host files to the container where the application is running. For example, the value can be [{"type":"", "nodePath":"/localfiles", "mountPath":"/app/files"}, {"type":"Directory", "nodePath":"/mnt", "mountPath":"/app/storage"}].
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosK8sApplication.LocalVolumeProperty"]]]], jsii.get(self, "localVolume"))
 
     @local_volume.setter
     def local_volume(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosK8sApplication.LocalVolumeProperty"]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosK8sApplication, "local_volume").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "localVolume", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="logicalRegionId")
     def logical_region_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: logicalRegionId: The ID of the EDAS namespace. This parameter is required for a non-default namespace.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "logicalRegionId"))
 
     @logical_region_id.setter
     def logical_region_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosK8sApplication, "logical_region_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "logicalRegionId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="mountDescs")
     def mount_descs(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosK8sApplication.MountDescsProperty"]]]]:
         '''
         :Property: mountDescs: The description of the NAS mounting configuration. For example, the value can be [{"NasPath": "/k8s","MountPath": "/mnt"}, {"NasPath": "/files", "MountPath": "/app/files"}].
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosK8sApplication.MountDescsProperty"]]]], jsii.get(self, "mountDescs"))
 
     @mount_descs.setter
     def mount_descs(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosK8sApplication.MountDescsProperty"]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosK8sApplication, "mount_descs").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "mountDescs", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="namespace")
     def namespace(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: namespace: The namespace of the Kubernetes cluster. This parameter determines the Kubernetes namespace where your application is deployed. By default, this parameter is set to default.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "namespace"))
 
     @namespace.setter
     def namespace(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosK8sApplication, "namespace").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "namespace", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="nasId")
     def nas_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -3499,34 +3880,40 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "nasId"))
 
     @nas_id.setter
     def nas_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosK8sApplication, "nas_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "nasId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="packageType")
     def package_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: packageType: The type of the deployment package. Valid values: FatJar, WAR, and Image.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "packageType"))
 
     @package_type.setter
     def package_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosK8sApplication, "package_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "packageType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="packageUrl")
     def package_url(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -3537,17 +3924,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "packageUrl"))
 
     @package_url.setter
     def package_url(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosK8sApplication, "package_url").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "packageUrl", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="packageVersion")
     def package_version(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -3557,119 +3947,140 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "packageVersion"))
 
     @package_version.setter
     def package_version(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosK8sApplication, "package_version").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "packageVersion", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="postStart")
     def post_start(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosK8sApplication.PostStartProperty"]]:
         '''
         :Property: postStart: The post-start script. For example, {"Exec": {"Command": ["ls", "/"]}}.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosK8sApplication.PostStartProperty"]], jsii.get(self, "postStart"))
 
     @post_start.setter
     def post_start(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosK8sApplication.PostStartProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosK8sApplication, "post_start").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "postStart", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="preStop")
     def pre_stop(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosK8sApplication.PreStopProperty"]]:
         '''
         :Property: preStop: The pre-stop script. For example, {"Exec": {"Command": ["ls", "/"]}}.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosK8sApplication.PreStopProperty"]], jsii.get(self, "preStop"))
 
     @pre_stop.setter
     def pre_stop(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosK8sApplication.PreStopProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosK8sApplication, "pre_stop").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "preStop", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="readiness")
     def readiness(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosK8sApplication.ReadinessProperty"]]:
         '''
         :Property: readiness: The readiness check on the container.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosK8sApplication.ReadinessProperty"]], jsii.get(self, "readiness"))
 
     @readiness.setter
     def readiness(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosK8sApplication.ReadinessProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosK8sApplication, "readiness").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "readiness", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="replicas")
     def replicas(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: replicas: The number of instances for the application that you want to create. Default: 1
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "replicas"))
 
     @replicas.setter
     def replicas(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosK8sApplication, "replicas").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "replicas", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="repoId")
     def repo_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: repoId: The ID of the image repository.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "repoId"))
 
     @repo_id.setter
     def repo_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosK8sApplication, "repo_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "repoId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="requestsCpu")
     def requests_cpu(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: requestsCpu: The maximum number of CPUs allowed for each application instance when the application is created. Unit: cores. The value 0 indicates no limit.
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "requestsCpu"))
 
     @requests_cpu.setter
     def requests_cpu(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosK8sApplication, "requests_cpu").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "requestsCpu", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="requestsMem")
     def requests_mem(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -3679,85 +4090,100 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "requestsMem"))
 
     @requests_mem.setter
     def requests_mem(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosK8sApplication, "requests_mem").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "requestsMem", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="runtimeClassName")
     def runtime_class_name(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: runtimeClassName: The type of the container runtime. This parameter is applicable only to clusters that use sandboxed containers.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "runtimeClassName"))
 
     @runtime_class_name.setter
     def runtime_class_name(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosK8sApplication, "runtime_class_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "runtimeClassName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="slsConfigs")
     def sls_configs(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosK8sApplication.SlsConfigsProperty"]]]]:
         '''
         :Property: slsConfigs: The Logstore configurations.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosK8sApplication.SlsConfigsProperty"]]]], jsii.get(self, "slsConfigs"))
 
     @sls_configs.setter
     def sls_configs(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosK8sApplication.SlsConfigsProperty"]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosK8sApplication, "sls_configs").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "slsConfigs", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="storageType")
     def storage_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: storageType: Only SSD is supported.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "storageType"))
 
     @storage_type.setter
     def storage_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosK8sApplication, "storage_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "storageType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="timeout")
     def timeout(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: timeout: The timeout interval of the change process. Unit: seconds.
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "timeout"))
 
     @timeout.setter
     def timeout(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosK8sApplication, "timeout").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "timeout", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="uriEncoding")
     def uri_encoding(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -3768,17 +4194,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "uriEncoding"))
 
     @uri_encoding.setter
     def uri_encoding(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosK8sApplication, "uri_encoding").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "uriEncoding", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="useBodyEncoding")
     def use_body_encoding(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -3789,48 +4218,57 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "useBodyEncoding"))
 
     @use_body_encoding.setter
     def use_body_encoding(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosK8sApplication, "use_body_encoding").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "useBodyEncoding", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="webContainer")
     def web_container(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: webContainer: The version of the Tomcat container on which the deployment package of the application depends. This parameter is applicable to Spring Cloud and Apache Dubbo applications that are deployed by using WAR packages. This parameter is not supported when you deploy an application by using images.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "webContainer"))
 
     @web_container.setter
     def web_container(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosK8sApplication, "web_container").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "webContainer", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="webContainerConfig")
     def web_container_config(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosK8sApplication.WebContainerConfigProperty"]]:
         '''
         :Property: webContainerConfig: The Tomcat container configuration.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosK8sApplication.WebContainerConfigProperty"]], jsii.get(self, "webContainerConfig"))
 
     @web_container_config.setter
     def web_container_config(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosK8sApplication.WebContainerConfigProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosK8sApplication, "web_container_config").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "webContainerConfig", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-edas.RosK8sApplication.CommandArgsProperty",
         jsii_struct_bases=[],
         name_mapping={"argument": "argument"},
     )
@@ -3839,14 +4277,17 @@
             self,
             *,
             argument: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param argument: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosK8sApplication.CommandArgsProperty.__init__)
+                check_type(argname="argument argument", value=argument, expected_type=type_hints["argument"])
             self._values: typing.Dict[str, typing.Any] = {}
             if argument is not None:
                 self._values["argument"] = argument
 
         @builtins.property
         def argument(
             self,
@@ -3880,14 +4321,18 @@
             original: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
             startup: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param original: 
             :param startup: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosK8sApplication.ConcGCThreadsProperty.__init__)
+                check_type(argname="argument original", value=original, expected_type=type_hints["original"])
+                check_type(argname="argument startup", value=startup, expected_type=type_hints["startup"])
             self._values: typing.Dict[str, typing.Any] = {}
             if original is not None:
                 self._values["original"] = original
             if startup is not None:
                 self._values["startup"] = startup
 
         @builtins.property
@@ -3933,14 +4378,18 @@
             original: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
             startup: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param original: 
             :param startup: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosK8sApplication.CustomParamsProperty.__init__)
+                check_type(argname="argument original", value=original, expected_type=type_hints["original"])
+                check_type(argname="argument startup", value=startup, expected_type=type_hints["startup"])
             self._values: typing.Dict[str, typing.Any] = {}
             if original is not None:
                 self._values["original"] = original
             if startup is not None:
                 self._values["startup"] = startup
 
         @builtins.property
@@ -3986,14 +4435,18 @@
             name: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
             value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param name: 
             :param value: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosK8sApplication.EnvsProperty.__init__)
+                check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+                check_type(argname="argument value", value=value, expected_type=type_hints["value"])
             self._values: typing.Dict[str, typing.Any] = {}
             if name is not None:
                 self._values["name"] = name
             if value is not None:
                 self._values["value"] = value
 
         @builtins.property
@@ -4037,14 +4490,17 @@
             self,
             *,
             command: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]] = None,
         ) -> None:
             '''
             :param command: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosK8sApplication.ExecProperty.__init__)
+                check_type(argname="argument command", value=command, expected_type=type_hints["command"])
             self._values: typing.Dict[str, typing.Any] = {}
             if command is not None:
                 self._values["command"] = command
 
         @builtins.property
         def command(
             self,
@@ -4078,14 +4534,18 @@
             original: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
             startup: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param original: 
             :param startup: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosK8sApplication.G1HeapRegionSizeProperty.__init__)
+                check_type(argname="argument original", value=original, expected_type=type_hints["original"])
+                check_type(argname="argument startup", value=startup, expected_type=type_hints["startup"])
             self._values: typing.Dict[str, typing.Any] = {}
             if original is not None:
                 self._values["original"] = original
             if startup is not None:
                 self._values["startup"] = startup
 
         @builtins.property
@@ -4131,14 +4591,18 @@
             original: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
             startup: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param original: 
             :param startup: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosK8sApplication.GCLogFilePathProperty.__init__)
+                check_type(argname="argument original", value=original, expected_type=type_hints["original"])
+                check_type(argname="argument startup", value=startup, expected_type=type_hints["startup"])
             self._values: typing.Dict[str, typing.Any] = {}
             if original is not None:
                 self._values["original"] = original
             if startup is not None:
                 self._values["startup"] = startup
 
         @builtins.property
@@ -4184,14 +4648,18 @@
             original: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
             startup: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param original: 
             :param startup: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosK8sApplication.GCLogFileSizeProperty.__init__)
+                check_type(argname="argument original", value=original, expected_type=type_hints["original"])
+                check_type(argname="argument startup", value=startup, expected_type=type_hints["startup"])
             self._values: typing.Dict[str, typing.Any] = {}
             if original is not None:
                 self._values["original"] = original
             if startup is not None:
                 self._values["startup"] = startup
 
         @builtins.property
@@ -4237,14 +4705,18 @@
             original: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
             startup: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param original: 
             :param startup: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosK8sApplication.HeapDumpOnOutOfMemoryErrorProperty.__init__)
+                check_type(argname="argument original", value=original, expected_type=type_hints["original"])
+                check_type(argname="argument startup", value=startup, expected_type=type_hints["startup"])
             self._values: typing.Dict[str, typing.Any] = {}
             if original is not None:
                 self._values["original"] = original
             if startup is not None:
                 self._values["startup"] = startup
 
         @builtins.property
@@ -4290,14 +4762,18 @@
             original: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
             startup: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param original: 
             :param startup: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosK8sApplication.HeapDumpPathProperty.__init__)
+                check_type(argname="argument original", value=original, expected_type=type_hints["original"])
+                check_type(argname="argument startup", value=startup, expected_type=type_hints["startup"])
             self._values: typing.Dict[str, typing.Any] = {}
             if original is not None:
                 self._values["original"] = original
             if startup is not None:
                 self._values["startup"] = startup
 
         @builtins.property
@@ -4343,14 +4819,18 @@
             name: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
             value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param name: 
             :param value: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosK8sApplication.HttpGetHttpHeadersProperty.__init__)
+                check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+                check_type(argname="argument value", value=value, expected_type=type_hints["value"])
             self._values: typing.Dict[str, typing.Any] = {}
             if name is not None:
                 self._values["name"] = name
             if value is not None:
                 self._values["value"] = value
 
         @builtins.property
@@ -4396,26 +4876,33 @@
         },
     )
     class HttpGetProperty:
         def __init__(
             self,
             *,
             host: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-            http_headers: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosK8sApplication.HttpHeadersProperty"]]]] = None,
+            http_headers: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosK8sApplication.HttpHeadersProperty", typing.Dict[str, typing.Any]]]]]] = None,
             path: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
             port: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
             scheme: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param host: 
             :param http_headers: 
             :param path: 
             :param port: 
             :param scheme: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosK8sApplication.HttpGetProperty.__init__)
+                check_type(argname="argument host", value=host, expected_type=type_hints["host"])
+                check_type(argname="argument http_headers", value=http_headers, expected_type=type_hints["http_headers"])
+                check_type(argname="argument path", value=path, expected_type=type_hints["path"])
+                check_type(argname="argument port", value=port, expected_type=type_hints["port"])
+                check_type(argname="argument scheme", value=scheme, expected_type=type_hints["scheme"])
             self._values: typing.Dict[str, typing.Any] = {}
             if host is not None:
                 self._values["host"] = host
             if http_headers is not None:
                 self._values["http_headers"] = http_headers
             if path is not None:
                 self._values["path"] = path
@@ -4497,14 +4984,18 @@
             name: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
             value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param name: 
             :param value: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosK8sApplication.HttpHeadersProperty.__init__)
+                check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+                check_type(argname="argument value", value=value, expected_type=type_hints["value"])
             self._values: typing.Dict[str, typing.Any] = {}
             if name is not None:
                 self._values["name"] = name
             if value is not None:
                 self._values["value"] = value
 
         @builtins.property
@@ -4550,14 +5041,18 @@
             original: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
             startup: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param original: 
             :param startup: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosK8sApplication.InitialHeapSizeProperty.__init__)
+                check_type(argname="argument original", value=original, expected_type=type_hints["original"])
+                check_type(argname="argument startup", value=startup, expected_type=type_hints["startup"])
             self._values: typing.Dict[str, typing.Any] = {}
             if original is not None:
                 self._values["original"] = original
             if startup is not None:
                 self._values["startup"] = startup
 
         @builtins.property
@@ -4622,39 +5117,39 @@
             "young_garbage_collector": "youngGarbageCollector",
         },
     )
     class JavaStartUpConfigProperty:
         def __init__(
             self,
             *,
-            conc_gc_threads: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosK8sApplication.ConcGCThreadsProperty"]] = None,
-            custom_params: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosK8sApplication.CustomParamsProperty"]] = None,
-            g1_heap_region_size: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosK8sApplication.G1HeapRegionSizeProperty"]] = None,
-            gc_log_file_path: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosK8sApplication.GCLogFilePathProperty"]] = None,
-            gc_log_file_size: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosK8sApplication.GCLogFileSizeProperty"]] = None,
-            heap_dump_on_out_of_memory_error: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosK8sApplication.HeapDumpOnOutOfMemoryErrorProperty"]] = None,
-            heap_dump_path: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosK8sApplication.HeapDumpPathProperty"]] = None,
-            initial_heap_size: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosK8sApplication.InitialHeapSizeProperty"]] = None,
-            max_direct_memory_size: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosK8sApplication.MaxDirectMemorySizeProperty"]] = None,
-            max_heap_size: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosK8sApplication.MaxHeapSizeProperty"]] = None,
-            max_new_size: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosK8sApplication.MaxNewSizeProperty"]] = None,
-            max_perm_size: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosK8sApplication.MaxPermSizeProperty"]] = None,
-            nacos_use_cloud_namespace_parsing: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosK8sApplication.NacosUseCloudNamespaceParsingProperty"]] = None,
-            nacos_use_endpoint_parsing_rule: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosK8sApplication.NacosUseEndpointParsingRuleProperty"]] = None,
-            new_ratio: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosK8sApplication.NewRatioProperty"]] = None,
-            new_size: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosK8sApplication.NewSizeProperty"]] = None,
-            old_garbage_collector: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosK8sApplication.OldGarbageCollectorProperty"]] = None,
-            parallel_gc_threads: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosK8sApplication.ParallelGCThreadsProperty"]] = None,
-            perm_size: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosK8sApplication.PermSizeProperty"]] = None,
-            print_gc: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosK8sApplication.PrintGCProperty"]] = None,
-            print_gc_date_stamps: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosK8sApplication.PrintGCDateStampsProperty"]] = None,
-            survivor_ratio: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosK8sApplication.SurvivorRatioProperty"]] = None,
-            thread_stack_size: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosK8sApplication.ThreadStackSizeProperty"]] = None,
-            use_gc_log_file_rotation: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosK8sApplication.UseGCLogFileRotationProperty"]] = None,
-            young_garbage_collector: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosK8sApplication.YoungGarbageCollectorProperty"]] = None,
+            conc_gc_threads: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosK8sApplication.ConcGCThreadsProperty", typing.Dict[str, typing.Any]]]] = None,
+            custom_params: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosK8sApplication.CustomParamsProperty", typing.Dict[str, typing.Any]]]] = None,
+            g1_heap_region_size: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosK8sApplication.G1HeapRegionSizeProperty", typing.Dict[str, typing.Any]]]] = None,
+            gc_log_file_path: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosK8sApplication.GCLogFilePathProperty", typing.Dict[str, typing.Any]]]] = None,
+            gc_log_file_size: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosK8sApplication.GCLogFileSizeProperty", typing.Dict[str, typing.Any]]]] = None,
+            heap_dump_on_out_of_memory_error: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosK8sApplication.HeapDumpOnOutOfMemoryErrorProperty", typing.Dict[str, typing.Any]]]] = None,
+            heap_dump_path: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosK8sApplication.HeapDumpPathProperty", typing.Dict[str, typing.Any]]]] = None,
+            initial_heap_size: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosK8sApplication.InitialHeapSizeProperty", typing.Dict[str, typing.Any]]]] = None,
+            max_direct_memory_size: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosK8sApplication.MaxDirectMemorySizeProperty", typing.Dict[str, typing.Any]]]] = None,
+            max_heap_size: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosK8sApplication.MaxHeapSizeProperty", typing.Dict[str, typing.Any]]]] = None,
+            max_new_size: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosK8sApplication.MaxNewSizeProperty", typing.Dict[str, typing.Any]]]] = None,
+            max_perm_size: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosK8sApplication.MaxPermSizeProperty", typing.Dict[str, typing.Any]]]] = None,
+            nacos_use_cloud_namespace_parsing: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosK8sApplication.NacosUseCloudNamespaceParsingProperty", typing.Dict[str, typing.Any]]]] = None,
+            nacos_use_endpoint_parsing_rule: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosK8sApplication.NacosUseEndpointParsingRuleProperty", typing.Dict[str, typing.Any]]]] = None,
+            new_ratio: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosK8sApplication.NewRatioProperty", typing.Dict[str, typing.Any]]]] = None,
+            new_size: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosK8sApplication.NewSizeProperty", typing.Dict[str, typing.Any]]]] = None,
+            old_garbage_collector: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosK8sApplication.OldGarbageCollectorProperty", typing.Dict[str, typing.Any]]]] = None,
+            parallel_gc_threads: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosK8sApplication.ParallelGCThreadsProperty", typing.Dict[str, typing.Any]]]] = None,
+            perm_size: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosK8sApplication.PermSizeProperty", typing.Dict[str, typing.Any]]]] = None,
+            print_gc: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosK8sApplication.PrintGCProperty", typing.Dict[str, typing.Any]]]] = None,
+            print_gc_date_stamps: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosK8sApplication.PrintGCDateStampsProperty", typing.Dict[str, typing.Any]]]] = None,
+            survivor_ratio: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosK8sApplication.SurvivorRatioProperty", typing.Dict[str, typing.Any]]]] = None,
+            thread_stack_size: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosK8sApplication.ThreadStackSizeProperty", typing.Dict[str, typing.Any]]]] = None,
+            use_gc_log_file_rotation: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosK8sApplication.UseGCLogFileRotationProperty", typing.Dict[str, typing.Any]]]] = None,
+            young_garbage_collector: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosK8sApplication.YoungGarbageCollectorProperty", typing.Dict[str, typing.Any]]]] = None,
         ) -> None:
             '''
             :param conc_gc_threads: 
             :param custom_params: 
             :param g1_heap_region_size: 
             :param gc_log_file_path: 
             :param gc_log_file_size: 
@@ -4675,14 +5170,41 @@
             :param print_gc: 
             :param print_gc_date_stamps: 
             :param survivor_ratio: 
             :param thread_stack_size: 
             :param use_gc_log_file_rotation: 
             :param young_garbage_collector: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosK8sApplication.JavaStartUpConfigProperty.__init__)
+                check_type(argname="argument conc_gc_threads", value=conc_gc_threads, expected_type=type_hints["conc_gc_threads"])
+                check_type(argname="argument custom_params", value=custom_params, expected_type=type_hints["custom_params"])
+                check_type(argname="argument g1_heap_region_size", value=g1_heap_region_size, expected_type=type_hints["g1_heap_region_size"])
+                check_type(argname="argument gc_log_file_path", value=gc_log_file_path, expected_type=type_hints["gc_log_file_path"])
+                check_type(argname="argument gc_log_file_size", value=gc_log_file_size, expected_type=type_hints["gc_log_file_size"])
+                check_type(argname="argument heap_dump_on_out_of_memory_error", value=heap_dump_on_out_of_memory_error, expected_type=type_hints["heap_dump_on_out_of_memory_error"])
+                check_type(argname="argument heap_dump_path", value=heap_dump_path, expected_type=type_hints["heap_dump_path"])
+                check_type(argname="argument initial_heap_size", value=initial_heap_size, expected_type=type_hints["initial_heap_size"])
+                check_type(argname="argument max_direct_memory_size", value=max_direct_memory_size, expected_type=type_hints["max_direct_memory_size"])
+                check_type(argname="argument max_heap_size", value=max_heap_size, expected_type=type_hints["max_heap_size"])
+                check_type(argname="argument max_new_size", value=max_new_size, expected_type=type_hints["max_new_size"])
+                check_type(argname="argument max_perm_size", value=max_perm_size, expected_type=type_hints["max_perm_size"])
+                check_type(argname="argument nacos_use_cloud_namespace_parsing", value=nacos_use_cloud_namespace_parsing, expected_type=type_hints["nacos_use_cloud_namespace_parsing"])
+                check_type(argname="argument nacos_use_endpoint_parsing_rule", value=nacos_use_endpoint_parsing_rule, expected_type=type_hints["nacos_use_endpoint_parsing_rule"])
+                check_type(argname="argument new_ratio", value=new_ratio, expected_type=type_hints["new_ratio"])
+                check_type(argname="argument new_size", value=new_size, expected_type=type_hints["new_size"])
+                check_type(argname="argument old_garbage_collector", value=old_garbage_collector, expected_type=type_hints["old_garbage_collector"])
+                check_type(argname="argument parallel_gc_threads", value=parallel_gc_threads, expected_type=type_hints["parallel_gc_threads"])
+                check_type(argname="argument perm_size", value=perm_size, expected_type=type_hints["perm_size"])
+                check_type(argname="argument print_gc", value=print_gc, expected_type=type_hints["print_gc"])
+                check_type(argname="argument print_gc_date_stamps", value=print_gc_date_stamps, expected_type=type_hints["print_gc_date_stamps"])
+                check_type(argname="argument survivor_ratio", value=survivor_ratio, expected_type=type_hints["survivor_ratio"])
+                check_type(argname="argument thread_stack_size", value=thread_stack_size, expected_type=type_hints["thread_stack_size"])
+                check_type(argname="argument use_gc_log_file_rotation", value=use_gc_log_file_rotation, expected_type=type_hints["use_gc_log_file_rotation"])
+                check_type(argname="argument young_garbage_collector", value=young_garbage_collector, expected_type=type_hints["young_garbage_collector"])
             self._values: typing.Dict[str, typing.Any] = {}
             if conc_gc_threads is not None:
                 self._values["conc_gc_threads"] = conc_gc_threads
             if custom_params is not None:
                 self._values["custom_params"] = custom_params
             if g1_heap_region_size is not None:
                 self._values["g1_heap_region_size"] = g1_heap_region_size
@@ -5006,33 +5528,43 @@
             "timeout_seconds": "timeoutSeconds",
         },
     )
     class LivenessProperty:
         def __init__(
             self,
             *,
-            exec: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosK8sApplication.ExecProperty"]] = None,
+            exec: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosK8sApplication.ExecProperty", typing.Dict[str, typing.Any]]]] = None,
             failure_threshold: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
-            http_get: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosK8sApplication.HttpGetProperty"]] = None,
+            http_get: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosK8sApplication.HttpGetProperty", typing.Dict[str, typing.Any]]]] = None,
             initial_delay_seconds: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
             period_seconds: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
             success_threshold: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
-            tcp_socket: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosK8sApplication.TcpSocketProperty"]] = None,
+            tcp_socket: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosK8sApplication.TcpSocketProperty", typing.Dict[str, typing.Any]]]] = None,
             timeout_seconds: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param exec: 
             :param failure_threshold: 
             :param http_get: 
             :param initial_delay_seconds: 
             :param period_seconds: 
             :param success_threshold: 
             :param tcp_socket: 
             :param timeout_seconds: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosK8sApplication.LivenessProperty.__init__)
+                check_type(argname="argument exec", value=exec, expected_type=type_hints["exec"])
+                check_type(argname="argument failure_threshold", value=failure_threshold, expected_type=type_hints["failure_threshold"])
+                check_type(argname="argument http_get", value=http_get, expected_type=type_hints["http_get"])
+                check_type(argname="argument initial_delay_seconds", value=initial_delay_seconds, expected_type=type_hints["initial_delay_seconds"])
+                check_type(argname="argument period_seconds", value=period_seconds, expected_type=type_hints["period_seconds"])
+                check_type(argname="argument success_threshold", value=success_threshold, expected_type=type_hints["success_threshold"])
+                check_type(argname="argument tcp_socket", value=tcp_socket, expected_type=type_hints["tcp_socket"])
+                check_type(argname="argument timeout_seconds", value=timeout_seconds, expected_type=type_hints["timeout_seconds"])
             self._values: typing.Dict[str, typing.Any] = {}
             if exec is not None:
                 self._values["exec"] = exec
             if failure_threshold is not None:
                 self._values["failure_threshold"] = failure_threshold
             if http_get is not None:
                 self._values["http_get"] = http_get
@@ -5156,14 +5688,19 @@
             type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param mount_path: 
             :param node_path: 
             :param type: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosK8sApplication.LocalVolumeProperty.__init__)
+                check_type(argname="argument mount_path", value=mount_path, expected_type=type_hints["mount_path"])
+                check_type(argname="argument node_path", value=node_path, expected_type=type_hints["node_path"])
+                check_type(argname="argument type", value=type, expected_type=type_hints["type"])
             self._values: typing.Dict[str, typing.Any] = {}
             if mount_path is not None:
                 self._values["mount_path"] = mount_path
             if node_path is not None:
                 self._values["node_path"] = node_path
             if type is not None:
                 self._values["type"] = type
@@ -5221,14 +5758,18 @@
             original: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
             startup: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param original: 
             :param startup: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosK8sApplication.MaxDirectMemorySizeProperty.__init__)
+                check_type(argname="argument original", value=original, expected_type=type_hints["original"])
+                check_type(argname="argument startup", value=startup, expected_type=type_hints["startup"])
             self._values: typing.Dict[str, typing.Any] = {}
             if original is not None:
                 self._values["original"] = original
             if startup is not None:
                 self._values["startup"] = startup
 
         @builtins.property
@@ -5274,14 +5815,18 @@
             original: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
             startup: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param original: 
             :param startup: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosK8sApplication.MaxHeapSizeProperty.__init__)
+                check_type(argname="argument original", value=original, expected_type=type_hints["original"])
+                check_type(argname="argument startup", value=startup, expected_type=type_hints["startup"])
             self._values: typing.Dict[str, typing.Any] = {}
             if original is not None:
                 self._values["original"] = original
             if startup is not None:
                 self._values["startup"] = startup
 
         @builtins.property
@@ -5327,14 +5872,18 @@
             original: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
             startup: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param original: 
             :param startup: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosK8sApplication.MaxNewSizeProperty.__init__)
+                check_type(argname="argument original", value=original, expected_type=type_hints["original"])
+                check_type(argname="argument startup", value=startup, expected_type=type_hints["startup"])
             self._values: typing.Dict[str, typing.Any] = {}
             if original is not None:
                 self._values["original"] = original
             if startup is not None:
                 self._values["startup"] = startup
 
         @builtins.property
@@ -5380,14 +5929,18 @@
             original: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
             startup: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param original: 
             :param startup: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosK8sApplication.MaxPermSizeProperty.__init__)
+                check_type(argname="argument original", value=original, expected_type=type_hints["original"])
+                check_type(argname="argument startup", value=startup, expected_type=type_hints["startup"])
             self._values: typing.Dict[str, typing.Any] = {}
             if original is not None:
                 self._values["original"] = original
             if startup is not None:
                 self._values["startup"] = startup
 
         @builtins.property
@@ -5433,14 +5986,18 @@
             mount_path: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
             nas_path: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param mount_path: 
             :param nas_path: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosK8sApplication.MountDescsProperty.__init__)
+                check_type(argname="argument mount_path", value=mount_path, expected_type=type_hints["mount_path"])
+                check_type(argname="argument nas_path", value=nas_path, expected_type=type_hints["nas_path"])
             self._values: typing.Dict[str, typing.Any] = {}
             if mount_path is not None:
                 self._values["mount_path"] = mount_path
             if nas_path is not None:
                 self._values["nas_path"] = nas_path
 
         @builtins.property
@@ -5486,14 +6043,18 @@
             original: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
             startup: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param original: 
             :param startup: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosK8sApplication.NacosUseCloudNamespaceParsingProperty.__init__)
+                check_type(argname="argument original", value=original, expected_type=type_hints["original"])
+                check_type(argname="argument startup", value=startup, expected_type=type_hints["startup"])
             self._values: typing.Dict[str, typing.Any] = {}
             if original is not None:
                 self._values["original"] = original
             if startup is not None:
                 self._values["startup"] = startup
 
         @builtins.property
@@ -5539,14 +6100,18 @@
             original: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
             startup: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param original: 
             :param startup: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosK8sApplication.NacosUseEndpointParsingRuleProperty.__init__)
+                check_type(argname="argument original", value=original, expected_type=type_hints["original"])
+                check_type(argname="argument startup", value=startup, expected_type=type_hints["startup"])
             self._values: typing.Dict[str, typing.Any] = {}
             if original is not None:
                 self._values["original"] = original
             if startup is not None:
                 self._values["startup"] = startup
 
         @builtins.property
@@ -5592,14 +6157,18 @@
             original: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
             startup: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param original: 
             :param startup: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosK8sApplication.NewRatioProperty.__init__)
+                check_type(argname="argument original", value=original, expected_type=type_hints["original"])
+                check_type(argname="argument startup", value=startup, expected_type=type_hints["startup"])
             self._values: typing.Dict[str, typing.Any] = {}
             if original is not None:
                 self._values["original"] = original
             if startup is not None:
                 self._values["startup"] = startup
 
         @builtins.property
@@ -5645,14 +6214,18 @@
             original: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
             startup: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param original: 
             :param startup: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosK8sApplication.NewSizeProperty.__init__)
+                check_type(argname="argument original", value=original, expected_type=type_hints["original"])
+                check_type(argname="argument startup", value=startup, expected_type=type_hints["startup"])
             self._values: typing.Dict[str, typing.Any] = {}
             if original is not None:
                 self._values["original"] = original
             if startup is not None:
                 self._values["startup"] = startup
 
         @builtins.property
@@ -5698,14 +6271,18 @@
             original: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
             startup: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param original: 
             :param startup: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosK8sApplication.OldGarbageCollectorProperty.__init__)
+                check_type(argname="argument original", value=original, expected_type=type_hints["original"])
+                check_type(argname="argument startup", value=startup, expected_type=type_hints["startup"])
             self._values: typing.Dict[str, typing.Any] = {}
             if original is not None:
                 self._values["original"] = original
             if startup is not None:
                 self._values["startup"] = startup
 
         @builtins.property
@@ -5751,14 +6328,18 @@
             original: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
             startup: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param original: 
             :param startup: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosK8sApplication.ParallelGCThreadsProperty.__init__)
+                check_type(argname="argument original", value=original, expected_type=type_hints["original"])
+                check_type(argname="argument startup", value=startup, expected_type=type_hints["startup"])
             self._values: typing.Dict[str, typing.Any] = {}
             if original is not None:
                 self._values["original"] = original
             if startup is not None:
                 self._values["startup"] = startup
 
         @builtins.property
@@ -5804,14 +6385,18 @@
             original: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
             startup: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param original: 
             :param startup: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosK8sApplication.PermSizeProperty.__init__)
+                check_type(argname="argument original", value=original, expected_type=type_hints["original"])
+                check_type(argname="argument startup", value=startup, expected_type=type_hints["startup"])
             self._values: typing.Dict[str, typing.Any] = {}
             if original is not None:
                 self._values["original"] = original
             if startup is not None:
                 self._values["startup"] = startup
 
         @builtins.property
@@ -5855,14 +6440,17 @@
             self,
             *,
             command: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]] = None,
         ) -> None:
             '''
             :param command: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosK8sApplication.PostStartExecProperty.__init__)
+                check_type(argname="argument command", value=command, expected_type=type_hints["command"])
             self._values: typing.Dict[str, typing.Any] = {}
             if command is not None:
                 self._values["command"] = command
 
         @builtins.property
         def command(
             self,
@@ -5896,26 +6484,33 @@
         },
     )
     class PostStartHttpGetProperty:
         def __init__(
             self,
             *,
             host: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-            http_headers: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosK8sApplication.HttpGetHttpHeadersProperty"]]]] = None,
+            http_headers: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosK8sApplication.HttpGetHttpHeadersProperty", typing.Dict[str, typing.Any]]]]]] = None,
             path: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
             port: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
             scheme: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param host: 
             :param http_headers: 
             :param path: 
             :param port: 
             :param scheme: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosK8sApplication.PostStartHttpGetProperty.__init__)
+                check_type(argname="argument host", value=host, expected_type=type_hints["host"])
+                check_type(argname="argument http_headers", value=http_headers, expected_type=type_hints["http_headers"])
+                check_type(argname="argument path", value=path, expected_type=type_hints["path"])
+                check_type(argname="argument port", value=port, expected_type=type_hints["port"])
+                check_type(argname="argument scheme", value=scheme, expected_type=type_hints["scheme"])
             self._values: typing.Dict[str, typing.Any] = {}
             if host is not None:
                 self._values["host"] = host
             if http_headers is not None:
                 self._values["http_headers"] = http_headers
             if path is not None:
                 self._values["path"] = path
@@ -5990,21 +6585,25 @@
         jsii_struct_bases=[],
         name_mapping={"exec": "exec", "http_get": "httpGet"},
     )
     class PostStartProperty:
         def __init__(
             self,
             *,
-            exec: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosK8sApplication.PostStartExecProperty"]] = None,
-            http_get: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosK8sApplication.PostStartHttpGetProperty"]] = None,
+            exec: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosK8sApplication.PostStartExecProperty", typing.Dict[str, typing.Any]]]] = None,
+            http_get: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosK8sApplication.PostStartHttpGetProperty", typing.Dict[str, typing.Any]]]] = None,
         ) -> None:
             '''
             :param exec: 
             :param http_get: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosK8sApplication.PostStartProperty.__init__)
+                check_type(argname="argument exec", value=exec, expected_type=type_hints["exec"])
+                check_type(argname="argument http_get", value=http_get, expected_type=type_hints["http_get"])
             self._values: typing.Dict[str, typing.Any] = {}
             if exec is not None:
                 self._values["exec"] = exec
             if http_get is not None:
                 self._values["http_get"] = http_get
 
         @builtins.property
@@ -6048,14 +6647,17 @@
             self,
             *,
             command: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]] = None,
         ) -> None:
             '''
             :param command: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosK8sApplication.PreStopExecProperty.__init__)
+                check_type(argname="argument command", value=command, expected_type=type_hints["command"])
             self._values: typing.Dict[str, typing.Any] = {}
             if command is not None:
                 self._values["command"] = command
 
         @builtins.property
         def command(
             self,
@@ -6089,14 +6691,18 @@
             name: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
             value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param name: 
             :param value: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosK8sApplication.PreStopHttpGetHttpHeadersProperty.__init__)
+                check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+                check_type(argname="argument value", value=value, expected_type=type_hints["value"])
             self._values: typing.Dict[str, typing.Any] = {}
             if name is not None:
                 self._values["name"] = name
             if value is not None:
                 self._values["value"] = value
 
         @builtins.property
@@ -6142,26 +6748,33 @@
         },
     )
     class PreStopHttpGetProperty:
         def __init__(
             self,
             *,
             host: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-            http_headers: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosK8sApplication.PreStopHttpGetHttpHeadersProperty"]]]] = None,
+            http_headers: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosK8sApplication.PreStopHttpGetHttpHeadersProperty", typing.Dict[str, typing.Any]]]]]] = None,
             path: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
             port: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
             scheme: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param host: 
             :param http_headers: 
             :param path: 
             :param port: 
             :param scheme: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosK8sApplication.PreStopHttpGetProperty.__init__)
+                check_type(argname="argument host", value=host, expected_type=type_hints["host"])
+                check_type(argname="argument http_headers", value=http_headers, expected_type=type_hints["http_headers"])
+                check_type(argname="argument path", value=path, expected_type=type_hints["path"])
+                check_type(argname="argument port", value=port, expected_type=type_hints["port"])
+                check_type(argname="argument scheme", value=scheme, expected_type=type_hints["scheme"])
             self._values: typing.Dict[str, typing.Any] = {}
             if host is not None:
                 self._values["host"] = host
             if http_headers is not None:
                 self._values["http_headers"] = http_headers
             if path is not None:
                 self._values["path"] = path
@@ -6236,21 +6849,25 @@
         jsii_struct_bases=[],
         name_mapping={"exec": "exec", "http_get": "httpGet"},
     )
     class PreStopProperty:
         def __init__(
             self,
             *,
-            exec: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosK8sApplication.PreStopExecProperty"]] = None,
-            http_get: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosK8sApplication.PreStopHttpGetProperty"]] = None,
+            exec: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosK8sApplication.PreStopExecProperty", typing.Dict[str, typing.Any]]]] = None,
+            http_get: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosK8sApplication.PreStopHttpGetProperty", typing.Dict[str, typing.Any]]]] = None,
         ) -> None:
             '''
             :param exec: 
             :param http_get: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosK8sApplication.PreStopProperty.__init__)
+                check_type(argname="argument exec", value=exec, expected_type=type_hints["exec"])
+                check_type(argname="argument http_get", value=http_get, expected_type=type_hints["http_get"])
             self._values: typing.Dict[str, typing.Any] = {}
             if exec is not None:
                 self._values["exec"] = exec
             if http_get is not None:
                 self._values["http_get"] = http_get
 
         @builtins.property
@@ -6296,14 +6913,18 @@
             original: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
             startup: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param original: 
             :param startup: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosK8sApplication.PrintGCDateStampsProperty.__init__)
+                check_type(argname="argument original", value=original, expected_type=type_hints["original"])
+                check_type(argname="argument startup", value=startup, expected_type=type_hints["startup"])
             self._values: typing.Dict[str, typing.Any] = {}
             if original is not None:
                 self._values["original"] = original
             if startup is not None:
                 self._values["startup"] = startup
 
         @builtins.property
@@ -6349,14 +6970,18 @@
             original: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
             startup: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param original: 
             :param startup: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosK8sApplication.PrintGCProperty.__init__)
+                check_type(argname="argument original", value=original, expected_type=type_hints["original"])
+                check_type(argname="argument startup", value=startup, expected_type=type_hints["startup"])
             self._values: typing.Dict[str, typing.Any] = {}
             if original is not None:
                 self._values["original"] = original
             if startup is not None:
                 self._values["startup"] = startup
 
         @builtins.property
@@ -6400,14 +7025,17 @@
             self,
             *,
             command: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]] = None,
         ) -> None:
             '''
             :param command: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosK8sApplication.ReadinessExecProperty.__init__)
+                check_type(argname="argument command", value=command, expected_type=type_hints["command"])
             self._values: typing.Dict[str, typing.Any] = {}
             if command is not None:
                 self._values["command"] = command
 
         @builtins.property
         def command(
             self,
@@ -6441,14 +7069,18 @@
             name: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
             value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param name: 
             :param value: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosK8sApplication.ReadinessHttpGetHttpHeadersProperty.__init__)
+                check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+                check_type(argname="argument value", value=value, expected_type=type_hints["value"])
             self._values: typing.Dict[str, typing.Any] = {}
             if name is not None:
                 self._values["name"] = name
             if value is not None:
                 self._values["value"] = value
 
         @builtins.property
@@ -6494,26 +7126,33 @@
         },
     )
     class ReadinessHttpGetProperty:
         def __init__(
             self,
             *,
             host: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-            http_headers: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosK8sApplication.ReadinessHttpGetHttpHeadersProperty"]]]] = None,
+            http_headers: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosK8sApplication.ReadinessHttpGetHttpHeadersProperty", typing.Dict[str, typing.Any]]]]]] = None,
             path: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
             port: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
             scheme: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param host: 
             :param http_headers: 
             :param path: 
             :param port: 
             :param scheme: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosK8sApplication.ReadinessHttpGetProperty.__init__)
+                check_type(argname="argument host", value=host, expected_type=type_hints["host"])
+                check_type(argname="argument http_headers", value=http_headers, expected_type=type_hints["http_headers"])
+                check_type(argname="argument path", value=path, expected_type=type_hints["path"])
+                check_type(argname="argument port", value=port, expected_type=type_hints["port"])
+                check_type(argname="argument scheme", value=scheme, expected_type=type_hints["scheme"])
             self._values: typing.Dict[str, typing.Any] = {}
             if host is not None:
                 self._values["host"] = host
             if http_headers is not None:
                 self._values["http_headers"] = http_headers
             if path is not None:
                 self._values["path"] = path
@@ -6597,33 +7236,43 @@
             "timeout_seconds": "timeoutSeconds",
         },
     )
     class ReadinessProperty:
         def __init__(
             self,
             *,
-            exec: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosK8sApplication.ReadinessExecProperty"]] = None,
+            exec: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosK8sApplication.ReadinessExecProperty", typing.Dict[str, typing.Any]]]] = None,
             failure_threshold: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
-            http_get: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosK8sApplication.ReadinessHttpGetProperty"]] = None,
+            http_get: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosK8sApplication.ReadinessHttpGetProperty", typing.Dict[str, typing.Any]]]] = None,
             initial_delay_seconds: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
             period_seconds: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
             success_threshold: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
-            tcp_socket: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosK8sApplication.ReadinessTcpSocketProperty"]] = None,
+            tcp_socket: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosK8sApplication.ReadinessTcpSocketProperty", typing.Dict[str, typing.Any]]]] = None,
             timeout_seconds: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param exec: 
             :param failure_threshold: 
             :param http_get: 
             :param initial_delay_seconds: 
             :param period_seconds: 
             :param success_threshold: 
             :param tcp_socket: 
             :param timeout_seconds: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosK8sApplication.ReadinessProperty.__init__)
+                check_type(argname="argument exec", value=exec, expected_type=type_hints["exec"])
+                check_type(argname="argument failure_threshold", value=failure_threshold, expected_type=type_hints["failure_threshold"])
+                check_type(argname="argument http_get", value=http_get, expected_type=type_hints["http_get"])
+                check_type(argname="argument initial_delay_seconds", value=initial_delay_seconds, expected_type=type_hints["initial_delay_seconds"])
+                check_type(argname="argument period_seconds", value=period_seconds, expected_type=type_hints["period_seconds"])
+                check_type(argname="argument success_threshold", value=success_threshold, expected_type=type_hints["success_threshold"])
+                check_type(argname="argument tcp_socket", value=tcp_socket, expected_type=type_hints["tcp_socket"])
+                check_type(argname="argument timeout_seconds", value=timeout_seconds, expected_type=type_hints["timeout_seconds"])
             self._values: typing.Dict[str, typing.Any] = {}
             if exec is not None:
                 self._values["exec"] = exec
             if failure_threshold is not None:
                 self._values["failure_threshold"] = failure_threshold
             if http_get is not None:
                 self._values["http_get"] = http_get
@@ -6741,14 +7390,18 @@
             host: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
             port: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param host: 
             :param port: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosK8sApplication.ReadinessTcpSocketProperty.__init__)
+                check_type(argname="argument host", value=host, expected_type=type_hints["host"])
+                check_type(argname="argument port", value=port, expected_type=type_hints["port"])
             self._values: typing.Dict[str, typing.Any] = {}
             if host is not None:
                 self._values["host"] = host
             if port is not None:
                 self._values["port"] = port
 
         @builtins.property
@@ -6796,14 +7449,19 @@
             type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param log_dir: 
             :param logstore: 
             :param type: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosK8sApplication.SlsConfigsProperty.__init__)
+                check_type(argname="argument log_dir", value=log_dir, expected_type=type_hints["log_dir"])
+                check_type(argname="argument logstore", value=logstore, expected_type=type_hints["logstore"])
+                check_type(argname="argument type", value=type, expected_type=type_hints["type"])
             self._values: typing.Dict[str, typing.Any] = {}
             if log_dir is not None:
                 self._values["log_dir"] = log_dir
             if logstore is not None:
                 self._values["logstore"] = logstore
             if type is not None:
                 self._values["type"] = type
@@ -6868,14 +7526,18 @@
             original: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
             startup: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param original: 
             :param startup: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosK8sApplication.SurvivorRatioProperty.__init__)
+                check_type(argname="argument original", value=original, expected_type=type_hints["original"])
+                check_type(argname="argument startup", value=startup, expected_type=type_hints["startup"])
             self._values: typing.Dict[str, typing.Any] = {}
             if original is not None:
                 self._values["original"] = original
             if startup is not None:
                 self._values["startup"] = startup
 
         @builtins.property
@@ -6921,14 +7583,18 @@
             host: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
             port: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param host: 
             :param port: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosK8sApplication.TcpSocketProperty.__init__)
+                check_type(argname="argument host", value=host, expected_type=type_hints["host"])
+                check_type(argname="argument port", value=port, expected_type=type_hints["port"])
             self._values: typing.Dict[str, typing.Any] = {}
             if host is not None:
                 self._values["host"] = host
             if port is not None:
                 self._values["port"] = port
 
         @builtins.property
@@ -6974,14 +7640,18 @@
             original: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
             startup: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param original: 
             :param startup: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosK8sApplication.ThreadStackSizeProperty.__init__)
+                check_type(argname="argument original", value=original, expected_type=type_hints["original"])
+                check_type(argname="argument startup", value=startup, expected_type=type_hints["startup"])
             self._values: typing.Dict[str, typing.Any] = {}
             if original is not None:
                 self._values["original"] = original
             if startup is not None:
                 self._values["startup"] = startup
 
         @builtins.property
@@ -7027,14 +7697,18 @@
             original: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
             startup: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param original: 
             :param startup: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosK8sApplication.UseGCLogFileRotationProperty.__init__)
+                check_type(argname="argument original", value=original, expected_type=type_hints["original"])
+                check_type(argname="argument startup", value=startup, expected_type=type_hints["startup"])
             self._values: typing.Dict[str, typing.Any] = {}
             if original is not None:
                 self._values["original"] = original
             if startup is not None:
                 self._values["startup"] = startup
 
         @builtins.property
@@ -7104,14 +7778,25 @@
             :param max_threads: 
             :param server_xml: 
             :param uri_encoding: 
             :param use_advanced_server_xml: 
             :param use_body_encoding: 
             :param use_default_config: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosK8sApplication.WebContainerConfigProperty.__init__)
+                check_type(argname="argument context_input_type", value=context_input_type, expected_type=type_hints["context_input_type"])
+                check_type(argname="argument context_path", value=context_path, expected_type=type_hints["context_path"])
+                check_type(argname="argument http_port", value=http_port, expected_type=type_hints["http_port"])
+                check_type(argname="argument max_threads", value=max_threads, expected_type=type_hints["max_threads"])
+                check_type(argname="argument server_xml", value=server_xml, expected_type=type_hints["server_xml"])
+                check_type(argname="argument uri_encoding", value=uri_encoding, expected_type=type_hints["uri_encoding"])
+                check_type(argname="argument use_advanced_server_xml", value=use_advanced_server_xml, expected_type=type_hints["use_advanced_server_xml"])
+                check_type(argname="argument use_body_encoding", value=use_body_encoding, expected_type=type_hints["use_body_encoding"])
+                check_type(argname="argument use_default_config", value=use_default_config, expected_type=type_hints["use_default_config"])
             self._values: typing.Dict[str, typing.Any] = {}
             if context_input_type is not None:
                 self._values["context_input_type"] = context_input_type
             if context_path is not None:
                 self._values["context_path"] = context_path
             if http_port is not None:
                 self._values["http_port"] = http_port
@@ -7252,14 +7937,18 @@
             original: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
             startup: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param original: 
             :param startup: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosK8sApplication.YoungGarbageCollectorProperty.__init__)
+                check_type(argname="argument original", value=original, expected_type=type_hints["original"])
+                check_type(argname="argument startup", value=startup, expected_type=type_hints["startup"])
             self._values: typing.Dict[str, typing.Any] = {}
             if original is not None:
                 self._values["original"] = original
             if startup is not None:
                 self._values["startup"] = startup
 
         @builtins.property
@@ -7352,58 +8041,58 @@
     def __init__(
         self,
         *,
         app_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         cluster_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         application_description: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         command: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        command_args: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosK8sApplication.CommandArgsProperty]]]] = None,
+        command_args: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosK8sApplication.CommandArgsProperty, typing.Dict[str, typing.Any]]]]]] = None,
         deploy_across_nodes: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         deploy_across_zones: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         edas_container_version: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         enable_ahas: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
-        envs: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosK8sApplication.EnvsProperty]]]] = None,
+        envs: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosK8sApplication.EnvsProperty, typing.Dict[str, typing.Any]]]]]] = None,
         image_url: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         internet_slb_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         internet_slb_port: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         internet_slb_protocol: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         internet_target_port: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         intranet_slb_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         intranet_slb_port: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         intranet_slb_protocol: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         intranet_target_port: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         is_multilingual_app: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
-        java_start_up_config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, RosK8sApplication.JavaStartUpConfigProperty]] = None,
+        java_start_up_config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosK8sApplication.JavaStartUpConfigProperty, typing.Dict[str, typing.Any]]]] = None,
         jdk: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         limit_cpu: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         limit_mem: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
-        liveness: typing.Optional[typing.Union[ros_cdk_core.IResolvable, RosK8sApplication.LivenessProperty]] = None,
-        local_volume: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosK8sApplication.LocalVolumeProperty]]]] = None,
+        liveness: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosK8sApplication.LivenessProperty, typing.Dict[str, typing.Any]]]] = None,
+        local_volume: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosK8sApplication.LocalVolumeProperty, typing.Dict[str, typing.Any]]]]]] = None,
         logical_region_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        mount_descs: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosK8sApplication.MountDescsProperty]]]] = None,
+        mount_descs: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosK8sApplication.MountDescsProperty, typing.Dict[str, typing.Any]]]]]] = None,
         namespace: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         nas_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         package_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         package_url: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         package_version: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        post_start: typing.Optional[typing.Union[ros_cdk_core.IResolvable, RosK8sApplication.PostStartProperty]] = None,
-        pre_stop: typing.Optional[typing.Union[ros_cdk_core.IResolvable, RosK8sApplication.PreStopProperty]] = None,
-        readiness: typing.Optional[typing.Union[ros_cdk_core.IResolvable, RosK8sApplication.ReadinessProperty]] = None,
+        post_start: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosK8sApplication.PostStartProperty, typing.Dict[str, typing.Any]]]] = None,
+        pre_stop: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosK8sApplication.PreStopProperty, typing.Dict[str, typing.Any]]]] = None,
+        readiness: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosK8sApplication.ReadinessProperty, typing.Dict[str, typing.Any]]]] = None,
         replicas: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         repo_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         requests_cpu: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         requests_mem: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         runtime_class_name: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        sls_configs: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosK8sApplication.SlsConfigsProperty]]]] = None,
+        sls_configs: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosK8sApplication.SlsConfigsProperty, typing.Dict[str, typing.Any]]]]]] = None,
         storage_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         timeout: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         uri_encoding: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         use_body_encoding: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         web_container: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        web_container_config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, RosK8sApplication.WebContainerConfigProperty]] = None,
+        web_container_config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosK8sApplication.WebContainerConfigProperty, typing.Dict[str, typing.Any]]]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::EDAS::K8sApplication``.
 
         :param app_name: 
         :param cluster_id: 
         :param application_description: 
         :param command: 
@@ -7448,14 +8137,64 @@
         :param storage_type: 
         :param timeout: 
         :param uri_encoding: 
         :param use_body_encoding: 
         :param web_container: 
         :param web_container_config: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosK8sApplicationProps.__init__)
+            check_type(argname="argument app_name", value=app_name, expected_type=type_hints["app_name"])
+            check_type(argname="argument cluster_id", value=cluster_id, expected_type=type_hints["cluster_id"])
+            check_type(argname="argument application_description", value=application_description, expected_type=type_hints["application_description"])
+            check_type(argname="argument command", value=command, expected_type=type_hints["command"])
+            check_type(argname="argument command_args", value=command_args, expected_type=type_hints["command_args"])
+            check_type(argname="argument deploy_across_nodes", value=deploy_across_nodes, expected_type=type_hints["deploy_across_nodes"])
+            check_type(argname="argument deploy_across_zones", value=deploy_across_zones, expected_type=type_hints["deploy_across_zones"])
+            check_type(argname="argument edas_container_version", value=edas_container_version, expected_type=type_hints["edas_container_version"])
+            check_type(argname="argument enable_ahas", value=enable_ahas, expected_type=type_hints["enable_ahas"])
+            check_type(argname="argument envs", value=envs, expected_type=type_hints["envs"])
+            check_type(argname="argument image_url", value=image_url, expected_type=type_hints["image_url"])
+            check_type(argname="argument internet_slb_id", value=internet_slb_id, expected_type=type_hints["internet_slb_id"])
+            check_type(argname="argument internet_slb_port", value=internet_slb_port, expected_type=type_hints["internet_slb_port"])
+            check_type(argname="argument internet_slb_protocol", value=internet_slb_protocol, expected_type=type_hints["internet_slb_protocol"])
+            check_type(argname="argument internet_target_port", value=internet_target_port, expected_type=type_hints["internet_target_port"])
+            check_type(argname="argument intranet_slb_id", value=intranet_slb_id, expected_type=type_hints["intranet_slb_id"])
+            check_type(argname="argument intranet_slb_port", value=intranet_slb_port, expected_type=type_hints["intranet_slb_port"])
+            check_type(argname="argument intranet_slb_protocol", value=intranet_slb_protocol, expected_type=type_hints["intranet_slb_protocol"])
+            check_type(argname="argument intranet_target_port", value=intranet_target_port, expected_type=type_hints["intranet_target_port"])
+            check_type(argname="argument is_multilingual_app", value=is_multilingual_app, expected_type=type_hints["is_multilingual_app"])
+            check_type(argname="argument java_start_up_config", value=java_start_up_config, expected_type=type_hints["java_start_up_config"])
+            check_type(argname="argument jdk", value=jdk, expected_type=type_hints["jdk"])
+            check_type(argname="argument limit_cpu", value=limit_cpu, expected_type=type_hints["limit_cpu"])
+            check_type(argname="argument limit_mem", value=limit_mem, expected_type=type_hints["limit_mem"])
+            check_type(argname="argument liveness", value=liveness, expected_type=type_hints["liveness"])
+            check_type(argname="argument local_volume", value=local_volume, expected_type=type_hints["local_volume"])
+            check_type(argname="argument logical_region_id", value=logical_region_id, expected_type=type_hints["logical_region_id"])
+            check_type(argname="argument mount_descs", value=mount_descs, expected_type=type_hints["mount_descs"])
+            check_type(argname="argument namespace", value=namespace, expected_type=type_hints["namespace"])
+            check_type(argname="argument nas_id", value=nas_id, expected_type=type_hints["nas_id"])
+            check_type(argname="argument package_type", value=package_type, expected_type=type_hints["package_type"])
+            check_type(argname="argument package_url", value=package_url, expected_type=type_hints["package_url"])
+            check_type(argname="argument package_version", value=package_version, expected_type=type_hints["package_version"])
+            check_type(argname="argument post_start", value=post_start, expected_type=type_hints["post_start"])
+            check_type(argname="argument pre_stop", value=pre_stop, expected_type=type_hints["pre_stop"])
+            check_type(argname="argument readiness", value=readiness, expected_type=type_hints["readiness"])
+            check_type(argname="argument replicas", value=replicas, expected_type=type_hints["replicas"])
+            check_type(argname="argument repo_id", value=repo_id, expected_type=type_hints["repo_id"])
+            check_type(argname="argument requests_cpu", value=requests_cpu, expected_type=type_hints["requests_cpu"])
+            check_type(argname="argument requests_mem", value=requests_mem, expected_type=type_hints["requests_mem"])
+            check_type(argname="argument runtime_class_name", value=runtime_class_name, expected_type=type_hints["runtime_class_name"])
+            check_type(argname="argument sls_configs", value=sls_configs, expected_type=type_hints["sls_configs"])
+            check_type(argname="argument storage_type", value=storage_type, expected_type=type_hints["storage_type"])
+            check_type(argname="argument timeout", value=timeout, expected_type=type_hints["timeout"])
+            check_type(argname="argument uri_encoding", value=uri_encoding, expected_type=type_hints["uri_encoding"])
+            check_type(argname="argument use_body_encoding", value=use_body_encoding, expected_type=type_hints["use_body_encoding"])
+            check_type(argname="argument web_container", value=web_container, expected_type=type_hints["web_container"])
+            check_type(argname="argument web_container_config", value=web_container_config, expected_type=type_hints["web_container_config"])
         self._values: typing.Dict[str, typing.Any] = {
             "app_name": app_name,
             "cluster_id": cluster_id,
         }
         if application_description is not None:
             self._values["application_description"] = application_description
         if command is not None:
@@ -8088,183 +8827,204 @@
 ):
     '''A ROS template type:  ``ALIYUN::EDAS::K8sCluster``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosK8sClusterProps",
+        props: typing.Union["RosK8sClusterProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::EDAS::K8sCluster``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosK8sCluster.__init__)
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
+            type_hints = typing.get_type_hints(RosK8sCluster._render_properties)
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
         :Attribute: ClusterId: The ID of the cluster.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrClusterId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrClusterName")
     def attr_cluster_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ClusterName: The name of the cluster.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrClusterName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrClusterType")
     def attr_cluster_type(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute:
 
         ClusterType: The type of the cluster:
         2: ECS cluster
         5: Container Service K8s cluster or Serverless K8s cluster
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrClusterType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrCsClusterId")
     def attr_cs_cluster_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: CsClusterId: The ID of the K8s cluster.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrCsClusterId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrNetworkMode")
     def attr_network_mode(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute:
 
         NetworkMode: Network node:
         1: Classic network
         2: VPC
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrNetworkMode"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrNodeNum")
     def attr_node_num(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: NodeNum: Number of nodes.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrNodeNum"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrSubNetCidr")
     def attr_sub_net_cidr(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: SubNetCidr: Sub net CIDR.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrSubNetCidr"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVpcId")
     def attr_vpc_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: VpcId: The ID of the cluster.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVpcId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVswitchId")
     def attr_vswitch_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: VswitchId: The ID of the cluster.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVswitchId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="csClusterId")
     def cs_cluster_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: csClusterId: The ID of the CS cluster.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "csClusterId"))
 
     @cs_cluster_id.setter
     def cs_cluster_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosK8sCluster, "cs_cluster_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "csClusterId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosK8sCluster, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableAsm")
     def enable_asm(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: enableAsm: Whether enable ASM.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "enableAsm"))
 
     @enable_asm.setter
     def enable_asm(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosK8sCluster, "enable_asm").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableAsm", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="namespaceId")
     def namespace_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: namespaceId: The ID of the namespace to which the cluster that you want to import belongs.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "namespaceId"))
 
     @namespace_id.setter
     def namespace_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosK8sCluster, "namespace_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "namespaceId", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-edas.RosK8sClusterProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -8283,14 +9043,19 @@
     ) -> None:
         '''Properties for defining a ``ALIYUN::EDAS::K8sCluster``.
 
         :param cs_cluster_id: 
         :param enable_asm: 
         :param namespace_id: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosK8sClusterProps.__init__)
+            check_type(argname="argument cs_cluster_id", value=cs_cluster_id, expected_type=type_hints["cs_cluster_id"])
+            check_type(argname="argument enable_asm", value=enable_asm, expected_type=type_hints["enable_asm"])
+            check_type(argname="argument namespace_id", value=namespace_id, expected_type=type_hints["namespace_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "cs_cluster_id": cs_cluster_id,
         }
         if enable_asm is not None:
             self._values["enable_asm"] = enable_asm
         if namespace_id is not None:
             self._values["namespace_id"] = namespace_id
@@ -8343,173 +9108,200 @@
 ):
     '''A ROS template type:  ``ALIYUN::EDAS::K8sSlbBinding``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosK8sSlbBindingProps",
+        props: typing.Union["RosK8sSlbBindingProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::EDAS::K8sSlbBinding``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosK8sSlbBinding.__init__)
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
+            type_hints = typing.get_type_hints(RosK8sSlbBinding._render_properties)
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
     @jsii.member(jsii_name="attrAddress")
     def attr_address(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Address: The address of load balancer instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAddress"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrAppId")
     def attr_app_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: AppId: The ID of the application.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAppId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrChangeOrderId")
     def attr_change_order_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ChangeOrderId: The ID of the change process.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrChangeOrderId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrLoadBalancerId")
     def attr_load_balancer_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: LoadBalancerId: The ID of load balancer instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrLoadBalancerId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrLoadBalancerName")
     def attr_load_balancer_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: LoadBalancerName: The name of load balancer instance defined in EDAS.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrLoadBalancerName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="appId")
     def app_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: appId: The ID of the application.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "appId"))
 
     @app_id.setter
     def app_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosK8sSlbBinding, "app_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "appId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="clusterId")
     def cluster_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: clusterId: The ID of the cluster.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "clusterId"))
 
     @cluster_id.setter
     def cluster_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosK8sSlbBinding, "cluster_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "clusterId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosK8sSlbBinding, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="servicePortInfos")
     def service_port_infos(
         self,
     ) -> typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosK8sSlbBinding.ServicePortInfosProperty"]]]:
         '''
         :Property: servicePortInfos: The information about the ports.
         '''
         return typing.cast(typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosK8sSlbBinding.ServicePortInfosProperty"]]], jsii.get(self, "servicePortInfos"))
 
     @service_port_infos.setter
     def service_port_infos(
         self,
         value: typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosK8sSlbBinding.ServicePortInfosProperty"]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosK8sSlbBinding, "service_port_infos").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "servicePortInfos", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="type")
     def type(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: type: The type of the SLB instance. Valid values: internet and intranet.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "type"))
 
     @type.setter
     def type(self, value: typing.Union[builtins.str, ros_cdk_core.IResolvable]) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosK8sSlbBinding, "type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "type", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="loadBalancerId")
     def load_balancer_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: loadBalancerId: The ID of the load balancer instance. If you leave this parameter empty, Enterprise Distributed Application Service (EDAS) automatically purchases an SLB instance.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "loadBalancerId"))
 
     @load_balancer_id.setter
     def load_balancer_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosK8sSlbBinding, "load_balancer_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "loadBalancerId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="scheduler")
     def scheduler(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -8521,31 +9313,37 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "scheduler"))
 
     @scheduler.setter
     def scheduler(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosK8sSlbBinding, "scheduler").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "scheduler", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="specification")
     def specification(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: specification: The specification of the load balancer instance.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "specification"))
 
     @specification.setter
     def specification(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosK8sSlbBinding, "specification").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "specification", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-edas.RosK8sSlbBinding.ServicePortInfosProperty",
         jsii_struct_bases=[],
         name_mapping={
             "load_balancer_protocol": "loadBalancerProtocol",
@@ -8565,14 +9363,20 @@
         ) -> None:
             '''
             :param load_balancer_protocol: 
             :param port: 
             :param target_port: 
             :param cert_id: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosK8sSlbBinding.ServicePortInfosProperty.__init__)
+                check_type(argname="argument load_balancer_protocol", value=load_balancer_protocol, expected_type=type_hints["load_balancer_protocol"])
+                check_type(argname="argument port", value=port, expected_type=type_hints["port"])
+                check_type(argname="argument target_port", value=target_port, expected_type=type_hints["target_port"])
+                check_type(argname="argument cert_id", value=cert_id, expected_type=type_hints["cert_id"])
             self._values: typing.Dict[str, typing.Any] = {
                 "load_balancer_protocol": load_balancer_protocol,
                 "port": port,
                 "target_port": target_port,
             }
             if cert_id is not None:
                 self._values["cert_id"] = cert_id
@@ -8643,15 +9447,15 @@
 )
 class RosK8sSlbBindingProps:
     def __init__(
         self,
         *,
         app_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         cluster_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
-        service_port_infos: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosK8sSlbBinding.ServicePortInfosProperty]]],
+        service_port_infos: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosK8sSlbBinding.ServicePortInfosProperty, typing.Dict[str, typing.Any]]]]],
         type: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         load_balancer_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         scheduler: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         specification: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::EDAS::K8sSlbBinding``.
 
@@ -8659,14 +9463,23 @@
         :param cluster_id: 
         :param service_port_infos: 
         :param type: 
         :param load_balancer_id: 
         :param scheduler: 
         :param specification: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosK8sSlbBindingProps.__init__)
+            check_type(argname="argument app_id", value=app_id, expected_type=type_hints["app_id"])
+            check_type(argname="argument cluster_id", value=cluster_id, expected_type=type_hints["cluster_id"])
+            check_type(argname="argument service_port_infos", value=service_port_infos, expected_type=type_hints["service_port_infos"])
+            check_type(argname="argument type", value=type, expected_type=type_hints["type"])
+            check_type(argname="argument load_balancer_id", value=load_balancer_id, expected_type=type_hints["load_balancer_id"])
+            check_type(argname="argument scheduler", value=scheduler, expected_type=type_hints["scheduler"])
+            check_type(argname="argument specification", value=specification, expected_type=type_hints["specification"])
         self._values: typing.Dict[str, typing.Any] = {
             "app_id": app_id,
             "cluster_id": cluster_id,
             "service_port_infos": service_port_infos,
             "type": type,
         }
         if load_balancer_id is not None:
@@ -8768,158 +9581,182 @@
 ):
     '''A ROS template type:  ``ALIYUN::EDAS::UserDefineRegion``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosUserDefineRegionProps",
+        props: typing.Union["RosUserDefineRegionProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::EDAS::UserDefineRegion``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosUserDefineRegion.__init__)
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
+            type_hints = typing.get_type_hints(RosUserDefineRegion._render_properties)
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
     @jsii.member(jsii_name="attrBelongRegion")
     def attr_belong_region(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: BelongRegion: Under the physical region ID
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrBelongRegion"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDebugEnable")
     def attr_debug_enable(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: DebugEnable: Whether debug is enable
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDebugEnable"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrId")
     def attr_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Id: Resource ID
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrRegionName")
     def attr_region_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: RegionName: Region name
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrRegionName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrUserId")
     def attr_user_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: UserId: User account ID
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrUserId"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosUserDefineRegion, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="regionName")
     def region_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: regionName: Logical region (or namespace) name
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "regionName"))
 
     @region_name.setter
     def region_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosUserDefineRegion, "region_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "regionName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="regionTag")
     def region_tag(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: regionTag: Logic region (or namespace) ID (format: "physical region ID: logical zone identifier", or "logical zone identifier")
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "regionTag"))
 
     @region_tag.setter
     def region_tag(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosUserDefineRegion, "region_tag").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "regionTag", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="debugEnable")
     def debug_enable(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property: debugEnable: Whether debug is enable
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "debugEnable"))
 
     @debug_enable.setter
     def debug_enable(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosUserDefineRegion, "debug_enable").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "debugEnable", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="description")
     def description(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: description: Logic region (or namespace) description
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "description"))
 
     @description.setter
     def description(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosUserDefineRegion, "description").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "description", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-edas.RosUserDefineRegionProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -8941,14 +9778,20 @@
         '''Properties for defining a ``ALIYUN::EDAS::UserDefineRegion``.
 
         :param region_name: 
         :param region_tag: 
         :param debug_enable: 
         :param description: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosUserDefineRegionProps.__init__)
+            check_type(argname="argument region_name", value=region_name, expected_type=type_hints["region_name"])
+            check_type(argname="argument region_tag", value=region_tag, expected_type=type_hints["region_tag"])
+            check_type(argname="argument debug_enable", value=debug_enable, expected_type=type_hints["debug_enable"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
         self._values: typing.Dict[str, typing.Any] = {
             "region_name": region_name,
             "region_tag": region_tag,
         }
         if debug_enable is not None:
             self._values["debug_enable"] = debug_enable
         if description is not None:
@@ -9011,55 +9854,61 @@
 ):
     '''A ROS resource type:  ``ALIYUN::EDAS::UserDefineRegion``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "UserDefineRegionProps",
+        props: typing.Union["UserDefineRegionProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::EDAS::UserDefineRegion``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(UserDefineRegion.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrBelongRegion")
     def attr_belong_region(self) -> ros_cdk_core.IResolvable:
         '''Attribute BelongRegion: Under the physical region ID.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrBelongRegion"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDebugEnable")
     def attr_debug_enable(self) -> ros_cdk_core.IResolvable:
         '''Attribute DebugEnable: Whether debug is enable.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDebugEnable"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrId")
     def attr_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute Id: Resource ID.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrRegionName")
     def attr_region_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute RegionName: Region name.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrRegionName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrUserId")
     def attr_user_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute UserId: User account ID.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrUserId"))
 
 
 @jsii.data_type(
@@ -9084,14 +9933,20 @@
         '''Properties for defining a ``ALIYUN::EDAS::UserDefineRegion``.
 
         :param region_name: Property regionName: Logical region (or namespace) name.
         :param region_tag: Property regionTag: Logic region (or namespace) ID (format: "physical region ID: logical zone identifier", or "logical zone identifier").
         :param debug_enable: Property debugEnable: Whether debug is enable.
         :param description: Property description: Logic region (or namespace) description.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(UserDefineRegionProps.__init__)
+            check_type(argname="argument region_name", value=region_name, expected_type=type_hints["region_name"])
+            check_type(argname="argument region_tag", value=region_tag, expected_type=type_hints["region_tag"])
+            check_type(argname="argument debug_enable", value=debug_enable, expected_type=type_hints["debug_enable"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
         self._values: typing.Dict[str, typing.Any] = {
             "region_name": region_name,
             "region_tag": region_tag,
         }
         if debug_enable is not None:
             self._values["debug_enable"] = debug_enable
         if description is not None:
```

### Comparing `ros-cdk-edas-1.0.8/src/ros_cdk_edas.egg-info/PKG-INFO` & `ros-cdk-edas-1.0.9/src/ros_cdk_edas.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-edas
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS EDAS Construct Library
```

