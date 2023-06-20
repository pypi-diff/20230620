# Comparing `tmp/ros-cdk-cs-1.0.8.tar.gz` & `tmp/ros-cdk-cs-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-cs-1.0.8.tar", last modified: Thu Jul 14 02:19:27 2022, max compression
+gzip compressed data, was "dist/ros-cdk-cs-1.0.9.tar", last modified: Fri Sep 23 11:34:09 2022, max compression
```

## Comparing `ros-cdk-cs-1.0.8.tar` & `ros-cdk-cs-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:19:27.000000 ros-cdk-cs-1.0.8/
--rw-r--r--   0 root         (0) root         (0)    10279 2022-07-14 02:19:27.000000 ros-cdk-cs-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2022-07-14 02:19:27.000000 ros-cdk-cs-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2022-07-14 02:19:27.000000 ros-cdk-cs-1.0.8/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1236 2022-07-14 02:19:27.000000 ros-cdk-cs-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      176 2022-07-14 02:19:27.000000 ros-cdk-cs-1.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)      106 2022-07-14 02:19:27.000000 ros-cdk-cs-1.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-07-14 02:19:27.000000 ros-cdk-cs-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1788 2022-07-14 02:19:27.000000 ros-cdk-cs-1.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:19:27.000000 ros-cdk-cs-1.0.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:19:27.000000 ros-cdk-cs-1.0.8/src/ros_cdk_cs/
--rw-r--r--   0 root         (0) root         (0)   685134 2022-07-14 02:19:27.000000 ros-cdk-cs-1.0.8/src/ros_cdk_cs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:19:27.000000 ros-cdk-cs-1.0.8/src/ros_cdk_cs/_jsii/
--rw-r--r--   0 root         (0) root         (0)      368 2022-07-14 02:19:27.000000 ros-cdk-cs-1.0.8/src/ros_cdk_cs/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)   251871 2022-07-14 02:19:27.000000 ros-cdk-cs-1.0.8/src/ros_cdk_cs/_jsii/ros-cdk-cs@1.0.8.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:19:27.000000 ros-cdk-cs-1.0.8/src/ros_cdk_cs/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:19:27.000000 ros-cdk-cs-1.0.8/src/ros_cdk_cs.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1236 2022-07-14 02:19:27.000000 ros-cdk-cs-1.0.8/src/ros_cdk_cs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      390 2022-07-14 02:19:27.000000 ros-cdk-cs-1.0.8/src/ros_cdk_cs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:19:27.000000 ros-cdk-cs-1.0.8/src/ros_cdk_cs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2022-07-14 02:19:27.000000 ros-cdk-cs-1.0.8/src/ros_cdk_cs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2022-07-14 02:19:27.000000 ros-cdk-cs-1.0.8/src/ros_cdk_cs.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:34:09.000000 ros-cdk-cs-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)    10279 2022-09-23 11:34:09.000000 ros-cdk-cs-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-09-23 11:34:09.000000 ros-cdk-cs-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2022-09-23 11:34:09.000000 ros-cdk-cs-1.0.9/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1236 2022-09-23 11:34:09.000000 ros-cdk-cs-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      176 2022-09-23 11:34:09.000000 ros-cdk-cs-1.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      236 2022-09-23 11:34:09.000000 ros-cdk-cs-1.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-09-23 11:34:09.000000 ros-cdk-cs-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1817 2022-09-23 11:34:09.000000 ros-cdk-cs-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:34:09.000000 ros-cdk-cs-1.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:34:09.000000 ros-cdk-cs-1.0.9/src/ros_cdk_cs/
+-rw-r--r--   0 root         (0) root         (0)   809387 2022-09-23 11:34:09.000000 ros-cdk-cs-1.0.9/src/ros_cdk_cs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:34:09.000000 ros-cdk-cs-1.0.9/src/ros_cdk_cs/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      402 2022-09-23 11:34:09.000000 ros-cdk-cs-1.0.9/src/ros_cdk_cs/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   255064 2022-09-23 11:34:09.000000 ros-cdk-cs-1.0.9/src/ros_cdk_cs/_jsii/ros-cdk-cs@1.0.9.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 11:34:09.000000 ros-cdk-cs-1.0.9/src/ros_cdk_cs/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:34:09.000000 ros-cdk-cs-1.0.9/src/ros_cdk_cs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1236 2022-09-23 11:34:09.000000 ros-cdk-cs-1.0.9/src/ros_cdk_cs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      390 2022-09-23 11:34:09.000000 ros-cdk-cs-1.0.9/src/ros_cdk_cs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 11:34:09.000000 ros-cdk-cs-1.0.9/src/ros_cdk_cs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2022-09-23 11:34:09.000000 ros-cdk-cs-1.0.9/src/ros_cdk_cs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2022-09-23 11:34:09.000000 ros-cdk-cs-1.0.9/src/ros_cdk_cs.egg-info/top_level.txt
```

### Comparing `ros-cdk-cs-1.0.8/LICENSE` & `ros-cdk-cs-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-cs-1.0.8/PKG-INFO` & `ros-cdk-cs-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-cs
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS CS Construct Library
```

### Comparing `ros-cdk-cs-1.0.8/setup.py` & `ros-cdk-cs-1.0.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-cs",
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
         "ros_cdk_cs",
         "ros_cdk_cs._jsii"
     ],
     "package_data": {
         "ros_cdk_cs._jsii": [
-            "ros-cdk-cs@1.0.8.jsii.tgz"
+            "ros-cdk-cs@1.0.9.jsii.tgz"
         ],
         "ros_cdk_cs": [
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

### Comparing `ros-cdk-cs-1.0.8/src/ros_cdk_cs/__init__.py` & `ros-cdk-cs-1.0.9/src/ros_cdk_cs/__init__.py`

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
 
 
 class AnyCluster(
     ros_cdk_core.Resource,
@@ -29,88 +31,94 @@
 ):
     '''A ROS resource type:  ``ALIYUN::CS::AnyCluster``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "AnyClusterProps",
+        props: typing.Union["AnyClusterProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::CS::AnyCluster``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(AnyCluster.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrApiServerSlbId")
     def attr_api_server_slb_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute APIServerSLBId: The id of API server SLB.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrApiServerSlbId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrClusterId")
     def attr_cluster_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute ClusterId: Cluster instance ID.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrClusterId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDefaultUserKubeConfig")
     def attr_default_user_kube_config(self) -> ros_cdk_core.IResolvable:
         '''Attribute DefaultUserKubeConfig: Default user kubernetes config which is used for configuring cluster credentials.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDefaultUserKubeConfig"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrNodes")
     def attr_nodes(self) -> ros_cdk_core.IResolvable:
         '''Attribute Nodes: The list of cluster nodes.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrNodes"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPrivateUserKubConfig")
     def attr_private_user_kub_config(self) -> ros_cdk_core.IResolvable:
         '''Attribute PrivateUserKubConfig: Private user kubernetes config which is used for configuring cluster credentials.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPrivateUserKubConfig"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrScalingConfigurationId")
     def attr_scaling_configuration_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute ScalingConfigurationId: Scaling configuration id.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrScalingConfigurationId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrScalingGroupId")
     def attr_scaling_group_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute ScalingGroupId: Scaling group id.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrScalingGroupId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrScalingRuleId")
     def attr_scaling_rule_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute ScalingRuleId: Scaling rule id.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrScalingRuleId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTaskId")
     def attr_task_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute TaskId: Task ID.
 
         Automatically assigned by the system, the user queries the task status.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTaskId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrWorkerRamRoleName")
     def attr_worker_ram_role_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute WorkerRamRoleName: Worker ram role name.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrWorkerRamRoleName"))
 
 
 @jsii.data_type(
@@ -124,14 +132,17 @@
         *,
         cluster_config: typing.Union[typing.Mapping[builtins.str, typing.Any], ros_cdk_core.IResolvable],
     ) -> None:
         '''Properties for defining a ``ALIYUN::CS::AnyCluster``.
 
         :param cluster_config: Property clusterConfig: Cluster config.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(AnyClusterProps.__init__)
+            check_type(argname="argument cluster_config", value=cluster_config, expected_type=type_hints["cluster_config"])
         self._values: typing.Dict[str, typing.Any] = {
             "cluster_config": cluster_config,
         }
 
     @builtins.property
     def cluster_config(
         self,
@@ -160,31 +171,37 @@
 ):
     '''A ROS resource type:  ``ALIYUN::CS::ClusterNodePool``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "ClusterNodePoolProps",
+        props: typing.Union["ClusterNodePoolProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::CS::ClusterNodePool``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(ClusterNodePool.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrNodePoolId")
     def attr_node_pool_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute NodePoolId: Cluster node pool ID.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrNodePoolId"))
 
 
 @jsii.data_type(
@@ -202,33 +219,43 @@
     },
 )
 class ClusterNodePoolProps:
     def __init__(
         self,
         *,
         cluster_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
-        scaling_group: typing.Union[ros_cdk_core.IResolvable, "RosClusterNodePool.ScalingGroupProperty"],
-        auto_scaling: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosClusterNodePool.AutoScalingProperty"]] = None,
+        scaling_group: typing.Union[ros_cdk_core.IResolvable, typing.Union["RosClusterNodePool.ScalingGroupProperty", typing.Dict[str, typing.Any]]],
+        auto_scaling: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosClusterNodePool.AutoScalingProperty", typing.Dict[str, typing.Any]]]] = None,
         count: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
-        kubernetes_config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosClusterNodePool.KubernetesConfigProperty"]] = None,
-        management: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosClusterNodePool.ManagementProperty"]] = None,
-        node_pool_info: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosClusterNodePool.NodePoolInfoProperty"]] = None,
-        tee_config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosClusterNodePool.TeeConfigProperty"]] = None,
+        kubernetes_config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosClusterNodePool.KubernetesConfigProperty", typing.Dict[str, typing.Any]]]] = None,
+        management: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosClusterNodePool.ManagementProperty", typing.Dict[str, typing.Any]]]] = None,
+        node_pool_info: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosClusterNodePool.NodePoolInfoProperty", typing.Dict[str, typing.Any]]]] = None,
+        tee_config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosClusterNodePool.TeeConfigProperty", typing.Dict[str, typing.Any]]]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::CS::ClusterNodePool``.
 
         :param cluster_id: Property clusterId: Cluster ID.
         :param scaling_group: Property scalingGroup: The configurations of the scaling group used by the node pool.
         :param auto_scaling: Property autoScaling: The configurations of auto scaling.
         :param count: Property count: The number of nodes in the node pool.
         :param kubernetes_config: Property kubernetesConfig: The configurations of the ACK cluster.
         :param management: Property management: The configurations of the managed node pool.
         :param node_pool_info: Property nodePoolInfo: The configurations of the node pool.
         :param tee_config: Property teeConfig: The configurations of confidential computing.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(ClusterNodePoolProps.__init__)
+            check_type(argname="argument cluster_id", value=cluster_id, expected_type=type_hints["cluster_id"])
+            check_type(argname="argument scaling_group", value=scaling_group, expected_type=type_hints["scaling_group"])
+            check_type(argname="argument auto_scaling", value=auto_scaling, expected_type=type_hints["auto_scaling"])
+            check_type(argname="argument count", value=count, expected_type=type_hints["count"])
+            check_type(argname="argument kubernetes_config", value=kubernetes_config, expected_type=type_hints["kubernetes_config"])
+            check_type(argname="argument management", value=management, expected_type=type_hints["management"])
+            check_type(argname="argument node_pool_info", value=node_pool_info, expected_type=type_hints["node_pool_info"])
+            check_type(argname="argument tee_config", value=tee_config, expected_type=type_hints["tee_config"])
         self._values: typing.Dict[str, typing.Any] = {
             "cluster_id": cluster_id,
             "scaling_group": scaling_group,
         }
         if auto_scaling is not None:
             self._values["auto_scaling"] = auto_scaling
         if count is not None:
@@ -325,88 +352,94 @@
 ):
     '''A ROS resource type:  ``ALIYUN::CS::KubernetesCluster``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "KubernetesClusterProps",
+        props: typing.Union["KubernetesClusterProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::CS::KubernetesCluster``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(KubernetesCluster.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrApiServerSlbId")
     def attr_api_server_slb_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute APIServerSLBId: The id of API server SLB.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrApiServerSlbId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrClusterId")
     def attr_cluster_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute ClusterId: Cluster instance ID.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrClusterId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDefaultUserKubeConfig")
     def attr_default_user_kube_config(self) -> ros_cdk_core.IResolvable:
         '''Attribute DefaultUserKubeConfig: Default user kubernetes config which is used for configuring cluster credentials.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDefaultUserKubeConfig"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrNodes")
     def attr_nodes(self) -> ros_cdk_core.IResolvable:
         '''Attribute Nodes: The list of cluster nodes.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrNodes"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPrivateUserKubConfig")
     def attr_private_user_kub_config(self) -> ros_cdk_core.IResolvable:
         '''Attribute PrivateUserKubConfig: Private user kubernetes config which is used for configuring cluster credentials.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPrivateUserKubConfig"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrScalingConfigurationId")
     def attr_scaling_configuration_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute ScalingConfigurationId: Scaling configuration id.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrScalingConfigurationId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrScalingGroupId")
     def attr_scaling_group_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute ScalingGroupId: Scaling group id.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrScalingGroupId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrScalingRuleId")
     def attr_scaling_rule_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute ScalingRuleId: Scaling rule id.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrScalingRuleId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTaskId")
     def attr_task_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute TaskId: Task ID.
 
         Automatically assigned by the system, the user queries the task status.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTaskId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrWorkerRamRoleName")
     def attr_worker_ram_role_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute WorkerRamRoleName: Worker ram role name.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrWorkerRamRoleName"))
 
 
 @jsii.data_type(
@@ -482,15 +515,15 @@
         self,
         *,
         master_instance_types: typing.Union[typing.Sequence[typing.Any], ros_cdk_core.IResolvable],
         master_v_switch_ids: typing.Union[typing.Sequence[typing.Any], ros_cdk_core.IResolvable],
         name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         vpc_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         worker_v_switch_ids: typing.Union[typing.Sequence[typing.Any], ros_cdk_core.IResolvable],
-        addons: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosKubernetesCluster.AddonsProperty"]]]] = None,
+        addons: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosKubernetesCluster.AddonsProperty", typing.Dict[str, typing.Any]]]]]] = None,
         auto_renew: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         auto_renew_period: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         charge_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         cis_enabled: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         cloud_monitor_flags: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         container_cidr: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         cpu_policy: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
@@ -502,46 +535,46 @@
         keep_instance_name: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         key_pair: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         kubernetes_version: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         load_balancer_spec: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         login_password: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         master_count: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         master_data_disk: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
-        master_data_disks: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosKubernetesCluster.MasterDataDisksProperty"]]]] = None,
+        master_data_disks: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosKubernetesCluster.MasterDataDisksProperty", typing.Dict[str, typing.Any]]]]]] = None,
         master_system_disk_category: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         master_system_disk_performance_level: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         master_system_disk_size: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         master_system_disk_snapshot_policy_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         master_zone_ids: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]] = None,
         node_cidr_mask: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         node_name_mode: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        node_pools: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosKubernetesCluster.NodePoolsProperty"]]]] = None,
+        node_pools: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosKubernetesCluster.NodePoolsProperty", typing.Dict[str, typing.Any]]]]]] = None,
         node_port_range: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         num_of_nodes: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         os_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         period: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         period_unit: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         platform: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         pod_vswitch_ids: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]] = None,
         proxy_mode: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         resource_group_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        runtime: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosKubernetesCluster.RuntimeProperty"]] = None,
+        runtime: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosKubernetesCluster.RuntimeProperty", typing.Dict[str, typing.Any]]]] = None,
         security_group_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         service_cidr: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         snat_entry: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         soc_enabled: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         ssh_flags: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
-        tags: typing.Optional[typing.Sequence["RosKubernetesCluster.TagsProperty"]] = None,
+        tags: typing.Optional[typing.Sequence[typing.Union["RosKubernetesCluster.TagsProperty", typing.Dict[str, typing.Any]]]] = None,
         taint: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Mapping[builtins.str, typing.Any]]]] = None,
         timeout_mins: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         time_zone: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         user_ca: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         user_data: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         worker_data_disk: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
-        worker_data_disks: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosKubernetesCluster.WorkerDataDisksProperty"]]]] = None,
+        worker_data_disks: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosKubernetesCluster.WorkerDataDisksProperty", typing.Dict[str, typing.Any]]]]]] = None,
         worker_instance_types: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]] = None,
         worker_system_disk_category: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         worker_system_disk_size: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         worker_system_disk_snapshot_policy_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         worker_zone_ids: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::CS::KubernetesCluster``.
@@ -579,16 +612,16 @@
         :param master_zone_ids: Property masterZoneIds: Zone ids of master node virtual switches belongs to.
         :param node_cidr_mask: Property nodeCidrMask: The maximum number of IP addresses that can be assigned to nodes. This number is determined by the specified pod CIDR block. This parameter takes effect only if the cluster uses the Flannel plug-in.Default value: 25.
         :param node_name_mode: Property nodeNameMode: A custom node name consists of a prefix, an IP substring, and a suffix. The format iscustomized,{prefix},{ip_substring},{suffix}, for example: customized,aliyun.com,5,test. - The prefix and suffix can contain one or more parts that are separated by periods (.). Each part can contain lowercase letters, digits, and hyphens (-). The node name must start and end with a lowercase letter or digit. - The IP substring length specifies the number of digits to be truncated from the end of the node IP address. Valid values: 5 to 12. For example, if the node IP address is 192.168.0.55, the prefix is aliyun.com, the IP substring length is 5, and the suffix is test, the node name will be aliyun.com00055test.
         :param node_pools: Property nodePools: The configurations of Node pools.
         :param node_port_range: Property nodePortRange: Node service port. The value range is [30000, 65535]. Default to 30000-65535.
         :param num_of_nodes: Property numOfNodes: Number of worker nodes. The range is [0,300]. Default to 3.
         :param os_type: Property osType: The type of operating system. Valid values: Windows Linux Default value: Linux.
-        :param period: Property period: The duration of the annual subscription and monthly subscription. It takes effect when the ChargeType value is PrePaid and is a required value. The value range is: When PeriodUnit = Week, Period values are: {"1", "2", "3", "4"} When PeriodUnit = Month, Period values are: {"1", "2", "3", "4", "5", "6", "7", "8", "9", "12", "24", "36", "48", "60"} Default to 1.
-        :param period_unit: Property periodUnit: When you specify PrePaid, you need to specify the period. The options are: Week: Time is measured in weeks Month: time in months Default to Month
+        :param period: Property period: The duration of the annual subscription and monthly subscription. It takes effect when the ChargeType value is PrePaid and is a required value. The value range is: When PeriodUnit = Week, Period values are: {"1", "2", "3", "4"} When PeriodUnit = Month, Period values are: {"1", "2", "3", "4", "5", "6", "7", "8", "9", "12", "24", "36", "48", "60"} When PeriodUnit = Year, Period values are: {"1", "2", "3", "4", "5"} Default to 1.
+        :param period_unit: Property periodUnit: When you specify PrePaid, you need to specify the period. The options are: Week: Time is measured in weeks Month: time in months Year: time in years Default to Month
         :param platform: Property platform: The release version of the operating system. Valid values: CentOS AliyunLinux QbootAliyunLinux Qboot Windows WindowsCore Default value: CentOS.
         :param pod_vswitch_ids: Property podVswitchIds: The list of pod vSwitches. For each vSwitch that is allocated to nodes, you must specify at least one pod vSwitch in the same zone. The pod vSwitches cannot be the same as the node vSwitches. We recommend that you set the mask length of the CIDR block to a value no greater than 19 for the pod vSwitches. The pod_vswitch_ids parameter is required when the Terway network plug-in is selected for the cluster.
         :param proxy_mode: Property proxyMode: kube-proxy proxy mode, supports both iptables and ipvs modes. The default is iptables.
         :param resource_group_id: Property resourceGroupId: The ID of resource group.
         :param runtime: Property runtime: The container runtime of the cluster. The default runtime is Docker.
         :param security_group_id: Property securityGroupId: Specifies the ID of the security group to which the cluster ECS instance belongs.
         :param service_cidr: Property serviceCidr: The service network segment cannot conflict with the VPC network segment and the container network segment. When the system is selected to automatically create a VPC, the network segment 172.19.0.0/20 is used by default.
@@ -605,14 +638,78 @@
         :param worker_data_disks: Property workerDataDisks: A combination of configurations such as worker data disk type and size. This parameter is valid only when the worker node data disk is mounted.
         :param worker_instance_types: Property workerInstanceTypes: Worker node ECS specification type code. For more details, see Instance Specification Family.
         :param worker_system_disk_category: Property workerSystemDiskCategory: Worker node system disk type. The value includes: cloud_efficiency: efficient cloud disk cloud_ssd: SSD cloud disk Default to cloud_efficiency.
         :param worker_system_disk_size: Property workerSystemDiskSize: Worker disk system disk size, the unit is GiB. Default to 120.
         :param worker_system_disk_snapshot_policy_id: Property workerSystemDiskSnapshotPolicyId: The ID of the policy that is used to back up the data disk of the worker node.
         :param worker_zone_ids: Property workerZoneIds: Zone ids of worker node virtual switches belongs to.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(KubernetesClusterProps.__init__)
+            check_type(argname="argument master_instance_types", value=master_instance_types, expected_type=type_hints["master_instance_types"])
+            check_type(argname="argument master_v_switch_ids", value=master_v_switch_ids, expected_type=type_hints["master_v_switch_ids"])
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+            check_type(argname="argument vpc_id", value=vpc_id, expected_type=type_hints["vpc_id"])
+            check_type(argname="argument worker_v_switch_ids", value=worker_v_switch_ids, expected_type=type_hints["worker_v_switch_ids"])
+            check_type(argname="argument addons", value=addons, expected_type=type_hints["addons"])
+            check_type(argname="argument auto_renew", value=auto_renew, expected_type=type_hints["auto_renew"])
+            check_type(argname="argument auto_renew_period", value=auto_renew_period, expected_type=type_hints["auto_renew_period"])
+            check_type(argname="argument charge_type", value=charge_type, expected_type=type_hints["charge_type"])
+            check_type(argname="argument cis_enabled", value=cis_enabled, expected_type=type_hints["cis_enabled"])
+            check_type(argname="argument cloud_monitor_flags", value=cloud_monitor_flags, expected_type=type_hints["cloud_monitor_flags"])
+            check_type(argname="argument container_cidr", value=container_cidr, expected_type=type_hints["container_cidr"])
+            check_type(argname="argument cpu_policy", value=cpu_policy, expected_type=type_hints["cpu_policy"])
+            check_type(argname="argument deletion_protection", value=deletion_protection, expected_type=type_hints["deletion_protection"])
+            check_type(argname="argument disable_rollback", value=disable_rollback, expected_type=type_hints["disable_rollback"])
+            check_type(argname="argument endpoint_public_access", value=endpoint_public_access, expected_type=type_hints["endpoint_public_access"])
+            check_type(argname="argument format_disk", value=format_disk, expected_type=type_hints["format_disk"])
+            check_type(argname="argument is_enterprise_security_group", value=is_enterprise_security_group, expected_type=type_hints["is_enterprise_security_group"])
+            check_type(argname="argument keep_instance_name", value=keep_instance_name, expected_type=type_hints["keep_instance_name"])
+            check_type(argname="argument key_pair", value=key_pair, expected_type=type_hints["key_pair"])
+            check_type(argname="argument kubernetes_version", value=kubernetes_version, expected_type=type_hints["kubernetes_version"])
+            check_type(argname="argument load_balancer_spec", value=load_balancer_spec, expected_type=type_hints["load_balancer_spec"])
+            check_type(argname="argument login_password", value=login_password, expected_type=type_hints["login_password"])
+            check_type(argname="argument master_count", value=master_count, expected_type=type_hints["master_count"])
+            check_type(argname="argument master_data_disk", value=master_data_disk, expected_type=type_hints["master_data_disk"])
+            check_type(argname="argument master_data_disks", value=master_data_disks, expected_type=type_hints["master_data_disks"])
+            check_type(argname="argument master_system_disk_category", value=master_system_disk_category, expected_type=type_hints["master_system_disk_category"])
+            check_type(argname="argument master_system_disk_performance_level", value=master_system_disk_performance_level, expected_type=type_hints["master_system_disk_performance_level"])
+            check_type(argname="argument master_system_disk_size", value=master_system_disk_size, expected_type=type_hints["master_system_disk_size"])
+            check_type(argname="argument master_system_disk_snapshot_policy_id", value=master_system_disk_snapshot_policy_id, expected_type=type_hints["master_system_disk_snapshot_policy_id"])
+            check_type(argname="argument master_zone_ids", value=master_zone_ids, expected_type=type_hints["master_zone_ids"])
+            check_type(argname="argument node_cidr_mask", value=node_cidr_mask, expected_type=type_hints["node_cidr_mask"])
+            check_type(argname="argument node_name_mode", value=node_name_mode, expected_type=type_hints["node_name_mode"])
+            check_type(argname="argument node_pools", value=node_pools, expected_type=type_hints["node_pools"])
+            check_type(argname="argument node_port_range", value=node_port_range, expected_type=type_hints["node_port_range"])
+            check_type(argname="argument num_of_nodes", value=num_of_nodes, expected_type=type_hints["num_of_nodes"])
+            check_type(argname="argument os_type", value=os_type, expected_type=type_hints["os_type"])
+            check_type(argname="argument period", value=period, expected_type=type_hints["period"])
+            check_type(argname="argument period_unit", value=period_unit, expected_type=type_hints["period_unit"])
+            check_type(argname="argument platform", value=platform, expected_type=type_hints["platform"])
+            check_type(argname="argument pod_vswitch_ids", value=pod_vswitch_ids, expected_type=type_hints["pod_vswitch_ids"])
+            check_type(argname="argument proxy_mode", value=proxy_mode, expected_type=type_hints["proxy_mode"])
+            check_type(argname="argument resource_group_id", value=resource_group_id, expected_type=type_hints["resource_group_id"])
+            check_type(argname="argument runtime", value=runtime, expected_type=type_hints["runtime"])
+            check_type(argname="argument security_group_id", value=security_group_id, expected_type=type_hints["security_group_id"])
+            check_type(argname="argument service_cidr", value=service_cidr, expected_type=type_hints["service_cidr"])
+            check_type(argname="argument snat_entry", value=snat_entry, expected_type=type_hints["snat_entry"])
+            check_type(argname="argument soc_enabled", value=soc_enabled, expected_type=type_hints["soc_enabled"])
+            check_type(argname="argument ssh_flags", value=ssh_flags, expected_type=type_hints["ssh_flags"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
+            check_type(argname="argument taint", value=taint, expected_type=type_hints["taint"])
+            check_type(argname="argument timeout_mins", value=timeout_mins, expected_type=type_hints["timeout_mins"])
+            check_type(argname="argument time_zone", value=time_zone, expected_type=type_hints["time_zone"])
+            check_type(argname="argument user_ca", value=user_ca, expected_type=type_hints["user_ca"])
+            check_type(argname="argument user_data", value=user_data, expected_type=type_hints["user_data"])
+            check_type(argname="argument worker_data_disk", value=worker_data_disk, expected_type=type_hints["worker_data_disk"])
+            check_type(argname="argument worker_data_disks", value=worker_data_disks, expected_type=type_hints["worker_data_disks"])
+            check_type(argname="argument worker_instance_types", value=worker_instance_types, expected_type=type_hints["worker_instance_types"])
+            check_type(argname="argument worker_system_disk_category", value=worker_system_disk_category, expected_type=type_hints["worker_system_disk_category"])
+            check_type(argname="argument worker_system_disk_size", value=worker_system_disk_size, expected_type=type_hints["worker_system_disk_size"])
+            check_type(argname="argument worker_system_disk_snapshot_policy_id", value=worker_system_disk_snapshot_policy_id, expected_type=type_hints["worker_system_disk_snapshot_policy_id"])
+            check_type(argname="argument worker_zone_ids", value=worker_zone_ids, expected_type=type_hints["worker_zone_ids"])
         self._values: typing.Dict[str, typing.Any] = {
             "master_instance_types": master_instance_types,
             "master_v_switch_ids": master_v_switch_ids,
             "name": name,
             "vpc_id": vpc_id,
             "worker_v_switch_ids": worker_v_switch_ids,
         }
@@ -1162,28 +1259,30 @@
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''Property period: The duration of the annual subscription and monthly subscription.
 
         It takes effect when the ChargeType value is PrePaid and is a required value. The value range is:
         When PeriodUnit = Week, Period values are: {"1", "2", "3", "4"}
         When PeriodUnit = Month, Period values are: {"1", "2", "3", "4", "5", "6", "7", "8", "9", "12", "24", "36", "48", "60"}
+        When PeriodUnit = Year, Period values are: {"1", "2", "3", "4", "5"}
         Default to 1.
         '''
         result = self._values.get("period")
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], result)
 
     @builtins.property
     def period_unit(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''Property periodUnit: When you specify PrePaid, you need to specify the period.
 
         The options are:
         Week: Time is measured in weeks
         Month: time in months
+        Year: time in years
         Default to Month
         '''
         result = self._values.get("period_unit")
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], result)
 
     @builtins.property
     def platform(
@@ -1455,88 +1554,94 @@
 ):
     '''A ROS resource type:  ``ALIYUN::CS::ManagedEdgeKubernetesCluster``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "ManagedEdgeKubernetesClusterProps",
+        props: typing.Union["ManagedEdgeKubernetesClusterProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::CS::ManagedEdgeKubernetesCluster``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(ManagedEdgeKubernetesCluster.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrApiServerSlbId")
     def attr_api_server_slb_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute APIServerSLBId: The id of API server SLB.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrApiServerSlbId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrClusterId")
     def attr_cluster_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute ClusterId: Cluster instance ID.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrClusterId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDefaultUserKubeConfig")
     def attr_default_user_kube_config(self) -> ros_cdk_core.IResolvable:
         '''Attribute DefaultUserKubeConfig: Default user kubernetes config which is used for configuring cluster credentials.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDefaultUserKubeConfig"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrNodes")
     def attr_nodes(self) -> ros_cdk_core.IResolvable:
         '''Attribute Nodes: The list of cluster nodes.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrNodes"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPrivateUserKubConfig")
     def attr_private_user_kub_config(self) -> ros_cdk_core.IResolvable:
         '''Attribute PrivateUserKubConfig: Private user kubernetes config which is used for configuring cluster credentials.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPrivateUserKubConfig"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrScalingConfigurationId")
     def attr_scaling_configuration_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute ScalingConfigurationId: Scaling configuration id.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrScalingConfigurationId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrScalingGroupId")
     def attr_scaling_group_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute ScalingGroupId: Scaling group id.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrScalingGroupId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrScalingRuleId")
     def attr_scaling_rule_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute ScalingRuleId: Scaling rule id.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrScalingRuleId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTaskId")
     def attr_task_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute TaskId: Task ID.
 
         Automatically assigned by the system, the user queries the task status.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTaskId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrWorkerRamRoleName")
     def attr_worker_ram_role_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute WorkerRamRoleName: Worker ram role name.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrWorkerRamRoleName"))
 
 
 @jsii.data_type(
@@ -1568,28 +1673,29 @@
         "snat_entry": "snatEntry",
         "tags": "tags",
         "timeout_mins": "timeoutMins",
         "vpc_id": "vpcId",
         "v_switch_ids": "vSwitchIds",
         "worker_data_disk": "workerDataDisk",
         "worker_data_disk_category": "workerDataDiskCategory",
+        "worker_data_disks": "workerDataDisks",
         "worker_data_disk_size": "workerDataDiskSize",
         "worker_instance_types": "workerInstanceTypes",
         "worker_system_disk_category": "workerSystemDiskCategory",
         "worker_system_disk_size": "workerSystemDiskSize",
         "zone_ids": "zoneIds",
     },
 )
 class ManagedEdgeKubernetesClusterProps:
     def __init__(
         self,
         *,
         name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         num_of_nodes: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
-        addons: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosManagedEdgeKubernetesCluster.AddonsProperty"]]]] = None,
+        addons: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosManagedEdgeKubernetesCluster.AddonsProperty", typing.Dict[str, typing.Any]]]]]] = None,
         auto_renew: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         auto_renew_period: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         charge_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         cloud_monitor_flags: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         cluster_spec: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         container_cidr: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         deletion_protection: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
@@ -1602,20 +1708,21 @@
         period: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         period_unit: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         profile: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         proxy_mode: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         resource_group_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         service_cidr: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         snat_entry: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
-        tags: typing.Optional[typing.Sequence["RosManagedEdgeKubernetesCluster.TagsProperty"]] = None,
+        tags: typing.Optional[typing.Sequence[typing.Union["RosManagedEdgeKubernetesCluster.TagsProperty", typing.Dict[str, typing.Any]]]] = None,
         timeout_mins: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         vpc_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         v_switch_ids: typing.Optional[typing.Union[typing.Sequence[typing.Any], ros_cdk_core.IResolvable]] = None,
         worker_data_disk: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         worker_data_disk_category: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
+        worker_data_disks: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosManagedEdgeKubernetesCluster.WorkerDataDisksProperty", typing.Dict[str, typing.Any]]]]]] = None,
         worker_data_disk_size: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         worker_instance_types: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]] = None,
         worker_system_disk_category: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         worker_system_disk_size: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         zone_ids: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::CS::ManagedEdgeKubernetesCluster``.
@@ -1632,33 +1739,71 @@
         :param deletion_protection: Property deletionProtection: Specifies whether to enable deletion protection for the cluster. After deletion protection is enabled, the cluster cannot be deleted in the ACK console or by calling API operations. Valid values:true: enables deletion protection for the cluster. false: disables deletion protection for the cluster. Default value: false.
         :param disable_rollback: Property disableRollback: Whether the failure was rolled back: true: indicates that it fails to roll back false: rollback failed The default is true. If rollback fails, resources produced during the creation process will be released. False is not recommended.
         :param endpoint_public_access: Property endpointPublicAccess: Whether to enable the public network API Server: true: which means that the public network API Server is open. false: If set to false, the API server on the public network will not be created, only the API server on the private network will be created.Default to true.
         :param is_enterprise_security_group: Property isEnterpriseSecurityGroup: Specifies whether to create an advanced security group. This parameter takes effect only if security_group_id is left empty. Note You must specify an advanced security group for a cluster that has Terway installed. true: creates an advanced security group. false: does not create an advanced security group. Default value: false.
         :param key_pair: Property keyPair: Key pair name. Specify one of KeyPair or LoginPassword.
         :param login_password: Property loginPassword: SSH login password. Password rules are 8-30 characters and contain three items (upper and lower case letters, numbers, and special symbols). Specify one of KeyPair or LoginPassword.
         :param node_cidr_mask: Property nodeCidrMask: The maximum number of IP addresses that can be assigned to nodes. This number is determined by the specified pod CIDR block. This parameter takes effect only if the cluster uses the Flannel plug-in.Default value: 25.
-        :param period: Property period: The duration of the annual subscription and monthly subscription. It takes effect when the ChargeType value is PrePaid and is a required value. The value range is: When PeriodUnit = Week, Period values are: {"1", "2", "3", "4"} When PeriodUnit = Month, Period values are: {"1", "2", "3", "4", "5", "6", "7", "8", "9", "12", "24", "36", "48", "60"} Default to 1.
-        :param period_unit: Property periodUnit: When you specify PrePaid, you need to specify the period. The options are: Week: Time is measured in weeks Month: time in months Default to Month
+        :param period: Property period: The duration of the annual subscription and monthly subscription. It takes effect when the ChargeType value is PrePaid and is a required value. The value range is: When PeriodUnit = Week, Period values are: {"1", "2", "3", "4"} When PeriodUnit = Month, Period values are: {"1", "2", "3", "4", "5", "6", "7", "8", "9", "12", "24", "36", "48", "60"} When PeriodUnit = Year, Period values are: {"1", "2", "3", "4", "5"} Default to 1.
+        :param period_unit: Property periodUnit: When you specify PrePaid, you need to specify the period. The options are: Week: Time is measured in weeks Month: time in months Year: time in years Default to Month
         :param profile: Property profile: Edge cluster ID. The default value is Edge.
         :param proxy_mode: Property proxyMode: kube-proxy proxy mode, supports both iptables and ipvs modes. The default is iptables.
         :param resource_group_id: Property resourceGroupId: The ID of resource group.
         :param service_cidr: Property serviceCidr: The service network segment cannot conflict with the VPC network segment and the container network segment. When the system is selected to automatically create a VPC, the network segment 172.19.0.0/20 is used by default.
         :param snat_entry: Property snatEntry: Whether to configure SNAT for the network. When a VPC can access the public network environment, set it to false. When an existing VPC cannot access the public network environment: When set to True, SNAT is configured and the public network environment can be accessed at this time. If set to false, it means that SNAT is not configured and the public network environment cannot be accessed at this time. Default to true.
         :param tags: Property tags: Tag the cluster.
         :param timeout_mins: Property timeoutMins: Cluster resource stack creation timeout, in minutes. The default value is 60.
         :param vpc_id: Property vpcId: VPC ID. If not set, the system will automatically create a VPC, and the VPC network segment created by the system is 192.168.0.0/16. VpcId and VSwitchId can only be empty at the same time or set the corresponding values at the same time.
         :param v_switch_ids: Property vSwitchIds: The virtual switch ID of the worker node.
         :param worker_data_disk: Property workerDataDisk: Whether to mount the data disk. The options are as follows: true: indicates that the worker node mounts data disks. false: indicates that the worker node does not mount data disks. Default to false.
         :param worker_data_disk_category: Property workerDataDiskCategory: Data disk type.
+        :param worker_data_disks: Property workerDataDisks: A combination of configurations such as worker data disk type and size. This parameter is valid only when the worker node data disk is mounted.
         :param worker_data_disk_size: Property workerDataDiskSize: Data disk size in GiB.
         :param worker_instance_types: Property workerInstanceTypes: Worker node ECS specification type code. For more details, see Instance Specification Family.
         :param worker_system_disk_category: Property workerSystemDiskCategory: Worker node system disk type. Default to cloud_efficiency.
         :param worker_system_disk_size: Property workerSystemDiskSize: Worker disk system disk size, the unit is GiB. Default to 120.
         :param zone_ids: Property zoneIds: Zone ids of worker node virtual switches belongs to.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(ManagedEdgeKubernetesClusterProps.__init__)
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+            check_type(argname="argument num_of_nodes", value=num_of_nodes, expected_type=type_hints["num_of_nodes"])
+            check_type(argname="argument addons", value=addons, expected_type=type_hints["addons"])
+            check_type(argname="argument auto_renew", value=auto_renew, expected_type=type_hints["auto_renew"])
+            check_type(argname="argument auto_renew_period", value=auto_renew_period, expected_type=type_hints["auto_renew_period"])
+            check_type(argname="argument charge_type", value=charge_type, expected_type=type_hints["charge_type"])
+            check_type(argname="argument cloud_monitor_flags", value=cloud_monitor_flags, expected_type=type_hints["cloud_monitor_flags"])
+            check_type(argname="argument cluster_spec", value=cluster_spec, expected_type=type_hints["cluster_spec"])
+            check_type(argname="argument container_cidr", value=container_cidr, expected_type=type_hints["container_cidr"])
+            check_type(argname="argument deletion_protection", value=deletion_protection, expected_type=type_hints["deletion_protection"])
+            check_type(argname="argument disable_rollback", value=disable_rollback, expected_type=type_hints["disable_rollback"])
+            check_type(argname="argument endpoint_public_access", value=endpoint_public_access, expected_type=type_hints["endpoint_public_access"])
+            check_type(argname="argument is_enterprise_security_group", value=is_enterprise_security_group, expected_type=type_hints["is_enterprise_security_group"])
+            check_type(argname="argument key_pair", value=key_pair, expected_type=type_hints["key_pair"])
+            check_type(argname="argument login_password", value=login_password, expected_type=type_hints["login_password"])
+            check_type(argname="argument node_cidr_mask", value=node_cidr_mask, expected_type=type_hints["node_cidr_mask"])
+            check_type(argname="argument period", value=period, expected_type=type_hints["period"])
+            check_type(argname="argument period_unit", value=period_unit, expected_type=type_hints["period_unit"])
+            check_type(argname="argument profile", value=profile, expected_type=type_hints["profile"])
+            check_type(argname="argument proxy_mode", value=proxy_mode, expected_type=type_hints["proxy_mode"])
+            check_type(argname="argument resource_group_id", value=resource_group_id, expected_type=type_hints["resource_group_id"])
+            check_type(argname="argument service_cidr", value=service_cidr, expected_type=type_hints["service_cidr"])
+            check_type(argname="argument snat_entry", value=snat_entry, expected_type=type_hints["snat_entry"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
+            check_type(argname="argument timeout_mins", value=timeout_mins, expected_type=type_hints["timeout_mins"])
+            check_type(argname="argument vpc_id", value=vpc_id, expected_type=type_hints["vpc_id"])
+            check_type(argname="argument v_switch_ids", value=v_switch_ids, expected_type=type_hints["v_switch_ids"])
+            check_type(argname="argument worker_data_disk", value=worker_data_disk, expected_type=type_hints["worker_data_disk"])
+            check_type(argname="argument worker_data_disk_category", value=worker_data_disk_category, expected_type=type_hints["worker_data_disk_category"])
+            check_type(argname="argument worker_data_disks", value=worker_data_disks, expected_type=type_hints["worker_data_disks"])
+            check_type(argname="argument worker_data_disk_size", value=worker_data_disk_size, expected_type=type_hints["worker_data_disk_size"])
+            check_type(argname="argument worker_instance_types", value=worker_instance_types, expected_type=type_hints["worker_instance_types"])
+            check_type(argname="argument worker_system_disk_category", value=worker_system_disk_category, expected_type=type_hints["worker_system_disk_category"])
+            check_type(argname="argument worker_system_disk_size", value=worker_system_disk_size, expected_type=type_hints["worker_system_disk_size"])
+            check_type(argname="argument zone_ids", value=zone_ids, expected_type=type_hints["zone_ids"])
         self._values: typing.Dict[str, typing.Any] = {
             "name": name,
             "num_of_nodes": num_of_nodes,
         }
         if addons is not None:
             self._values["addons"] = addons
         if auto_renew is not None:
@@ -1709,14 +1854,16 @@
             self._values["vpc_id"] = vpc_id
         if v_switch_ids is not None:
             self._values["v_switch_ids"] = v_switch_ids
         if worker_data_disk is not None:
             self._values["worker_data_disk"] = worker_data_disk
         if worker_data_disk_category is not None:
             self._values["worker_data_disk_category"] = worker_data_disk_category
+        if worker_data_disks is not None:
+            self._values["worker_data_disks"] = worker_data_disks
         if worker_data_disk_size is not None:
             self._values["worker_data_disk_size"] = worker_data_disk_size
         if worker_instance_types is not None:
             self._values["worker_instance_types"] = worker_instance_types
         if worker_system_disk_category is not None:
             self._values["worker_system_disk_category"] = worker_system_disk_category
         if worker_system_disk_size is not None:
@@ -1911,28 +2058,30 @@
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''Property period: The duration of the annual subscription and monthly subscription.
 
         It takes effect when the ChargeType value is PrePaid and is a required value. The value range is:
         When PeriodUnit = Week, Period values are: {"1", "2", "3", "4"}
         When PeriodUnit = Month, Period values are: {"1", "2", "3", "4", "5", "6", "7", "8", "9", "12", "24", "36", "48", "60"}
+        When PeriodUnit = Year, Period values are: {"1", "2", "3", "4", "5"}
         Default to 1.
         '''
         result = self._values.get("period")
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], result)
 
     @builtins.property
     def period_unit(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''Property periodUnit: When you specify PrePaid, you need to specify the period.
 
         The options are:
         Week: Time is measured in weeks
         Month: time in months
+        Year: time in years
         Default to Month
         '''
         result = self._values.get("period_unit")
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], result)
 
     @builtins.property
     def profile(
@@ -2048,14 +2197,25 @@
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''Property workerDataDiskCategory: Data disk type.'''
         result = self._values.get("worker_data_disk_category")
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], result)
 
     @builtins.property
+    def worker_data_disks(
+        self,
+    ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosManagedEdgeKubernetesCluster.WorkerDataDisksProperty"]]]]:
+        '''Property workerDataDisks: A combination of configurations such as worker data disk type and size.
+
+        This parameter is valid only when the worker node data disk is mounted.
+        '''
+        result = self._values.get("worker_data_disks")
+        return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosManagedEdgeKubernetesCluster.WorkerDataDisksProperty"]]]], result)
+
+    @builtins.property
     def worker_data_disk_size(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''Property workerDataDiskSize: Data disk size in GiB.'''
         result = self._values.get("worker_data_disk_size")
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], result)
 
@@ -2119,88 +2279,94 @@
 ):
     '''A ROS resource type:  ``ALIYUN::CS::ManagedKubernetesCluster``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "ManagedKubernetesClusterProps",
+        props: typing.Union["ManagedKubernetesClusterProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::CS::ManagedKubernetesCluster``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(ManagedKubernetesCluster.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrApiServerSlbId")
     def attr_api_server_slb_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute APIServerSLBId: The id of API server SLB.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrApiServerSlbId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrClusterId")
     def attr_cluster_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute ClusterId: Cluster instance ID.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrClusterId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDefaultUserKubeConfig")
     def attr_default_user_kube_config(self) -> ros_cdk_core.IResolvable:
         '''Attribute DefaultUserKubeConfig: Default user kubernetes config which is used for configuring cluster credentials.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDefaultUserKubeConfig"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrNodes")
     def attr_nodes(self) -> ros_cdk_core.IResolvable:
         '''Attribute Nodes: The list of cluster nodes.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrNodes"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPrivateUserKubConfig")
     def attr_private_user_kub_config(self) -> ros_cdk_core.IResolvable:
         '''Attribute PrivateUserKubConfig: Private user kubernetes config which is used for configuring cluster credentials.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPrivateUserKubConfig"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrScalingConfigurationId")
     def attr_scaling_configuration_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute ScalingConfigurationId: Scaling configuration id.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrScalingConfigurationId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrScalingGroupId")
     def attr_scaling_group_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute ScalingGroupId: Scaling group id.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrScalingGroupId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrScalingRuleId")
     def attr_scaling_rule_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute ScalingRuleId: Scaling rule id.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrScalingRuleId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTaskId")
     def attr_task_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute TaskId: Task ID.
 
         Automatically assigned by the system, the user queries the task status.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTaskId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrWorkerRamRoleName")
     def attr_worker_ram_role_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute WorkerRamRoleName: Worker ram role name.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrWorkerRamRoleName"))
 
 
 @jsii.data_type(
@@ -2260,15 +2426,15 @@
 class ManagedKubernetesClusterProps:
     def __init__(
         self,
         *,
         name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         vpc_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         v_switch_ids: typing.Union[typing.Sequence[typing.Any], ros_cdk_core.IResolvable],
-        addons: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosManagedKubernetesCluster.AddonsProperty"]]]] = None,
+        addons: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosManagedKubernetesCluster.AddonsProperty", typing.Dict[str, typing.Any]]]]]] = None,
         auto_renew: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         auto_renew_period: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         charge_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         cis_enabled: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         cloud_monitor_flags: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         cluster_spec: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         container_cidr: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
@@ -2281,34 +2447,34 @@
         keep_instance_name: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         key_pair: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         kubernetes_version: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         load_balancer_spec: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         login_password: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         node_cidr_mask: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         node_name_mode: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        node_pools: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosManagedKubernetesCluster.NodePoolsProperty"]]]] = None,
+        node_pools: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosManagedKubernetesCluster.NodePoolsProperty", typing.Dict[str, typing.Any]]]]]] = None,
         num_of_nodes: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         os_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         period: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         period_unit: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         platform: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         pod_vswitch_ids: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]] = None,
         proxy_mode: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         resource_group_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        runtime: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosManagedKubernetesCluster.RuntimeProperty"]] = None,
+        runtime: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosManagedKubernetesCluster.RuntimeProperty", typing.Dict[str, typing.Any]]]] = None,
         security_group_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         service_cidr: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         snat_entry: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         soc_enabled: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
-        tags: typing.Optional[typing.Sequence["RosManagedKubernetesCluster.TagsProperty"]] = None,
+        tags: typing.Optional[typing.Sequence[typing.Union["RosManagedKubernetesCluster.TagsProperty", typing.Dict[str, typing.Any]]]] = None,
         taint: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Mapping[builtins.str, typing.Any]]]] = None,
         timeout_mins: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         user_data: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         worker_data_disk: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
-        worker_data_disks: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosManagedKubernetesCluster.WorkerDataDisksProperty"]]]] = None,
+        worker_data_disks: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosManagedKubernetesCluster.WorkerDataDisksProperty", typing.Dict[str, typing.Any]]]]]] = None,
         worker_instance_types: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]] = None,
         worker_system_disk_category: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         worker_system_disk_size: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         zone_ids: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::CS::ManagedKubernetesCluster``.
 
@@ -2335,16 +2501,16 @@
         :param load_balancer_spec: Property loadBalancerSpec: The specification of the Server Load Balancer instance. Allowed value: slb.s1.small|slb.s2.small|slb.s2.medium|slb.s3.small|slb.s3.medium|slb.s3.large
         :param login_password: Property loginPassword: SSH login password. Password rules are 8-30 characters and contain three items (upper and lower case letters, numbers, and special symbols). Specify one of KeyPair or LoginPassword.
         :param node_cidr_mask: Property nodeCidrMask: The maximum number of IP addresses that can be assigned to nodes. This number is determined by the specified pod CIDR block. This parameter takes effect only if the cluster uses the Flannel plug-in.Default value: 25.
         :param node_name_mode: Property nodeNameMode: A custom node name consists of a prefix, an IP substring, and a suffix. The format iscustomized,{prefix},{ip_substring},{suffix}, for example: customized,aliyun.com,5,test. - The prefix and suffix can contain one or more parts that are separated by periods (.). Each part can contain lowercase letters, digits, and hyphens (-). The node name must start and end with a lowercase letter or digit. - The IP substring length specifies the number of digits to be truncated from the end of the node IP address. Valid values: 5 to 12. For example, if the node IP address is 192.168.0.55, the prefix is aliyun.com, the IP substring length is 5, and the suffix is test, the node name will be aliyun.com00055test.
         :param node_pools: Property nodePools: The configurations of Node pools.
         :param num_of_nodes: Property numOfNodes: Number of worker nodes. The range is [0,300]. Default to 3.
         :param os_type: Property osType: The type of operating system. Valid values: Windows Linux Default value: Linux.
-        :param period: Property period: The duration of the annual subscription and monthly subscription. It takes effect when the ChargeType value is PrePaid and is a required value. The value range is: When PeriodUnit = Week, Period values are: {"1", "2", "3", "4"} When PeriodUnit = Month, Period values are: {"1", "2", "3", "4", "5", "6", "7", "8", "9", "12", "24", "36", "48", "60"} Default to 1.
-        :param period_unit: Property periodUnit: When you specify PrePaid, you need to specify the period. The options are: Week: Time is measured in weeks Month: time in months Default to Month
+        :param period: Property period: The duration of the annual subscription and monthly subscription. It takes effect when the ChargeType value is PrePaid and is a required value. The value range is: When PeriodUnit = Week, Period values are: {"1", "2", "3", "4"} When PeriodUnit = Month, Period values are: {"1", "2", "3", "4", "5", "6", "7", "8", "9", "12", "24", "36", "48", "60"} When PeriodUnit = Year, Period values are: {"1", "2", "3", "4", "5"} Default to 1.
+        :param period_unit: Property periodUnit: When you specify PrePaid, you need to specify the period. The options are: Week: Time is measured in weeks Month: time in months Year: time in years Default to Month
         :param platform: Property platform: The release version of the operating system. Valid values: CentOS AliyunLinux QbootAliyunLinux Qboot Windows WindowsCore Default value: CentOS.
         :param pod_vswitch_ids: Property podVswitchIds: The list of pod vSwitches. For each vSwitch that is allocated to nodes, you must specify at least one pod vSwitch in the same zone. The pod vSwitches cannot be the same as the node vSwitches. We recommend that you set the mask length of the CIDR block to a value no greater than 19 for the pod vSwitches. The pod_vswitch_ids parameter is required when the Terway network plug-in is selected for the cluster.
         :param proxy_mode: Property proxyMode: kube-proxy proxy mode, supports both iptables and ipvs modes. The default is iptables.
         :param resource_group_id: Property resourceGroupId: The ID of resource group.
         :param runtime: Property runtime: The container runtime of the cluster. The default runtime is Docker.
         :param security_group_id: Property securityGroupId: Specifies the ID of the security group to which the cluster ECS instance belongs.
         :param service_cidr: Property serviceCidr: The service network segment cannot conflict with the VPC network segment and the container network segment. When the system is selected to automatically create a VPC, the network segment 172.19.0.0/20 is used by default.
@@ -2357,14 +2523,64 @@
         :param worker_data_disk: Property workerDataDisk: Whether to mount the data disk. The options are as follows: true: indicates that the worker node mounts data disks. false: indicates that the worker node does not mount data disks. Default to false.
         :param worker_data_disks: Property workerDataDisks: A combination of configurations such as worker data disk type and size. This parameter is valid only when the worker node data disk is mounted.
         :param worker_instance_types: Property workerInstanceTypes: Worker node ECS specification type code. For more details, see Instance Specification Family.
         :param worker_system_disk_category: Property workerSystemDiskCategory: Worker node system disk type. The value includes: cloud_efficiency: efficient cloud disk cloud_ssd: SSD cloud disk Default to cloud_efficiency.
         :param worker_system_disk_size: Property workerSystemDiskSize: Worker disk system disk size, the unit is GiB. Default to 120.
         :param zone_ids: Property zoneIds: Zone ids of worker node virtual switches belongs to.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(ManagedKubernetesClusterProps.__init__)
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+            check_type(argname="argument vpc_id", value=vpc_id, expected_type=type_hints["vpc_id"])
+            check_type(argname="argument v_switch_ids", value=v_switch_ids, expected_type=type_hints["v_switch_ids"])
+            check_type(argname="argument addons", value=addons, expected_type=type_hints["addons"])
+            check_type(argname="argument auto_renew", value=auto_renew, expected_type=type_hints["auto_renew"])
+            check_type(argname="argument auto_renew_period", value=auto_renew_period, expected_type=type_hints["auto_renew_period"])
+            check_type(argname="argument charge_type", value=charge_type, expected_type=type_hints["charge_type"])
+            check_type(argname="argument cis_enabled", value=cis_enabled, expected_type=type_hints["cis_enabled"])
+            check_type(argname="argument cloud_monitor_flags", value=cloud_monitor_flags, expected_type=type_hints["cloud_monitor_flags"])
+            check_type(argname="argument cluster_spec", value=cluster_spec, expected_type=type_hints["cluster_spec"])
+            check_type(argname="argument container_cidr", value=container_cidr, expected_type=type_hints["container_cidr"])
+            check_type(argname="argument deletion_protection", value=deletion_protection, expected_type=type_hints["deletion_protection"])
+            check_type(argname="argument disable_rollback", value=disable_rollback, expected_type=type_hints["disable_rollback"])
+            check_type(argname="argument encryption_provider_key", value=encryption_provider_key, expected_type=type_hints["encryption_provider_key"])
+            check_type(argname="argument endpoint_public_access", value=endpoint_public_access, expected_type=type_hints["endpoint_public_access"])
+            check_type(argname="argument format_disk", value=format_disk, expected_type=type_hints["format_disk"])
+            check_type(argname="argument is_enterprise_security_group", value=is_enterprise_security_group, expected_type=type_hints["is_enterprise_security_group"])
+            check_type(argname="argument keep_instance_name", value=keep_instance_name, expected_type=type_hints["keep_instance_name"])
+            check_type(argname="argument key_pair", value=key_pair, expected_type=type_hints["key_pair"])
+            check_type(argname="argument kubernetes_version", value=kubernetes_version, expected_type=type_hints["kubernetes_version"])
+            check_type(argname="argument load_balancer_spec", value=load_balancer_spec, expected_type=type_hints["load_balancer_spec"])
+            check_type(argname="argument login_password", value=login_password, expected_type=type_hints["login_password"])
+            check_type(argname="argument node_cidr_mask", value=node_cidr_mask, expected_type=type_hints["node_cidr_mask"])
+            check_type(argname="argument node_name_mode", value=node_name_mode, expected_type=type_hints["node_name_mode"])
+            check_type(argname="argument node_pools", value=node_pools, expected_type=type_hints["node_pools"])
+            check_type(argname="argument num_of_nodes", value=num_of_nodes, expected_type=type_hints["num_of_nodes"])
+            check_type(argname="argument os_type", value=os_type, expected_type=type_hints["os_type"])
+            check_type(argname="argument period", value=period, expected_type=type_hints["period"])
+            check_type(argname="argument period_unit", value=period_unit, expected_type=type_hints["period_unit"])
+            check_type(argname="argument platform", value=platform, expected_type=type_hints["platform"])
+            check_type(argname="argument pod_vswitch_ids", value=pod_vswitch_ids, expected_type=type_hints["pod_vswitch_ids"])
+            check_type(argname="argument proxy_mode", value=proxy_mode, expected_type=type_hints["proxy_mode"])
+            check_type(argname="argument resource_group_id", value=resource_group_id, expected_type=type_hints["resource_group_id"])
+            check_type(argname="argument runtime", value=runtime, expected_type=type_hints["runtime"])
+            check_type(argname="argument security_group_id", value=security_group_id, expected_type=type_hints["security_group_id"])
+            check_type(argname="argument service_cidr", value=service_cidr, expected_type=type_hints["service_cidr"])
+            check_type(argname="argument snat_entry", value=snat_entry, expected_type=type_hints["snat_entry"])
+            check_type(argname="argument soc_enabled", value=soc_enabled, expected_type=type_hints["soc_enabled"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
+            check_type(argname="argument taint", value=taint, expected_type=type_hints["taint"])
+            check_type(argname="argument timeout_mins", value=timeout_mins, expected_type=type_hints["timeout_mins"])
+            check_type(argname="argument user_data", value=user_data, expected_type=type_hints["user_data"])
+            check_type(argname="argument worker_data_disk", value=worker_data_disk, expected_type=type_hints["worker_data_disk"])
+            check_type(argname="argument worker_data_disks", value=worker_data_disks, expected_type=type_hints["worker_data_disks"])
+            check_type(argname="argument worker_instance_types", value=worker_instance_types, expected_type=type_hints["worker_instance_types"])
+            check_type(argname="argument worker_system_disk_category", value=worker_system_disk_category, expected_type=type_hints["worker_system_disk_category"])
+            check_type(argname="argument worker_system_disk_size", value=worker_system_disk_size, expected_type=type_hints["worker_system_disk_size"])
+            check_type(argname="argument zone_ids", value=zone_ids, expected_type=type_hints["zone_ids"])
         self._values: typing.Dict[str, typing.Any] = {
             "name": name,
             "vpc_id": vpc_id,
             "v_switch_ids": v_switch_ids,
         }
         if addons is not None:
             self._values["addons"] = addons
@@ -2783,28 +2999,30 @@
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''Property period: The duration of the annual subscription and monthly subscription.
 
         It takes effect when the ChargeType value is PrePaid and is a required value. The value range is:
         When PeriodUnit = Week, Period values are: {"1", "2", "3", "4"}
         When PeriodUnit = Month, Period values are: {"1", "2", "3", "4", "5", "6", "7", "8", "9", "12", "24", "36", "48", "60"}
+        When PeriodUnit = Year, Period values are: {"1", "2", "3", "4", "5"}
         Default to 1.
         '''
         result = self._values.get("period")
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], result)
 
     @builtins.property
     def period_unit(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''Property periodUnit: When you specify PrePaid, you need to specify the period.
 
         The options are:
         Week: Time is measured in weeks
         Month: time in months
+        Year: time in years
         Default to Month
         '''
         result = self._values.get("period_unit")
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], result)
 
     @builtins.property
     def platform(
@@ -3046,151 +3264,166 @@
 ):
     '''A ROS template type:  ``ALIYUN::CS::AnyCluster``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosAnyClusterProps",
+        props: typing.Union["RosAnyClusterProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::CS::AnyCluster``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosAnyCluster.__init__)
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
+            type_hints = typing.get_type_hints(RosAnyCluster._render_properties)
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
     @jsii.member(jsii_name="attrApiServerSlbId")
     def attr_api_server_slb_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: APIServerSLBId: The id of API server SLB
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrApiServerSlbId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrClusterId")
     def attr_cluster_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ClusterId: Cluster instance ID.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrClusterId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDefaultUserKubeConfig")
     def attr_default_user_kube_config(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: DefaultUserKubeConfig: Default user kubernetes config which is used for configuring cluster credentials.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDefaultUserKubeConfig"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrNodes")
     def attr_nodes(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Nodes: The list of cluster nodes.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrNodes"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPrivateUserKubConfig")
     def attr_private_user_kub_config(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: PrivateUserKubConfig: Private user kubernetes config which is used for configuring cluster credentials.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPrivateUserKubConfig"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrScalingConfigurationId")
     def attr_scaling_configuration_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ScalingConfigurationId: Scaling configuration id
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrScalingConfigurationId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrScalingGroupId")
     def attr_scaling_group_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ScalingGroupId: Scaling group id
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrScalingGroupId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrScalingRuleId")
     def attr_scaling_rule_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ScalingRuleId: Scaling rule id
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrScalingRuleId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTaskId")
     def attr_task_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: TaskId: Task ID. Automatically assigned by the system, the user queries the task status.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTaskId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrWorkerRamRoleName")
     def attr_worker_ram_role_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: WorkerRamRoleName: Worker ram role name.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrWorkerRamRoleName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="clusterConfig")
     def cluster_config(
         self,
     ) -> typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]]:
         '''
         :Property: clusterConfig: Cluster config.
         '''
         return typing.cast(typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]], jsii.get(self, "clusterConfig"))
 
     @cluster_config.setter
     def cluster_config(
         self,
         value: typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAnyCluster, "cluster_config").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "clusterConfig", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAnyCluster, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-cs.RosAnyClusterProps",
     jsii_struct_bases=[],
     name_mapping={"cluster_config": "clusterConfig"},
@@ -3201,14 +3434,17 @@
         *,
         cluster_config: typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]],
     ) -> None:
         '''Properties for defining a ``ALIYUN::CS::AnyCluster``.
 
         :param cluster_config: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosAnyClusterProps.__init__)
+            check_type(argname="argument cluster_config", value=cluster_config, expected_type=type_hints["cluster_config"])
         self._values: typing.Dict[str, typing.Any] = {
             "cluster_config": cluster_config,
         }
 
     @builtins.property
     def cluster_config(
         self,
@@ -3239,196 +3475,232 @@
 ):
     '''A ROS template type:  ``ALIYUN::CS::ClusterNodePool``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosClusterNodePoolProps",
+        props: typing.Union["RosClusterNodePoolProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::CS::ClusterNodePool``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosClusterNodePool.__init__)
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
+            type_hints = typing.get_type_hints(RosClusterNodePool._render_properties)
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
     @jsii.member(jsii_name="attrNodePoolId")
     def attr_node_pool_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: NodePoolId: Cluster node pool ID.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrNodePoolId"))
 
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
         :Property: clusterId: Cluster ID.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "clusterId"))
 
     @cluster_id.setter
     def cluster_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosClusterNodePool, "cluster_id").fset)
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
+            type_hints = typing.get_type_hints(getattr(RosClusterNodePool, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="scalingGroup")
     def scaling_group(
         self,
     ) -> typing.Union[ros_cdk_core.IResolvable, "RosClusterNodePool.ScalingGroupProperty"]:
         '''
         :Property: scalingGroup: The configurations of the scaling group used by the node pool.
         '''
         return typing.cast(typing.Union[ros_cdk_core.IResolvable, "RosClusterNodePool.ScalingGroupProperty"], jsii.get(self, "scalingGroup"))
 
     @scaling_group.setter
     def scaling_group(
         self,
         value: typing.Union[ros_cdk_core.IResolvable, "RosClusterNodePool.ScalingGroupProperty"],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosClusterNodePool, "scaling_group").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "scalingGroup", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="autoScaling")
     def auto_scaling(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosClusterNodePool.AutoScalingProperty"]]:
         '''
         :Property: autoScaling: The configurations of auto scaling.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosClusterNodePool.AutoScalingProperty"]], jsii.get(self, "autoScaling"))
 
     @auto_scaling.setter
     def auto_scaling(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosClusterNodePool.AutoScalingProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosClusterNodePool, "auto_scaling").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "autoScaling", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="count")
     def count(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: count: The number of nodes in the node pool.
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "count"))
 
     @count.setter
     def count(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosClusterNodePool, "count").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "count", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="kubernetesConfig")
     def kubernetes_config(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosClusterNodePool.KubernetesConfigProperty"]]:
         '''
         :Property: kubernetesConfig: The configurations of the ACK cluster.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosClusterNodePool.KubernetesConfigProperty"]], jsii.get(self, "kubernetesConfig"))
 
     @kubernetes_config.setter
     def kubernetes_config(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosClusterNodePool.KubernetesConfigProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosClusterNodePool, "kubernetes_config").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "kubernetesConfig", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="management")
     def management(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosClusterNodePool.ManagementProperty"]]:
         '''
         :Property: management: The configurations of the managed node pool.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosClusterNodePool.ManagementProperty"]], jsii.get(self, "management"))
 
     @management.setter
     def management(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosClusterNodePool.ManagementProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosClusterNodePool, "management").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "management", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="nodePoolInfo")
     def node_pool_info(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosClusterNodePool.NodePoolInfoProperty"]]:
         '''
         :Property: nodePoolInfo: The configurations of the node pool.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosClusterNodePool.NodePoolInfoProperty"]], jsii.get(self, "nodePoolInfo"))
 
     @node_pool_info.setter
     def node_pool_info(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosClusterNodePool.NodePoolInfoProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosClusterNodePool, "node_pool_info").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "nodePoolInfo", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="teeConfig")
     def tee_config(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosClusterNodePool.TeeConfigProperty"]]:
         '''
         :Property: teeConfig: The configurations of confidential computing.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosClusterNodePool.TeeConfigProperty"]], jsii.get(self, "teeConfig"))
 
     @tee_config.setter
     def tee_config(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosClusterNodePool.TeeConfigProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosClusterNodePool, "tee_config").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "teeConfig", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-cs.RosClusterNodePool.AutoScalingProperty",
         jsii_struct_bases=[],
         name_mapping={
             "enable": "enable",
@@ -3457,14 +3729,23 @@
             :param eip_bandwidth: 
             :param eip_internet_charge_type: 
             :param is_bond_eip: 
             :param max_instances: 
             :param min_instances: 
             :param type: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosClusterNodePool.AutoScalingProperty.__init__)
+                check_type(argname="argument enable", value=enable, expected_type=type_hints["enable"])
+                check_type(argname="argument eip_bandwidth", value=eip_bandwidth, expected_type=type_hints["eip_bandwidth"])
+                check_type(argname="argument eip_internet_charge_type", value=eip_internet_charge_type, expected_type=type_hints["eip_internet_charge_type"])
+                check_type(argname="argument is_bond_eip", value=is_bond_eip, expected_type=type_hints["is_bond_eip"])
+                check_type(argname="argument max_instances", value=max_instances, expected_type=type_hints["max_instances"])
+                check_type(argname="argument min_instances", value=min_instances, expected_type=type_hints["min_instances"])
+                check_type(argname="argument type", value=type, expected_type=type_hints["type"])
             self._values: typing.Dict[str, typing.Any] = {
                 "enable": enable,
             }
             if eip_bandwidth is not None:
                 self._values["eip_bandwidth"] = eip_bandwidth
             if eip_internet_charge_type is not None:
                 self._values["eip_internet_charge_type"] = eip_internet_charge_type
@@ -3603,14 +3884,21 @@
             '''
             :param auto_snapshot_policy_id: 
             :param category: 
             :param encrypted: 
             :param performance_level: 
             :param size: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosClusterNodePool.DataDisksProperty.__init__)
+                check_type(argname="argument auto_snapshot_policy_id", value=auto_snapshot_policy_id, expected_type=type_hints["auto_snapshot_policy_id"])
+                check_type(argname="argument category", value=category, expected_type=type_hints["category"])
+                check_type(argname="argument encrypted", value=encrypted, expected_type=type_hints["encrypted"])
+                check_type(argname="argument performance_level", value=performance_level, expected_type=type_hints["performance_level"])
+                check_type(argname="argument size", value=size, expected_type=type_hints["size"])
             self._values: typing.Dict[str, typing.Any] = {}
             if auto_snapshot_policy_id is not None:
                 self._values["auto_snapshot_policy_id"] = auto_snapshot_policy_id
             if category is not None:
                 self._values["category"] = category
             if encrypted is not None:
                 self._values["encrypted"] = encrypted
@@ -3723,31 +4011,42 @@
         def __init__(
             self,
             *,
             runtime: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             runtime_version: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             cms_enabled: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
             cpu_policy: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-            labels: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosClusterNodePool.LabelsProperty"]]]] = None,
+            labels: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosClusterNodePool.LabelsProperty", typing.Dict[str, typing.Any]]]]]] = None,
             node_name_mode: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-            taints: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosClusterNodePool.TaintsProperty"]]]] = None,
+            taints: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosClusterNodePool.TaintsProperty", typing.Dict[str, typing.Any]]]]]] = None,
             unschedulable: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
             user_data: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param runtime: 
             :param runtime_version: 
             :param cms_enabled: 
             :param cpu_policy: 
             :param labels: 
             :param node_name_mode: 
             :param taints: 
             :param unschedulable: 
             :param user_data: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosClusterNodePool.KubernetesConfigProperty.__init__)
+                check_type(argname="argument runtime", value=runtime, expected_type=type_hints["runtime"])
+                check_type(argname="argument runtime_version", value=runtime_version, expected_type=type_hints["runtime_version"])
+                check_type(argname="argument cms_enabled", value=cms_enabled, expected_type=type_hints["cms_enabled"])
+                check_type(argname="argument cpu_policy", value=cpu_policy, expected_type=type_hints["cpu_policy"])
+                check_type(argname="argument labels", value=labels, expected_type=type_hints["labels"])
+                check_type(argname="argument node_name_mode", value=node_name_mode, expected_type=type_hints["node_name_mode"])
+                check_type(argname="argument taints", value=taints, expected_type=type_hints["taints"])
+                check_type(argname="argument unschedulable", value=unschedulable, expected_type=type_hints["unschedulable"])
+                check_type(argname="argument user_data", value=user_data, expected_type=type_hints["user_data"])
             self._values: typing.Dict[str, typing.Any] = {
                 "runtime": runtime,
                 "runtime_version": runtime_version,
             }
             if cms_enabled is not None:
                 self._values["cms_enabled"] = cms_enabled
             if cpu_policy is not None:
@@ -3891,14 +4190,18 @@
             key: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         ) -> None:
             '''
             :param key: 
             :param value: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosClusterNodePool.LabelsProperty.__init__)
+                check_type(argname="argument key", value=key, expected_type=type_hints["key"])
+                check_type(argname="argument value", value=value, expected_type=type_hints["value"])
             self._values: typing.Dict[str, typing.Any] = {
                 "key": key,
                 "value": value,
             }
 
         @builtins.property
         def key(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
@@ -3940,21 +4243,26 @@
     )
     class ManagementProperty:
         def __init__(
             self,
             *,
             enable: typing.Union[builtins.bool, ros_cdk_core.IResolvable],
             auto_repair: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
-            upgrade_config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosClusterNodePool.UpgradeConfigProperty"]] = None,
+            upgrade_config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosClusterNodePool.UpgradeConfigProperty", typing.Dict[str, typing.Any]]]] = None,
         ) -> None:
             '''
             :param enable: 
             :param auto_repair: 
             :param upgrade_config: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosClusterNodePool.ManagementProperty.__init__)
+                check_type(argname="argument enable", value=enable, expected_type=type_hints["enable"])
+                check_type(argname="argument auto_repair", value=auto_repair, expected_type=type_hints["auto_repair"])
+                check_type(argname="argument upgrade_config", value=upgrade_config, expected_type=type_hints["upgrade_config"])
             self._values: typing.Dict[str, typing.Any] = {
                 "enable": enable,
             }
             if auto_repair is not None:
                 self._values["auto_repair"] = auto_repair
             if upgrade_config is not None:
                 self._values["upgrade_config"] = upgrade_config
@@ -4019,14 +4327,18 @@
             name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             resource_group_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param name: 
             :param resource_group_id: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosClusterNodePool.NodePoolInfoProperty.__init__)
+                check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+                check_type(argname="argument resource_group_id", value=resource_group_id, expected_type=type_hints["resource_group_id"])
             self._values: typing.Dict[str, typing.Any] = {
                 "name": name,
             }
             if resource_group_id is not None:
                 self._values["resource_group_id"] = resource_group_id
 
         @builtins.property
@@ -4088,27 +4400,28 @@
             "spot_instance_pools": "spotInstancePools",
             "spot_instance_remedy": "spotInstanceRemedy",
             "spot_price_limit": "spotPriceLimit",
             "spot_strategy": "spotStrategy",
             "system_disk_category": "systemDiskCategory",
             "system_disk_performance_level": "systemDiskPerformanceLevel",
             "tags": "tags",
+            "zone_ids": "zoneIds",
         },
     )
     class ScalingGroupProperty:
         def __init__(
             self,
             *,
             instance_types: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]],
             system_disk_size: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
             v_switch_ids: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]],
             auto_renew: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
             auto_renew_period: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
             compensate_with_on_demand: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
-            data_disks: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosClusterNodePool.DataDisksProperty"]]]] = None,
+            data_disks: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosClusterNodePool.DataDisksProperty", typing.Dict[str, typing.Any]]]]]] = None,
             image_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
             instance_charge_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
             internet_charge_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
             internet_max_bandwidth_out: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
             key_pair: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
             login_password: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
             multi_az_policy: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
@@ -4118,19 +4431,20 @@
             period_unit: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
             platform: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
             rds_instances: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]] = None,
             scaling_policy: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
             security_group_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
             spot_instance_pools: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
             spot_instance_remedy: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
-            spot_price_limit: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosClusterNodePool.SpotPriceLimitProperty"]]]] = None,
+            spot_price_limit: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosClusterNodePool.SpotPriceLimitProperty", typing.Dict[str, typing.Any]]]]]] = None,
             spot_strategy: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
             system_disk_category: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
             system_disk_performance_level: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-            tags: typing.Optional[typing.Sequence["RosClusterNodePool.TagsProperty"]] = None,
+            tags: typing.Optional[typing.Sequence[typing.Union["RosClusterNodePool.TagsProperty", typing.Dict[str, typing.Any]]]] = None,
+            zone_ids: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]] = None,
         ) -> None:
             '''
             :param instance_types: 
             :param system_disk_size: 
             :param v_switch_ids: 
             :param auto_renew: 
             :param auto_renew_period: 
@@ -4154,15 +4468,48 @@
             :param spot_instance_pools: 
             :param spot_instance_remedy: 
             :param spot_price_limit: 
             :param spot_strategy: 
             :param system_disk_category: 
             :param system_disk_performance_level: 
             :param tags: 
+            :param zone_ids: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosClusterNodePool.ScalingGroupProperty.__init__)
+                check_type(argname="argument instance_types", value=instance_types, expected_type=type_hints["instance_types"])
+                check_type(argname="argument system_disk_size", value=system_disk_size, expected_type=type_hints["system_disk_size"])
+                check_type(argname="argument v_switch_ids", value=v_switch_ids, expected_type=type_hints["v_switch_ids"])
+                check_type(argname="argument auto_renew", value=auto_renew, expected_type=type_hints["auto_renew"])
+                check_type(argname="argument auto_renew_period", value=auto_renew_period, expected_type=type_hints["auto_renew_period"])
+                check_type(argname="argument compensate_with_on_demand", value=compensate_with_on_demand, expected_type=type_hints["compensate_with_on_demand"])
+                check_type(argname="argument data_disks", value=data_disks, expected_type=type_hints["data_disks"])
+                check_type(argname="argument image_id", value=image_id, expected_type=type_hints["image_id"])
+                check_type(argname="argument instance_charge_type", value=instance_charge_type, expected_type=type_hints["instance_charge_type"])
+                check_type(argname="argument internet_charge_type", value=internet_charge_type, expected_type=type_hints["internet_charge_type"])
+                check_type(argname="argument internet_max_bandwidth_out", value=internet_max_bandwidth_out, expected_type=type_hints["internet_max_bandwidth_out"])
+                check_type(argname="argument key_pair", value=key_pair, expected_type=type_hints["key_pair"])
+                check_type(argname="argument login_password", value=login_password, expected_type=type_hints["login_password"])
+                check_type(argname="argument multi_az_policy", value=multi_az_policy, expected_type=type_hints["multi_az_policy"])
+                check_type(argname="argument on_demand_base_capacity", value=on_demand_base_capacity, expected_type=type_hints["on_demand_base_capacity"])
+                check_type(argname="argument on_demand_percentage_above_base_capacity", value=on_demand_percentage_above_base_capacity, expected_type=type_hints["on_demand_percentage_above_base_capacity"])
+                check_type(argname="argument period", value=period, expected_type=type_hints["period"])
+                check_type(argname="argument period_unit", value=period_unit, expected_type=type_hints["period_unit"])
+                check_type(argname="argument platform", value=platform, expected_type=type_hints["platform"])
+                check_type(argname="argument rds_instances", value=rds_instances, expected_type=type_hints["rds_instances"])
+                check_type(argname="argument scaling_policy", value=scaling_policy, expected_type=type_hints["scaling_policy"])
+                check_type(argname="argument security_group_id", value=security_group_id, expected_type=type_hints["security_group_id"])
+                check_type(argname="argument spot_instance_pools", value=spot_instance_pools, expected_type=type_hints["spot_instance_pools"])
+                check_type(argname="argument spot_instance_remedy", value=spot_instance_remedy, expected_type=type_hints["spot_instance_remedy"])
+                check_type(argname="argument spot_price_limit", value=spot_price_limit, expected_type=type_hints["spot_price_limit"])
+                check_type(argname="argument spot_strategy", value=spot_strategy, expected_type=type_hints["spot_strategy"])
+                check_type(argname="argument system_disk_category", value=system_disk_category, expected_type=type_hints["system_disk_category"])
+                check_type(argname="argument system_disk_performance_level", value=system_disk_performance_level, expected_type=type_hints["system_disk_performance_level"])
+                check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
+                check_type(argname="argument zone_ids", value=zone_ids, expected_type=type_hints["zone_ids"])
             self._values: typing.Dict[str, typing.Any] = {
                 "instance_types": instance_types,
                 "system_disk_size": system_disk_size,
                 "v_switch_ids": v_switch_ids,
             }
             if auto_renew is not None:
                 self._values["auto_renew"] = auto_renew
@@ -4212,14 +4559,16 @@
                 self._values["spot_strategy"] = spot_strategy
             if system_disk_category is not None:
                 self._values["system_disk_category"] = system_disk_category
             if system_disk_performance_level is not None:
                 self._values["system_disk_performance_level"] = system_disk_performance_level
             if tags is not None:
                 self._values["tags"] = tags
+            if zone_ids is not None:
+                self._values["zone_ids"] = zone_ids
 
         @builtins.property
         def instance_types(
             self,
         ) -> typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]:
             '''
             :Property: instanceTypes: The ECS instance types of the nodes.
@@ -4569,14 +4918,24 @@
 
             tags: Adds labels only to ECS instances.
             A key must be unique and cannot exceed 128 characters in length. Neither keys nor values can start with aliyun or acs:. Neither keys nor values can contain https:// or http://.
             '''
             result = self._values.get("tags")
             return typing.cast(typing.Optional[typing.List["RosClusterNodePool.TagsProperty"]], result)
 
+        @builtins.property
+        def zone_ids(
+            self,
+        ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]]:
+            '''
+            :Property: zoneIds: Zone ids of virtual switches belongs to.
+            '''
+            result = self._values.get("zone_ids")
+            return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]], result)
+
         def __eq__(self, rhs: typing.Any) -> builtins.bool:
             return isinstance(rhs, self.__class__) and rhs._values == self._values
 
         def __ne__(self, rhs: typing.Any) -> builtins.bool:
             return not (rhs == self)
 
         def __repr__(self) -> str:
@@ -4596,14 +4955,18 @@
             instance_type: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             price_limit: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
         ) -> None:
             '''
             :param instance_type: 
             :param price_limit: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosClusterNodePool.SpotPriceLimitProperty.__init__)
+                check_type(argname="argument instance_type", value=instance_type, expected_type=type_hints["instance_type"])
+                check_type(argname="argument price_limit", value=price_limit, expected_type=type_hints["price_limit"])
             self._values: typing.Dict[str, typing.Any] = {
                 "instance_type": instance_type,
                 "price_limit": price_limit,
             }
 
         @builtins.property
         def instance_type(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
@@ -4646,14 +5009,18 @@
             key: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         ) -> None:
             '''
             :param key: 
             :param value: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosClusterNodePool.TagsProperty.__init__)
+                check_type(argname="argument key", value=key, expected_type=type_hints["key"])
+                check_type(argname="argument value", value=value, expected_type=type_hints["value"])
             self._values: typing.Dict[str, typing.Any] = {
                 "key": key,
                 "value": value,
             }
 
         @builtins.property
         def key(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
@@ -4698,14 +5065,19 @@
             effect: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param key: 
             :param value: 
             :param effect: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosClusterNodePool.TaintsProperty.__init__)
+                check_type(argname="argument key", value=key, expected_type=type_hints["key"])
+                check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+                check_type(argname="argument effect", value=effect, expected_type=type_hints["effect"])
             self._values: typing.Dict[str, typing.Any] = {
                 "key": key,
                 "value": value,
             }
             if effect is not None:
                 self._values["effect"] = effect
 
@@ -4764,14 +5136,17 @@
             self,
             *,
             tee_enable: typing.Union[builtins.bool, ros_cdk_core.IResolvable],
         ) -> None:
             '''
             :param tee_enable: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosClusterNodePool.TeeConfigProperty.__init__)
+                check_type(argname="argument tee_enable", value=tee_enable, expected_type=type_hints["tee_enable"])
             self._values: typing.Dict[str, typing.Any] = {
                 "tee_enable": tee_enable,
             }
 
         @builtins.property
         def tee_enable(self) -> typing.Union[builtins.bool, ros_cdk_core.IResolvable]:
             '''
@@ -4813,14 +5188,20 @@
         ) -> None:
             '''
             :param auto_upgrade: 
             :param max_unavailable: 
             :param surge: 
             :param surge_percentage: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosClusterNodePool.UpgradeConfigProperty.__init__)
+                check_type(argname="argument auto_upgrade", value=auto_upgrade, expected_type=type_hints["auto_upgrade"])
+                check_type(argname="argument max_unavailable", value=max_unavailable, expected_type=type_hints["max_unavailable"])
+                check_type(argname="argument surge", value=surge, expected_type=type_hints["surge"])
+                check_type(argname="argument surge_percentage", value=surge_percentage, expected_type=type_hints["surge_percentage"])
             self._values: typing.Dict[str, typing.Any] = {}
             if auto_upgrade is not None:
                 self._values["auto_upgrade"] = auto_upgrade
             if max_unavailable is not None:
                 self._values["max_unavailable"] = max_unavailable
             if surge is not None:
                 self._values["surge"] = surge
@@ -4902,33 +5283,43 @@
     },
 )
 class RosClusterNodePoolProps:
     def __init__(
         self,
         *,
         cluster_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
-        scaling_group: typing.Union[ros_cdk_core.IResolvable, RosClusterNodePool.ScalingGroupProperty],
-        auto_scaling: typing.Optional[typing.Union[ros_cdk_core.IResolvable, RosClusterNodePool.AutoScalingProperty]] = None,
+        scaling_group: typing.Union[ros_cdk_core.IResolvable, typing.Union[RosClusterNodePool.ScalingGroupProperty, typing.Dict[str, typing.Any]]],
+        auto_scaling: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosClusterNodePool.AutoScalingProperty, typing.Dict[str, typing.Any]]]] = None,
         count: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
-        kubernetes_config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, RosClusterNodePool.KubernetesConfigProperty]] = None,
-        management: typing.Optional[typing.Union[ros_cdk_core.IResolvable, RosClusterNodePool.ManagementProperty]] = None,
-        node_pool_info: typing.Optional[typing.Union[ros_cdk_core.IResolvable, RosClusterNodePool.NodePoolInfoProperty]] = None,
-        tee_config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, RosClusterNodePool.TeeConfigProperty]] = None,
+        kubernetes_config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosClusterNodePool.KubernetesConfigProperty, typing.Dict[str, typing.Any]]]] = None,
+        management: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosClusterNodePool.ManagementProperty, typing.Dict[str, typing.Any]]]] = None,
+        node_pool_info: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosClusterNodePool.NodePoolInfoProperty, typing.Dict[str, typing.Any]]]] = None,
+        tee_config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosClusterNodePool.TeeConfigProperty, typing.Dict[str, typing.Any]]]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::CS::ClusterNodePool``.
 
         :param cluster_id: 
         :param scaling_group: 
         :param auto_scaling: 
         :param count: 
         :param kubernetes_config: 
         :param management: 
         :param node_pool_info: 
         :param tee_config: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosClusterNodePoolProps.__init__)
+            check_type(argname="argument cluster_id", value=cluster_id, expected_type=type_hints["cluster_id"])
+            check_type(argname="argument scaling_group", value=scaling_group, expected_type=type_hints["scaling_group"])
+            check_type(argname="argument auto_scaling", value=auto_scaling, expected_type=type_hints["auto_scaling"])
+            check_type(argname="argument count", value=count, expected_type=type_hints["count"])
+            check_type(argname="argument kubernetes_config", value=kubernetes_config, expected_type=type_hints["kubernetes_config"])
+            check_type(argname="argument management", value=management, expected_type=type_hints["management"])
+            check_type(argname="argument node_pool_info", value=node_pool_info, expected_type=type_hints["node_pool_info"])
+            check_type(argname="argument tee_config", value=tee_config, expected_type=type_hints["tee_config"])
         self._values: typing.Dict[str, typing.Any] = {
             "cluster_id": cluster_id,
             "scaling_group": scaling_group,
         }
         if auto_scaling is not None:
             self._values["auto_scaling"] = auto_scaling
         if count is not None:
@@ -5041,137 +5432,149 @@
 ):
     '''A ROS template type:  ``ALIYUN::CS::KubernetesCluster``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosKubernetesClusterProps",
+        props: typing.Union["RosKubernetesClusterProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::CS::KubernetesCluster``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosKubernetesCluster.__init__)
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
+            type_hints = typing.get_type_hints(RosKubernetesCluster._render_properties)
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
     @jsii.member(jsii_name="attrApiServerSlbId")
     def attr_api_server_slb_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: APIServerSLBId: The id of API server SLB
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrApiServerSlbId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrClusterId")
     def attr_cluster_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ClusterId: Cluster instance ID.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrClusterId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDefaultUserKubeConfig")
     def attr_default_user_kube_config(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: DefaultUserKubeConfig: Default user kubernetes config which is used for configuring cluster credentials.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDefaultUserKubeConfig"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrNodes")
     def attr_nodes(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Nodes: The list of cluster nodes.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrNodes"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPrivateUserKubConfig")
     def attr_private_user_kub_config(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: PrivateUserKubConfig: Private user kubernetes config which is used for configuring cluster credentials.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPrivateUserKubConfig"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrScalingConfigurationId")
     def attr_scaling_configuration_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ScalingConfigurationId: Scaling configuration id
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrScalingConfigurationId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrScalingGroupId")
     def attr_scaling_group_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ScalingGroupId: Scaling group id
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrScalingGroupId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrScalingRuleId")
     def attr_scaling_rule_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ScalingRuleId: Scaling rule id
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrScalingRuleId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTaskId")
     def attr_task_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: TaskId: Task ID. Automatically assigned by the system, the user queries the task status.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTaskId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrWorkerRamRoleName")
     def attr_worker_ram_role_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: WorkerRamRoleName: Worker ram role name.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrWorkerRamRoleName"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosKubernetesCluster, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="masterInstanceTypes")
     def master_instance_types(
         self,
     ) -> typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]:
         '''
         :Property:
 
@@ -5181,78 +5584,93 @@
         return typing.cast(typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable], jsii.get(self, "masterInstanceTypes"))
 
     @master_instance_types.setter
     def master_instance_types(
         self,
         value: typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosKubernetesCluster, "master_instance_types").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "masterInstanceTypes", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="masterVSwitchIds")
     def master_v_switch_ids(
         self,
     ) -> typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]:
         '''
         :Property: masterVSwitchIds: Master node switch ID. To ensure high availability of the cluster, it is recommended that you select 3 switches and distribute them in different Availability Zones.
         '''
         return typing.cast(typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable], jsii.get(self, "masterVSwitchIds"))
 
     @master_v_switch_ids.setter
     def master_v_switch_ids(
         self,
         value: typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosKubernetesCluster, "master_v_switch_ids").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "masterVSwitchIds", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="name")
     def name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: name: The name of the cluster. The cluster name can use uppercase and lowercase letters, Chinese characters, numbers, and dashes.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "name"))
 
     @name.setter
     def name(self, value: typing.Union[builtins.str, ros_cdk_core.IResolvable]) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosKubernetesCluster, "name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "name", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vpcId")
     def vpc_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: vpcId: VPC ID.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "vpcId"))
 
     @vpc_id.setter
     def vpc_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosKubernetesCluster, "vpc_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "vpcId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="workerVSwitchIds")
     def worker_v_switch_ids(
         self,
     ) -> typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]:
         '''
         :Property: workerVSwitchIds: The virtual switch ID of the worker node.
         '''
         return typing.cast(typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable], jsii.get(self, "workerVSwitchIds"))
 
     @worker_v_switch_ids.setter
     def worker_v_switch_ids(
         self,
         value: typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosKubernetesCluster, "worker_v_switch_ids").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "workerVSwitchIds", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="addons")
     def addons(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosKubernetesCluster.AddonsProperty"]]]]:
         '''
         :Property:
 
@@ -5264,17 +5682,20 @@
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosKubernetesCluster.AddonsProperty"]]]], jsii.get(self, "addons"))
 
     @addons.setter
     def addons(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosKubernetesCluster.AddonsProperty"]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosKubernetesCluster, "addons").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "addons", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="autoRenew")
     def auto_renew(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -5286,17 +5707,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "autoRenew"))
 
     @auto_renew.setter
     def auto_renew(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosKubernetesCluster, "auto_renew").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "autoRenew", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="autoRenewPeriod")
     def auto_renew_period(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -5308,17 +5732,20 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "autoRenewPeriod"))
 
     @auto_renew_period.setter
     def auto_renew_period(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosKubernetesCluster, "auto_renew_period").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "autoRenewPeriod", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="chargeType")
     def charge_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -5330,17 +5757,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "chargeType"))
 
     @charge_type.setter
     def charge_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosKubernetesCluster, "charge_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "chargeType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="cisEnabled")
     def cis_enabled(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -5354,17 +5784,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "cisEnabled"))
 
     @cis_enabled.setter
     def cis_enabled(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosKubernetesCluster, "cis_enabled").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "cisEnabled", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="cloudMonitorFlags")
     def cloud_monitor_flags(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -5376,51 +5809,60 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "cloudMonitorFlags"))
 
     @cloud_monitor_flags.setter
     def cloud_monitor_flags(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosKubernetesCluster, "cloud_monitor_flags").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "cloudMonitorFlags", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="containerCidr")
     def container_cidr(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: containerCidr: The container network segment cannot conflict with the VPC network segment. When the sytem is selected to automatically create a VPC, the network segment 172.16.0.0/16 is used by default.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "containerCidr"))
 
     @container_cidr.setter
     def container_cidr(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosKubernetesCluster, "container_cidr").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "containerCidr", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="cpuPolicy")
     def cpu_policy(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: cpuPolicy: CPU policy. The cluster version is 1.12.6 and above supports both static and none strategies.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "cpuPolicy"))
 
     @cpu_policy.setter
     def cpu_policy(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosKubernetesCluster, "cpu_policy").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "cpuPolicy", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="deletionProtection")
     def deletion_protection(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -5433,17 +5875,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "deletionProtection"))
 
     @deletion_protection.setter
     def deletion_protection(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosKubernetesCluster, "deletion_protection").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "deletionProtection", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="disableRollback")
     def disable_rollback(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -5455,17 +5900,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "disableRollback"))
 
     @disable_rollback.setter
     def disable_rollback(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosKubernetesCluster, "disable_rollback").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "disableRollback", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="endpointPublicAccess")
     def endpoint_public_access(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -5476,17 +5924,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "endpointPublicAccess"))
 
     @endpoint_public_access.setter
     def endpoint_public_access(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosKubernetesCluster, "endpoint_public_access").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "endpointPublicAccess", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="formatDisk")
     def format_disk(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -5507,17 +5958,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "formatDisk"))
 
     @format_disk.setter
     def format_disk(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosKubernetesCluster, "format_disk").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "formatDisk", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="isEnterpriseSecurityGroup")
     def is_enterprise_security_group(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -5531,17 +5985,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "isEnterpriseSecurityGroup"))
 
     @is_enterprise_security_group.setter
     def is_enterprise_security_group(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosKubernetesCluster, "is_enterprise_security_group").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "isEnterpriseSecurityGroup", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="keepInstanceName")
     def keep_instance_name(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -5553,102 +6010,120 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "keepInstanceName"))
 
     @keep_instance_name.setter
     def keep_instance_name(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosKubernetesCluster, "keep_instance_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "keepInstanceName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="keyPair")
     def key_pair(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: keyPair: Key pair name. Specify one of KeyPair or LoginPassword.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "keyPair"))
 
     @key_pair.setter
     def key_pair(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosKubernetesCluster, "key_pair").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "keyPair", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="kubernetesVersion")
     def kubernetes_version(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: kubernetesVersion: The version of the Kubernetes cluster.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "kubernetesVersion"))
 
     @kubernetes_version.setter
     def kubernetes_version(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosKubernetesCluster, "kubernetes_version").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "kubernetesVersion", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="loadBalancerSpec")
     def load_balancer_spec(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: loadBalancerSpec: The specification of the Server Load Balancer instance. Allowed value: slb.s1.small|slb.s2.small|slb.s2.medium|slb.s3.small|slb.s3.medium|slb.s3.large
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "loadBalancerSpec"))
 
     @load_balancer_spec.setter
     def load_balancer_spec(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosKubernetesCluster, "load_balancer_spec").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "loadBalancerSpec", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="loginPassword")
     def login_password(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: loginPassword: SSH login password. Password rules are 8-30 characters and contain three items (upper and lower case letters, numbers, and special symbols). Specify one of KeyPair or LoginPassword.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "loginPassword"))
 
     @login_password.setter
     def login_password(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosKubernetesCluster, "login_password").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "loginPassword", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="masterCount")
     def master_count(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: masterCount: Number of master instances. The value can be 3 or 5. The default value is 3.
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "masterCount"))
 
     @master_count.setter
     def master_count(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosKubernetesCluster, "master_count").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "masterCount", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="masterDataDisk")
     def master_data_disk(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -5659,34 +6134,40 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "masterDataDisk"))
 
     @master_data_disk.setter
     def master_data_disk(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosKubernetesCluster, "master_data_disk").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "masterDataDisk", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="masterDataDisks")
     def master_data_disks(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosKubernetesCluster.MasterDataDisksProperty"]]]]:
         '''
         :Property: masterDataDisks: Master data disk type, size and other configuration combinations. This parameter is valid only when the master node data disk is mounted.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosKubernetesCluster.MasterDataDisksProperty"]]]], jsii.get(self, "masterDataDisks"))
 
     @master_data_disks.setter
     def master_data_disks(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosKubernetesCluster.MasterDataDisksProperty"]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosKubernetesCluster, "master_data_disks").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "masterDataDisks", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="masterSystemDiskCategory")
     def master_system_disk_category(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -5698,17 +6179,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "masterSystemDiskCategory"))
 
     @master_system_disk_category.setter
     def master_system_disk_category(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosKubernetesCluster, "master_system_disk_category").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "masterSystemDiskCategory", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="masterSystemDiskPerformanceLevel")
     def master_system_disk_performance_level(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -5718,17 +6202,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "masterSystemDiskPerformanceLevel"))
 
     @master_system_disk_performance_level.setter
     def master_system_disk_performance_level(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosKubernetesCluster, "master_system_disk_performance_level").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "masterSystemDiskPerformanceLevel", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="masterSystemDiskSize")
     def master_system_disk_size(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -5738,51 +6225,60 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "masterSystemDiskSize"))
 
     @master_system_disk_size.setter
     def master_system_disk_size(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosKubernetesCluster, "master_system_disk_size").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "masterSystemDiskSize", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="masterSystemDiskSnapshotPolicyId")
     def master_system_disk_snapshot_policy_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: masterSystemDiskSnapshotPolicyId: The ID of the policy that is used to back up the data disk of the master node.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "masterSystemDiskSnapshotPolicyId"))
 
     @master_system_disk_snapshot_policy_id.setter
     def master_system_disk_snapshot_policy_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosKubernetesCluster, "master_system_disk_snapshot_policy_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "masterSystemDiskSnapshotPolicyId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="masterZoneIds")
     def master_zone_ids(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]]:
         '''
         :Property: masterZoneIds: Zone ids of master node virtual switches belongs to.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]], jsii.get(self, "masterZoneIds"))
 
     @master_zone_ids.setter
     def master_zone_ids(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosKubernetesCluster, "master_zone_ids").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "masterZoneIds", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="nodeCidrMask")
     def node_cidr_mask(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -5793,17 +6289,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "nodeCidrMask"))
 
     @node_cidr_mask.setter
     def node_cidr_mask(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosKubernetesCluster, "node_cidr_mask").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "nodeCidrMask", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="nodeNameMode")
     def node_name_mode(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -5815,34 +6314,40 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "nodeNameMode"))
 
     @node_name_mode.setter
     def node_name_mode(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosKubernetesCluster, "node_name_mode").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "nodeNameMode", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="nodePools")
     def node_pools(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosKubernetesCluster.NodePoolsProperty"]]]]:
         '''
         :Property: nodePools: The configurations of Node pools.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosKubernetesCluster.NodePoolsProperty"]]]], jsii.get(self, "nodePools"))
 
     @node_pools.setter
     def node_pools(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosKubernetesCluster.NodePoolsProperty"]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosKubernetesCluster, "node_pools").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "nodePools", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="nodePortRange")
     def node_port_range(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -5852,17 +6357,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "nodePortRange"))
 
     @node_port_range.setter
     def node_port_range(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosKubernetesCluster, "node_port_range").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "nodePortRange", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="numOfNodes")
     def num_of_nodes(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -5872,17 +6380,20 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "numOfNodes"))
 
     @num_of_nodes.setter
     def num_of_nodes(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosKubernetesCluster, "num_of_nodes").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "numOfNodes", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="osType")
     def os_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -5894,61 +6405,72 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "osType"))
 
     @os_type.setter
     def os_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosKubernetesCluster, "os_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "osType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="period")
     def period(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
         period: The duration of the annual subscription and monthly subscription. It takes effect when the ChargeType value is PrePaid and is a required value. The value range is:
         When PeriodUnit = Week, Period values are: {"1", "2", "3", "4"}
         When PeriodUnit = Month, Period values are: {"1", "2", "3", "4", "5", "6", "7", "8", "9", "12", "24", "36", "48", "60"}
+        When PeriodUnit = Year, Period values are: {"1", "2", "3", "4", "5"}
         Default to 1.
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "period"))
 
     @period.setter
     def period(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosKubernetesCluster, "period").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "period", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="periodUnit")
     def period_unit(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
         periodUnit: When you specify PrePaid, you need to specify the period. The options are:
         Week: Time is measured in weeks
         Month: time in months
+        Year: time in years
         Default to Month
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "periodUnit"))
 
     @period_unit.setter
     def period_unit(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosKubernetesCluster, "period_unit").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "periodUnit", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="platform")
     def platform(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -5964,17 +6486,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "platform"))
 
     @platform.setter
     def platform(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosKubernetesCluster, "platform").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "platform", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="podVswitchIds")
     def pod_vswitch_ids(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]]:
         '''
         :Property:
 
@@ -5989,102 +6514,120 @@
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]], jsii.get(self, "podVswitchIds"))
 
     @pod_vswitch_ids.setter
     def pod_vswitch_ids(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosKubernetesCluster, "pod_vswitch_ids").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "podVswitchIds", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="proxyMode")
     def proxy_mode(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: proxyMode: kube-proxy proxy mode, supports both iptables and ipvs modes. The default is iptables.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "proxyMode"))
 
     @proxy_mode.setter
     def proxy_mode(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosKubernetesCluster, "proxy_mode").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "proxyMode", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="resourceGroupId")
     def resource_group_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: resourceGroupId: The ID of resource group.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "resourceGroupId"))
 
     @resource_group_id.setter
     def resource_group_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosKubernetesCluster, "resource_group_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "resourceGroupId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="runtime")
     def runtime(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosKubernetesCluster.RuntimeProperty"]]:
         '''
         :Property: runtime: The container runtime of the cluster. The default runtime is Docker.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosKubernetesCluster.RuntimeProperty"]], jsii.get(self, "runtime"))
 
     @runtime.setter
     def runtime(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosKubernetesCluster.RuntimeProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosKubernetesCluster, "runtime").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "runtime", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="securityGroupId")
     def security_group_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: securityGroupId: Specifies the ID of the security group to which the cluster ECS instance belongs.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "securityGroupId"))
 
     @security_group_id.setter
     def security_group_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosKubernetesCluster, "security_group_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "securityGroupId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="serviceCidr")
     def service_cidr(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: serviceCidr: The service network segment cannot conflict with the VPC network segment and the container network segment. When the system is selected to automatically create a VPC, the network segment 172.19.0.0/20 is used by default.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "serviceCidr"))
 
     @service_cidr.setter
     def service_cidr(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosKubernetesCluster, "service_cidr").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "serviceCidr", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="snatEntry")
     def snat_entry(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -6098,17 +6641,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "snatEntry"))
 
     @snat_entry.setter
     def snat_entry(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosKubernetesCluster, "snat_entry").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "snatEntry", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="socEnabled")
     def soc_enabled(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -6120,17 +6666,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "socEnabled"))
 
     @soc_enabled.setter
     def soc_enabled(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosKubernetesCluster, "soc_enabled").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "socEnabled", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="sshFlags")
     def ssh_flags(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -6141,117 +6690,138 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "sshFlags"))
 
     @ssh_flags.setter
     def ssh_flags(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosKubernetesCluster, "ssh_flags").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "sshFlags", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="tags")
     def tags(self) -> typing.Optional[typing.List["RosKubernetesCluster.TagsProperty"]]:
         '''
         :Property: tags: Tag the cluster.
         '''
         return typing.cast(typing.Optional[typing.List["RosKubernetesCluster.TagsProperty"]], jsii.get(self, "tags"))
 
     @tags.setter
     def tags(
         self,
         value: typing.Optional[typing.List["RosKubernetesCluster.TagsProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosKubernetesCluster, "tags").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "tags", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="taint")
     def taint(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Mapping[builtins.str, typing.Any]]]]:
         '''
         :Property: taint: It is used to mark nodes with taints. It is usually used for the scheduling strategy of Pods. The corresponding concept is: tolerance. If there is a corresponding tolerance mark on the Pods, the stain on the node can be tolerated and scheduled to the node.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Mapping[builtins.str, typing.Any]]]], jsii.get(self, "taint"))
 
     @taint.setter
     def taint(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Mapping[builtins.str, typing.Any]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosKubernetesCluster, "taint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "taint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="timeoutMins")
     def timeout_mins(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: timeoutMins: Cluster resource stack creation timeout, in minutes. The default value is 60.
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "timeoutMins"))
 
     @timeout_mins.setter
     def timeout_mins(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosKubernetesCluster, "timeout_mins").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "timeoutMins", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="timeZone")
     def time_zone(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: timeZone: The time zone of the cluster.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "timeZone"))
 
     @time_zone.setter
     def time_zone(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosKubernetesCluster, "time_zone").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "timeZone", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="userCa")
     def user_ca(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: userCa: The CA of cluster
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "userCa"))
 
     @user_ca.setter
     def user_ca(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosKubernetesCluster, "user_ca").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "userCa", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="userData")
     def user_data(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: userData: The user-defined data. [1, 16KB] characters.User data should not be base64 encoded. If you want to pass base64 encoded string to the property, use function Fn::Base64Decode to decode the base64 string first.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "userData"))
 
     @user_data.setter
     def user_data(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosKubernetesCluster, "user_data").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "userData", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="workerDataDisk")
     def worker_data_disk(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -6263,51 +6833,60 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "workerDataDisk"))
 
     @worker_data_disk.setter
     def worker_data_disk(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosKubernetesCluster, "worker_data_disk").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "workerDataDisk", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="workerDataDisks")
     def worker_data_disks(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosKubernetesCluster.WorkerDataDisksProperty"]]]]:
         '''
         :Property: workerDataDisks: A combination of configurations such as worker data disk type and size. This parameter is valid only when the worker node data disk is mounted.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosKubernetesCluster.WorkerDataDisksProperty"]]]], jsii.get(self, "workerDataDisks"))
 
     @worker_data_disks.setter
     def worker_data_disks(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosKubernetesCluster.WorkerDataDisksProperty"]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosKubernetesCluster, "worker_data_disks").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "workerDataDisks", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="workerInstanceTypes")
     def worker_instance_types(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]]:
         '''
         :Property: workerInstanceTypes: Worker node ECS specification type code. For more details, see Instance Specification Family.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]], jsii.get(self, "workerInstanceTypes"))
 
     @worker_instance_types.setter
     def worker_instance_types(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosKubernetesCluster, "worker_instance_types").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "workerInstanceTypes", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="workerSystemDiskCategory")
     def worker_system_disk_category(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -6319,17 +6898,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "workerSystemDiskCategory"))
 
     @worker_system_disk_category.setter
     def worker_system_disk_category(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosKubernetesCluster, "worker_system_disk_category").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "workerSystemDiskCategory", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="workerSystemDiskSize")
     def worker_system_disk_size(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -6339,48 +6921,57 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "workerSystemDiskSize"))
 
     @worker_system_disk_size.setter
     def worker_system_disk_size(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosKubernetesCluster, "worker_system_disk_size").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "workerSystemDiskSize", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="workerSystemDiskSnapshotPolicyId")
     def worker_system_disk_snapshot_policy_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: workerSystemDiskSnapshotPolicyId: The ID of the policy that is used to back up the data disk of the worker node.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "workerSystemDiskSnapshotPolicyId"))
 
     @worker_system_disk_snapshot_policy_id.setter
     def worker_system_disk_snapshot_policy_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosKubernetesCluster, "worker_system_disk_snapshot_policy_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "workerSystemDiskSnapshotPolicyId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="workerZoneIds")
     def worker_zone_ids(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]]:
         '''
         :Property: workerZoneIds: Zone ids of worker node virtual switches belongs to.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]], jsii.get(self, "workerZoneIds"))
 
     @worker_zone_ids.setter
     def worker_zone_ids(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosKubernetesCluster, "worker_zone_ids").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "workerZoneIds", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-cs.RosKubernetesCluster.AddonsProperty",
         jsii_struct_bases=[],
         name_mapping={"name": "name", "config": "config", "disabled": "disabled"},
     )
@@ -6393,14 +6984,19 @@
             disabled: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param name: 
             :param config: 
             :param disabled: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosKubernetesCluster.AddonsProperty.__init__)
+                check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+                check_type(argname="argument config", value=config, expected_type=type_hints["config"])
+                check_type(argname="argument disabled", value=disabled, expected_type=type_hints["disabled"])
             self._values: typing.Dict[str, typing.Any] = {
                 "name": name,
             }
             if config is not None:
                 self._values["config"] = config
             if disabled is not None:
                 self._values["disabled"] = disabled
@@ -6469,14 +7065,21 @@
             '''
             :param auto_snapshot_policy_id: 
             :param category: 
             :param encrypted: 
             :param performance_level: 
             :param size: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosKubernetesCluster.DataDisksProperty.__init__)
+                check_type(argname="argument auto_snapshot_policy_id", value=auto_snapshot_policy_id, expected_type=type_hints["auto_snapshot_policy_id"])
+                check_type(argname="argument category", value=category, expected_type=type_hints["category"])
+                check_type(argname="argument encrypted", value=encrypted, expected_type=type_hints["encrypted"])
+                check_type(argname="argument performance_level", value=performance_level, expected_type=type_hints["performance_level"])
+                check_type(argname="argument size", value=size, expected_type=type_hints["size"])
             self._values: typing.Dict[str, typing.Any] = {}
             if auto_snapshot_policy_id is not None:
                 self._values["auto_snapshot_policy_id"] = auto_snapshot_policy_id
             if category is not None:
                 self._values["category"] = category
             if encrypted is not None:
                 self._values["encrypted"] = encrypted
@@ -6585,26 +7188,34 @@
     class KubernetesConfigProperty:
         def __init__(
             self,
             *,
             runtime: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             runtime_version: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             cpu_policy: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-            labels: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosKubernetesCluster.LabelsProperty"]]]] = None,
+            labels: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosKubernetesCluster.LabelsProperty", typing.Dict[str, typing.Any]]]]]] = None,
             node_name_mode: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-            taints: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosKubernetesCluster.TaintsProperty"]]]] = None,
+            taints: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosKubernetesCluster.TaintsProperty", typing.Dict[str, typing.Any]]]]]] = None,
         ) -> None:
             '''
             :param runtime: 
             :param runtime_version: 
             :param cpu_policy: 
             :param labels: 
             :param node_name_mode: 
             :param taints: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosKubernetesCluster.KubernetesConfigProperty.__init__)
+                check_type(argname="argument runtime", value=runtime, expected_type=type_hints["runtime"])
+                check_type(argname="argument runtime_version", value=runtime_version, expected_type=type_hints["runtime_version"])
+                check_type(argname="argument cpu_policy", value=cpu_policy, expected_type=type_hints["cpu_policy"])
+                check_type(argname="argument labels", value=labels, expected_type=type_hints["labels"])
+                check_type(argname="argument node_name_mode", value=node_name_mode, expected_type=type_hints["node_name_mode"])
+                check_type(argname="argument taints", value=taints, expected_type=type_hints["taints"])
             self._values: typing.Dict[str, typing.Any] = {
                 "runtime": runtime,
                 "runtime_version": runtime_version,
             }
             if cpu_policy is not None:
                 self._values["cpu_policy"] = cpu_policy
             if labels is not None:
@@ -6707,14 +7318,18 @@
             key: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         ) -> None:
             '''
             :param key: 
             :param value: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosKubernetesCluster.LabelsProperty.__init__)
+                check_type(argname="argument key", value=key, expected_type=type_hints["key"])
+                check_type(argname="argument value", value=value, expected_type=type_hints["value"])
             self._values: typing.Dict[str, typing.Any] = {
                 "key": key,
                 "value": value,
             }
 
         @builtins.property
         def key(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
@@ -6757,14 +7372,18 @@
             category: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             size: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
         ) -> None:
             '''
             :param category: 
             :param size: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosKubernetesCluster.MasterDataDisksProperty.__init__)
+                check_type(argname="argument category", value=category, expected_type=type_hints["category"])
+                check_type(argname="argument size", value=size, expected_type=type_hints["size"])
             self._values: typing.Dict[str, typing.Any] = {
                 "category": category,
                 "size": size,
             }
 
         @builtins.property
         def category(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
@@ -6810,14 +7429,17 @@
             self,
             *,
             name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         ) -> None:
             '''
             :param name: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosKubernetesCluster.NodePoolInfoProperty.__init__)
+                check_type(argname="argument name", value=name, expected_type=type_hints["name"])
             self._values: typing.Dict[str, typing.Any] = {
                 "name": name,
             }
 
         @builtins.property
         def name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
             '''
@@ -6848,25 +7470,31 @@
             "node_pool_info": "nodePoolInfo",
         },
     )
     class NodePoolsProperty:
         def __init__(
             self,
             *,
-            scaling_group: typing.Union[ros_cdk_core.IResolvable, "RosKubernetesCluster.ScalingGroupProperty"],
+            scaling_group: typing.Union[ros_cdk_core.IResolvable, typing.Union["RosKubernetesCluster.ScalingGroupProperty", typing.Dict[str, typing.Any]]],
             count: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
-            kubernetes_config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosKubernetesCluster.KubernetesConfigProperty"]] = None,
-            node_pool_info: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosKubernetesCluster.NodePoolInfoProperty"]] = None,
+            kubernetes_config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosKubernetesCluster.KubernetesConfigProperty", typing.Dict[str, typing.Any]]]] = None,
+            node_pool_info: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosKubernetesCluster.NodePoolInfoProperty", typing.Dict[str, typing.Any]]]] = None,
         ) -> None:
             '''
             :param scaling_group: 
             :param count: 
             :param kubernetes_config: 
             :param node_pool_info: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosKubernetesCluster.NodePoolsProperty.__init__)
+                check_type(argname="argument scaling_group", value=scaling_group, expected_type=type_hints["scaling_group"])
+                check_type(argname="argument count", value=count, expected_type=type_hints["count"])
+                check_type(argname="argument kubernetes_config", value=kubernetes_config, expected_type=type_hints["kubernetes_config"])
+                check_type(argname="argument node_pool_info", value=node_pool_info, expected_type=type_hints["node_pool_info"])
             self._values: typing.Dict[str, typing.Any] = {
                 "scaling_group": scaling_group,
             }
             if count is not None:
                 self._values["count"] = count
             if kubernetes_config is not None:
                 self._values["kubernetes_config"] = kubernetes_config
@@ -6937,14 +7565,18 @@
             name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             version: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param name: 
             :param version: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosKubernetesCluster.RuntimeProperty.__init__)
+                check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+                check_type(argname="argument version", value=version, expected_type=type_hints["version"])
             self._values: typing.Dict[str, typing.Any] = {
                 "name": name,
             }
             if version is not None:
                 self._values["version"] = version
 
         @builtins.property
@@ -6995,38 +7627,40 @@
             "period": "period",
             "period_unit": "periodUnit",
             "platform": "platform",
             "rds_instances": "rdsInstances",
             "system_disk_category": "systemDiskCategory",
             "system_disk_performance_level": "systemDiskPerformanceLevel",
             "tags": "tags",
+            "zone_ids": "zoneIds",
         },
     )
     class ScalingGroupProperty:
         def __init__(
             self,
             *,
             instance_types: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]],
             system_disk_size: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
             v_switch_ids: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]],
-            data_disks: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosKubernetesCluster.DataDisksProperty"]]]] = None,
+            data_disks: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosKubernetesCluster.DataDisksProperty", typing.Dict[str, typing.Any]]]]]] = None,
             image_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
             instance_charge_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
             internet_charge_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
             internet_max_bandwidth_out: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
             is_enterprise_security_group: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
             key_pair: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
             login_password: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
             period: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
             period_unit: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
             platform: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
             rds_instances: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]] = None,
             system_disk_category: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
             system_disk_performance_level: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-            tags: typing.Optional[typing.Sequence["RosKubernetesCluster.ScalingGroupTagsProperty"]] = None,
+            tags: typing.Optional[typing.Sequence[typing.Union["RosKubernetesCluster.ScalingGroupTagsProperty", typing.Dict[str, typing.Any]]]] = None,
+            zone_ids: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]] = None,
         ) -> None:
             '''
             :param instance_types: 
             :param system_disk_size: 
             :param v_switch_ids: 
             :param data_disks: 
             :param image_id: 
@@ -7039,15 +7673,37 @@
             :param period: 
             :param period_unit: 
             :param platform: 
             :param rds_instances: 
             :param system_disk_category: 
             :param system_disk_performance_level: 
             :param tags: 
+            :param zone_ids: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosKubernetesCluster.ScalingGroupProperty.__init__)
+                check_type(argname="argument instance_types", value=instance_types, expected_type=type_hints["instance_types"])
+                check_type(argname="argument system_disk_size", value=system_disk_size, expected_type=type_hints["system_disk_size"])
+                check_type(argname="argument v_switch_ids", value=v_switch_ids, expected_type=type_hints["v_switch_ids"])
+                check_type(argname="argument data_disks", value=data_disks, expected_type=type_hints["data_disks"])
+                check_type(argname="argument image_id", value=image_id, expected_type=type_hints["image_id"])
+                check_type(argname="argument instance_charge_type", value=instance_charge_type, expected_type=type_hints["instance_charge_type"])
+                check_type(argname="argument internet_charge_type", value=internet_charge_type, expected_type=type_hints["internet_charge_type"])
+                check_type(argname="argument internet_max_bandwidth_out", value=internet_max_bandwidth_out, expected_type=type_hints["internet_max_bandwidth_out"])
+                check_type(argname="argument is_enterprise_security_group", value=is_enterprise_security_group, expected_type=type_hints["is_enterprise_security_group"])
+                check_type(argname="argument key_pair", value=key_pair, expected_type=type_hints["key_pair"])
+                check_type(argname="argument login_password", value=login_password, expected_type=type_hints["login_password"])
+                check_type(argname="argument period", value=period, expected_type=type_hints["period"])
+                check_type(argname="argument period_unit", value=period_unit, expected_type=type_hints["period_unit"])
+                check_type(argname="argument platform", value=platform, expected_type=type_hints["platform"])
+                check_type(argname="argument rds_instances", value=rds_instances, expected_type=type_hints["rds_instances"])
+                check_type(argname="argument system_disk_category", value=system_disk_category, expected_type=type_hints["system_disk_category"])
+                check_type(argname="argument system_disk_performance_level", value=system_disk_performance_level, expected_type=type_hints["system_disk_performance_level"])
+                check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
+                check_type(argname="argument zone_ids", value=zone_ids, expected_type=type_hints["zone_ids"])
             self._values: typing.Dict[str, typing.Any] = {
                 "instance_types": instance_types,
                 "system_disk_size": system_disk_size,
                 "v_switch_ids": v_switch_ids,
             }
             if data_disks is not None:
                 self._values["data_disks"] = data_disks
@@ -7075,14 +7731,16 @@
                 self._values["rds_instances"] = rds_instances
             if system_disk_category is not None:
                 self._values["system_disk_category"] = system_disk_category
             if system_disk_performance_level is not None:
                 self._values["system_disk_performance_level"] = system_disk_performance_level
             if tags is not None:
                 self._values["tags"] = tags
+            if zone_ids is not None:
+                self._values["zone_ids"] = zone_ids
 
         @builtins.property
         def instance_types(
             self,
         ) -> typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]:
             '''
             :Property: instanceTypes: The ECS instance types of the nodes.
@@ -7297,14 +7955,24 @@
 
             tags: Adds labels only to ECS instances.
             A key must be unique and cannot exceed 128 characters in length. Neither keys nor values can start with aliyun or acs:. Neither keys nor values can contain https:// or http://.
             '''
             result = self._values.get("tags")
             return typing.cast(typing.Optional[typing.List["RosKubernetesCluster.ScalingGroupTagsProperty"]], result)
 
+        @builtins.property
+        def zone_ids(
+            self,
+        ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]]:
+            '''
+            :Property: zoneIds: Zone ids of virtual switches belongs to.
+            '''
+            result = self._values.get("zone_ids")
+            return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]], result)
+
         def __eq__(self, rhs: typing.Any) -> builtins.bool:
             return isinstance(rhs, self.__class__) and rhs._values == self._values
 
         def __ne__(self, rhs: typing.Any) -> builtins.bool:
             return not (rhs == self)
 
         def __repr__(self) -> str:
@@ -7324,14 +7992,18 @@
             key: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         ) -> None:
             '''
             :param key: 
             :param value: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosKubernetesCluster.ScalingGroupTagsProperty.__init__)
+                check_type(argname="argument key", value=key, expected_type=type_hints["key"])
+                check_type(argname="argument value", value=value, expected_type=type_hints["value"])
             self._values: typing.Dict[str, typing.Any] = {
                 "key": key,
                 "value": value,
             }
 
         @builtins.property
         def key(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
@@ -7374,14 +8046,18 @@
             key: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param key: 
             :param value: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosKubernetesCluster.TagsProperty.__init__)
+                check_type(argname="argument key", value=key, expected_type=type_hints["key"])
+                check_type(argname="argument value", value=value, expected_type=type_hints["value"])
             self._values: typing.Dict[str, typing.Any] = {
                 "key": key,
             }
             if value is not None:
                 self._values["value"] = value
 
         @builtins.property
@@ -7428,14 +8104,19 @@
             effect: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param key: 
             :param value: 
             :param effect: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosKubernetesCluster.TaintsProperty.__init__)
+                check_type(argname="argument key", value=key, expected_type=type_hints["key"])
+                check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+                check_type(argname="argument effect", value=effect, expected_type=type_hints["effect"])
             self._values: typing.Dict[str, typing.Any] = {
                 "key": key,
                 "value": value,
             }
             if effect is not None:
                 self._values["effect"] = effect
 
@@ -7496,14 +8177,18 @@
             category: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             size: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
         ) -> None:
             '''
             :param category: 
             :param size: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosKubernetesCluster.WorkerDataDisksProperty.__init__)
+                check_type(argname="argument category", value=category, expected_type=type_hints["category"])
+                check_type(argname="argument size", value=size, expected_type=type_hints["size"])
             self._values: typing.Dict[str, typing.Any] = {
                 "category": category,
                 "size": size,
             }
 
         @builtins.property
         def category(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
@@ -7613,15 +8298,15 @@
         self,
         *,
         master_instance_types: typing.Union[typing.Sequence[typing.Any], ros_cdk_core.IResolvable],
         master_v_switch_ids: typing.Union[typing.Sequence[typing.Any], ros_cdk_core.IResolvable],
         name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         vpc_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         worker_v_switch_ids: typing.Union[typing.Sequence[typing.Any], ros_cdk_core.IResolvable],
-        addons: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosKubernetesCluster.AddonsProperty]]]] = None,
+        addons: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosKubernetesCluster.AddonsProperty, typing.Dict[str, typing.Any]]]]]] = None,
         auto_renew: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         auto_renew_period: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         charge_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         cis_enabled: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         cloud_monitor_flags: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         container_cidr: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         cpu_policy: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
@@ -7633,46 +8318,46 @@
         keep_instance_name: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         key_pair: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         kubernetes_version: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         load_balancer_spec: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         login_password: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         master_count: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         master_data_disk: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
-        master_data_disks: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosKubernetesCluster.MasterDataDisksProperty]]]] = None,
+        master_data_disks: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosKubernetesCluster.MasterDataDisksProperty, typing.Dict[str, typing.Any]]]]]] = None,
         master_system_disk_category: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         master_system_disk_performance_level: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         master_system_disk_size: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         master_system_disk_snapshot_policy_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         master_zone_ids: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]] = None,
         node_cidr_mask: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         node_name_mode: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        node_pools: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosKubernetesCluster.NodePoolsProperty]]]] = None,
+        node_pools: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosKubernetesCluster.NodePoolsProperty, typing.Dict[str, typing.Any]]]]]] = None,
         node_port_range: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         num_of_nodes: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         os_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         period: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         period_unit: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         platform: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         pod_vswitch_ids: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]] = None,
         proxy_mode: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         resource_group_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        runtime: typing.Optional[typing.Union[ros_cdk_core.IResolvable, RosKubernetesCluster.RuntimeProperty]] = None,
+        runtime: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosKubernetesCluster.RuntimeProperty, typing.Dict[str, typing.Any]]]] = None,
         security_group_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         service_cidr: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         snat_entry: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         soc_enabled: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         ssh_flags: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
-        tags: typing.Optional[typing.Sequence[RosKubernetesCluster.TagsProperty]] = None,
+        tags: typing.Optional[typing.Sequence[typing.Union[RosKubernetesCluster.TagsProperty, typing.Dict[str, typing.Any]]]] = None,
         taint: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Mapping[builtins.str, typing.Any]]]] = None,
         timeout_mins: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         time_zone: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         user_ca: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         user_data: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         worker_data_disk: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
-        worker_data_disks: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosKubernetesCluster.WorkerDataDisksProperty]]]] = None,
+        worker_data_disks: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosKubernetesCluster.WorkerDataDisksProperty, typing.Dict[str, typing.Any]]]]]] = None,
         worker_instance_types: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]] = None,
         worker_system_disk_category: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         worker_system_disk_size: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         worker_system_disk_snapshot_policy_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         worker_zone_ids: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::CS::KubernetesCluster``.
@@ -7736,14 +8421,78 @@
         :param worker_data_disks: 
         :param worker_instance_types: 
         :param worker_system_disk_category: 
         :param worker_system_disk_size: 
         :param worker_system_disk_snapshot_policy_id: 
         :param worker_zone_ids: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosKubernetesClusterProps.__init__)
+            check_type(argname="argument master_instance_types", value=master_instance_types, expected_type=type_hints["master_instance_types"])
+            check_type(argname="argument master_v_switch_ids", value=master_v_switch_ids, expected_type=type_hints["master_v_switch_ids"])
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+            check_type(argname="argument vpc_id", value=vpc_id, expected_type=type_hints["vpc_id"])
+            check_type(argname="argument worker_v_switch_ids", value=worker_v_switch_ids, expected_type=type_hints["worker_v_switch_ids"])
+            check_type(argname="argument addons", value=addons, expected_type=type_hints["addons"])
+            check_type(argname="argument auto_renew", value=auto_renew, expected_type=type_hints["auto_renew"])
+            check_type(argname="argument auto_renew_period", value=auto_renew_period, expected_type=type_hints["auto_renew_period"])
+            check_type(argname="argument charge_type", value=charge_type, expected_type=type_hints["charge_type"])
+            check_type(argname="argument cis_enabled", value=cis_enabled, expected_type=type_hints["cis_enabled"])
+            check_type(argname="argument cloud_monitor_flags", value=cloud_monitor_flags, expected_type=type_hints["cloud_monitor_flags"])
+            check_type(argname="argument container_cidr", value=container_cidr, expected_type=type_hints["container_cidr"])
+            check_type(argname="argument cpu_policy", value=cpu_policy, expected_type=type_hints["cpu_policy"])
+            check_type(argname="argument deletion_protection", value=deletion_protection, expected_type=type_hints["deletion_protection"])
+            check_type(argname="argument disable_rollback", value=disable_rollback, expected_type=type_hints["disable_rollback"])
+            check_type(argname="argument endpoint_public_access", value=endpoint_public_access, expected_type=type_hints["endpoint_public_access"])
+            check_type(argname="argument format_disk", value=format_disk, expected_type=type_hints["format_disk"])
+            check_type(argname="argument is_enterprise_security_group", value=is_enterprise_security_group, expected_type=type_hints["is_enterprise_security_group"])
+            check_type(argname="argument keep_instance_name", value=keep_instance_name, expected_type=type_hints["keep_instance_name"])
+            check_type(argname="argument key_pair", value=key_pair, expected_type=type_hints["key_pair"])
+            check_type(argname="argument kubernetes_version", value=kubernetes_version, expected_type=type_hints["kubernetes_version"])
+            check_type(argname="argument load_balancer_spec", value=load_balancer_spec, expected_type=type_hints["load_balancer_spec"])
+            check_type(argname="argument login_password", value=login_password, expected_type=type_hints["login_password"])
+            check_type(argname="argument master_count", value=master_count, expected_type=type_hints["master_count"])
+            check_type(argname="argument master_data_disk", value=master_data_disk, expected_type=type_hints["master_data_disk"])
+            check_type(argname="argument master_data_disks", value=master_data_disks, expected_type=type_hints["master_data_disks"])
+            check_type(argname="argument master_system_disk_category", value=master_system_disk_category, expected_type=type_hints["master_system_disk_category"])
+            check_type(argname="argument master_system_disk_performance_level", value=master_system_disk_performance_level, expected_type=type_hints["master_system_disk_performance_level"])
+            check_type(argname="argument master_system_disk_size", value=master_system_disk_size, expected_type=type_hints["master_system_disk_size"])
+            check_type(argname="argument master_system_disk_snapshot_policy_id", value=master_system_disk_snapshot_policy_id, expected_type=type_hints["master_system_disk_snapshot_policy_id"])
+            check_type(argname="argument master_zone_ids", value=master_zone_ids, expected_type=type_hints["master_zone_ids"])
+            check_type(argname="argument node_cidr_mask", value=node_cidr_mask, expected_type=type_hints["node_cidr_mask"])
+            check_type(argname="argument node_name_mode", value=node_name_mode, expected_type=type_hints["node_name_mode"])
+            check_type(argname="argument node_pools", value=node_pools, expected_type=type_hints["node_pools"])
+            check_type(argname="argument node_port_range", value=node_port_range, expected_type=type_hints["node_port_range"])
+            check_type(argname="argument num_of_nodes", value=num_of_nodes, expected_type=type_hints["num_of_nodes"])
+            check_type(argname="argument os_type", value=os_type, expected_type=type_hints["os_type"])
+            check_type(argname="argument period", value=period, expected_type=type_hints["period"])
+            check_type(argname="argument period_unit", value=period_unit, expected_type=type_hints["period_unit"])
+            check_type(argname="argument platform", value=platform, expected_type=type_hints["platform"])
+            check_type(argname="argument pod_vswitch_ids", value=pod_vswitch_ids, expected_type=type_hints["pod_vswitch_ids"])
+            check_type(argname="argument proxy_mode", value=proxy_mode, expected_type=type_hints["proxy_mode"])
+            check_type(argname="argument resource_group_id", value=resource_group_id, expected_type=type_hints["resource_group_id"])
+            check_type(argname="argument runtime", value=runtime, expected_type=type_hints["runtime"])
+            check_type(argname="argument security_group_id", value=security_group_id, expected_type=type_hints["security_group_id"])
+            check_type(argname="argument service_cidr", value=service_cidr, expected_type=type_hints["service_cidr"])
+            check_type(argname="argument snat_entry", value=snat_entry, expected_type=type_hints["snat_entry"])
+            check_type(argname="argument soc_enabled", value=soc_enabled, expected_type=type_hints["soc_enabled"])
+            check_type(argname="argument ssh_flags", value=ssh_flags, expected_type=type_hints["ssh_flags"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
+            check_type(argname="argument taint", value=taint, expected_type=type_hints["taint"])
+            check_type(argname="argument timeout_mins", value=timeout_mins, expected_type=type_hints["timeout_mins"])
+            check_type(argname="argument time_zone", value=time_zone, expected_type=type_hints["time_zone"])
+            check_type(argname="argument user_ca", value=user_ca, expected_type=type_hints["user_ca"])
+            check_type(argname="argument user_data", value=user_data, expected_type=type_hints["user_data"])
+            check_type(argname="argument worker_data_disk", value=worker_data_disk, expected_type=type_hints["worker_data_disk"])
+            check_type(argname="argument worker_data_disks", value=worker_data_disks, expected_type=type_hints["worker_data_disks"])
+            check_type(argname="argument worker_instance_types", value=worker_instance_types, expected_type=type_hints["worker_instance_types"])
+            check_type(argname="argument worker_system_disk_category", value=worker_system_disk_category, expected_type=type_hints["worker_system_disk_category"])
+            check_type(argname="argument worker_system_disk_size", value=worker_system_disk_size, expected_type=type_hints["worker_system_disk_size"])
+            check_type(argname="argument worker_system_disk_snapshot_policy_id", value=worker_system_disk_snapshot_policy_id, expected_type=type_hints["worker_system_disk_snapshot_policy_id"])
+            check_type(argname="argument worker_zone_ids", value=worker_zone_ids, expected_type=type_hints["worker_zone_ids"])
         self._values: typing.Dict[str, typing.Any] = {
             "master_instance_types": master_instance_types,
             "master_v_switch_ids": master_v_switch_ids,
             "name": name,
             "vpc_id": vpc_id,
             "worker_v_switch_ids": worker_v_switch_ids,
         }
@@ -8350,14 +9099,15 @@
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
         period: The duration of the annual subscription and monthly subscription. It takes effect when the ChargeType value is PrePaid and is a required value. The value range is:
         When PeriodUnit = Week, Period values are: {"1", "2", "3", "4"}
         When PeriodUnit = Month, Period values are: {"1", "2", "3", "4", "5", "6", "7", "8", "9", "12", "24", "36", "48", "60"}
+        When PeriodUnit = Year, Period values are: {"1", "2", "3", "4", "5"}
         Default to 1.
         '''
         result = self._values.get("period")
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], result)
 
     @builtins.property
     def period_unit(
@@ -8365,14 +9115,15 @@
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
         periodUnit: When you specify PrePaid, you need to specify the period. The options are:
         Week: Time is measured in weeks
         Month: time in months
+        Year: time in years
         Default to Month
         '''
         result = self._values.get("period_unit")
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], result)
 
     @builtins.property
     def platform(
@@ -8667,181 +9418,202 @@
 ):
     '''A ROS template type:  ``ALIYUN::CS::ManagedEdgeKubernetesCluster``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosManagedEdgeKubernetesClusterProps",
+        props: typing.Union["RosManagedEdgeKubernetesClusterProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::CS::ManagedEdgeKubernetesCluster``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosManagedEdgeKubernetesCluster.__init__)
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
+            type_hints = typing.get_type_hints(RosManagedEdgeKubernetesCluster._render_properties)
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
     @jsii.member(jsii_name="attrApiServerSlbId")
     def attr_api_server_slb_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: APIServerSLBId: The id of API server SLB
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrApiServerSlbId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrClusterId")
     def attr_cluster_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ClusterId: Cluster instance ID.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrClusterId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDefaultUserKubeConfig")
     def attr_default_user_kube_config(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: DefaultUserKubeConfig: Default user kubernetes config which is used for configuring cluster credentials.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDefaultUserKubeConfig"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrNodes")
     def attr_nodes(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Nodes: The list of cluster nodes.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrNodes"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPrivateUserKubConfig")
     def attr_private_user_kub_config(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: PrivateUserKubConfig: Private user kubernetes config which is used for configuring cluster credentials.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPrivateUserKubConfig"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrScalingConfigurationId")
     def attr_scaling_configuration_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ScalingConfigurationId: Scaling configuration id
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrScalingConfigurationId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrScalingGroupId")
     def attr_scaling_group_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ScalingGroupId: Scaling group id
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrScalingGroupId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrScalingRuleId")
     def attr_scaling_rule_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ScalingRuleId: Scaling rule id
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrScalingRuleId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTaskId")
     def attr_task_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: TaskId: Task ID. Automatically assigned by the system, the user queries the task status.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTaskId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrWorkerRamRoleName")
     def attr_worker_ram_role_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: WorkerRamRoleName: Worker ram role name.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrWorkerRamRoleName"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosManagedEdgeKubernetesCluster, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="name")
     def name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: name: The name of the cluster. The cluster name can use uppercase and lowercase letters, Chinese characters, numbers, and dashes.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "name"))
 
     @name.setter
     def name(self, value: typing.Union[builtins.str, ros_cdk_core.IResolvable]) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosManagedEdgeKubernetesCluster, "name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "name", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="numOfNodes")
     def num_of_nodes(self) -> typing.Union[jsii.Number, ros_cdk_core.IResolvable]:
         '''
         :Property: numOfNodes: Number of worker nodes. The range is [0,300]
         '''
         return typing.cast(typing.Union[jsii.Number, ros_cdk_core.IResolvable], jsii.get(self, "numOfNodes"))
 
     @num_of_nodes.setter
     def num_of_nodes(
         self,
         value: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosManagedEdgeKubernetesCluster, "num_of_nodes").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "numOfNodes", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="addons")
     def addons(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosManagedEdgeKubernetesCluster.AddonsProperty"]]]]:
         '''
         :Property: addons: The add-ons to be installed for the cluster.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosManagedEdgeKubernetesCluster.AddonsProperty"]]]], jsii.get(self, "addons"))
 
     @addons.setter
     def addons(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosManagedEdgeKubernetesCluster.AddonsProperty"]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosManagedEdgeKubernetesCluster, "addons").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "addons", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="autoRenew")
     def auto_renew(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -8853,17 +9625,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "autoRenew"))
 
     @auto_renew.setter
     def auto_renew(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosManagedEdgeKubernetesCluster, "auto_renew").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "autoRenew", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="autoRenewPeriod")
     def auto_renew_period(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -8875,17 +9650,20 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "autoRenewPeriod"))
 
     @auto_renew_period.setter
     def auto_renew_period(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosManagedEdgeKubernetesCluster, "auto_renew_period").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "autoRenewPeriod", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="chargeType")
     def charge_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -8897,17 +9675,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "chargeType"))
 
     @charge_type.setter
     def charge_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosManagedEdgeKubernetesCluster, "charge_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "chargeType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="cloudMonitorFlags")
     def cloud_monitor_flags(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -8919,17 +9700,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "cloudMonitorFlags"))
 
     @cloud_monitor_flags.setter
     def cloud_monitor_flags(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosManagedEdgeKubernetesCluster, "cloud_monitor_flags").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "cloudMonitorFlags", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="clusterSpec")
     def cluster_spec(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -8941,34 +9725,40 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "clusterSpec"))
 
     @cluster_spec.setter
     def cluster_spec(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosManagedEdgeKubernetesCluster, "cluster_spec").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "clusterSpec", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="containerCidr")
     def container_cidr(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: containerCidr: The container network segment cannot conflict with the VPC network segment. When the system is selected to automatically create a VPC, the network segment 172.16.0.0/16 is used by default.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "containerCidr"))
 
     @container_cidr.setter
     def container_cidr(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosManagedEdgeKubernetesCluster, "container_cidr").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "containerCidr", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="deletionProtection")
     def deletion_protection(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -8981,17 +9771,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "deletionProtection"))
 
     @deletion_protection.setter
     def deletion_protection(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosManagedEdgeKubernetesCluster, "deletion_protection").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "deletionProtection", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="disableRollback")
     def disable_rollback(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -9003,17 +9796,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "disableRollback"))
 
     @disable_rollback.setter
     def disable_rollback(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosManagedEdgeKubernetesCluster, "disable_rollback").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "disableRollback", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="endpointPublicAccess")
     def endpoint_public_access(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -9024,17 +9820,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "endpointPublicAccess"))
 
     @endpoint_public_access.setter
     def endpoint_public_access(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosManagedEdgeKubernetesCluster, "endpoint_public_access").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "endpointPublicAccess", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="isEnterpriseSecurityGroup")
     def is_enterprise_security_group(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -9048,51 +9847,60 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "isEnterpriseSecurityGroup"))
 
     @is_enterprise_security_group.setter
     def is_enterprise_security_group(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosManagedEdgeKubernetesCluster, "is_enterprise_security_group").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "isEnterpriseSecurityGroup", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="keyPair")
     def key_pair(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: keyPair: Key pair name. Specify one of KeyPair or LoginPassword.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "keyPair"))
 
     @key_pair.setter
     def key_pair(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosManagedEdgeKubernetesCluster, "key_pair").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "keyPair", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="loginPassword")
     def login_password(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: loginPassword: SSH login password. Password rules are 8-30 characters and contain three items (upper and lower case letters, numbers, and special symbols). Specify one of KeyPair or LoginPassword.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "loginPassword"))
 
     @login_password.setter
     def login_password(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosManagedEdgeKubernetesCluster, "login_password").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "loginPassword", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="nodeCidrMask")
     def node_cidr_mask(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -9103,129 +9911,152 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "nodeCidrMask"))
 
     @node_cidr_mask.setter
     def node_cidr_mask(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosManagedEdgeKubernetesCluster, "node_cidr_mask").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "nodeCidrMask", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="period")
     def period(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
         period: The duration of the annual subscription and monthly subscription. It takes effect when the ChargeType value is PrePaid and is a required value. The value range is:
         When PeriodUnit = Week, Period values are: {"1", "2", "3", "4"}
         When PeriodUnit = Month, Period values are: {"1", "2", "3", "4", "5", "6", "7", "8", "9", "12", "24", "36", "48", "60"}
+        When PeriodUnit = Year, Period values are: {"1", "2", "3", "4", "5"}
         Default to 1.
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "period"))
 
     @period.setter
     def period(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosManagedEdgeKubernetesCluster, "period").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "period", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="periodUnit")
     def period_unit(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
         periodUnit: When you specify PrePaid, you need to specify the period. The options are:
         Week: Time is measured in weeks
         Month: time in months
+        Year: time in years
         Default to Month
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "periodUnit"))
 
     @period_unit.setter
     def period_unit(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosManagedEdgeKubernetesCluster, "period_unit").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "periodUnit", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="profile")
     def profile(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: profile: Edge cluster ID. The default value is Edge.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "profile"))
 
     @profile.setter
     def profile(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosManagedEdgeKubernetesCluster, "profile").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "profile", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="proxyMode")
     def proxy_mode(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: proxyMode: kube-proxy proxy mode, supports both iptables and ipvs modes. The default is iptables.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "proxyMode"))
 
     @proxy_mode.setter
     def proxy_mode(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosManagedEdgeKubernetesCluster, "proxy_mode").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "proxyMode", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="resourceGroupId")
     def resource_group_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: resourceGroupId: The ID of resource group.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "resourceGroupId"))
 
     @resource_group_id.setter
     def resource_group_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosManagedEdgeKubernetesCluster, "resource_group_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "resourceGroupId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="serviceCidr")
     def service_cidr(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: serviceCidr: The service network segment cannot conflict with the VPC network segment and the container network segment. When the system is selected to automatically create a VPC, the network segment 172.19.0.0/20 is used by default.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "serviceCidr"))
 
     @service_cidr.setter
     def service_cidr(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosManagedEdgeKubernetesCluster, "service_cidr").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "serviceCidr", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="snatEntry")
     def snat_entry(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -9239,51 +10070,60 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "snatEntry"))
 
     @snat_entry.setter
     def snat_entry(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosManagedEdgeKubernetesCluster, "snat_entry").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "snatEntry", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="tags")
     def tags(
         self,
     ) -> typing.Optional[typing.List["RosManagedEdgeKubernetesCluster.TagsProperty"]]:
         '''
         :Property: tags: Tag the cluster.
         '''
         return typing.cast(typing.Optional[typing.List["RosManagedEdgeKubernetesCluster.TagsProperty"]], jsii.get(self, "tags"))
 
     @tags.setter
     def tags(
         self,
         value: typing.Optional[typing.List["RosManagedEdgeKubernetesCluster.TagsProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosManagedEdgeKubernetesCluster, "tags").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "tags", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="timeoutMins")
     def timeout_mins(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: timeoutMins: Cluster resource stack creation timeout, in minutes. The default value is 60.
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "timeoutMins"))
 
     @timeout_mins.setter
     def timeout_mins(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosManagedEdgeKubernetesCluster, "timeout_mins").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "timeoutMins", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vpcId")
     def vpc_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -9293,34 +10133,40 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "vpcId"))
 
     @vpc_id.setter
     def vpc_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosManagedEdgeKubernetesCluster, "vpc_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "vpcId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vSwitchIds")
     def v_switch_ids(
         self,
     ) -> typing.Optional[typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]]:
         '''
         :Property: vSwitchIds: The virtual switch ID of the worker node.
         '''
         return typing.cast(typing.Optional[typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]], jsii.get(self, "vSwitchIds"))
 
     @v_switch_ids.setter
     def v_switch_ids(
         self,
         value: typing.Optional[typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosManagedEdgeKubernetesCluster, "v_switch_ids").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "vSwitchIds", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="workerDataDisk")
     def worker_data_disk(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -9332,68 +10178,100 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "workerDataDisk"))
 
     @worker_data_disk.setter
     def worker_data_disk(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosManagedEdgeKubernetesCluster, "worker_data_disk").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "workerDataDisk", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="workerDataDiskCategory")
     def worker_data_disk_category(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: workerDataDiskCategory: Data disk type.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "workerDataDiskCategory"))
 
     @worker_data_disk_category.setter
     def worker_data_disk_category(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosManagedEdgeKubernetesCluster, "worker_data_disk_category").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "workerDataDiskCategory", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
+    @jsii.member(jsii_name="workerDataDisks")
+    def worker_data_disks(
+        self,
+    ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosManagedEdgeKubernetesCluster.WorkerDataDisksProperty"]]]]:
+        '''
+        :Property: workerDataDisks: A combination of configurations such as worker data disk type and size. This parameter is valid only when the worker node data disk is mounted.
+        '''
+        return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosManagedEdgeKubernetesCluster.WorkerDataDisksProperty"]]]], jsii.get(self, "workerDataDisks"))
+
+    @worker_data_disks.setter
+    def worker_data_disks(
+        self,
+        value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosManagedEdgeKubernetesCluster.WorkerDataDisksProperty"]]]],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosManagedEdgeKubernetesCluster, "worker_data_disks").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "workerDataDisks", value)
+
+    @builtins.property
     @jsii.member(jsii_name="workerDataDiskSize")
     def worker_data_disk_size(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: workerDataDiskSize: Data disk size in GiB.
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "workerDataDiskSize"))
 
     @worker_data_disk_size.setter
     def worker_data_disk_size(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosManagedEdgeKubernetesCluster, "worker_data_disk_size").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "workerDataDiskSize", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="workerInstanceTypes")
     def worker_instance_types(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]]:
         '''
         :Property: workerInstanceTypes: Worker node ECS specification type code. For more details, see Instance Specification Family.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]], jsii.get(self, "workerInstanceTypes"))
 
     @worker_instance_types.setter
     def worker_instance_types(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosManagedEdgeKubernetesCluster, "worker_instance_types").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "workerInstanceTypes", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="workerSystemDiskCategory")
     def worker_system_disk_category(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -9403,17 +10281,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "workerSystemDiskCategory"))
 
     @worker_system_disk_category.setter
     def worker_system_disk_category(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosManagedEdgeKubernetesCluster, "worker_system_disk_category").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "workerSystemDiskCategory", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="workerSystemDiskSize")
     def worker_system_disk_size(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -9423,31 +10304,37 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "workerSystemDiskSize"))
 
     @worker_system_disk_size.setter
     def worker_system_disk_size(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosManagedEdgeKubernetesCluster, "worker_system_disk_size").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "workerSystemDiskSize", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="zoneIds")
     def zone_ids(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]]:
         '''
         :Property: zoneIds: Zone ids of worker node virtual switches belongs to.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]], jsii.get(self, "zoneIds"))
 
     @zone_ids.setter
     def zone_ids(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosManagedEdgeKubernetesCluster, "zone_ids").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "zoneIds", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-cs.RosManagedEdgeKubernetesCluster.AddonsProperty",
         jsii_struct_bases=[],
         name_mapping={"name": "name", "config": "config", "disabled": "disabled"},
     )
@@ -9460,14 +10347,19 @@
             disabled: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param name: 
             :param config: 
             :param disabled: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosManagedEdgeKubernetesCluster.AddonsProperty.__init__)
+                check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+                check_type(argname="argument config", value=config, expected_type=type_hints["config"])
+                check_type(argname="argument disabled", value=disabled, expected_type=type_hints["disabled"])
             self._values: typing.Dict[str, typing.Any] = {
                 "name": name,
             }
             if config is not None:
                 self._values["config"] = config
             if disabled is not None:
                 self._values["disabled"] = disabled
@@ -9524,14 +10416,18 @@
             key: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param key: 
             :param value: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosManagedEdgeKubernetesCluster.TagsProperty.__init__)
+                check_type(argname="argument key", value=key, expected_type=type_hints["key"])
+                check_type(argname="argument value", value=value, expected_type=type_hints["value"])
             self._values: typing.Dict[str, typing.Any] = {
                 "key": key,
             }
             if value is not None:
                 self._values["value"] = value
 
         @builtins.property
@@ -9560,14 +10456,73 @@
             return not (rhs == self)
 
         def __repr__(self) -> str:
             return "TagsProperty(%s)" % ", ".join(
                 k + "=" + repr(v) for k, v in self._values.items()
             )
 
+    @jsii.data_type(
+        jsii_type="@alicloud/ros-cdk-cs.RosManagedEdgeKubernetesCluster.WorkerDataDisksProperty",
+        jsii_struct_bases=[],
+        name_mapping={"category": "category", "size": "size"},
+    )
+    class WorkerDataDisksProperty:
+        def __init__(
+            self,
+            *,
+            category: typing.Union[builtins.str, ros_cdk_core.IResolvable],
+            size: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
+        ) -> None:
+            '''
+            :param category: 
+            :param size: 
+            '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosManagedEdgeKubernetesCluster.WorkerDataDisksProperty.__init__)
+                check_type(argname="argument category", value=category, expected_type=type_hints["category"])
+                check_type(argname="argument size", value=size, expected_type=type_hints["size"])
+            self._values: typing.Dict[str, typing.Any] = {
+                "category": category,
+                "size": size,
+            }
+
+        @builtins.property
+        def category(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
+            '''
+            :Property:
+
+            category: Data disk type. Value includes:
+            cloud: ordinary cloud disk
+            cloud_efficiency: efficient cloud disk
+            cloud_ssd: SSD cloud disk
+            '''
+            result = self._values.get("category")
+            assert result is not None, "Required property 'category' is missing"
+            return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], result)
+
+        @builtins.property
+        def size(self) -> typing.Union[jsii.Number, ros_cdk_core.IResolvable]:
+            '''
+            :Property: size: Data disk size in GiB.
+            '''
+            result = self._values.get("size")
+            assert result is not None, "Required property 'size' is missing"
+            return typing.cast(typing.Union[jsii.Number, ros_cdk_core.IResolvable], result)
+
+        def __eq__(self, rhs: typing.Any) -> builtins.bool:
+            return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+        def __ne__(self, rhs: typing.Any) -> builtins.bool:
+            return not (rhs == self)
+
+        def __repr__(self) -> str:
+            return "WorkerDataDisksProperty(%s)" % ", ".join(
+                k + "=" + repr(v) for k, v in self._values.items()
+            )
+
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-cs.RosManagedEdgeKubernetesClusterProps",
     jsii_struct_bases=[],
     name_mapping={
         "name": "name",
         "num_of_nodes": "numOfNodes",
@@ -9594,28 +10549,29 @@
         "snat_entry": "snatEntry",
         "tags": "tags",
         "timeout_mins": "timeoutMins",
         "vpc_id": "vpcId",
         "v_switch_ids": "vSwitchIds",
         "worker_data_disk": "workerDataDisk",
         "worker_data_disk_category": "workerDataDiskCategory",
+        "worker_data_disks": "workerDataDisks",
         "worker_data_disk_size": "workerDataDiskSize",
         "worker_instance_types": "workerInstanceTypes",
         "worker_system_disk_category": "workerSystemDiskCategory",
         "worker_system_disk_size": "workerSystemDiskSize",
         "zone_ids": "zoneIds",
     },
 )
 class RosManagedEdgeKubernetesClusterProps:
     def __init__(
         self,
         *,
         name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         num_of_nodes: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
-        addons: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosManagedEdgeKubernetesCluster.AddonsProperty]]]] = None,
+        addons: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosManagedEdgeKubernetesCluster.AddonsProperty, typing.Dict[str, typing.Any]]]]]] = None,
         auto_renew: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         auto_renew_period: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         charge_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         cloud_monitor_flags: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         cluster_spec: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         container_cidr: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         deletion_protection: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
@@ -9628,20 +10584,21 @@
         period: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         period_unit: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         profile: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         proxy_mode: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         resource_group_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         service_cidr: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         snat_entry: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
-        tags: typing.Optional[typing.Sequence[RosManagedEdgeKubernetesCluster.TagsProperty]] = None,
+        tags: typing.Optional[typing.Sequence[typing.Union[RosManagedEdgeKubernetesCluster.TagsProperty, typing.Dict[str, typing.Any]]]] = None,
         timeout_mins: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         vpc_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         v_switch_ids: typing.Optional[typing.Union[typing.Sequence[typing.Any], ros_cdk_core.IResolvable]] = None,
         worker_data_disk: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         worker_data_disk_category: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
+        worker_data_disks: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosManagedEdgeKubernetesCluster.WorkerDataDisksProperty, typing.Dict[str, typing.Any]]]]]] = None,
         worker_data_disk_size: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         worker_instance_types: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]] = None,
         worker_system_disk_category: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         worker_system_disk_size: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         zone_ids: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::CS::ManagedEdgeKubernetesCluster``.
@@ -9671,20 +10628,58 @@
         :param snat_entry: 
         :param tags: 
         :param timeout_mins: 
         :param vpc_id: 
         :param v_switch_ids: 
         :param worker_data_disk: 
         :param worker_data_disk_category: 
+        :param worker_data_disks: 
         :param worker_data_disk_size: 
         :param worker_instance_types: 
         :param worker_system_disk_category: 
         :param worker_system_disk_size: 
         :param zone_ids: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosManagedEdgeKubernetesClusterProps.__init__)
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+            check_type(argname="argument num_of_nodes", value=num_of_nodes, expected_type=type_hints["num_of_nodes"])
+            check_type(argname="argument addons", value=addons, expected_type=type_hints["addons"])
+            check_type(argname="argument auto_renew", value=auto_renew, expected_type=type_hints["auto_renew"])
+            check_type(argname="argument auto_renew_period", value=auto_renew_period, expected_type=type_hints["auto_renew_period"])
+            check_type(argname="argument charge_type", value=charge_type, expected_type=type_hints["charge_type"])
+            check_type(argname="argument cloud_monitor_flags", value=cloud_monitor_flags, expected_type=type_hints["cloud_monitor_flags"])
+            check_type(argname="argument cluster_spec", value=cluster_spec, expected_type=type_hints["cluster_spec"])
+            check_type(argname="argument container_cidr", value=container_cidr, expected_type=type_hints["container_cidr"])
+            check_type(argname="argument deletion_protection", value=deletion_protection, expected_type=type_hints["deletion_protection"])
+            check_type(argname="argument disable_rollback", value=disable_rollback, expected_type=type_hints["disable_rollback"])
+            check_type(argname="argument endpoint_public_access", value=endpoint_public_access, expected_type=type_hints["endpoint_public_access"])
+            check_type(argname="argument is_enterprise_security_group", value=is_enterprise_security_group, expected_type=type_hints["is_enterprise_security_group"])
+            check_type(argname="argument key_pair", value=key_pair, expected_type=type_hints["key_pair"])
+            check_type(argname="argument login_password", value=login_password, expected_type=type_hints["login_password"])
+            check_type(argname="argument node_cidr_mask", value=node_cidr_mask, expected_type=type_hints["node_cidr_mask"])
+            check_type(argname="argument period", value=period, expected_type=type_hints["period"])
+            check_type(argname="argument period_unit", value=period_unit, expected_type=type_hints["period_unit"])
+            check_type(argname="argument profile", value=profile, expected_type=type_hints["profile"])
+            check_type(argname="argument proxy_mode", value=proxy_mode, expected_type=type_hints["proxy_mode"])
+            check_type(argname="argument resource_group_id", value=resource_group_id, expected_type=type_hints["resource_group_id"])
+            check_type(argname="argument service_cidr", value=service_cidr, expected_type=type_hints["service_cidr"])
+            check_type(argname="argument snat_entry", value=snat_entry, expected_type=type_hints["snat_entry"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
+            check_type(argname="argument timeout_mins", value=timeout_mins, expected_type=type_hints["timeout_mins"])
+            check_type(argname="argument vpc_id", value=vpc_id, expected_type=type_hints["vpc_id"])
+            check_type(argname="argument v_switch_ids", value=v_switch_ids, expected_type=type_hints["v_switch_ids"])
+            check_type(argname="argument worker_data_disk", value=worker_data_disk, expected_type=type_hints["worker_data_disk"])
+            check_type(argname="argument worker_data_disk_category", value=worker_data_disk_category, expected_type=type_hints["worker_data_disk_category"])
+            check_type(argname="argument worker_data_disks", value=worker_data_disks, expected_type=type_hints["worker_data_disks"])
+            check_type(argname="argument worker_data_disk_size", value=worker_data_disk_size, expected_type=type_hints["worker_data_disk_size"])
+            check_type(argname="argument worker_instance_types", value=worker_instance_types, expected_type=type_hints["worker_instance_types"])
+            check_type(argname="argument worker_system_disk_category", value=worker_system_disk_category, expected_type=type_hints["worker_system_disk_category"])
+            check_type(argname="argument worker_system_disk_size", value=worker_system_disk_size, expected_type=type_hints["worker_system_disk_size"])
+            check_type(argname="argument zone_ids", value=zone_ids, expected_type=type_hints["zone_ids"])
         self._values: typing.Dict[str, typing.Any] = {
             "name": name,
             "num_of_nodes": num_of_nodes,
         }
         if addons is not None:
             self._values["addons"] = addons
         if auto_renew is not None:
@@ -9735,14 +10730,16 @@
             self._values["vpc_id"] = vpc_id
         if v_switch_ids is not None:
             self._values["v_switch_ids"] = v_switch_ids
         if worker_data_disk is not None:
             self._values["worker_data_disk"] = worker_data_disk
         if worker_data_disk_category is not None:
             self._values["worker_data_disk_category"] = worker_data_disk_category
+        if worker_data_disks is not None:
+            self._values["worker_data_disks"] = worker_data_disks
         if worker_data_disk_size is not None:
             self._values["worker_data_disk_size"] = worker_data_disk_size
         if worker_instance_types is not None:
             self._values["worker_instance_types"] = worker_instance_types
         if worker_system_disk_category is not None:
             self._values["worker_system_disk_category"] = worker_system_disk_category
         if worker_system_disk_size is not None:
@@ -9965,14 +10962,15 @@
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
         period: The duration of the annual subscription and monthly subscription. It takes effect when the ChargeType value is PrePaid and is a required value. The value range is:
         When PeriodUnit = Week, Period values are: {"1", "2", "3", "4"}
         When PeriodUnit = Month, Period values are: {"1", "2", "3", "4", "5", "6", "7", "8", "9", "12", "24", "36", "48", "60"}
+        When PeriodUnit = Year, Period values are: {"1", "2", "3", "4", "5"}
         Default to 1.
         '''
         result = self._values.get("period")
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], result)
 
     @builtins.property
     def period_unit(
@@ -9980,14 +10978,15 @@
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
         periodUnit: When you specify PrePaid, you need to specify the period. The options are:
         Week: Time is measured in weeks
         Month: time in months
+        Year: time in years
         Default to Month
         '''
         result = self._values.get("period_unit")
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], result)
 
     @builtins.property
     def profile(
@@ -10111,14 +11110,24 @@
         '''
         :Property: workerDataDiskCategory: Data disk type.
         '''
         result = self._values.get("worker_data_disk_category")
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], result)
 
     @builtins.property
+    def worker_data_disks(
+        self,
+    ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, RosManagedEdgeKubernetesCluster.WorkerDataDisksProperty]]]]:
+        '''
+        :Property: workerDataDisks: A combination of configurations such as worker data disk type and size. This parameter is valid only when the worker node data disk is mounted.
+        '''
+        result = self._values.get("worker_data_disks")
+        return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, RosManagedEdgeKubernetesCluster.WorkerDataDisksProperty]]]], result)
+
+    @builtins.property
     def worker_data_disk_size(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: workerDataDiskSize: Data disk size in GiB.
         '''
         result = self._values.get("worker_data_disk_size")
@@ -10189,181 +11198,202 @@
 ):
     '''A ROS template type:  ``ALIYUN::CS::ManagedKubernetesCluster``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosManagedKubernetesClusterProps",
+        props: typing.Union["RosManagedKubernetesClusterProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::CS::ManagedKubernetesCluster``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosManagedKubernetesCluster.__init__)
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
+            type_hints = typing.get_type_hints(RosManagedKubernetesCluster._render_properties)
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
     @jsii.member(jsii_name="attrApiServerSlbId")
     def attr_api_server_slb_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: APIServerSLBId: The id of API server SLB
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrApiServerSlbId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrClusterId")
     def attr_cluster_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ClusterId: Cluster instance ID.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrClusterId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDefaultUserKubeConfig")
     def attr_default_user_kube_config(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: DefaultUserKubeConfig: Default user kubernetes config which is used for configuring cluster credentials.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDefaultUserKubeConfig"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrNodes")
     def attr_nodes(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Nodes: The list of cluster nodes.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrNodes"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPrivateUserKubConfig")
     def attr_private_user_kub_config(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: PrivateUserKubConfig: Private user kubernetes config which is used for configuring cluster credentials.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPrivateUserKubConfig"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrScalingConfigurationId")
     def attr_scaling_configuration_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ScalingConfigurationId: Scaling configuration id
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrScalingConfigurationId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrScalingGroupId")
     def attr_scaling_group_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ScalingGroupId: Scaling group id
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrScalingGroupId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrScalingRuleId")
     def attr_scaling_rule_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ScalingRuleId: Scaling rule id
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrScalingRuleId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTaskId")
     def attr_task_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: TaskId: Task ID. Automatically assigned by the system, the user queries the task status.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTaskId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrWorkerRamRoleName")
     def attr_worker_ram_role_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: WorkerRamRoleName: Worker ram role name.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrWorkerRamRoleName"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosManagedKubernetesCluster, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="name")
     def name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: name: The name of the cluster. The cluster name can use uppercase and lowercase letters, Chinese characters, numbers, and dashes.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "name"))
 
     @name.setter
     def name(self, value: typing.Union[builtins.str, ros_cdk_core.IResolvable]) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosManagedKubernetesCluster, "name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "name", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vpcId")
     def vpc_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: vpcId: VPC ID.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "vpcId"))
 
     @vpc_id.setter
     def vpc_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosManagedKubernetesCluster, "vpc_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "vpcId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vSwitchIds")
     def v_switch_ids(
         self,
     ) -> typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]:
         '''
         :Property: vSwitchIds: The virtual switch ID of the worker node.
         '''
         return typing.cast(typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable], jsii.get(self, "vSwitchIds"))
 
     @v_switch_ids.setter
     def v_switch_ids(
         self,
         value: typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosManagedKubernetesCluster, "v_switch_ids").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "vSwitchIds", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="addons")
     def addons(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosManagedKubernetesCluster.AddonsProperty"]]]]:
         '''
         :Property:
 
@@ -10375,17 +11405,20 @@
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosManagedKubernetesCluster.AddonsProperty"]]]], jsii.get(self, "addons"))
 
     @addons.setter
     def addons(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosManagedKubernetesCluster.AddonsProperty"]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosManagedKubernetesCluster, "addons").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "addons", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="autoRenew")
     def auto_renew(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -10397,17 +11430,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "autoRenew"))
 
     @auto_renew.setter
     def auto_renew(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosManagedKubernetesCluster, "auto_renew").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "autoRenew", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="autoRenewPeriod")
     def auto_renew_period(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -10419,17 +11455,20 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "autoRenewPeriod"))
 
     @auto_renew_period.setter
     def auto_renew_period(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosManagedKubernetesCluster, "auto_renew_period").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "autoRenewPeriod", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="chargeType")
     def charge_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -10441,17 +11480,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "chargeType"))
 
     @charge_type.setter
     def charge_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosManagedKubernetesCluster, "charge_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "chargeType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="cisEnabled")
     def cis_enabled(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -10465,17 +11507,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "cisEnabled"))
 
     @cis_enabled.setter
     def cis_enabled(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosManagedKubernetesCluster, "cis_enabled").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "cisEnabled", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="cloudMonitorFlags")
     def cloud_monitor_flags(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -10487,17 +11532,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "cloudMonitorFlags"))
 
     @cloud_monitor_flags.setter
     def cloud_monitor_flags(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosManagedKubernetesCluster, "cloud_monitor_flags").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "cloudMonitorFlags", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="clusterSpec")
     def cluster_spec(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -10509,34 +11557,40 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "clusterSpec"))
 
     @cluster_spec.setter
     def cluster_spec(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosManagedKubernetesCluster, "cluster_spec").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "clusterSpec", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="containerCidr")
     def container_cidr(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: containerCidr: The container network segment cannot conflict with the VPC network segment. When the system is selected to automatically create a VPC, the network segment 172.16.0.0/16 is used by default.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "containerCidr"))
 
     @container_cidr.setter
     def container_cidr(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosManagedKubernetesCluster, "container_cidr").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "containerCidr", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="deletionProtection")
     def deletion_protection(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -10549,17 +11603,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "deletionProtection"))
 
     @deletion_protection.setter
     def deletion_protection(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosManagedKubernetesCluster, "deletion_protection").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "deletionProtection", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="disableRollback")
     def disable_rollback(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -10571,34 +11628,40 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "disableRollback"))
 
     @disable_rollback.setter
     def disable_rollback(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosManagedKubernetesCluster, "disable_rollback").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "disableRollback", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="encryptionProviderKey")
     def encryption_provider_key(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: encryptionProviderKey: The ID of the key that is managed by Key Management Service (KMS). This key is used to encrypt data disks.You can use KMS in only professional managed Kubernetes clusters.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "encryptionProviderKey"))
 
     @encryption_provider_key.setter
     def encryption_provider_key(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosManagedKubernetesCluster, "encryption_provider_key").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "encryptionProviderKey", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="endpointPublicAccess")
     def endpoint_public_access(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -10609,17 +11672,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "endpointPublicAccess"))
 
     @endpoint_public_access.setter
     def endpoint_public_access(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosManagedKubernetesCluster, "endpoint_public_access").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "endpointPublicAccess", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="formatDisk")
     def format_disk(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -10640,17 +11706,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "formatDisk"))
 
     @format_disk.setter
     def format_disk(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosManagedKubernetesCluster, "format_disk").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "formatDisk", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="isEnterpriseSecurityGroup")
     def is_enterprise_security_group(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -10664,17 +11733,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "isEnterpriseSecurityGroup"))
 
     @is_enterprise_security_group.setter
     def is_enterprise_security_group(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosManagedKubernetesCluster, "is_enterprise_security_group").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "isEnterpriseSecurityGroup", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="keepInstanceName")
     def keep_instance_name(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -10686,85 +11758,100 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "keepInstanceName"))
 
     @keep_instance_name.setter
     def keep_instance_name(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosManagedKubernetesCluster, "keep_instance_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "keepInstanceName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="keyPair")
     def key_pair(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: keyPair: Key pair name. Specify one of KeyPair or LoginPassword.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "keyPair"))
 
     @key_pair.setter
     def key_pair(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosManagedKubernetesCluster, "key_pair").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "keyPair", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="kubernetesVersion")
     def kubernetes_version(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: kubernetesVersion: The version of the Kubernetes cluster.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "kubernetesVersion"))
 
     @kubernetes_version.setter
     def kubernetes_version(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosManagedKubernetesCluster, "kubernetes_version").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "kubernetesVersion", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="loadBalancerSpec")
     def load_balancer_spec(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: loadBalancerSpec: The specification of the Server Load Balancer instance. Allowed value: slb.s1.small|slb.s2.small|slb.s2.medium|slb.s3.small|slb.s3.medium|slb.s3.large
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "loadBalancerSpec"))
 
     @load_balancer_spec.setter
     def load_balancer_spec(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosManagedKubernetesCluster, "load_balancer_spec").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "loadBalancerSpec", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="loginPassword")
     def login_password(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: loginPassword: SSH login password. Password rules are 8-30 characters and contain three items (upper and lower case letters, numbers, and special symbols). Specify one of KeyPair or LoginPassword.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "loginPassword"))
 
     @login_password.setter
     def login_password(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosManagedKubernetesCluster, "login_password").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "loginPassword", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="nodeCidrMask")
     def node_cidr_mask(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -10775,17 +11862,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "nodeCidrMask"))
 
     @node_cidr_mask.setter
     def node_cidr_mask(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosManagedKubernetesCluster, "node_cidr_mask").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "nodeCidrMask", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="nodeNameMode")
     def node_name_mode(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -10797,34 +11887,40 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "nodeNameMode"))
 
     @node_name_mode.setter
     def node_name_mode(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosManagedKubernetesCluster, "node_name_mode").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "nodeNameMode", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="nodePools")
     def node_pools(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosManagedKubernetesCluster.NodePoolsProperty"]]]]:
         '''
         :Property: nodePools: The configurations of Node pools.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosManagedKubernetesCluster.NodePoolsProperty"]]]], jsii.get(self, "nodePools"))
 
     @node_pools.setter
     def node_pools(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosManagedKubernetesCluster.NodePoolsProperty"]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosManagedKubernetesCluster, "node_pools").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "nodePools", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="numOfNodes")
     def num_of_nodes(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -10834,17 +11930,20 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "numOfNodes"))
 
     @num_of_nodes.setter
     def num_of_nodes(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosManagedKubernetesCluster, "num_of_nodes").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "numOfNodes", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="osType")
     def os_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -10856,61 +11955,72 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "osType"))
 
     @os_type.setter
     def os_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosManagedKubernetesCluster, "os_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "osType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="period")
     def period(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
         period: The duration of the annual subscription and monthly subscription. It takes effect when the ChargeType value is PrePaid and is a required value. The value range is:
         When PeriodUnit = Week, Period values are: {"1", "2", "3", "4"}
         When PeriodUnit = Month, Period values are: {"1", "2", "3", "4", "5", "6", "7", "8", "9", "12", "24", "36", "48", "60"}
+        When PeriodUnit = Year, Period values are: {"1", "2", "3", "4", "5"}
         Default to 1.
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "period"))
 
     @period.setter
     def period(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosManagedKubernetesCluster, "period").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "period", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="periodUnit")
     def period_unit(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
         periodUnit: When you specify PrePaid, you need to specify the period. The options are:
         Week: Time is measured in weeks
         Month: time in months
+        Year: time in years
         Default to Month
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "periodUnit"))
 
     @period_unit.setter
     def period_unit(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosManagedKubernetesCluster, "period_unit").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "periodUnit", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="platform")
     def platform(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -10926,17 +12036,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "platform"))
 
     @platform.setter
     def platform(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosManagedKubernetesCluster, "platform").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "platform", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="podVswitchIds")
     def pod_vswitch_ids(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]]:
         '''
         :Property:
 
@@ -10951,102 +12064,120 @@
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]], jsii.get(self, "podVswitchIds"))
 
     @pod_vswitch_ids.setter
     def pod_vswitch_ids(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosManagedKubernetesCluster, "pod_vswitch_ids").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "podVswitchIds", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="proxyMode")
     def proxy_mode(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: proxyMode: kube-proxy proxy mode, supports both iptables and ipvs modes. The default is iptables.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "proxyMode"))
 
     @proxy_mode.setter
     def proxy_mode(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosManagedKubernetesCluster, "proxy_mode").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "proxyMode", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="resourceGroupId")
     def resource_group_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: resourceGroupId: The ID of resource group.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "resourceGroupId"))
 
     @resource_group_id.setter
     def resource_group_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosManagedKubernetesCluster, "resource_group_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "resourceGroupId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="runtime")
     def runtime(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosManagedKubernetesCluster.RuntimeProperty"]]:
         '''
         :Property: runtime: The container runtime of the cluster. The default runtime is Docker.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosManagedKubernetesCluster.RuntimeProperty"]], jsii.get(self, "runtime"))
 
     @runtime.setter
     def runtime(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosManagedKubernetesCluster.RuntimeProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosManagedKubernetesCluster, "runtime").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "runtime", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="securityGroupId")
     def security_group_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: securityGroupId: Specifies the ID of the security group to which the cluster ECS instance belongs.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "securityGroupId"))
 
     @security_group_id.setter
     def security_group_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosManagedKubernetesCluster, "security_group_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "securityGroupId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="serviceCidr")
     def service_cidr(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: serviceCidr: The service network segment cannot conflict with the VPC network segment and the container network segment. When the system is selected to automatically create a VPC, the network segment 172.19.0.0/20 is used by default.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "serviceCidr"))
 
     @service_cidr.setter
     def service_cidr(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosManagedKubernetesCluster, "service_cidr").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "serviceCidr", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="snatEntry")
     def snat_entry(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -11060,17 +12191,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "snatEntry"))
 
     @snat_entry.setter
     def snat_entry(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosManagedKubernetesCluster, "snat_entry").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "snatEntry", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="socEnabled")
     def soc_enabled(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -11082,85 +12216,100 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "socEnabled"))
 
     @soc_enabled.setter
     def soc_enabled(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosManagedKubernetesCluster, "soc_enabled").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "socEnabled", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="tags")
     def tags(
         self,
     ) -> typing.Optional[typing.List["RosManagedKubernetesCluster.TagsProperty"]]:
         '''
         :Property: tags: Tag the cluster.
         '''
         return typing.cast(typing.Optional[typing.List["RosManagedKubernetesCluster.TagsProperty"]], jsii.get(self, "tags"))
 
     @tags.setter
     def tags(
         self,
         value: typing.Optional[typing.List["RosManagedKubernetesCluster.TagsProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosManagedKubernetesCluster, "tags").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "tags", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="taint")
     def taint(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Mapping[builtins.str, typing.Any]]]]:
         '''
         :Property: taint: It is used to mark nodes with taints. It is usually used for the scheduling strategy of Pods. The corresponding concept is: tolerance. If there is a corresponding tolerance mark on the Pods, the stain on the node can be tolerated and scheduled to the node.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Mapping[builtins.str, typing.Any]]]], jsii.get(self, "taint"))
 
     @taint.setter
     def taint(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Mapping[builtins.str, typing.Any]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosManagedKubernetesCluster, "taint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "taint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="timeoutMins")
     def timeout_mins(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: timeoutMins: Cluster resource stack creation timeout, in minutes. The default value is 60.
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "timeoutMins"))
 
     @timeout_mins.setter
     def timeout_mins(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosManagedKubernetesCluster, "timeout_mins").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "timeoutMins", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="userData")
     def user_data(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: userData: The user-defined data. [1, 16KB] characters.User data should not be base64 encoded. If you want to pass base64 encoded string to the property, use function Fn::Base64Decode to decode the base64 string first.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "userData"))
 
     @user_data.setter
     def user_data(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosManagedKubernetesCluster, "user_data").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "userData", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="workerDataDisk")
     def worker_data_disk(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -11172,51 +12321,60 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "workerDataDisk"))
 
     @worker_data_disk.setter
     def worker_data_disk(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosManagedKubernetesCluster, "worker_data_disk").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "workerDataDisk", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="workerDataDisks")
     def worker_data_disks(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosManagedKubernetesCluster.WorkerDataDisksProperty"]]]]:
         '''
         :Property: workerDataDisks: A combination of configurations such as worker data disk type and size. This parameter is valid only when the worker node data disk is mounted.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosManagedKubernetesCluster.WorkerDataDisksProperty"]]]], jsii.get(self, "workerDataDisks"))
 
     @worker_data_disks.setter
     def worker_data_disks(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosManagedKubernetesCluster.WorkerDataDisksProperty"]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosManagedKubernetesCluster, "worker_data_disks").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "workerDataDisks", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="workerInstanceTypes")
     def worker_instance_types(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]]:
         '''
         :Property: workerInstanceTypes: Worker node ECS specification type code. For more details, see Instance Specification Family.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]], jsii.get(self, "workerInstanceTypes"))
 
     @worker_instance_types.setter
     def worker_instance_types(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosManagedKubernetesCluster, "worker_instance_types").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "workerInstanceTypes", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="workerSystemDiskCategory")
     def worker_system_disk_category(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -11228,17 +12386,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "workerSystemDiskCategory"))
 
     @worker_system_disk_category.setter
     def worker_system_disk_category(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosManagedKubernetesCluster, "worker_system_disk_category").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "workerSystemDiskCategory", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="workerSystemDiskSize")
     def worker_system_disk_size(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -11248,31 +12409,37 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "workerSystemDiskSize"))
 
     @worker_system_disk_size.setter
     def worker_system_disk_size(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosManagedKubernetesCluster, "worker_system_disk_size").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "workerSystemDiskSize", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="zoneIds")
     def zone_ids(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]]:
         '''
         :Property: zoneIds: Zone ids of worker node virtual switches belongs to.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]], jsii.get(self, "zoneIds"))
 
     @zone_ids.setter
     def zone_ids(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosManagedKubernetesCluster, "zone_ids").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "zoneIds", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-cs.RosManagedKubernetesCluster.AddonsProperty",
         jsii_struct_bases=[],
         name_mapping={
             "name": "name",
@@ -11292,14 +12459,20 @@
         ) -> None:
             '''
             :param name: 
             :param config: 
             :param disabled: 
             :param version: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosManagedKubernetesCluster.AddonsProperty.__init__)
+                check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+                check_type(argname="argument config", value=config, expected_type=type_hints["config"])
+                check_type(argname="argument disabled", value=disabled, expected_type=type_hints["disabled"])
+                check_type(argname="argument version", value=version, expected_type=type_hints["version"])
             self._values: typing.Dict[str, typing.Any] = {
                 "name": name,
             }
             if config is not None:
                 self._values["config"] = config
             if disabled is not None:
                 self._values["disabled"] = disabled
@@ -11380,14 +12553,21 @@
             '''
             :param auto_snapshot_policy_id: 
             :param category: 
             :param encrypted: 
             :param performance_level: 
             :param size: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosManagedKubernetesCluster.DataDisksProperty.__init__)
+                check_type(argname="argument auto_snapshot_policy_id", value=auto_snapshot_policy_id, expected_type=type_hints["auto_snapshot_policy_id"])
+                check_type(argname="argument category", value=category, expected_type=type_hints["category"])
+                check_type(argname="argument encrypted", value=encrypted, expected_type=type_hints["encrypted"])
+                check_type(argname="argument performance_level", value=performance_level, expected_type=type_hints["performance_level"])
+                check_type(argname="argument size", value=size, expected_type=type_hints["size"])
             self._values: typing.Dict[str, typing.Any] = {}
             if auto_snapshot_policy_id is not None:
                 self._values["auto_snapshot_policy_id"] = auto_snapshot_policy_id
             if category is not None:
                 self._values["category"] = category
             if encrypted is not None:
                 self._values["encrypted"] = encrypted
@@ -11496,26 +12676,34 @@
     class KubernetesConfigProperty:
         def __init__(
             self,
             *,
             runtime: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             runtime_version: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             cpu_policy: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-            labels: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosManagedKubernetesCluster.LabelsProperty"]]]] = None,
+            labels: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosManagedKubernetesCluster.LabelsProperty", typing.Dict[str, typing.Any]]]]]] = None,
             node_name_mode: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-            taints: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosManagedKubernetesCluster.TaintsProperty"]]]] = None,
+            taints: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosManagedKubernetesCluster.TaintsProperty", typing.Dict[str, typing.Any]]]]]] = None,
         ) -> None:
             '''
             :param runtime: 
             :param runtime_version: 
             :param cpu_policy: 
             :param labels: 
             :param node_name_mode: 
             :param taints: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosManagedKubernetesCluster.KubernetesConfigProperty.__init__)
+                check_type(argname="argument runtime", value=runtime, expected_type=type_hints["runtime"])
+                check_type(argname="argument runtime_version", value=runtime_version, expected_type=type_hints["runtime_version"])
+                check_type(argname="argument cpu_policy", value=cpu_policy, expected_type=type_hints["cpu_policy"])
+                check_type(argname="argument labels", value=labels, expected_type=type_hints["labels"])
+                check_type(argname="argument node_name_mode", value=node_name_mode, expected_type=type_hints["node_name_mode"])
+                check_type(argname="argument taints", value=taints, expected_type=type_hints["taints"])
             self._values: typing.Dict[str, typing.Any] = {
                 "runtime": runtime,
                 "runtime_version": runtime_version,
             }
             if cpu_policy is not None:
                 self._values["cpu_policy"] = cpu_policy
             if labels is not None:
@@ -11618,14 +12806,18 @@
             key: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         ) -> None:
             '''
             :param key: 
             :param value: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosManagedKubernetesCluster.LabelsProperty.__init__)
+                check_type(argname="argument key", value=key, expected_type=type_hints["key"])
+                check_type(argname="argument value", value=value, expected_type=type_hints["value"])
             self._values: typing.Dict[str, typing.Any] = {
                 "key": key,
                 "value": value,
             }
 
         @builtins.property
         def key(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
@@ -11666,14 +12858,17 @@
             self,
             *,
             name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         ) -> None:
             '''
             :param name: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosManagedKubernetesCluster.NodePoolInfoProperty.__init__)
+                check_type(argname="argument name", value=name, expected_type=type_hints["name"])
             self._values: typing.Dict[str, typing.Any] = {
                 "name": name,
             }
 
         @builtins.property
         def name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
             '''
@@ -11704,25 +12899,31 @@
             "node_pool_info": "nodePoolInfo",
         },
     )
     class NodePoolsProperty:
         def __init__(
             self,
             *,
-            scaling_group: typing.Union[ros_cdk_core.IResolvable, "RosManagedKubernetesCluster.ScalingGroupProperty"],
+            scaling_group: typing.Union[ros_cdk_core.IResolvable, typing.Union["RosManagedKubernetesCluster.ScalingGroupProperty", typing.Dict[str, typing.Any]]],
             count: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
-            kubernetes_config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosManagedKubernetesCluster.KubernetesConfigProperty"]] = None,
-            node_pool_info: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosManagedKubernetesCluster.NodePoolInfoProperty"]] = None,
+            kubernetes_config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosManagedKubernetesCluster.KubernetesConfigProperty", typing.Dict[str, typing.Any]]]] = None,
+            node_pool_info: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosManagedKubernetesCluster.NodePoolInfoProperty", typing.Dict[str, typing.Any]]]] = None,
         ) -> None:
             '''
             :param scaling_group: 
             :param count: 
             :param kubernetes_config: 
             :param node_pool_info: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosManagedKubernetesCluster.NodePoolsProperty.__init__)
+                check_type(argname="argument scaling_group", value=scaling_group, expected_type=type_hints["scaling_group"])
+                check_type(argname="argument count", value=count, expected_type=type_hints["count"])
+                check_type(argname="argument kubernetes_config", value=kubernetes_config, expected_type=type_hints["kubernetes_config"])
+                check_type(argname="argument node_pool_info", value=node_pool_info, expected_type=type_hints["node_pool_info"])
             self._values: typing.Dict[str, typing.Any] = {
                 "scaling_group": scaling_group,
             }
             if count is not None:
                 self._values["count"] = count
             if kubernetes_config is not None:
                 self._values["kubernetes_config"] = kubernetes_config
@@ -11793,14 +12994,18 @@
             name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             version: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param name: 
             :param version: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosManagedKubernetesCluster.RuntimeProperty.__init__)
+                check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+                check_type(argname="argument version", value=version, expected_type=type_hints["version"])
             self._values: typing.Dict[str, typing.Any] = {
                 "name": name,
             }
             if version is not None:
                 self._values["version"] = version
 
         @builtins.property
@@ -11851,38 +13056,40 @@
             "period": "period",
             "period_unit": "periodUnit",
             "platform": "platform",
             "rds_instances": "rdsInstances",
             "system_disk_category": "systemDiskCategory",
             "system_disk_performance_level": "systemDiskPerformanceLevel",
             "tags": "tags",
+            "zone_ids": "zoneIds",
         },
     )
     class ScalingGroupProperty:
         def __init__(
             self,
             *,
             instance_types: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]],
             system_disk_size: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
             v_switch_ids: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]],
-            data_disks: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosManagedKubernetesCluster.DataDisksProperty"]]]] = None,
+            data_disks: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosManagedKubernetesCluster.DataDisksProperty", typing.Dict[str, typing.Any]]]]]] = None,
             image_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
             instance_charge_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
             internet_charge_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
             internet_max_bandwidth_out: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
             is_enterprise_security_group: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
             key_pair: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
             login_password: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
             period: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
             period_unit: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
             platform: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
             rds_instances: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]] = None,
             system_disk_category: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
             system_disk_performance_level: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-            tags: typing.Optional[typing.Sequence["RosManagedKubernetesCluster.ScalingGroupTagsProperty"]] = None,
+            tags: typing.Optional[typing.Sequence[typing.Union["RosManagedKubernetesCluster.ScalingGroupTagsProperty", typing.Dict[str, typing.Any]]]] = None,
+            zone_ids: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]] = None,
         ) -> None:
             '''
             :param instance_types: 
             :param system_disk_size: 
             :param v_switch_ids: 
             :param data_disks: 
             :param image_id: 
@@ -11895,15 +13102,37 @@
             :param period: 
             :param period_unit: 
             :param platform: 
             :param rds_instances: 
             :param system_disk_category: 
             :param system_disk_performance_level: 
             :param tags: 
+            :param zone_ids: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosManagedKubernetesCluster.ScalingGroupProperty.__init__)
+                check_type(argname="argument instance_types", value=instance_types, expected_type=type_hints["instance_types"])
+                check_type(argname="argument system_disk_size", value=system_disk_size, expected_type=type_hints["system_disk_size"])
+                check_type(argname="argument v_switch_ids", value=v_switch_ids, expected_type=type_hints["v_switch_ids"])
+                check_type(argname="argument data_disks", value=data_disks, expected_type=type_hints["data_disks"])
+                check_type(argname="argument image_id", value=image_id, expected_type=type_hints["image_id"])
+                check_type(argname="argument instance_charge_type", value=instance_charge_type, expected_type=type_hints["instance_charge_type"])
+                check_type(argname="argument internet_charge_type", value=internet_charge_type, expected_type=type_hints["internet_charge_type"])
+                check_type(argname="argument internet_max_bandwidth_out", value=internet_max_bandwidth_out, expected_type=type_hints["internet_max_bandwidth_out"])
+                check_type(argname="argument is_enterprise_security_group", value=is_enterprise_security_group, expected_type=type_hints["is_enterprise_security_group"])
+                check_type(argname="argument key_pair", value=key_pair, expected_type=type_hints["key_pair"])
+                check_type(argname="argument login_password", value=login_password, expected_type=type_hints["login_password"])
+                check_type(argname="argument period", value=period, expected_type=type_hints["period"])
+                check_type(argname="argument period_unit", value=period_unit, expected_type=type_hints["period_unit"])
+                check_type(argname="argument platform", value=platform, expected_type=type_hints["platform"])
+                check_type(argname="argument rds_instances", value=rds_instances, expected_type=type_hints["rds_instances"])
+                check_type(argname="argument system_disk_category", value=system_disk_category, expected_type=type_hints["system_disk_category"])
+                check_type(argname="argument system_disk_performance_level", value=system_disk_performance_level, expected_type=type_hints["system_disk_performance_level"])
+                check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
+                check_type(argname="argument zone_ids", value=zone_ids, expected_type=type_hints["zone_ids"])
             self._values: typing.Dict[str, typing.Any] = {
                 "instance_types": instance_types,
                 "system_disk_size": system_disk_size,
                 "v_switch_ids": v_switch_ids,
             }
             if data_disks is not None:
                 self._values["data_disks"] = data_disks
@@ -11931,14 +13160,16 @@
                 self._values["rds_instances"] = rds_instances
             if system_disk_category is not None:
                 self._values["system_disk_category"] = system_disk_category
             if system_disk_performance_level is not None:
                 self._values["system_disk_performance_level"] = system_disk_performance_level
             if tags is not None:
                 self._values["tags"] = tags
+            if zone_ids is not None:
+                self._values["zone_ids"] = zone_ids
 
         @builtins.property
         def instance_types(
             self,
         ) -> typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]:
             '''
             :Property: instanceTypes: The ECS instance types of the nodes.
@@ -12153,14 +13384,24 @@
 
             tags: Adds labels only to ECS instances.
             A key must be unique and cannot exceed 128 characters in length. Neither keys nor values can start with aliyun or acs:. Neither keys nor values can contain https:// or http://.
             '''
             result = self._values.get("tags")
             return typing.cast(typing.Optional[typing.List["RosManagedKubernetesCluster.ScalingGroupTagsProperty"]], result)
 
+        @builtins.property
+        def zone_ids(
+            self,
+        ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]]:
+            '''
+            :Property: zoneIds: Zone ids of virtual switches belongs to.
+            '''
+            result = self._values.get("zone_ids")
+            return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]], result)
+
         def __eq__(self, rhs: typing.Any) -> builtins.bool:
             return isinstance(rhs, self.__class__) and rhs._values == self._values
 
         def __ne__(self, rhs: typing.Any) -> builtins.bool:
             return not (rhs == self)
 
         def __repr__(self) -> str:
@@ -12180,14 +13421,18 @@
             key: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         ) -> None:
             '''
             :param key: 
             :param value: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosManagedKubernetesCluster.ScalingGroupTagsProperty.__init__)
+                check_type(argname="argument key", value=key, expected_type=type_hints["key"])
+                check_type(argname="argument value", value=value, expected_type=type_hints["value"])
             self._values: typing.Dict[str, typing.Any] = {
                 "key": key,
                 "value": value,
             }
 
         @builtins.property
         def key(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
@@ -12230,14 +13475,18 @@
             key: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param key: 
             :param value: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosManagedKubernetesCluster.TagsProperty.__init__)
+                check_type(argname="argument key", value=key, expected_type=type_hints["key"])
+                check_type(argname="argument value", value=value, expected_type=type_hints["value"])
             self._values: typing.Dict[str, typing.Any] = {
                 "key": key,
             }
             if value is not None:
                 self._values["value"] = value
 
         @builtins.property
@@ -12284,14 +13533,19 @@
             effect: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param key: 
             :param value: 
             :param effect: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosManagedKubernetesCluster.TaintsProperty.__init__)
+                check_type(argname="argument key", value=key, expected_type=type_hints["key"])
+                check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+                check_type(argname="argument effect", value=effect, expected_type=type_hints["effect"])
             self._values: typing.Dict[str, typing.Any] = {
                 "key": key,
                 "value": value,
             }
             if effect is not None:
                 self._values["effect"] = effect
 
@@ -12352,14 +13606,18 @@
             category: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             size: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
         ) -> None:
             '''
             :param category: 
             :param size: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosManagedKubernetesCluster.WorkerDataDisksProperty.__init__)
+                check_type(argname="argument category", value=category, expected_type=type_hints["category"])
+                check_type(argname="argument size", value=size, expected_type=type_hints["size"])
             self._values: typing.Dict[str, typing.Any] = {
                 "category": category,
                 "size": size,
             }
 
         @builtins.property
         def category(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
@@ -12453,15 +13711,15 @@
 class RosManagedKubernetesClusterProps:
     def __init__(
         self,
         *,
         name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         vpc_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         v_switch_ids: typing.Union[typing.Sequence[typing.Any], ros_cdk_core.IResolvable],
-        addons: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosManagedKubernetesCluster.AddonsProperty]]]] = None,
+        addons: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosManagedKubernetesCluster.AddonsProperty, typing.Dict[str, typing.Any]]]]]] = None,
         auto_renew: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         auto_renew_period: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         charge_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         cis_enabled: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         cloud_monitor_flags: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         cluster_spec: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         container_cidr: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
@@ -12474,34 +13732,34 @@
         keep_instance_name: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         key_pair: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         kubernetes_version: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         load_balancer_spec: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         login_password: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         node_cidr_mask: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         node_name_mode: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        node_pools: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosManagedKubernetesCluster.NodePoolsProperty]]]] = None,
+        node_pools: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosManagedKubernetesCluster.NodePoolsProperty, typing.Dict[str, typing.Any]]]]]] = None,
         num_of_nodes: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         os_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         period: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         period_unit: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         platform: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         pod_vswitch_ids: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]] = None,
         proxy_mode: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         resource_group_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        runtime: typing.Optional[typing.Union[ros_cdk_core.IResolvable, RosManagedKubernetesCluster.RuntimeProperty]] = None,
+        runtime: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosManagedKubernetesCluster.RuntimeProperty, typing.Dict[str, typing.Any]]]] = None,
         security_group_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         service_cidr: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         snat_entry: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         soc_enabled: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
-        tags: typing.Optional[typing.Sequence[RosManagedKubernetesCluster.TagsProperty]] = None,
+        tags: typing.Optional[typing.Sequence[typing.Union[RosManagedKubernetesCluster.TagsProperty, typing.Dict[str, typing.Any]]]] = None,
         taint: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Mapping[builtins.str, typing.Any]]]] = None,
         timeout_mins: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         user_data: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         worker_data_disk: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
-        worker_data_disks: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosManagedKubernetesCluster.WorkerDataDisksProperty]]]] = None,
+        worker_data_disks: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosManagedKubernetesCluster.WorkerDataDisksProperty, typing.Dict[str, typing.Any]]]]]] = None,
         worker_instance_types: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]] = None,
         worker_system_disk_category: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         worker_system_disk_size: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         zone_ids: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::CS::ManagedKubernetesCluster``.
 
@@ -12550,14 +13808,64 @@
         :param worker_data_disk: 
         :param worker_data_disks: 
         :param worker_instance_types: 
         :param worker_system_disk_category: 
         :param worker_system_disk_size: 
         :param zone_ids: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosManagedKubernetesClusterProps.__init__)
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+            check_type(argname="argument vpc_id", value=vpc_id, expected_type=type_hints["vpc_id"])
+            check_type(argname="argument v_switch_ids", value=v_switch_ids, expected_type=type_hints["v_switch_ids"])
+            check_type(argname="argument addons", value=addons, expected_type=type_hints["addons"])
+            check_type(argname="argument auto_renew", value=auto_renew, expected_type=type_hints["auto_renew"])
+            check_type(argname="argument auto_renew_period", value=auto_renew_period, expected_type=type_hints["auto_renew_period"])
+            check_type(argname="argument charge_type", value=charge_type, expected_type=type_hints["charge_type"])
+            check_type(argname="argument cis_enabled", value=cis_enabled, expected_type=type_hints["cis_enabled"])
+            check_type(argname="argument cloud_monitor_flags", value=cloud_monitor_flags, expected_type=type_hints["cloud_monitor_flags"])
+            check_type(argname="argument cluster_spec", value=cluster_spec, expected_type=type_hints["cluster_spec"])
+            check_type(argname="argument container_cidr", value=container_cidr, expected_type=type_hints["container_cidr"])
+            check_type(argname="argument deletion_protection", value=deletion_protection, expected_type=type_hints["deletion_protection"])
+            check_type(argname="argument disable_rollback", value=disable_rollback, expected_type=type_hints["disable_rollback"])
+            check_type(argname="argument encryption_provider_key", value=encryption_provider_key, expected_type=type_hints["encryption_provider_key"])
+            check_type(argname="argument endpoint_public_access", value=endpoint_public_access, expected_type=type_hints["endpoint_public_access"])
+            check_type(argname="argument format_disk", value=format_disk, expected_type=type_hints["format_disk"])
+            check_type(argname="argument is_enterprise_security_group", value=is_enterprise_security_group, expected_type=type_hints["is_enterprise_security_group"])
+            check_type(argname="argument keep_instance_name", value=keep_instance_name, expected_type=type_hints["keep_instance_name"])
+            check_type(argname="argument key_pair", value=key_pair, expected_type=type_hints["key_pair"])
+            check_type(argname="argument kubernetes_version", value=kubernetes_version, expected_type=type_hints["kubernetes_version"])
+            check_type(argname="argument load_balancer_spec", value=load_balancer_spec, expected_type=type_hints["load_balancer_spec"])
+            check_type(argname="argument login_password", value=login_password, expected_type=type_hints["login_password"])
+            check_type(argname="argument node_cidr_mask", value=node_cidr_mask, expected_type=type_hints["node_cidr_mask"])
+            check_type(argname="argument node_name_mode", value=node_name_mode, expected_type=type_hints["node_name_mode"])
+            check_type(argname="argument node_pools", value=node_pools, expected_type=type_hints["node_pools"])
+            check_type(argname="argument num_of_nodes", value=num_of_nodes, expected_type=type_hints["num_of_nodes"])
+            check_type(argname="argument os_type", value=os_type, expected_type=type_hints["os_type"])
+            check_type(argname="argument period", value=period, expected_type=type_hints["period"])
+            check_type(argname="argument period_unit", value=period_unit, expected_type=type_hints["period_unit"])
+            check_type(argname="argument platform", value=platform, expected_type=type_hints["platform"])
+            check_type(argname="argument pod_vswitch_ids", value=pod_vswitch_ids, expected_type=type_hints["pod_vswitch_ids"])
+            check_type(argname="argument proxy_mode", value=proxy_mode, expected_type=type_hints["proxy_mode"])
+            check_type(argname="argument resource_group_id", value=resource_group_id, expected_type=type_hints["resource_group_id"])
+            check_type(argname="argument runtime", value=runtime, expected_type=type_hints["runtime"])
+            check_type(argname="argument security_group_id", value=security_group_id, expected_type=type_hints["security_group_id"])
+            check_type(argname="argument service_cidr", value=service_cidr, expected_type=type_hints["service_cidr"])
+            check_type(argname="argument snat_entry", value=snat_entry, expected_type=type_hints["snat_entry"])
+            check_type(argname="argument soc_enabled", value=soc_enabled, expected_type=type_hints["soc_enabled"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
+            check_type(argname="argument taint", value=taint, expected_type=type_hints["taint"])
+            check_type(argname="argument timeout_mins", value=timeout_mins, expected_type=type_hints["timeout_mins"])
+            check_type(argname="argument user_data", value=user_data, expected_type=type_hints["user_data"])
+            check_type(argname="argument worker_data_disk", value=worker_data_disk, expected_type=type_hints["worker_data_disk"])
+            check_type(argname="argument worker_data_disks", value=worker_data_disks, expected_type=type_hints["worker_data_disks"])
+            check_type(argname="argument worker_instance_types", value=worker_instance_types, expected_type=type_hints["worker_instance_types"])
+            check_type(argname="argument worker_system_disk_category", value=worker_system_disk_category, expected_type=type_hints["worker_system_disk_category"])
+            check_type(argname="argument worker_system_disk_size", value=worker_system_disk_size, expected_type=type_hints["worker_system_disk_size"])
+            check_type(argname="argument zone_ids", value=zone_ids, expected_type=type_hints["zone_ids"])
         self._values: typing.Dict[str, typing.Any] = {
             "name": name,
             "vpc_id": vpc_id,
             "v_switch_ids": v_switch_ids,
         }
         if addons is not None:
             self._values["addons"] = addons
@@ -13020,14 +14328,15 @@
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
         period: The duration of the annual subscription and monthly subscription. It takes effect when the ChargeType value is PrePaid and is a required value. The value range is:
         When PeriodUnit = Week, Period values are: {"1", "2", "3", "4"}
         When PeriodUnit = Month, Period values are: {"1", "2", "3", "4", "5", "6", "7", "8", "9", "12", "24", "36", "48", "60"}
+        When PeriodUnit = Year, Period values are: {"1", "2", "3", "4", "5"}
         Default to 1.
         '''
         result = self._values.get("period")
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], result)
 
     @builtins.property
     def period_unit(
@@ -13035,14 +14344,15 @@
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
         periodUnit: When you specify PrePaid, you need to specify the period. The options are:
         Week: Time is measured in weeks
         Month: time in months
+        Year: time in years
         Default to Month
         '''
         result = self._values.get("period_unit")
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], result)
 
     @builtins.property
     def platform(
@@ -13295,166 +14605,184 @@
 ):
     '''A ROS template type:  ``ALIYUN::CS::ServerlessKubernetesCluster``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosServerlessKubernetesClusterProps",
+        props: typing.Union["RosServerlessKubernetesClusterProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::CS::ServerlessKubernetesCluster``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosServerlessKubernetesCluster.__init__)
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
+            type_hints = typing.get_type_hints(RosServerlessKubernetesCluster._render_properties)
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
     @jsii.member(jsii_name="attrApiServerSlbId")
     def attr_api_server_slb_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: APIServerSLBId: The id of API server SLB
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrApiServerSlbId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrClusterId")
     def attr_cluster_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ClusterId: Cluster instance ID.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrClusterId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDefaultUserKubeConfig")
     def attr_default_user_kube_config(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: DefaultUserKubeConfig: Default user kubernetes config which is used for configuring cluster credentials.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDefaultUserKubeConfig"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrNodes")
     def attr_nodes(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Nodes: The list of cluster nodes.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrNodes"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPrivateUserKubConfig")
     def attr_private_user_kub_config(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: PrivateUserKubConfig: Private user kubernetes config which is used for configuring cluster credentials.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPrivateUserKubConfig"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrScalingConfigurationId")
     def attr_scaling_configuration_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ScalingConfigurationId: Scaling configuration id
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrScalingConfigurationId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrScalingGroupId")
     def attr_scaling_group_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ScalingGroupId: Scaling group id
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrScalingGroupId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrScalingRuleId")
     def attr_scaling_rule_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ScalingRuleId: Scaling rule id
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrScalingRuleId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTaskId")
     def attr_task_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: TaskId: Task ID. Automatically assigned by the system, the user queries the task status.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTaskId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrWorkerRamRoleName")
     def attr_worker_ram_role_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: WorkerRamRoleName: Worker ram role name.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrWorkerRamRoleName"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosServerlessKubernetesCluster, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="name")
     def name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: name: The name of the cluster. The cluster name can use uppercase and lowercase letters, Chinese characters, numbers, and dashes.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "name"))
 
     @name.setter
     def name(self, value: typing.Union[builtins.str, ros_cdk_core.IResolvable]) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosServerlessKubernetesCluster, "name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "name", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="addons")
     def addons(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosServerlessKubernetesCluster.AddonsProperty"]]]]:
         '''
         :Property: addons: The add-ons to be installed for the cluster.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosServerlessKubernetesCluster.AddonsProperty"]]]], jsii.get(self, "addons"))
 
     @addons.setter
     def addons(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosServerlessKubernetesCluster.AddonsProperty"]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosServerlessKubernetesCluster, "addons").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "addons", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="endpointPublicAccess")
     def endpoint_public_access(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -13465,136 +14793,160 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "endpointPublicAccess"))
 
     @endpoint_public_access.setter
     def endpoint_public_access(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosServerlessKubernetesCluster, "endpoint_public_access").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "endpointPublicAccess", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="kubernetesVersion")
     def kubernetes_version(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: kubernetesVersion: The version of the Kubernetes cluster.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "kubernetesVersion"))
 
     @kubernetes_version.setter
     def kubernetes_version(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosServerlessKubernetesCluster, "kubernetes_version").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "kubernetesVersion", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="natGateway")
     def nat_gateway(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property: natGateway: Whether to create a NAT gateway. The value can be true or false. If not set, the system defaults to false.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "natGateway"))
 
     @nat_gateway.setter
     def nat_gateway(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosServerlessKubernetesCluster, "nat_gateway").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "natGateway", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="privateZone")
     def private_zone(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property: privateZone: Whether to enable PrivateZone for service discovery.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "privateZone"))
 
     @private_zone.setter
     def private_zone(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosServerlessKubernetesCluster, "private_zone").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "privateZone", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="resourceGroupId")
     def resource_group_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: resourceGroupId: The ID of resource group.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "resourceGroupId"))
 
     @resource_group_id.setter
     def resource_group_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosServerlessKubernetesCluster, "resource_group_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "resourceGroupId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="securityGroupId")
     def security_group_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: securityGroupId: Specifies the ID of the security group to which the cluster ECS instance belongs.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "securityGroupId"))
 
     @security_group_id.setter
     def security_group_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosServerlessKubernetesCluster, "security_group_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "securityGroupId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="serviceCidr")
     def service_cidr(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: serviceCidr: The service network segment cannot conflict with the VPC network segment and the container network segment. When the system is selected to automatically create a VPC, the network segment 172.19.0.0/20 is used by default.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "serviceCidr"))
 
     @service_cidr.setter
     def service_cidr(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosServerlessKubernetesCluster, "service_cidr").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "serviceCidr", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="tags")
     def tags(
         self,
     ) -> typing.Optional[typing.List["RosServerlessKubernetesCluster.TagsProperty"]]:
         '''
         :Property: tags: Tag the cluster.
         '''
         return typing.cast(typing.Optional[typing.List["RosServerlessKubernetesCluster.TagsProperty"]], jsii.get(self, "tags"))
 
     @tags.setter
     def tags(
         self,
         value: typing.Optional[typing.List["RosServerlessKubernetesCluster.TagsProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosServerlessKubernetesCluster, "tags").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "tags", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vpcId")
     def vpc_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -13604,34 +14956,40 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "vpcId"))
 
     @vpc_id.setter
     def vpc_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosServerlessKubernetesCluster, "vpc_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "vpcId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vSwitchId")
     def v_switch_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: vSwitchId: If not set, the system will automatically create a switch, and the network segment of the switch created by the system is 192.168.0.0/18.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "vSwitchId"))
 
     @v_switch_id.setter
     def v_switch_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosServerlessKubernetesCluster, "v_switch_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "vSwitchId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vSwitchIds")
     def v_switch_ids(
         self,
     ) -> typing.Optional[typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -13641,31 +14999,37 @@
         return typing.cast(typing.Optional[typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]], jsii.get(self, "vSwitchIds"))
 
     @v_switch_ids.setter
     def v_switch_ids(
         self,
         value: typing.Optional[typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosServerlessKubernetesCluster, "v_switch_ids").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "vSwitchIds", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="zoneId")
     def zone_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: zoneId: The zone ID.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "zoneId"))
 
     @zone_id.setter
     def zone_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosServerlessKubernetesCluster, "zone_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "zoneId", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-cs.RosServerlessKubernetesCluster.AddonsProperty",
         jsii_struct_bases=[],
         name_mapping={"name": "name", "config": "config", "disabled": "disabled"},
     )
@@ -13678,14 +15042,19 @@
             disabled: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param name: 
             :param config: 
             :param disabled: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosServerlessKubernetesCluster.AddonsProperty.__init__)
+                check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+                check_type(argname="argument config", value=config, expected_type=type_hints["config"])
+                check_type(argname="argument disabled", value=disabled, expected_type=type_hints["disabled"])
             self._values: typing.Dict[str, typing.Any] = {
                 "name": name,
             }
             if config is not None:
                 self._values["config"] = config
             if disabled is not None:
                 self._values["disabled"] = disabled
@@ -13742,14 +15111,18 @@
             key: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param key: 
             :param value: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosServerlessKubernetesCluster.TagsProperty.__init__)
+                check_type(argname="argument key", value=key, expected_type=type_hints["key"])
+                check_type(argname="argument value", value=value, expected_type=type_hints["value"])
             self._values: typing.Dict[str, typing.Any] = {
                 "key": key,
             }
             if value is not None:
                 self._values["value"] = value
 
         @builtins.property
@@ -13804,23 +15177,23 @@
     },
 )
 class RosServerlessKubernetesClusterProps:
     def __init__(
         self,
         *,
         name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
-        addons: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosServerlessKubernetesCluster.AddonsProperty]]]] = None,
+        addons: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosServerlessKubernetesCluster.AddonsProperty, typing.Dict[str, typing.Any]]]]]] = None,
         endpoint_public_access: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         kubernetes_version: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         nat_gateway: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         private_zone: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         resource_group_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         security_group_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         service_cidr: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        tags: typing.Optional[typing.Sequence[RosServerlessKubernetesCluster.TagsProperty]] = None,
+        tags: typing.Optional[typing.Sequence[typing.Union[RosServerlessKubernetesCluster.TagsProperty, typing.Dict[str, typing.Any]]]] = None,
         vpc_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         v_switch_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         v_switch_ids: typing.Optional[typing.Union[typing.Sequence[typing.Any], ros_cdk_core.IResolvable]] = None,
         zone_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::CS::ServerlessKubernetesCluster``.
 
@@ -13835,14 +15208,30 @@
         :param service_cidr: 
         :param tags: 
         :param vpc_id: 
         :param v_switch_id: 
         :param v_switch_ids: 
         :param zone_id: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosServerlessKubernetesClusterProps.__init__)
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+            check_type(argname="argument addons", value=addons, expected_type=type_hints["addons"])
+            check_type(argname="argument endpoint_public_access", value=endpoint_public_access, expected_type=type_hints["endpoint_public_access"])
+            check_type(argname="argument kubernetes_version", value=kubernetes_version, expected_type=type_hints["kubernetes_version"])
+            check_type(argname="argument nat_gateway", value=nat_gateway, expected_type=type_hints["nat_gateway"])
+            check_type(argname="argument private_zone", value=private_zone, expected_type=type_hints["private_zone"])
+            check_type(argname="argument resource_group_id", value=resource_group_id, expected_type=type_hints["resource_group_id"])
+            check_type(argname="argument security_group_id", value=security_group_id, expected_type=type_hints["security_group_id"])
+            check_type(argname="argument service_cidr", value=service_cidr, expected_type=type_hints["service_cidr"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
+            check_type(argname="argument vpc_id", value=vpc_id, expected_type=type_hints["vpc_id"])
+            check_type(argname="argument v_switch_id", value=v_switch_id, expected_type=type_hints["v_switch_id"])
+            check_type(argname="argument v_switch_ids", value=v_switch_ids, expected_type=type_hints["v_switch_ids"])
+            check_type(argname="argument zone_id", value=zone_id, expected_type=type_hints["zone_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "name": name,
         }
         if addons is not None:
             self._values["addons"] = addons
         if endpoint_public_access is not None:
             self._values["endpoint_public_access"] = endpoint_public_access
@@ -14037,88 +15426,94 @@
 ):
     '''A ROS resource type:  ``ALIYUN::CS::ServerlessKubernetesCluster``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "ServerlessKubernetesClusterProps",
+        props: typing.Union["ServerlessKubernetesClusterProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::CS::ServerlessKubernetesCluster``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(ServerlessKubernetesCluster.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrApiServerSlbId")
     def attr_api_server_slb_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute APIServerSLBId: The id of API server SLB.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrApiServerSlbId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrClusterId")
     def attr_cluster_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute ClusterId: Cluster instance ID.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrClusterId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDefaultUserKubeConfig")
     def attr_default_user_kube_config(self) -> ros_cdk_core.IResolvable:
         '''Attribute DefaultUserKubeConfig: Default user kubernetes config which is used for configuring cluster credentials.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDefaultUserKubeConfig"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrNodes")
     def attr_nodes(self) -> ros_cdk_core.IResolvable:
         '''Attribute Nodes: The list of cluster nodes.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrNodes"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPrivateUserKubConfig")
     def attr_private_user_kub_config(self) -> ros_cdk_core.IResolvable:
         '''Attribute PrivateUserKubConfig: Private user kubernetes config which is used for configuring cluster credentials.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPrivateUserKubConfig"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrScalingConfigurationId")
     def attr_scaling_configuration_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute ScalingConfigurationId: Scaling configuration id.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrScalingConfigurationId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrScalingGroupId")
     def attr_scaling_group_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute ScalingGroupId: Scaling group id.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrScalingGroupId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrScalingRuleId")
     def attr_scaling_rule_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute ScalingRuleId: Scaling rule id.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrScalingRuleId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTaskId")
     def attr_task_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute TaskId: Task ID.
 
         Automatically assigned by the system, the user queries the task status.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTaskId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrWorkerRamRoleName")
     def attr_worker_ram_role_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute WorkerRamRoleName: Worker ram role name.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrWorkerRamRoleName"))
 
 
 @jsii.data_type(
@@ -14142,23 +15537,23 @@
     },
 )
 class ServerlessKubernetesClusterProps:
     def __init__(
         self,
         *,
         name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
-        addons: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosServerlessKubernetesCluster.AddonsProperty]]]] = None,
+        addons: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosServerlessKubernetesCluster.AddonsProperty, typing.Dict[str, typing.Any]]]]]] = None,
         endpoint_public_access: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         kubernetes_version: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         nat_gateway: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         private_zone: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         resource_group_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         security_group_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         service_cidr: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        tags: typing.Optional[typing.Sequence[RosServerlessKubernetesCluster.TagsProperty]] = None,
+        tags: typing.Optional[typing.Sequence[typing.Union[RosServerlessKubernetesCluster.TagsProperty, typing.Dict[str, typing.Any]]]] = None,
         vpc_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         v_switch_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         v_switch_ids: typing.Optional[typing.Union[typing.Sequence[typing.Any], ros_cdk_core.IResolvable]] = None,
         zone_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::CS::ServerlessKubernetesCluster``.
 
@@ -14173,14 +15568,30 @@
         :param service_cidr: Property serviceCidr: The service network segment cannot conflict with the VPC network segment and the container network segment. When the system is selected to automatically create a VPC, the network segment 172.19.0.0/20 is used by default.
         :param tags: Property tags: Tag the cluster.
         :param vpc_id: Property vpcId: VPC ID. If not set, the system will automatically create a VPC, and the VPC network segment created by the system is 192.168.0.0/16. VpcId and VSwitchId can only be empty at the same time or set the corresponding values at the same time.
         :param v_switch_id: Property vSwitchId: If not set, the system will automatically create a switch, and the network segment of the switch created by the system is 192.168.0.0/18.
         :param v_switch_ids: Property vSwitchIds: The IDs of VSwitches. If you leave this property empty, the system automatically creates a VSwitch. Note You must specify both the VpcId and VSwitchIds or leave both of them empty.
         :param zone_id: Property zoneId: The zone ID.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(ServerlessKubernetesClusterProps.__init__)
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+            check_type(argname="argument addons", value=addons, expected_type=type_hints["addons"])
+            check_type(argname="argument endpoint_public_access", value=endpoint_public_access, expected_type=type_hints["endpoint_public_access"])
+            check_type(argname="argument kubernetes_version", value=kubernetes_version, expected_type=type_hints["kubernetes_version"])
+            check_type(argname="argument nat_gateway", value=nat_gateway, expected_type=type_hints["nat_gateway"])
+            check_type(argname="argument private_zone", value=private_zone, expected_type=type_hints["private_zone"])
+            check_type(argname="argument resource_group_id", value=resource_group_id, expected_type=type_hints["resource_group_id"])
+            check_type(argname="argument security_group_id", value=security_group_id, expected_type=type_hints["security_group_id"])
+            check_type(argname="argument service_cidr", value=service_cidr, expected_type=type_hints["service_cidr"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
+            check_type(argname="argument vpc_id", value=vpc_id, expected_type=type_hints["vpc_id"])
+            check_type(argname="argument v_switch_id", value=v_switch_id, expected_type=type_hints["v_switch_id"])
+            check_type(argname="argument v_switch_ids", value=v_switch_ids, expected_type=type_hints["v_switch_ids"])
+            check_type(argname="argument zone_id", value=zone_id, expected_type=type_hints["zone_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "name": name,
         }
         if addons is not None:
             self._values["addons"] = addons
         if endpoint_public_access is not None:
             self._values["endpoint_public_access"] = endpoint_public_access
```

### Comparing `ros-cdk-cs-1.0.8/src/ros_cdk_cs.egg-info/PKG-INFO` & `ros-cdk-cs-1.0.9/src/ros_cdk_cs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-cs
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS CS Construct Library
```

