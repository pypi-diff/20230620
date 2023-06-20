# Comparing `tmp/ros-cdk-emr-1.0.8.tar.gz` & `tmp/ros-cdk-emr-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-emr-1.0.8.tar", last modified: Thu Jul 14 02:30:12 2022, max compression
+gzip compressed data, was "dist/ros-cdk-emr-1.0.9.tar", last modified: Fri Sep 23 12:14:34 2022, max compression
```

## Comparing `ros-cdk-emr-1.0.8.tar` & `ros-cdk-emr-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:30:12.000000 ros-cdk-emr-1.0.8/
--rw-r--r--   0 root         (0) root         (0)    10279 2022-07-14 02:30:12.000000 ros-cdk-emr-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2022-07-14 02:30:12.000000 ros-cdk-emr-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2022-07-14 02:30:12.000000 ros-cdk-emr-1.0.8/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1240 2022-07-14 02:30:12.000000 ros-cdk-emr-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      179 2022-07-14 02:30:12.000000 ros-cdk-emr-1.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)      106 2022-07-14 02:30:12.000000 ros-cdk-emr-1.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-07-14 02:30:12.000000 ros-cdk-emr-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1794 2022-07-14 02:30:12.000000 ros-cdk-emr-1.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:30:12.000000 ros-cdk-emr-1.0.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:30:12.000000 ros-cdk-emr-1.0.8/src/ros_cdk_emr/
--rw-r--r--   0 root         (0) root         (0)   143975 2022-07-14 02:30:12.000000 ros-cdk-emr-1.0.8/src/ros_cdk_emr/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:30:12.000000 ros-cdk-emr-1.0.8/src/ros_cdk_emr/_jsii/
--rw-r--r--   0 root         (0) root         (0)      370 2022-07-14 02:30:12.000000 ros-cdk-emr-1.0.8/src/ros_cdk_emr/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    68714 2022-07-14 02:30:12.000000 ros-cdk-emr-1.0.8/src/ros_cdk_emr/_jsii/ros-cdk-emr@1.0.8.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:30:12.000000 ros-cdk-emr-1.0.8/src/ros_cdk_emr/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:30:12.000000 ros-cdk-emr-1.0.8/src/ros_cdk_emr.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1240 2022-07-14 02:30:12.000000 ros-cdk-emr-1.0.8/src/ros_cdk_emr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      400 2022-07-14 02:30:12.000000 ros-cdk-emr-1.0.8/src/ros_cdk_emr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:30:12.000000 ros-cdk-emr-1.0.8/src/ros_cdk_emr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2022-07-14 02:30:12.000000 ros-cdk-emr-1.0.8/src/ros_cdk_emr.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2022-07-14 02:30:12.000000 ros-cdk-emr-1.0.8/src/ros_cdk_emr.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:14:34.000000 ros-cdk-emr-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)    10279 2022-09-23 12:14:33.000000 ros-cdk-emr-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-09-23 12:14:33.000000 ros-cdk-emr-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2022-09-23 12:14:33.000000 ros-cdk-emr-1.0.9/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1240 2022-09-23 12:14:34.000000 ros-cdk-emr-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      179 2022-09-23 12:14:33.000000 ros-cdk-emr-1.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      236 2022-09-23 12:14:33.000000 ros-cdk-emr-1.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-09-23 12:14:34.000000 ros-cdk-emr-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1823 2022-09-23 12:14:33.000000 ros-cdk-emr-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:14:34.000000 ros-cdk-emr-1.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:14:34.000000 ros-cdk-emr-1.0.9/src/ros_cdk_emr/
+-rw-r--r--   0 root         (0) root         (0)   172332 2022-09-23 12:14:33.000000 ros-cdk-emr-1.0.9/src/ros_cdk_emr/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:14:34.000000 ros-cdk-emr-1.0.9/src/ros_cdk_emr/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      404 2022-09-23 12:14:33.000000 ros-cdk-emr-1.0.9/src/ros_cdk_emr/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    68762 2022-09-23 12:14:33.000000 ros-cdk-emr-1.0.9/src/ros_cdk_emr/_jsii/ros-cdk-emr@1.0.9.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 12:14:33.000000 ros-cdk-emr-1.0.9/src/ros_cdk_emr/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:14:34.000000 ros-cdk-emr-1.0.9/src/ros_cdk_emr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1240 2022-09-23 12:14:34.000000 ros-cdk-emr-1.0.9/src/ros_cdk_emr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      400 2022-09-23 12:14:34.000000 ros-cdk-emr-1.0.9/src/ros_cdk_emr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 12:14:34.000000 ros-cdk-emr-1.0.9/src/ros_cdk_emr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2022-09-23 12:14:34.000000 ros-cdk-emr-1.0.9/src/ros_cdk_emr.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2022-09-23 12:14:34.000000 ros-cdk-emr-1.0.9/src/ros_cdk_emr.egg-info/top_level.txt
```

### Comparing `ros-cdk-emr-1.0.8/LICENSE` & `ros-cdk-emr-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-emr-1.0.8/PKG-INFO` & `ros-cdk-emr-1.0.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-emr
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS EMR Construct Library
```

### Comparing `ros-cdk-emr-1.0.8/setup.py` & `ros-cdk-emr-1.0.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-emr",
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
         "ros_cdk_emr",
         "ros_cdk_emr._jsii"
     ],
     "package_data": {
         "ros_cdk_emr._jsii": [
-            "ros-cdk-emr@1.0.8.jsii.tgz"
+            "ros-cdk-emr@1.0.9.jsii.tgz"
         ],
         "ros_cdk_emr": [
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

### Comparing `ros-cdk-emr-1.0.8/src/ros_cdk_emr/__init__.py` & `ros-cdk-emr-1.0.9/src/ros_cdk_emr/__init__.py`

 * *Files 12% similar despite different names*

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
@@ -29,49 +31,55 @@
 ):
     '''A ROS resource type:  ``ALIYUN::EMR::Cluster``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "ClusterProps",
+        props: typing.Union["ClusterProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::EMR::Cluster``.
 
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
         '''Attribute ClusterId: The ID of the cluster.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrClusterId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrHostGroups")
     def attr_host_groups(self) -> ros_cdk_core.IResolvable:
         '''Attribute HostGroups: The host group list of the cluster.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrHostGroups"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrMasterNodeInnerIps")
     def attr_master_node_inner_ips(self) -> ros_cdk_core.IResolvable:
         '''Attribute MasterNodeInnerIps: The inner ip list of the cluster master nodes.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrMasterNodeInnerIps"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrMasterNodePubIps")
     def attr_master_node_pub_ips(self) -> ros_cdk_core.IResolvable:
         '''Attribute MasterNodePubIps: The public ip list of the cluster master nodes.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrMasterNodePubIps"))
 
 
 @jsii.data_type(
@@ -124,24 +132,24 @@
 class ClusterProps:
     def __init__(
         self,
         *,
         charge_type: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         cluster_type: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         emr_ver: typing.Union[builtins.str, ros_cdk_core.IResolvable],
-        host_group: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosCluster.HostGroupProperty"]]],
+        host_group: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosCluster.HostGroupProperty", typing.Dict[str, typing.Any]]]]],
         name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         net_type: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         use_local_meta_db: typing.Union[builtins.bool, ros_cdk_core.IResolvable],
         zone_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         authorize_content: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         auto_renew: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
-        bootstrap_action: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosCluster.BootstrapActionProperty"]]]] = None,
+        bootstrap_action: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosCluster.BootstrapActionProperty", typing.Dict[str, typing.Any]]]]]] = None,
         click_house_conf: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]]] = None,
-        config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosCluster.ConfigProperty"]]]] = None,
+        config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosCluster.ConfigProperty", typing.Dict[str, typing.Any]]]]]] = None,
         configurations: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         deposit_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         eas_enable: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         high_availability_enable: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         init_custom_hive_meta_db: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         instance_generation: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         io_optimized: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
@@ -155,18 +163,18 @@
         option_soft_ware_list: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]] = None,
         period: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         related_cluster_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         resource_group_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         security_group_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         security_group_name: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ssh_enable: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
-        tags: typing.Optional[typing.Sequence["RosCluster.TagsProperty"]] = None,
+        tags: typing.Optional[typing.Sequence[typing.Union["RosCluster.TagsProperty", typing.Dict[str, typing.Any]]]] = None,
         use_custom_hive_meta_db: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         user_defined_emr_ecs_role: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        user_info: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosCluster.UserInfoProperty"]]]] = None,
+        user_info: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosCluster.UserInfoProperty", typing.Dict[str, typing.Any]]]]]] = None,
         vpc_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         v_switch_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         white_list_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::EMR::Cluster``.
 
         :param charge_type: Property chargeType: The billing method. Valid values: PostPaid and PrePaid. PostPaid: pay-as-you-go. PrePaid: subscription.
@@ -207,14 +215,57 @@
         :param use_custom_hive_meta_db: Property useCustomHiveMetaDb: A reserved parameter. Not required.
         :param user_defined_emr_ecs_role: Property userDefinedEmrEcsRole: The role that is assigned to EMR for calling ECS resources.
         :param user_info: Property userInfo:.
         :param vpc_id: Property vpcId: The ID of the VPC. A value is required when NetType=vpc.
         :param v_switch_id: Property vSwitchId: The ID of the Vswitch. A value is required when NetType=vpc.
         :param white_list_type: Property whiteListType: Not required.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(ClusterProps.__init__)
+            check_type(argname="argument charge_type", value=charge_type, expected_type=type_hints["charge_type"])
+            check_type(argname="argument cluster_type", value=cluster_type, expected_type=type_hints["cluster_type"])
+            check_type(argname="argument emr_ver", value=emr_ver, expected_type=type_hints["emr_ver"])
+            check_type(argname="argument host_group", value=host_group, expected_type=type_hints["host_group"])
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+            check_type(argname="argument net_type", value=net_type, expected_type=type_hints["net_type"])
+            check_type(argname="argument use_local_meta_db", value=use_local_meta_db, expected_type=type_hints["use_local_meta_db"])
+            check_type(argname="argument zone_id", value=zone_id, expected_type=type_hints["zone_id"])
+            check_type(argname="argument authorize_content", value=authorize_content, expected_type=type_hints["authorize_content"])
+            check_type(argname="argument auto_renew", value=auto_renew, expected_type=type_hints["auto_renew"])
+            check_type(argname="argument bootstrap_action", value=bootstrap_action, expected_type=type_hints["bootstrap_action"])
+            check_type(argname="argument click_house_conf", value=click_house_conf, expected_type=type_hints["click_house_conf"])
+            check_type(argname="argument config", value=config, expected_type=type_hints["config"])
+            check_type(argname="argument configurations", value=configurations, expected_type=type_hints["configurations"])
+            check_type(argname="argument deposit_type", value=deposit_type, expected_type=type_hints["deposit_type"])
+            check_type(argname="argument eas_enable", value=eas_enable, expected_type=type_hints["eas_enable"])
+            check_type(argname="argument high_availability_enable", value=high_availability_enable, expected_type=type_hints["high_availability_enable"])
+            check_type(argname="argument init_custom_hive_meta_db", value=init_custom_hive_meta_db, expected_type=type_hints["init_custom_hive_meta_db"])
+            check_type(argname="argument instance_generation", value=instance_generation, expected_type=type_hints["instance_generation"])
+            check_type(argname="argument io_optimized", value=io_optimized, expected_type=type_hints["io_optimized"])
+            check_type(argname="argument is_open_public_ip", value=is_open_public_ip, expected_type=type_hints["is_open_public_ip"])
+            check_type(argname="argument key_pair_name", value=key_pair_name, expected_type=type_hints["key_pair_name"])
+            check_type(argname="argument log_path", value=log_path, expected_type=type_hints["log_path"])
+            check_type(argname="argument machine_type", value=machine_type, expected_type=type_hints["machine_type"])
+            check_type(argname="argument master_pwd", value=master_pwd, expected_type=type_hints["master_pwd"])
+            check_type(argname="argument meta_store_conf", value=meta_store_conf, expected_type=type_hints["meta_store_conf"])
+            check_type(argname="argument meta_store_type", value=meta_store_type, expected_type=type_hints["meta_store_type"])
+            check_type(argname="argument option_soft_ware_list", value=option_soft_ware_list, expected_type=type_hints["option_soft_ware_list"])
+            check_type(argname="argument period", value=period, expected_type=type_hints["period"])
+            check_type(argname="argument related_cluster_id", value=related_cluster_id, expected_type=type_hints["related_cluster_id"])
+            check_type(argname="argument resource_group_id", value=resource_group_id, expected_type=type_hints["resource_group_id"])
+            check_type(argname="argument security_group_id", value=security_group_id, expected_type=type_hints["security_group_id"])
+            check_type(argname="argument security_group_name", value=security_group_name, expected_type=type_hints["security_group_name"])
+            check_type(argname="argument ssh_enable", value=ssh_enable, expected_type=type_hints["ssh_enable"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
+            check_type(argname="argument use_custom_hive_meta_db", value=use_custom_hive_meta_db, expected_type=type_hints["use_custom_hive_meta_db"])
+            check_type(argname="argument user_defined_emr_ecs_role", value=user_defined_emr_ecs_role, expected_type=type_hints["user_defined_emr_ecs_role"])
+            check_type(argname="argument user_info", value=user_info, expected_type=type_hints["user_info"])
+            check_type(argname="argument vpc_id", value=vpc_id, expected_type=type_hints["vpc_id"])
+            check_type(argname="argument v_switch_id", value=v_switch_id, expected_type=type_hints["v_switch_id"])
+            check_type(argname="argument white_list_type", value=white_list_type, expected_type=type_hints["white_list_type"])
         self._values: typing.Dict[str, typing.Any] = {
             "charge_type": charge_type,
             "cluster_type": cluster_type,
             "emr_ver": emr_ver,
             "host_group": host_group,
             "name": name,
             "net_type": net_type,
@@ -699,31 +750,37 @@
 ):
     '''A ROS resource type:  ``ALIYUN::EMR::ClusterServiceConfigs``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "ClusterServiceConfigsProps",
+        props: typing.Union["ClusterServiceConfigsProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::EMR::ClusterServiceConfigs``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(ClusterServiceConfigs.__init__)
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
 
 
 @jsii.data_type(
@@ -732,21 +789,25 @@
     name_mapping={"cluster_id": "clusterId", "service_configs": "serviceConfigs"},
 )
 class ClusterServiceConfigsProps:
     def __init__(
         self,
         *,
         cluster_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
-        service_configs: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosClusterServiceConfigs.ServiceConfigsProperty"]]],
+        service_configs: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosClusterServiceConfigs.ServiceConfigsProperty", typing.Dict[str, typing.Any]]]]],
     ) -> None:
         '''Properties for defining a ``ALIYUN::EMR::ClusterServiceConfigs``.
 
         :param cluster_id: Property clusterId: The ID of the cluster.
         :param service_configs: Property serviceConfigs: Server configs.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(ClusterServiceConfigsProps.__init__)
+            check_type(argname="argument cluster_id", value=cluster_id, expected_type=type_hints["cluster_id"])
+            check_type(argname="argument service_configs", value=service_configs, expected_type=type_hints["service_configs"])
         self._values: typing.Dict[str, typing.Any] = {
             "cluster_id": cluster_id,
             "service_configs": service_configs,
         }
 
     @builtins.property
     def cluster_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
@@ -783,80 +844,89 @@
 ):
     '''A ROS template type:  ``ALIYUN::EMR::Cluster``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosClusterProps",
+        props: typing.Union["RosClusterProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::EMR::Cluster``.
 
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
         :Attribute: ClusterId: The ID of the cluster.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrClusterId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrHostGroups")
     def attr_host_groups(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: HostGroups: The host group list of the cluster.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrHostGroups"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrMasterNodeInnerIps")
     def attr_master_node_inner_ips(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: MasterNodeInnerIps: The inner ip list of the cluster master nodes.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrMasterNodeInnerIps"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrMasterNodePubIps")
     def attr_master_node_pub_ips(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: MasterNodePubIps: The public ip list of the cluster master nodes.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrMasterNodePubIps"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="chargeType")
     def charge_type(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         chargeType: The billing method. Valid values: PostPaid and PrePaid. PostPaid: pay-as-you-go. PrePaid:
         subscription.
@@ -864,271 +934,322 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "chargeType"))
 
     @charge_type.setter
     def charge_type(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "charge_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "chargeType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="clusterType")
     def cluster_type(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: clusterType: The type of the cluster. Allowd values: HADOOP, KAFKA, DRUID, ZOOKEEPER, DATA_SCIENCE, GATEWAY etc.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "clusterType"))
 
     @cluster_type.setter
     def cluster_type(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "cluster_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "clusterType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="emrVer")
     def emr_ver(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: emrVer: The version of EMR.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "emrVer"))
 
     @emr_ver.setter
     def emr_ver(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "emr_ver").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "emrVer", value)
 
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
     @jsii.member(jsii_name="hostGroup")
     def host_group(
         self,
     ) -> typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosCluster.HostGroupProperty"]]]:
         '''
         :Property: hostGroup:
         '''
         return typing.cast(typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosCluster.HostGroupProperty"]]], jsii.get(self, "hostGroup"))
 
     @host_group.setter
     def host_group(
         self,
         value: typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosCluster.HostGroupProperty"]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "host_group").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "hostGroup", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="name")
     def name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         name: The name of the cluster. The name can be 1 to 64 characters in length and only contain
         Chinese characters, letters, numbers, hyphens (-), and underscores (_).
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
     @jsii.member(jsii_name="netType")
     def net_type(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: netType: The type of the network.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "netType"))
 
     @net_type.setter
     def net_type(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "net_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "netType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="useLocalMetaDb")
     def use_local_meta_db(
         self,
     ) -> typing.Union[builtins.bool, ros_cdk_core.IResolvable]:
         '''
         :Property: useLocalMetaDb: Indicates whether the local Hive metadatabase is used.
         '''
         return typing.cast(typing.Union[builtins.bool, ros_cdk_core.IResolvable], jsii.get(self, "useLocalMetaDb"))
 
     @use_local_meta_db.setter
     def use_local_meta_db(
         self,
         value: typing.Union[builtins.bool, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "use_local_meta_db").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "useLocalMetaDb", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="zoneId")
     def zone_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: zoneId: The zone ID.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "zoneId"))
 
     @zone_id.setter
     def zone_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "zone_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "zoneId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="authorizeContent")
     def authorize_content(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: authorizeContent: Not required.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "authorizeContent"))
 
     @authorize_content.setter
     def authorize_content(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "authorize_content").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "authorizeContent", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="autoRenew")
     def auto_renew(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property: autoRenew: Indicates whether the subscription cluster is auto-renewed.
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
     @jsii.member(jsii_name="bootstrapAction")
     def bootstrap_action(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosCluster.BootstrapActionProperty"]]]]:
         '''
         :Property: bootstrapAction:
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosCluster.BootstrapActionProperty"]]]], jsii.get(self, "bootstrapAction"))
 
     @bootstrap_action.setter
     def bootstrap_action(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosCluster.BootstrapActionProperty"]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "bootstrap_action").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "bootstrapAction", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="clickHouseConf")
     def click_house_conf(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]]]:
         '''
         :Property: clickHouseConf: undefined
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]]], jsii.get(self, "clickHouseConf"))
 
     @click_house_conf.setter
     def click_house_conf(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "click_house_conf").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "clickHouseConf", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="config")
     def config(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosCluster.ConfigProperty"]]]]:
         '''
         :Property: config:
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosCluster.ConfigProperty"]]]], jsii.get(self, "config"))
 
     @config.setter
     def config(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosCluster.ConfigProperty"]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "config").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "config", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="configurations")
     def configurations(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: configurations: Not required.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "configurations"))
 
     @configurations.setter
     def configurations(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "configurations").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "configurations", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="depositType")
     def deposit_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: depositType: The hosting type.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "depositType"))
 
     @deposit_type.setter
     def deposit_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "deposit_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "depositType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="easEnable")
     def eas_enable(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property: easEnable: Indicates whether the cluster is a high-security cluster.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "easEnable"))
 
     @eas_enable.setter
     def eas_enable(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "eas_enable").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "easEnable", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="highAvailabilityEnable")
     def high_availability_enable(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -1138,68 +1259,80 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "highAvailabilityEnable"))
 
     @high_availability_enable.setter
     def high_availability_enable(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "high_availability_enable").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "highAvailabilityEnable", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="initCustomHiveMetaDb")
     def init_custom_hive_meta_db(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property: initCustomHiveMetaDb: A reserved parameter. Not required.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "initCustomHiveMetaDb"))
 
     @init_custom_hive_meta_db.setter
     def init_custom_hive_meta_db(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "init_custom_hive_meta_db").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "initCustomHiveMetaDb", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="instanceGeneration")
     def instance_generation(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: instanceGeneration: The generation of the ECS instances.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "instanceGeneration"))
 
     @instance_generation.setter
     def instance_generation(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "instance_generation").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "instanceGeneration", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="ioOptimized")
     def io_optimized(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property: ioOptimized: Indicates wether I/O optimization is enabled. Default value: true.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "ioOptimized"))
 
     @io_optimized.setter
     def io_optimized(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "io_optimized").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "ioOptimized", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="isOpenPublicIp")
     def is_open_public_ip(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -1209,68 +1342,80 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "isOpenPublicIp"))
 
     @is_open_public_ip.setter
     def is_open_public_ip(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "is_open_public_ip").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "isOpenPublicIp", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="keyPairName")
     def key_pair_name(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: keyPairName: The name of the key pair.
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
     @jsii.member(jsii_name="logPath")
     def log_path(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: logPath: The log path in OSS.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "logPath"))
 
     @log_path.setter
     def log_path(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "log_path").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "logPath", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="machineType")
     def machine_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: machineType: The type of the machine.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "machineType"))
 
     @machine_type.setter
     def machine_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "machine_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "machineType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="masterPwd")
     def master_pwd(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -1282,34 +1427,40 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "masterPwd"))
 
     @master_pwd.setter
     def master_pwd(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "master_pwd").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "masterPwd", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="metaStoreConf")
     def meta_store_conf(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: metaStoreConf: Meta store conf of specific meta store type. If MetaStoreType=user_rds, MetaStoreConf should be like {"dbUrl":"jdbc:mysql://xxxxxx", "dbUserName":"username", "dbPassword":"password"}
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "metaStoreConf"))
 
     @meta_store_conf.setter
     def meta_store_conf(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "meta_store_conf").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "metaStoreConf", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="metaStoreType")
     def meta_store_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -1321,34 +1472,40 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "metaStoreType"))
 
     @meta_store_type.setter
     def meta_store_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "meta_store_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "metaStoreType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="optionSoftWareList")
     def option_soft_ware_list(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]]:
         '''
         :Property: optionSoftWareList: The list of optional services.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]], jsii.get(self, "optionSoftWareList"))
 
     @option_soft_ware_list.setter
     def option_soft_ware_list(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "option_soft_ware_list").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "optionSoftWareList", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="period")
     def period(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -1358,51 +1515,60 @@
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
     @jsii.member(jsii_name="relatedClusterId")
     def related_cluster_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: relatedClusterId: The ID of the primary cluster (when the cluster that you create is a Gateway cluster).
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "relatedClusterId"))
 
     @related_cluster_id.setter
     def related_cluster_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "related_cluster_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "relatedClusterId", value)
 
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
     @jsii.member(jsii_name="securityGroupId")
     def security_group_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -1414,17 +1580,20 @@
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
         :Property:
 
@@ -1438,148 +1607,175 @@
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
     @jsii.member(jsii_name="sshEnable")
     def ssh_enable(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property: sshEnable: Indicates whether SSH is enabled.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "sshEnable"))
 
     @ssh_enable.setter
     def ssh_enable(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "ssh_enable").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "sshEnable", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="tags")
     def tags(self) -> typing.Optional[typing.List["RosCluster.TagsProperty"]]:
         '''
         :Property: tags: Tags to attach to instance. Max support 20 tags to add during create instance. Each tag with two properties Key and Value, and Key is required.
         '''
         return typing.cast(typing.Optional[typing.List["RosCluster.TagsProperty"]], jsii.get(self, "tags"))
 
     @tags.setter
     def tags(
         self,
         value: typing.Optional[typing.List["RosCluster.TagsProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "tags").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "tags", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="useCustomHiveMetaDb")
     def use_custom_hive_meta_db(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property: useCustomHiveMetaDb: A reserved parameter. Not required.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "useCustomHiveMetaDb"))
 
     @use_custom_hive_meta_db.setter
     def use_custom_hive_meta_db(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "use_custom_hive_meta_db").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "useCustomHiveMetaDb", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="userDefinedEmrEcsRole")
     def user_defined_emr_ecs_role(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: userDefinedEmrEcsRole: The role that is assigned to EMR for calling ECS resources.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "userDefinedEmrEcsRole"))
 
     @user_defined_emr_ecs_role.setter
     def user_defined_emr_ecs_role(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "user_defined_emr_ecs_role").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "userDefinedEmrEcsRole", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="userInfo")
     def user_info(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosCluster.UserInfoProperty"]]]]:
         '''
         :Property: userInfo:
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosCluster.UserInfoProperty"]]]], jsii.get(self, "userInfo"))
 
     @user_info.setter
     def user_info(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosCluster.UserInfoProperty"]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "user_info").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "userInfo", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vpcId")
     def vpc_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: vpcId: The ID of the VPC. A value is required when NetType=vpc.
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
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vSwitchId")
     def v_switch_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: vSwitchId: The ID of the Vswitch. A value is required when NetType=vpc.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "vSwitchId"))
 
     @v_switch_id.setter
     def v_switch_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "v_switch_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "vSwitchId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="whiteListType")
     def white_list_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: whiteListType: Not required.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "whiteListType"))
 
     @white_list_type.setter
     def white_list_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "white_list_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "whiteListType", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-emr.RosCluster.BootstrapActionProperty",
         jsii_struct_bases=[],
         name_mapping={"arg": "arg", "name": "name", "path": "path"},
     )
@@ -1592,14 +1788,19 @@
             path: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param arg: 
             :param name: 
             :param path: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosCluster.BootstrapActionProperty.__init__)
+                check_type(argname="argument arg", value=arg, expected_type=type_hints["arg"])
+                check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+                check_type(argname="argument path", value=path, expected_type=type_hints["path"])
             self._values: typing.Dict[str, typing.Any] = {}
             if arg is not None:
                 self._values["arg"] = arg
             if name is not None:
                 self._values["name"] = name
             if path is not None:
                 self._values["path"] = path
@@ -1672,14 +1873,22 @@
             :param config_key: 
             :param config_value: 
             :param encrypt: 
             :param file_name: 
             :param replace: 
             :param service_name: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosCluster.ConfigProperty.__init__)
+                check_type(argname="argument config_key", value=config_key, expected_type=type_hints["config_key"])
+                check_type(argname="argument config_value", value=config_value, expected_type=type_hints["config_value"])
+                check_type(argname="argument encrypt", value=encrypt, expected_type=type_hints["encrypt"])
+                check_type(argname="argument file_name", value=file_name, expected_type=type_hints["file_name"])
+                check_type(argname="argument replace", value=replace, expected_type=type_hints["replace"])
+                check_type(argname="argument service_name", value=service_name, expected_type=type_hints["service_name"])
             self._values: typing.Dict[str, typing.Any] = {}
             if config_key is not None:
                 self._values["config_key"] = config_key
             if config_value is not None:
                 self._values["config_value"] = config_value
             if encrypt is not None:
                 self._values["encrypt"] = encrypt
@@ -1833,14 +2042,36 @@
             :param host_group_id: 
             :param host_group_name: 
             :param host_key_pair_name: 
             :param host_password: 
             :param period: 
             :param v_switch_id: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosCluster.HostGroupProperty.__init__)
+                check_type(argname="argument charge_type", value=charge_type, expected_type=type_hints["charge_type"])
+                check_type(argname="argument disk_capacity", value=disk_capacity, expected_type=type_hints["disk_capacity"])
+                check_type(argname="argument disk_count", value=disk_count, expected_type=type_hints["disk_count"])
+                check_type(argname="argument disk_type", value=disk_type, expected_type=type_hints["disk_type"])
+                check_type(argname="argument host_group_type", value=host_group_type, expected_type=type_hints["host_group_type"])
+                check_type(argname="argument instance_type", value=instance_type, expected_type=type_hints["instance_type"])
+                check_type(argname="argument node_count", value=node_count, expected_type=type_hints["node_count"])
+                check_type(argname="argument sys_disk_capacity", value=sys_disk_capacity, expected_type=type_hints["sys_disk_capacity"])
+                check_type(argname="argument sys_disk_type", value=sys_disk_type, expected_type=type_hints["sys_disk_type"])
+                check_type(argname="argument auto_renew", value=auto_renew, expected_type=type_hints["auto_renew"])
+                check_type(argname="argument cluster_id", value=cluster_id, expected_type=type_hints["cluster_id"])
+                check_type(argname="argument comment", value=comment, expected_type=type_hints["comment"])
+                check_type(argname="argument create_type", value=create_type, expected_type=type_hints["create_type"])
+                check_type(argname="argument gpu_driver", value=gpu_driver, expected_type=type_hints["gpu_driver"])
+                check_type(argname="argument host_group_id", value=host_group_id, expected_type=type_hints["host_group_id"])
+                check_type(argname="argument host_group_name", value=host_group_name, expected_type=type_hints["host_group_name"])
+                check_type(argname="argument host_key_pair_name", value=host_key_pair_name, expected_type=type_hints["host_key_pair_name"])
+                check_type(argname="argument host_password", value=host_password, expected_type=type_hints["host_password"])
+                check_type(argname="argument period", value=period, expected_type=type_hints["period"])
+                check_type(argname="argument v_switch_id", value=v_switch_id, expected_type=type_hints["v_switch_id"])
             self._values: typing.Dict[str, typing.Any] = {
                 "charge_type": charge_type,
                 "disk_capacity": disk_capacity,
                 "disk_count": disk_count,
                 "disk_type": disk_type,
                 "host_group_type": host_group_type,
                 "instance_type": instance_type,
@@ -2095,14 +2326,18 @@
             key: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param key: 
             :param value: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosCluster.TagsProperty.__init__)
+                check_type(argname="argument key", value=key, expected_type=type_hints["key"])
+                check_type(argname="argument value", value=value, expected_type=type_hints["value"])
             self._values: typing.Dict[str, typing.Any] = {
                 "key": key,
             }
             if value is not None:
                 self._values["value"] = value
 
         @builtins.property
@@ -2153,14 +2388,19 @@
             user_name: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param password: 
             :param user_id: 
             :param user_name: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosCluster.UserInfoProperty.__init__)
+                check_type(argname="argument password", value=password, expected_type=type_hints["password"])
+                check_type(argname="argument user_id", value=user_id, expected_type=type_hints["user_id"])
+                check_type(argname="argument user_name", value=user_name, expected_type=type_hints["user_name"])
             self._values: typing.Dict[str, typing.Any] = {}
             if password is not None:
                 self._values["password"] = password
             if user_id is not None:
                 self._values["user_id"] = user_id
             if user_name is not None:
                 self._values["user_name"] = user_name
@@ -2257,24 +2497,24 @@
 class RosClusterProps:
     def __init__(
         self,
         *,
         charge_type: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         cluster_type: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         emr_ver: typing.Union[builtins.str, ros_cdk_core.IResolvable],
-        host_group: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosCluster.HostGroupProperty]]],
+        host_group: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosCluster.HostGroupProperty, typing.Dict[str, typing.Any]]]]],
         name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         net_type: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         use_local_meta_db: typing.Union[builtins.bool, ros_cdk_core.IResolvable],
         zone_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         authorize_content: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         auto_renew: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
-        bootstrap_action: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosCluster.BootstrapActionProperty]]]] = None,
+        bootstrap_action: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosCluster.BootstrapActionProperty, typing.Dict[str, typing.Any]]]]]] = None,
         click_house_conf: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]]] = None,
-        config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosCluster.ConfigProperty]]]] = None,
+        config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosCluster.ConfigProperty, typing.Dict[str, typing.Any]]]]]] = None,
         configurations: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         deposit_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         eas_enable: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         high_availability_enable: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         init_custom_hive_meta_db: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         instance_generation: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         io_optimized: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
@@ -2288,18 +2528,18 @@
         option_soft_ware_list: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]] = None,
         period: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         related_cluster_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         resource_group_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         security_group_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         security_group_name: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ssh_enable: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
-        tags: typing.Optional[typing.Sequence[RosCluster.TagsProperty]] = None,
+        tags: typing.Optional[typing.Sequence[typing.Union[RosCluster.TagsProperty, typing.Dict[str, typing.Any]]]] = None,
         use_custom_hive_meta_db: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         user_defined_emr_ecs_role: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        user_info: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosCluster.UserInfoProperty]]]] = None,
+        user_info: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosCluster.UserInfoProperty, typing.Dict[str, typing.Any]]]]]] = None,
         vpc_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         v_switch_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         white_list_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::EMR::Cluster``.
 
         :param charge_type: 
@@ -2340,14 +2580,57 @@
         :param use_custom_hive_meta_db: 
         :param user_defined_emr_ecs_role: 
         :param user_info: 
         :param vpc_id: 
         :param v_switch_id: 
         :param white_list_type: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosClusterProps.__init__)
+            check_type(argname="argument charge_type", value=charge_type, expected_type=type_hints["charge_type"])
+            check_type(argname="argument cluster_type", value=cluster_type, expected_type=type_hints["cluster_type"])
+            check_type(argname="argument emr_ver", value=emr_ver, expected_type=type_hints["emr_ver"])
+            check_type(argname="argument host_group", value=host_group, expected_type=type_hints["host_group"])
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+            check_type(argname="argument net_type", value=net_type, expected_type=type_hints["net_type"])
+            check_type(argname="argument use_local_meta_db", value=use_local_meta_db, expected_type=type_hints["use_local_meta_db"])
+            check_type(argname="argument zone_id", value=zone_id, expected_type=type_hints["zone_id"])
+            check_type(argname="argument authorize_content", value=authorize_content, expected_type=type_hints["authorize_content"])
+            check_type(argname="argument auto_renew", value=auto_renew, expected_type=type_hints["auto_renew"])
+            check_type(argname="argument bootstrap_action", value=bootstrap_action, expected_type=type_hints["bootstrap_action"])
+            check_type(argname="argument click_house_conf", value=click_house_conf, expected_type=type_hints["click_house_conf"])
+            check_type(argname="argument config", value=config, expected_type=type_hints["config"])
+            check_type(argname="argument configurations", value=configurations, expected_type=type_hints["configurations"])
+            check_type(argname="argument deposit_type", value=deposit_type, expected_type=type_hints["deposit_type"])
+            check_type(argname="argument eas_enable", value=eas_enable, expected_type=type_hints["eas_enable"])
+            check_type(argname="argument high_availability_enable", value=high_availability_enable, expected_type=type_hints["high_availability_enable"])
+            check_type(argname="argument init_custom_hive_meta_db", value=init_custom_hive_meta_db, expected_type=type_hints["init_custom_hive_meta_db"])
+            check_type(argname="argument instance_generation", value=instance_generation, expected_type=type_hints["instance_generation"])
+            check_type(argname="argument io_optimized", value=io_optimized, expected_type=type_hints["io_optimized"])
+            check_type(argname="argument is_open_public_ip", value=is_open_public_ip, expected_type=type_hints["is_open_public_ip"])
+            check_type(argname="argument key_pair_name", value=key_pair_name, expected_type=type_hints["key_pair_name"])
+            check_type(argname="argument log_path", value=log_path, expected_type=type_hints["log_path"])
+            check_type(argname="argument machine_type", value=machine_type, expected_type=type_hints["machine_type"])
+            check_type(argname="argument master_pwd", value=master_pwd, expected_type=type_hints["master_pwd"])
+            check_type(argname="argument meta_store_conf", value=meta_store_conf, expected_type=type_hints["meta_store_conf"])
+            check_type(argname="argument meta_store_type", value=meta_store_type, expected_type=type_hints["meta_store_type"])
+            check_type(argname="argument option_soft_ware_list", value=option_soft_ware_list, expected_type=type_hints["option_soft_ware_list"])
+            check_type(argname="argument period", value=period, expected_type=type_hints["period"])
+            check_type(argname="argument related_cluster_id", value=related_cluster_id, expected_type=type_hints["related_cluster_id"])
+            check_type(argname="argument resource_group_id", value=resource_group_id, expected_type=type_hints["resource_group_id"])
+            check_type(argname="argument security_group_id", value=security_group_id, expected_type=type_hints["security_group_id"])
+            check_type(argname="argument security_group_name", value=security_group_name, expected_type=type_hints["security_group_name"])
+            check_type(argname="argument ssh_enable", value=ssh_enable, expected_type=type_hints["ssh_enable"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
+            check_type(argname="argument use_custom_hive_meta_db", value=use_custom_hive_meta_db, expected_type=type_hints["use_custom_hive_meta_db"])
+            check_type(argname="argument user_defined_emr_ecs_role", value=user_defined_emr_ecs_role, expected_type=type_hints["user_defined_emr_ecs_role"])
+            check_type(argname="argument user_info", value=user_info, expected_type=type_hints["user_info"])
+            check_type(argname="argument vpc_id", value=vpc_id, expected_type=type_hints["vpc_id"])
+            check_type(argname="argument v_switch_id", value=v_switch_id, expected_type=type_hints["v_switch_id"])
+            check_type(argname="argument white_list_type", value=white_list_type, expected_type=type_hints["white_list_type"])
         self._values: typing.Dict[str, typing.Any] = {
             "charge_type": charge_type,
             "cluster_type": cluster_type,
             "emr_ver": emr_ver,
             "host_group": host_group,
             "name": name,
             "net_type": net_type,
@@ -2881,94 +3164,112 @@
 ):
     '''A ROS template type:  ``ALIYUN::EMR::ClusterServiceConfigs``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosClusterServiceConfigsProps",
+        props: typing.Union["RosClusterServiceConfigsProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::EMR::ClusterServiceConfigs``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosClusterServiceConfigs.__init__)
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
+            type_hints = typing.get_type_hints(RosClusterServiceConfigs._render_properties)
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
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosClusterServiceConfigs, "cluster_id").fset)
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
+            type_hints = typing.get_type_hints(getattr(RosClusterServiceConfigs, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="serviceConfigs")
     def service_configs(
         self,
     ) -> typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosClusterServiceConfigs.ServiceConfigsProperty"]]]:
         '''
         :Property: serviceConfigs: Server configs
         '''
         return typing.cast(typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosClusterServiceConfigs.ServiceConfigsProperty"]]], jsii.get(self, "serviceConfigs"))
 
     @service_configs.setter
     def service_configs(
         self,
         value: typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosClusterServiceConfigs.ServiceConfigsProperty"]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosClusterServiceConfigs, "service_configs").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "serviceConfigs", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-emr.RosClusterServiceConfigs.ServiceConfigsProperty",
         jsii_struct_bases=[],
         name_mapping={
             "config_params": "configParams",
@@ -3003,14 +3304,25 @@
             :param config_type: 
             :param custom_config_params: 
             :param gateway_cluster_id_list: 
             :param group_id: 
             :param host_instance_id: 
             :param refresh_host_config: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosClusterServiceConfigs.ServiceConfigsProperty.__init__)
+                check_type(argname="argument config_params", value=config_params, expected_type=type_hints["config_params"])
+                check_type(argname="argument service_name", value=service_name, expected_type=type_hints["service_name"])
+                check_type(argname="argument comment", value=comment, expected_type=type_hints["comment"])
+                check_type(argname="argument config_type", value=config_type, expected_type=type_hints["config_type"])
+                check_type(argname="argument custom_config_params", value=custom_config_params, expected_type=type_hints["custom_config_params"])
+                check_type(argname="argument gateway_cluster_id_list", value=gateway_cluster_id_list, expected_type=type_hints["gateway_cluster_id_list"])
+                check_type(argname="argument group_id", value=group_id, expected_type=type_hints["group_id"])
+                check_type(argname="argument host_instance_id", value=host_instance_id, expected_type=type_hints["host_instance_id"])
+                check_type(argname="argument refresh_host_config", value=refresh_host_config, expected_type=type_hints["refresh_host_config"])
             self._values: typing.Dict[str, typing.Any] = {
                 "config_params": config_params,
                 "service_name": service_name,
             }
             if comment is not None:
                 self._values["comment"] = comment
             if config_type is not None:
@@ -3132,21 +3444,25 @@
     name_mapping={"cluster_id": "clusterId", "service_configs": "serviceConfigs"},
 )
 class RosClusterServiceConfigsProps:
     def __init__(
         self,
         *,
         cluster_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
-        service_configs: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosClusterServiceConfigs.ServiceConfigsProperty]]],
+        service_configs: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosClusterServiceConfigs.ServiceConfigsProperty, typing.Dict[str, typing.Any]]]]],
     ) -> None:
         '''Properties for defining a ``ALIYUN::EMR::ClusterServiceConfigs``.
 
         :param cluster_id: 
         :param service_configs: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosClusterServiceConfigsProps.__init__)
+            check_type(argname="argument cluster_id", value=cluster_id, expected_type=type_hints["cluster_id"])
+            check_type(argname="argument service_configs", value=service_configs, expected_type=type_hints["service_configs"])
         self._values: typing.Dict[str, typing.Any] = {
             "cluster_id": cluster_id,
             "service_configs": service_configs,
         }
 
     @builtins.property
     def cluster_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
```

### Comparing `ros-cdk-emr-1.0.8/src/ros_cdk_emr.egg-info/PKG-INFO` & `ros-cdk-emr-1.0.9/src/ros_cdk_emr.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-emr
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS EMR Construct Library
```

