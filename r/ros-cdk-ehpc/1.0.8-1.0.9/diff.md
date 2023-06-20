# Comparing `tmp/ros-cdk-ehpc-1.0.8.tar.gz` & `tmp/ros-cdk-ehpc-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-ehpc-1.0.8.tar", last modified: Thu Jul 14 02:34:29 2022, max compression
+gzip compressed data, was "dist/ros-cdk-ehpc-1.0.9.tar", last modified: Fri Sep 23 11:03:07 2022, max compression
```

## Comparing `ros-cdk-ehpc-1.0.8.tar` & `ros-cdk-ehpc-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:34:29.000000 ros-cdk-ehpc-1.0.8/
--rw-r--r--   0 root         (0) root         (0)    10279 2022-07-14 02:34:29.000000 ros-cdk-ehpc-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2022-07-14 02:34:29.000000 ros-cdk-ehpc-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2022-07-14 02:34:29.000000 ros-cdk-ehpc-1.0.8/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1244 2022-07-14 02:34:29.000000 ros-cdk-ehpc-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      182 2022-07-14 02:34:29.000000 ros-cdk-ehpc-1.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)      106 2022-07-14 02:34:29.000000 ros-cdk-ehpc-1.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-07-14 02:34:29.000000 ros-cdk-ehpc-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1800 2022-07-14 02:34:29.000000 ros-cdk-ehpc-1.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:34:29.000000 ros-cdk-ehpc-1.0.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:34:29.000000 ros-cdk-ehpc-1.0.8/src/ros_cdk_ehpc/
--rw-r--r--   0 root         (0) root         (0)   137809 2022-07-14 02:34:29.000000 ros-cdk-ehpc-1.0.8/src/ros_cdk_ehpc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:34:29.000000 ros-cdk-ehpc-1.0.8/src/ros_cdk_ehpc/_jsii/
--rw-r--r--   0 root         (0) root         (0)      372 2022-07-14 02:34:29.000000 ros-cdk-ehpc-1.0.8/src/ros_cdk_ehpc/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    69915 2022-07-14 02:34:29.000000 ros-cdk-ehpc-1.0.8/src/ros_cdk_ehpc/_jsii/ros-cdk-ehpc@1.0.8.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:34:29.000000 ros-cdk-ehpc-1.0.8/src/ros_cdk_ehpc/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:34:29.000000 ros-cdk-ehpc-1.0.8/src/ros_cdk_ehpc.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1244 2022-07-14 02:34:29.000000 ros-cdk-ehpc-1.0.8/src/ros_cdk_ehpc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      410 2022-07-14 02:34:29.000000 ros-cdk-ehpc-1.0.8/src/ros_cdk_ehpc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:34:29.000000 ros-cdk-ehpc-1.0.8/src/ros_cdk_ehpc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2022-07-14 02:34:29.000000 ros-cdk-ehpc-1.0.8/src/ros_cdk_ehpc.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2022-07-14 02:34:29.000000 ros-cdk-ehpc-1.0.8/src/ros_cdk_ehpc.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:03:07.000000 ros-cdk-ehpc-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)    10279 2022-09-23 11:03:07.000000 ros-cdk-ehpc-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-09-23 11:03:07.000000 ros-cdk-ehpc-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2022-09-23 11:03:07.000000 ros-cdk-ehpc-1.0.9/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1244 2022-09-23 11:03:07.000000 ros-cdk-ehpc-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      182 2022-09-23 11:03:07.000000 ros-cdk-ehpc-1.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      236 2022-09-23 11:03:07.000000 ros-cdk-ehpc-1.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-09-23 11:03:07.000000 ros-cdk-ehpc-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1829 2022-09-23 11:03:07.000000 ros-cdk-ehpc-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:03:07.000000 ros-cdk-ehpc-1.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:03:07.000000 ros-cdk-ehpc-1.0.9/src/ros_cdk_ehpc/
+-rw-r--r--   0 root         (0) root         (0)   163127 2022-09-23 11:03:07.000000 ros-cdk-ehpc-1.0.9/src/ros_cdk_ehpc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:03:07.000000 ros-cdk-ehpc-1.0.9/src/ros_cdk_ehpc/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      406 2022-09-23 11:03:07.000000 ros-cdk-ehpc-1.0.9/src/ros_cdk_ehpc/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    69989 2022-09-23 11:03:07.000000 ros-cdk-ehpc-1.0.9/src/ros_cdk_ehpc/_jsii/ros-cdk-ehpc@1.0.9.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 11:03:07.000000 ros-cdk-ehpc-1.0.9/src/ros_cdk_ehpc/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:03:07.000000 ros-cdk-ehpc-1.0.9/src/ros_cdk_ehpc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1244 2022-09-23 11:03:07.000000 ros-cdk-ehpc-1.0.9/src/ros_cdk_ehpc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      410 2022-09-23 11:03:07.000000 ros-cdk-ehpc-1.0.9/src/ros_cdk_ehpc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 11:03:07.000000 ros-cdk-ehpc-1.0.9/src/ros_cdk_ehpc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2022-09-23 11:03:07.000000 ros-cdk-ehpc-1.0.9/src/ros_cdk_ehpc.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2022-09-23 11:03:07.000000 ros-cdk-ehpc-1.0.9/src/ros_cdk_ehpc.egg-info/top_level.txt
```

### Comparing `ros-cdk-ehpc-1.0.8/LICENSE` & `ros-cdk-ehpc-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-ehpc-1.0.8/PKG-INFO` & `ros-cdk-ehpc-1.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-ehpc
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS EHPC Construct Library
```

### Comparing `ros-cdk-ehpc-1.0.8/setup.py` & `ros-cdk-ehpc-1.0.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-ehpc",
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
         "ros_cdk_ehpc",
         "ros_cdk_ehpc._jsii"
     ],
     "package_data": {
         "ros_cdk_ehpc._jsii": [
-            "ros-cdk-ehpc@1.0.8.jsii.tgz"
+            "ros-cdk-ehpc@1.0.9.jsii.tgz"
         ],
         "ros_cdk_ehpc": [
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

### Comparing `ros-cdk-ehpc-1.0.8/src/ros_cdk_ehpc/__init__.py` & `ros-cdk-ehpc-1.0.9/src/ros_cdk_ehpc/__init__.py`

 * *Files 18% similar despite different names*

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
@@ -29,52 +31,58 @@
 ):
     '''A ROS resource type:  ``ALIYUN::EHPC::Cluster``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "ClusterProps",
+        props: typing.Union["ClusterProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::EHPC::Cluster``.
 
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
         '''Attribute ClusterId: Cluster Id.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrClusterId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrEcsInfo")
     def attr_ecs_info(self) -> ros_cdk_core.IResolvable:
         '''Attribute EcsInfo: A data structure describing the number and specifications of ECS for various components of the cluster.
 
         You will get results similar to the following: EcsInfo: {"Manager": {"Count": 2, "InstanceType": "ecs.n1.large"}, "Compute": {"Count": 8, "InstanceType": "ecs.n1.large"}, "Login": {"Count": 1, "InstanceType": "ecs.n1.large"}}
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrEcsInfo"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrName")
     def attr_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute Name: Cluster name.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrSecurityGroupId")
     def attr_security_group_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute SecurityGroupId: Security group ID.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrSecurityGroupId"))
 
 
 @jsii.data_type(
@@ -141,16 +149,16 @@
         ecs_order_login_count: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
         ecs_order_login_instance_type: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         ecs_order_manager_instance_type: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         os_tag: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         v_switch_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         account_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        additional_volumes: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosCluster.AdditionalVolumesProperty"]]]] = None,
-        application: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosCluster.ApplicationProperty"]]]] = None,
+        additional_volumes: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosCluster.AdditionalVolumesProperty", typing.Dict[str, typing.Any]]]]]] = None,
+        application: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosCluster.ApplicationProperty", typing.Dict[str, typing.Any]]]]]] = None,
         auto_renew: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         auto_renew_period: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         client_version: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         compute_enable_ht: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         compute_spot_price_limit: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         compute_spot_strategy: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         deploy_mode: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
@@ -164,15 +172,15 @@
         input_file_url: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         is_compute_ess: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         job_queue: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         key_pair_name: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         password: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         period: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         period_unit: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        post_install_script: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosCluster.PostInstallScriptProperty"]]]] = None,
+        post_install_script: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosCluster.PostInstallScriptProperty", typing.Dict[str, typing.Any]]]]]] = None,
         remote_directory: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         remote_vis_enable: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         resource_group_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         scc_cluster_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         scheduler_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         security_group_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         security_group_name: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
@@ -234,14 +242,65 @@
         :param volume_id: Property volumeId: The ID of the file system. If you leave the parameter empty, a Performance NAS file system is created by default.
         :param volume_mountpoint: Property volumeMountpoint: The mount target of the file system. Take note of the following information: If you do not specify the VolumeId parameter, you can leave the VolumeMountpoint parameter empty. A mount target is created by default. If you specify the VolumeId parameter, the VolumeMountpoint parameter is required.
         :param volume_protocol: Property volumeProtocol: The type of the protocol that is used by the file system. Valid values: nfs smb Default value: nfs
         :param volume_type: Property volumeType: The type of the shared storage. Only Apsara File Storage nas file systems are supported.
         :param without_elastic_ip: Property withoutElasticIp: Specifies whether the logon node uses an elastic IP address (EIP). Default value: false
         :param zone_id: Property zoneId: Available area ID.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(ClusterProps.__init__)
+            check_type(argname="argument ecs_order_compute_count", value=ecs_order_compute_count, expected_type=type_hints["ecs_order_compute_count"])
+            check_type(argname="argument ecs_order_compute_instance_type", value=ecs_order_compute_instance_type, expected_type=type_hints["ecs_order_compute_instance_type"])
+            check_type(argname="argument ecs_order_login_count", value=ecs_order_login_count, expected_type=type_hints["ecs_order_login_count"])
+            check_type(argname="argument ecs_order_login_instance_type", value=ecs_order_login_instance_type, expected_type=type_hints["ecs_order_login_instance_type"])
+            check_type(argname="argument ecs_order_manager_instance_type", value=ecs_order_manager_instance_type, expected_type=type_hints["ecs_order_manager_instance_type"])
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+            check_type(argname="argument os_tag", value=os_tag, expected_type=type_hints["os_tag"])
+            check_type(argname="argument v_switch_id", value=v_switch_id, expected_type=type_hints["v_switch_id"])
+            check_type(argname="argument account_type", value=account_type, expected_type=type_hints["account_type"])
+            check_type(argname="argument additional_volumes", value=additional_volumes, expected_type=type_hints["additional_volumes"])
+            check_type(argname="argument application", value=application, expected_type=type_hints["application"])
+            check_type(argname="argument auto_renew", value=auto_renew, expected_type=type_hints["auto_renew"])
+            check_type(argname="argument auto_renew_period", value=auto_renew_period, expected_type=type_hints["auto_renew_period"])
+            check_type(argname="argument client_version", value=client_version, expected_type=type_hints["client_version"])
+            check_type(argname="argument compute_enable_ht", value=compute_enable_ht, expected_type=type_hints["compute_enable_ht"])
+            check_type(argname="argument compute_spot_price_limit", value=compute_spot_price_limit, expected_type=type_hints["compute_spot_price_limit"])
+            check_type(argname="argument compute_spot_strategy", value=compute_spot_strategy, expected_type=type_hints["compute_spot_strategy"])
+            check_type(argname="argument deploy_mode", value=deploy_mode, expected_type=type_hints["deploy_mode"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument ecs_charge_type", value=ecs_charge_type, expected_type=type_hints["ecs_charge_type"])
+            check_type(argname="argument ecs_order_manager_count", value=ecs_order_manager_count, expected_type=type_hints["ecs_order_manager_count"])
+            check_type(argname="argument ehpc_version", value=ehpc_version, expected_type=type_hints["ehpc_version"])
+            check_type(argname="argument ha_enable", value=ha_enable, expected_type=type_hints["ha_enable"])
+            check_type(argname="argument image_id", value=image_id, expected_type=type_hints["image_id"])
+            check_type(argname="argument image_owner_alias", value=image_owner_alias, expected_type=type_hints["image_owner_alias"])
+            check_type(argname="argument input_file_url", value=input_file_url, expected_type=type_hints["input_file_url"])
+            check_type(argname="argument is_compute_ess", value=is_compute_ess, expected_type=type_hints["is_compute_ess"])
+            check_type(argname="argument job_queue", value=job_queue, expected_type=type_hints["job_queue"])
+            check_type(argname="argument key_pair_name", value=key_pair_name, expected_type=type_hints["key_pair_name"])
+            check_type(argname="argument password", value=password, expected_type=type_hints["password"])
+            check_type(argname="argument period", value=period, expected_type=type_hints["period"])
+            check_type(argname="argument period_unit", value=period_unit, expected_type=type_hints["period_unit"])
+            check_type(argname="argument post_install_script", value=post_install_script, expected_type=type_hints["post_install_script"])
+            check_type(argname="argument remote_directory", value=remote_directory, expected_type=type_hints["remote_directory"])
+            check_type(argname="argument remote_vis_enable", value=remote_vis_enable, expected_type=type_hints["remote_vis_enable"])
+            check_type(argname="argument resource_group_id", value=resource_group_id, expected_type=type_hints["resource_group_id"])
+            check_type(argname="argument scc_cluster_id", value=scc_cluster_id, expected_type=type_hints["scc_cluster_id"])
+            check_type(argname="argument scheduler_type", value=scheduler_type, expected_type=type_hints["scheduler_type"])
+            check_type(argname="argument security_group_id", value=security_group_id, expected_type=type_hints["security_group_id"])
+            check_type(argname="argument security_group_name", value=security_group_name, expected_type=type_hints["security_group_name"])
+            check_type(argname="argument system_disk_level", value=system_disk_level, expected_type=type_hints["system_disk_level"])
+            check_type(argname="argument system_disk_size", value=system_disk_size, expected_type=type_hints["system_disk_size"])
+            check_type(argname="argument system_disk_type", value=system_disk_type, expected_type=type_hints["system_disk_type"])
+            check_type(argname="argument volume_id", value=volume_id, expected_type=type_hints["volume_id"])
+            check_type(argname="argument volume_mountpoint", value=volume_mountpoint, expected_type=type_hints["volume_mountpoint"])
+            check_type(argname="argument volume_protocol", value=volume_protocol, expected_type=type_hints["volume_protocol"])
+            check_type(argname="argument volume_type", value=volume_type, expected_type=type_hints["volume_type"])
+            check_type(argname="argument without_elastic_ip", value=without_elastic_ip, expected_type=type_hints["without_elastic_ip"])
+            check_type(argname="argument zone_id", value=zone_id, expected_type=type_hints["zone_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "ecs_order_compute_count": ecs_order_compute_count,
             "ecs_order_compute_instance_type": ecs_order_compute_instance_type,
             "ecs_order_login_count": ecs_order_login_count,
             "ecs_order_login_instance_type": ecs_order_login_instance_type,
             "ecs_order_manager_instance_type": ecs_order_manager_instance_type,
             "name": name,
@@ -870,219 +929,255 @@
 ):
     '''A ROS template type:  ``ALIYUN::EHPC::Cluster``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosClusterProps",
+        props: typing.Union["RosClusterProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::EHPC::Cluster``.
 
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
         :Attribute: ClusterId: Cluster Id.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrClusterId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrEcsInfo")
     def attr_ecs_info(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute:
 
         EcsInfo: A data structure describing the number and specifications of ECS for various components of the cluster.
         You will get results similar to the following: EcsInfo: {"Manager": {"Count": 2, "InstanceType": "ecs.n1.large"}, "Compute": {"Count": 8, "InstanceType": "ecs.n1.large"}, "Login": {"Count": 1, "InstanceType": "ecs.n1.large"}}
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrEcsInfo"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrName")
     def attr_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Name: Cluster name.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrSecurityGroupId")
     def attr_security_group_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: SecurityGroupId: Security group ID.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrSecurityGroupId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="ecsOrderComputeCount")
     def ecs_order_compute_count(
         self,
     ) -> typing.Union[jsii.Number, ros_cdk_core.IResolvable]:
         '''
         :Property: ecsOrderComputeCount: Computing node number, which ranges from: 1-99.
         '''
         return typing.cast(typing.Union[jsii.Number, ros_cdk_core.IResolvable], jsii.get(self, "ecsOrderComputeCount"))
 
     @ecs_order_compute_count.setter
     def ecs_order_compute_count(
         self,
         value: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "ecs_order_compute_count").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "ecsOrderComputeCount", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="ecsOrderComputeInstanceType")
     def ecs_order_compute_instance_type(
         self,
     ) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: ecsOrderComputeInstanceType: Cluster computing node instance specifications.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "ecsOrderComputeInstanceType"))
 
     @ecs_order_compute_instance_type.setter
     def ecs_order_compute_instance_type(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "ecs_order_compute_instance_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "ecsOrderComputeInstanceType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="ecsOrderLoginCount")
     def ecs_order_login_count(
         self,
     ) -> typing.Union[jsii.Number, ros_cdk_core.IResolvable]:
         '''
         :Property: ecsOrderLoginCount: Login node number can only be 1.
         '''
         return typing.cast(typing.Union[jsii.Number, ros_cdk_core.IResolvable], jsii.get(self, "ecsOrderLoginCount"))
 
     @ecs_order_login_count.setter
     def ecs_order_login_count(
         self,
         value: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "ecs_order_login_count").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "ecsOrderLoginCount", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="ecsOrderLoginInstanceType")
     def ecs_order_login_instance_type(
         self,
     ) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: ecsOrderLoginInstanceType: Log cluster node instance specifications.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "ecsOrderLoginInstanceType"))
 
     @ecs_order_login_instance_type.setter
     def ecs_order_login_instance_type(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "ecs_order_login_instance_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "ecsOrderLoginInstanceType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="ecsOrderManagerInstanceType")
     def ecs_order_manager_instance_type(
         self,
     ) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: ecsOrderManagerInstanceType: Cluster control node instance specifications.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "ecsOrderManagerInstanceType"))
 
     @ecs_order_manager_instance_type.setter
     def ecs_order_manager_instance_type(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "ecs_order_manager_instance_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "ecsOrderManagerInstanceType", value)
 
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
     @jsii.member(jsii_name="name")
     def name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: name: Cluster name. 2-64 characters in length, allowing only include Chinese, letters, numbers, dashes (-) and underscore (_), must begin with a letter or Chinese.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "name"))
 
     @name.setter
     def name(self, value: typing.Union[builtins.str, ros_cdk_core.IResolvable]) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "name", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="osTag")
     def os_tag(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: osTag: Operating system image tag. You can call ListImages API to query.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "osTag"))
 
     @os_tag.setter
     def os_tag(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "os_tag").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "osTag", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vSwitchId")
     def v_switch_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: vSwitchId: VPC in switch ID. Products currently only supports VPC network.
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
     @jsii.member(jsii_name="accountType")
     def account_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -1094,85 +1189,100 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "accountType"))
 
     @account_type.setter
     def account_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "account_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "accountType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="additionalVolumes")
     def additional_volumes(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosCluster.AdditionalVolumesProperty"]]]]:
         '''
         :Property: additionalVolumes:
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosCluster.AdditionalVolumesProperty"]]]], jsii.get(self, "additionalVolumes"))
 
     @additional_volumes.setter
     def additional_volumes(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosCluster.AdditionalVolumesProperty"]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "additional_volumes").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "additionalVolumes", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="application")
     def application(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosCluster.ApplicationProperty"]]]]:
         '''
         :Property: application: Application software tag (SoftwareTag) list, You can call ListSoftwares API to query.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosCluster.ApplicationProperty"]]]], jsii.get(self, "application"))
 
     @application.setter
     def application(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosCluster.ApplicationProperty"]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "application").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "application", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="autoRenew")
     def auto_renew(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property: autoRenew: true: automatic renewals; false: no automatic renewals.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "autoRenew"))
 
     @auto_renew.setter
     def auto_renew(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "auto_renew").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "autoRenew", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="autoRenewPeriod")
     def auto_renew_period(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: autoRenewPeriod: Duration of each automatic renewals, AutoRenew take effect when AutoRenew is True.
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "autoRenewPeriod"))
 
     @auto_renew_period.setter
     def auto_renew_period(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "auto_renew_period").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "autoRenewPeriod", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="clientVersion")
     def client_version(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -1182,17 +1292,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "clientVersion"))
 
     @client_version.setter
     def client_version(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "client_version").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "clientVersion", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="computeEnableHt")
     def compute_enable_ht(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -1204,51 +1317,60 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "computeEnableHt"))
 
     @compute_enable_ht.setter
     def compute_enable_ht(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "compute_enable_ht").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "computeEnableHt", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="computeSpotPriceLimit")
     def compute_spot_price_limit(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: computeSpotPriceLimit: Set an example of the highest price per hour, are floating-point values, in the range of the current price range.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "computeSpotPriceLimit"))
 
     @compute_spot_price_limit.setter
     def compute_spot_price_limit(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "compute_spot_price_limit").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "computeSpotPriceLimit", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="computeSpotStrategy")
     def compute_spot_strategy(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: computeSpotStrategy: Compute nodes bidding strategy, value NoSpot, SpotWithPriceLimit or SpotAsPriceGo
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "computeSpotStrategy"))
 
     @compute_spot_strategy.setter
     def compute_spot_strategy(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "compute_spot_strategy").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "computeSpotStrategy", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="deployMode")
     def deploy_mode(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -1261,85 +1383,100 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "deployMode"))
 
     @deploy_mode.setter
     def deploy_mode(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "deploy_mode").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "deployMode", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="description")
     def description(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: description: Cluster description, 2 to 128 characters.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "description"))
 
     @description.setter
     def description(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "description").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "description", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="ecsChargeType")
     def ecs_charge_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: ecsChargeType: ECS instance payment type, PostPaid: Pay-As-You-Go.PrePaid: Subscription.If you choose PrePaid, automatic renewal will be enabled by default, and closed when node is released.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "ecsChargeType"))
 
     @ecs_charge_type.setter
     def ecs_charge_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "ecs_charge_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "ecsChargeType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="ecsOrderManagerCount")
     def ecs_order_manager_count(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: ecsOrderManagerCount: Control node number can be 1, 2
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "ecsOrderManagerCount"))
 
     @ecs_order_manager_count.setter
     def ecs_order_manager_count(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "ecs_order_manager_count").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "ecsOrderManagerCount", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="ehpcVersion")
     def ehpc_version(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: ehpcVersion: The version of E-HPC. By default, the parameter is set to the latest version number.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "ehpcVersion"))
 
     @ehpc_version.setter
     def ehpc_version(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "ehpc_version").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "ehpcVersion", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="haEnable")
     def ha_enable(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -1352,68 +1489,80 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "haEnable"))
 
     @ha_enable.setter
     def ha_enable(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "ha_enable").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "haEnable", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="imageId")
     def image_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: imageId: Mirror Id, if ImageType a system, based on the image ID is determined only according OsTag; if self, others, or marketplace, ImageId is mandatory.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "imageId"))
 
     @image_id.setter
     def image_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "image_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "imageId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="imageOwnerAlias")
     def image_owner_alias(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: imageOwnerAlias: Mirror type: system, self, others or marketplace
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "imageOwnerAlias"))
 
     @image_owner_alias.setter
     def image_owner_alias(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "image_owner_alias").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "imageOwnerAlias", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="inputFileUrl")
     def input_file_url(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: inputFileUrl: The URL of the job files that are uploaded to an Object Storage Service (OSS) bucket.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "inputFileUrl"))
 
     @input_file_url.setter
     def input_file_url(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "input_file_url").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "inputFileUrl", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="isComputeEss")
     def is_compute_ess(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -1425,136 +1574,160 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "isComputeEss"))
 
     @is_compute_ess.setter
     def is_compute_ess(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "is_compute_ess").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "isComputeEss", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="jobQueue")
     def job_queue(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: jobQueue: 	The queue to which the compute nodes are added.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "jobQueue"))
 
     @job_queue.setter
     def job_queue(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "job_queue").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "jobQueue", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="keyPairName")
     def key_pair_name(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: keyPairName: Key pair name.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "keyPairName"))
 
     @key_pair_name.setter
     def key_pair_name(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "key_pair_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "keyPairName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="password")
     def password(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: password: Root password of jump server (login node). 8 to 30 characters, must contain three (upper and lower case letters, numbers and special symbols). ! Supports the following special characters :() `~ @ # $% ^ & * - + = | {} []:; '<>, / Be sure to use the HTTPS protocol API call to avoid password leaks that may occur.?.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "password"))
 
     @password.setter
     def password(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "password").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "password", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="period")
     def period(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: period: The purchase of long resources, units: week / month / year. When the value of the parameter EcsChargeType when PrePaid take effect and for the selected value will be.
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "period"))
 
     @period.setter
     def period(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "period").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "period", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="periodUnit")
     def period_unit(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: periodUnit: The purchase of long-resources unit. Alternatively value Week / Month / year.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "periodUnit"))
 
     @period_unit.setter
     def period_unit(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "period_unit").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "periodUnit", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="postInstallScript")
     def post_install_script(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosCluster.PostInstallScriptProperty"]]]]:
         '''
         :Property: postInstallScript:
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosCluster.PostInstallScriptProperty"]]]], jsii.get(self, "postInstallScript"))
 
     @post_install_script.setter
     def post_install_script(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosCluster.PostInstallScriptProperty"]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "post_install_script").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "postInstallScript", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="remoteDirectory")
     def remote_directory(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: remoteDirectory: Mount shared storage remote directory. The final path to the mount point and mount the remote directory composition: NasMountpoint: / RemoteDirectory
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "remoteDirectory"))
 
     @remote_directory.setter
     def remote_directory(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "remote_directory").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "remoteDirectory", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="remoteVisEnable")
     def remote_vis_enable(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -1566,17 +1739,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "remoteVisEnable"))
 
     @remote_vis_enable.setter
     def remote_vis_enable(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "remote_vis_enable").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "remoteVisEnable", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="resourceGroupId")
     def resource_group_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -1586,34 +1762,40 @@
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
     @jsii.member(jsii_name="sccClusterId")
     def scc_cluster_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: sccClusterId: When SCC models, if you pass this field, then the specified SccCluster create Scc instance, otherwise it will create an instance for the user.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "sccClusterId"))
 
     @scc_cluster_id.setter
     def scc_cluster_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "scc_cluster_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "sccClusterId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="schedulerType")
     def scheduler_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -1627,51 +1809,60 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "schedulerType"))
 
     @scheduler_type.setter
     def scheduler_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "scheduler_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "schedulerType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="securityGroupId")
     def security_group_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: securityGroupId: Security group ID.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "securityGroupId"))
 
     @security_group_id.setter
     def security_group_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "security_group_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "securityGroupId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="securityGroupName")
     def security_group_name(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: securityGroupName: If you do not use an existing security group (SecurityGroupId is empty), then use this name to create a new security group, the default policy. Format Requirements Reference ECS security group name.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "securityGroupName"))
 
     @security_group_name.setter
     def security_group_name(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "security_group_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "securityGroupName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="systemDiskLevel")
     def system_disk_level(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -1685,17 +1876,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "systemDiskLevel"))
 
     @system_disk_level.setter
     def system_disk_level(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "system_disk_level").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "systemDiskLevel", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="systemDiskSize")
     def system_disk_size(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -1706,17 +1900,20 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "systemDiskSize"))
 
     @system_disk_size.setter
     def system_disk_size(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "system_disk_size").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "systemDiskSize", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="systemDiskType")
     def system_disk_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -1729,34 +1926,40 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "systemDiskType"))
 
     @system_disk_type.setter
     def system_disk_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "system_disk_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "systemDiskType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="volumeId")
     def volume_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: volumeId: The ID of the file system. If you leave the parameter empty, a Performance NAS file system is created by default.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "volumeId"))
 
     @volume_id.setter
     def volume_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "volume_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "volumeId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="volumeMountpoint")
     def volume_mountpoint(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -1767,17 +1970,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "volumeMountpoint"))
 
     @volume_mountpoint.setter
     def volume_mountpoint(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "volume_mountpoint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "volumeMountpoint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="volumeProtocol")
     def volume_protocol(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -1789,65 +1995,77 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "volumeProtocol"))
 
     @volume_protocol.setter
     def volume_protocol(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "volume_protocol").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "volumeProtocol", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="volumeType")
     def volume_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: volumeType: The type of the shared storage. Only Apsara File Storage nas file systems are supported.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "volumeType"))
 
     @volume_type.setter
     def volume_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "volume_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "volumeType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="withoutElasticIp")
     def without_elastic_ip(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property: withoutElasticIp: Specifies whether the logon node uses an elastic IP address (EIP). Default value: false
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "withoutElasticIp"))
 
     @without_elastic_ip.setter
     def without_elastic_ip(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "without_elastic_ip").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "withoutElasticIp", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="zoneId")
     def zone_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: zoneId: Available area ID.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "zoneId"))
 
     @zone_id.setter
     def zone_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "zone_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "zoneId", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-ehpc.RosCluster.AdditionalVolumesProperty",
         jsii_struct_bases=[],
         name_mapping={
             "local_directory": "localDirectory",
@@ -1879,14 +2097,24 @@
             :param volume_mountpoint: 
             :param job_queue: 
             :param location: 
             :param remote_directory: 
             :param volume_protocol: 
             :param volume_type: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosCluster.AdditionalVolumesProperty.__init__)
+                check_type(argname="argument local_directory", value=local_directory, expected_type=type_hints["local_directory"])
+                check_type(argname="argument volume_id", value=volume_id, expected_type=type_hints["volume_id"])
+                check_type(argname="argument volume_mountpoint", value=volume_mountpoint, expected_type=type_hints["volume_mountpoint"])
+                check_type(argname="argument job_queue", value=job_queue, expected_type=type_hints["job_queue"])
+                check_type(argname="argument location", value=location, expected_type=type_hints["location"])
+                check_type(argname="argument remote_directory", value=remote_directory, expected_type=type_hints["remote_directory"])
+                check_type(argname="argument volume_protocol", value=volume_protocol, expected_type=type_hints["volume_protocol"])
+                check_type(argname="argument volume_type", value=volume_type, expected_type=type_hints["volume_type"])
             self._values: typing.Dict[str, typing.Any] = {
                 "local_directory": local_directory,
                 "volume_id": volume_id,
                 "volume_mountpoint": volume_mountpoint,
             }
             if job_queue is not None:
                 self._values["job_queue"] = job_queue
@@ -2006,14 +2234,17 @@
             self,
             *,
             tag: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         ) -> None:
             '''
             :param tag: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosCluster.ApplicationProperty.__init__)
+                check_type(argname="argument tag", value=tag, expected_type=type_hints["tag"])
             self._values: typing.Dict[str, typing.Any] = {
                 "tag": tag,
             }
 
         @builtins.property
         def tag(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
             '''
@@ -2046,14 +2277,18 @@
             args: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
             url: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param args: 
             :param url: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosCluster.PostInstallScriptProperty.__init__)
+                check_type(argname="argument args", value=args, expected_type=type_hints["args"])
+                check_type(argname="argument url", value=url, expected_type=type_hints["url"])
             self._values: typing.Dict[str, typing.Any] = {}
             if args is not None:
                 self._values["args"] = args
             if url is not None:
                 self._values["url"] = url
 
         @builtins.property
@@ -2152,16 +2387,16 @@
         ecs_order_login_count: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
         ecs_order_login_instance_type: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         ecs_order_manager_instance_type: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         os_tag: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         v_switch_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         account_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        additional_volumes: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosCluster.AdditionalVolumesProperty]]]] = None,
-        application: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosCluster.ApplicationProperty]]]] = None,
+        additional_volumes: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosCluster.AdditionalVolumesProperty, typing.Dict[str, typing.Any]]]]]] = None,
+        application: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosCluster.ApplicationProperty, typing.Dict[str, typing.Any]]]]]] = None,
         auto_renew: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         auto_renew_period: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         client_version: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         compute_enable_ht: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         compute_spot_price_limit: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         compute_spot_strategy: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         deploy_mode: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
@@ -2175,15 +2410,15 @@
         input_file_url: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         is_compute_ess: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         job_queue: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         key_pair_name: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         password: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         period: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         period_unit: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        post_install_script: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosCluster.PostInstallScriptProperty]]]] = None,
+        post_install_script: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosCluster.PostInstallScriptProperty, typing.Dict[str, typing.Any]]]]]] = None,
         remote_directory: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         remote_vis_enable: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         resource_group_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         scc_cluster_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         scheduler_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         security_group_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         security_group_name: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
@@ -2245,14 +2480,65 @@
         :param volume_id: 
         :param volume_mountpoint: 
         :param volume_protocol: 
         :param volume_type: 
         :param without_elastic_ip: 
         :param zone_id: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosClusterProps.__init__)
+            check_type(argname="argument ecs_order_compute_count", value=ecs_order_compute_count, expected_type=type_hints["ecs_order_compute_count"])
+            check_type(argname="argument ecs_order_compute_instance_type", value=ecs_order_compute_instance_type, expected_type=type_hints["ecs_order_compute_instance_type"])
+            check_type(argname="argument ecs_order_login_count", value=ecs_order_login_count, expected_type=type_hints["ecs_order_login_count"])
+            check_type(argname="argument ecs_order_login_instance_type", value=ecs_order_login_instance_type, expected_type=type_hints["ecs_order_login_instance_type"])
+            check_type(argname="argument ecs_order_manager_instance_type", value=ecs_order_manager_instance_type, expected_type=type_hints["ecs_order_manager_instance_type"])
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+            check_type(argname="argument os_tag", value=os_tag, expected_type=type_hints["os_tag"])
+            check_type(argname="argument v_switch_id", value=v_switch_id, expected_type=type_hints["v_switch_id"])
+            check_type(argname="argument account_type", value=account_type, expected_type=type_hints["account_type"])
+            check_type(argname="argument additional_volumes", value=additional_volumes, expected_type=type_hints["additional_volumes"])
+            check_type(argname="argument application", value=application, expected_type=type_hints["application"])
+            check_type(argname="argument auto_renew", value=auto_renew, expected_type=type_hints["auto_renew"])
+            check_type(argname="argument auto_renew_period", value=auto_renew_period, expected_type=type_hints["auto_renew_period"])
+            check_type(argname="argument client_version", value=client_version, expected_type=type_hints["client_version"])
+            check_type(argname="argument compute_enable_ht", value=compute_enable_ht, expected_type=type_hints["compute_enable_ht"])
+            check_type(argname="argument compute_spot_price_limit", value=compute_spot_price_limit, expected_type=type_hints["compute_spot_price_limit"])
+            check_type(argname="argument compute_spot_strategy", value=compute_spot_strategy, expected_type=type_hints["compute_spot_strategy"])
+            check_type(argname="argument deploy_mode", value=deploy_mode, expected_type=type_hints["deploy_mode"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument ecs_charge_type", value=ecs_charge_type, expected_type=type_hints["ecs_charge_type"])
+            check_type(argname="argument ecs_order_manager_count", value=ecs_order_manager_count, expected_type=type_hints["ecs_order_manager_count"])
+            check_type(argname="argument ehpc_version", value=ehpc_version, expected_type=type_hints["ehpc_version"])
+            check_type(argname="argument ha_enable", value=ha_enable, expected_type=type_hints["ha_enable"])
+            check_type(argname="argument image_id", value=image_id, expected_type=type_hints["image_id"])
+            check_type(argname="argument image_owner_alias", value=image_owner_alias, expected_type=type_hints["image_owner_alias"])
+            check_type(argname="argument input_file_url", value=input_file_url, expected_type=type_hints["input_file_url"])
+            check_type(argname="argument is_compute_ess", value=is_compute_ess, expected_type=type_hints["is_compute_ess"])
+            check_type(argname="argument job_queue", value=job_queue, expected_type=type_hints["job_queue"])
+            check_type(argname="argument key_pair_name", value=key_pair_name, expected_type=type_hints["key_pair_name"])
+            check_type(argname="argument password", value=password, expected_type=type_hints["password"])
+            check_type(argname="argument period", value=period, expected_type=type_hints["period"])
+            check_type(argname="argument period_unit", value=period_unit, expected_type=type_hints["period_unit"])
+            check_type(argname="argument post_install_script", value=post_install_script, expected_type=type_hints["post_install_script"])
+            check_type(argname="argument remote_directory", value=remote_directory, expected_type=type_hints["remote_directory"])
+            check_type(argname="argument remote_vis_enable", value=remote_vis_enable, expected_type=type_hints["remote_vis_enable"])
+            check_type(argname="argument resource_group_id", value=resource_group_id, expected_type=type_hints["resource_group_id"])
+            check_type(argname="argument scc_cluster_id", value=scc_cluster_id, expected_type=type_hints["scc_cluster_id"])
+            check_type(argname="argument scheduler_type", value=scheduler_type, expected_type=type_hints["scheduler_type"])
+            check_type(argname="argument security_group_id", value=security_group_id, expected_type=type_hints["security_group_id"])
+            check_type(argname="argument security_group_name", value=security_group_name, expected_type=type_hints["security_group_name"])
+            check_type(argname="argument system_disk_level", value=system_disk_level, expected_type=type_hints["system_disk_level"])
+            check_type(argname="argument system_disk_size", value=system_disk_size, expected_type=type_hints["system_disk_size"])
+            check_type(argname="argument system_disk_type", value=system_disk_type, expected_type=type_hints["system_disk_type"])
+            check_type(argname="argument volume_id", value=volume_id, expected_type=type_hints["volume_id"])
+            check_type(argname="argument volume_mountpoint", value=volume_mountpoint, expected_type=type_hints["volume_mountpoint"])
+            check_type(argname="argument volume_protocol", value=volume_protocol, expected_type=type_hints["volume_protocol"])
+            check_type(argname="argument volume_type", value=volume_type, expected_type=type_hints["volume_type"])
+            check_type(argname="argument without_elastic_ip", value=without_elastic_ip, expected_type=type_hints["without_elastic_ip"])
+            check_type(argname="argument zone_id", value=zone_id, expected_type=type_hints["zone_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "ecs_order_compute_count": ecs_order_compute_count,
             "ecs_order_compute_instance_type": ecs_order_compute_instance_type,
             "ecs_order_login_count": ecs_order_login_count,
             "ecs_order_login_instance_type": ecs_order_login_instance_type,
             "ecs_order_manager_instance_type": ecs_order_manager_instance_type,
             "name": name,
```

### Comparing `ros-cdk-ehpc-1.0.8/src/ros_cdk_ehpc.egg-info/PKG-INFO` & `ros-cdk-ehpc-1.0.9/src/ros_cdk_ehpc.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-ehpc
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS EHPC Construct Library
```

