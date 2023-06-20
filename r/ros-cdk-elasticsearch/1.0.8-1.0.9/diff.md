# Comparing `tmp/ros-cdk-elasticsearch-1.0.8.tar.gz` & `tmp/ros-cdk-elasticsearch-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-elasticsearch-1.0.8.tar", last modified: Thu Jul 14 02:38:18 2022, max compression
+gzip compressed data, was "dist/ros-cdk-elasticsearch-1.0.9.tar", last modified: Fri Sep 23 12:17:05 2022, max compression
```

## Comparing `ros-cdk-elasticsearch-1.0.8.tar` & `ros-cdk-elasticsearch-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:38:18.000000 ros-cdk-elasticsearch-1.0.8/
--rw-r--r--   0 root         (0) root         (0)    10279 2022-07-14 02:38:18.000000 ros-cdk-elasticsearch-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2022-07-14 02:38:18.000000 ros-cdk-elasticsearch-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2022-07-14 02:38:18.000000 ros-cdk-elasticsearch-1.0.8/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1280 2022-07-14 02:38:18.000000 ros-cdk-elasticsearch-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      209 2022-07-14 02:38:18.000000 ros-cdk-elasticsearch-1.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)      106 2022-07-14 02:38:18.000000 ros-cdk-elasticsearch-1.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-07-14 02:38:18.000000 ros-cdk-elasticsearch-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1854 2022-07-14 02:38:18.000000 ros-cdk-elasticsearch-1.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:38:18.000000 ros-cdk-elasticsearch-1.0.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:38:18.000000 ros-cdk-elasticsearch-1.0.8/src/ros_cdk_elasticsearch/
--rw-r--r--   0 root         (0) root         (0)    73677 2022-07-14 02:38:18.000000 ros-cdk-elasticsearch-1.0.8/src/ros_cdk_elasticsearch/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:38:18.000000 ros-cdk-elasticsearch-1.0.8/src/ros_cdk_elasticsearch/_jsii/
--rw-r--r--   0 root         (0) root         (0)      403 2022-07-14 02:38:18.000000 ros-cdk-elasticsearch-1.0.8/src/ros_cdk_elasticsearch/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    51620 2022-07-14 02:38:18.000000 ros-cdk-elasticsearch-1.0.8/src/ros_cdk_elasticsearch/_jsii/ros-cdk-elasticsearch@1.0.8.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:38:18.000000 ros-cdk-elasticsearch-1.0.8/src/ros_cdk_elasticsearch/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:38:18.000000 ros-cdk-elasticsearch-1.0.8/src/ros_cdk_elasticsearch.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1280 2022-07-14 02:38:18.000000 ros-cdk-elasticsearch-1.0.8/src/ros_cdk_elasticsearch.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      500 2022-07-14 02:38:18.000000 ros-cdk-elasticsearch-1.0.8/src/ros_cdk_elasticsearch.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:38:18.000000 ros-cdk-elasticsearch-1.0.8/src/ros_cdk_elasticsearch.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2022-07-14 02:38:18.000000 ros-cdk-elasticsearch-1.0.8/src/ros_cdk_elasticsearch.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2022-07-14 02:38:18.000000 ros-cdk-elasticsearch-1.0.8/src/ros_cdk_elasticsearch.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:17:05.000000 ros-cdk-elasticsearch-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)    10279 2022-09-23 12:17:04.000000 ros-cdk-elasticsearch-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-09-23 12:17:04.000000 ros-cdk-elasticsearch-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2022-09-23 12:17:04.000000 ros-cdk-elasticsearch-1.0.9/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1280 2022-09-23 12:17:05.000000 ros-cdk-elasticsearch-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      209 2022-09-23 12:17:04.000000 ros-cdk-elasticsearch-1.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      236 2022-09-23 12:17:04.000000 ros-cdk-elasticsearch-1.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-09-23 12:17:05.000000 ros-cdk-elasticsearch-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1883 2022-09-23 12:17:04.000000 ros-cdk-elasticsearch-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:17:05.000000 ros-cdk-elasticsearch-1.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:17:05.000000 ros-cdk-elasticsearch-1.0.9/src/ros_cdk_elasticsearch/
+-rw-r--r--   0 root         (0) root         (0)    86634 2022-09-23 12:17:04.000000 ros-cdk-elasticsearch-1.0.9/src/ros_cdk_elasticsearch/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:17:05.000000 ros-cdk-elasticsearch-1.0.9/src/ros_cdk_elasticsearch/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      437 2022-09-23 12:17:04.000000 ros-cdk-elasticsearch-1.0.9/src/ros_cdk_elasticsearch/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    50920 2022-09-23 12:17:04.000000 ros-cdk-elasticsearch-1.0.9/src/ros_cdk_elasticsearch/_jsii/ros-cdk-elasticsearch@1.0.9.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 12:17:04.000000 ros-cdk-elasticsearch-1.0.9/src/ros_cdk_elasticsearch/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:17:05.000000 ros-cdk-elasticsearch-1.0.9/src/ros_cdk_elasticsearch.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1280 2022-09-23 12:17:04.000000 ros-cdk-elasticsearch-1.0.9/src/ros_cdk_elasticsearch.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      500 2022-09-23 12:17:04.000000 ros-cdk-elasticsearch-1.0.9/src/ros_cdk_elasticsearch.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 12:17:04.000000 ros-cdk-elasticsearch-1.0.9/src/ros_cdk_elasticsearch.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2022-09-23 12:17:04.000000 ros-cdk-elasticsearch-1.0.9/src/ros_cdk_elasticsearch.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2022-09-23 12:17:04.000000 ros-cdk-elasticsearch-1.0.9/src/ros_cdk_elasticsearch.egg-info/top_level.txt
```

### Comparing `ros-cdk-elasticsearch-1.0.8/LICENSE` & `ros-cdk-elasticsearch-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-elasticsearch-1.0.8/PKG-INFO` & `ros-cdk-elasticsearch-1.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-elasticsearch
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS ELASTICSEARCH Construct Library
```

### Comparing `ros-cdk-elasticsearch-1.0.8/setup.py` & `ros-cdk-elasticsearch-1.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-elasticsearch",
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
         "ros_cdk_elasticsearch",
         "ros_cdk_elasticsearch._jsii"
     ],
     "package_data": {
         "ros_cdk_elasticsearch._jsii": [
-            "ros-cdk-elasticsearch@1.0.8.jsii.tgz"
+            "ros-cdk-elasticsearch@1.0.9.jsii.tgz"
         ],
         "ros_cdk_elasticsearch": [
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

### Comparing `ros-cdk-elasticsearch-1.0.8/src/ros_cdk_elasticsearch/__init__.py` & `ros-cdk-elasticsearch-1.0.9/src/ros_cdk_elasticsearch/__init__.py`

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
 
 
 class Instance(
     ros_cdk_core.Resource,
@@ -29,88 +31,94 @@
 ):
     '''A ROS resource type:  ``ALIYUN::ElasticSearch::Instance``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "InstanceProps",
+        props: typing.Union["InstanceProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::ElasticSearch::Instance``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(Instance.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDomain")
     def attr_domain(self) -> ros_cdk_core.IResolvable:
         '''Attribute Domain: Instance connection domain (only VPC network access supported).'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDomain"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInstanceChargeType")
     def attr_instance_charge_type(self) -> ros_cdk_core.IResolvable:
         '''Attribute InstanceChargeType: Instance charge type.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInstanceChargeType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInstanceId")
     def attr_instance_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute InstanceId: The ID of the Elasticsearch instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInstanceId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrKibanaDomain")
     def attr_kibana_domain(self) -> ros_cdk_core.IResolvable:
         '''Attribute KibanaDomain: Kibana console domain (Internet access supported).'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrKibanaDomain"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrKibanaPort")
     def attr_kibana_port(self) -> ros_cdk_core.IResolvable:
         '''Attribute KibanaPort: Kibana console port.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrKibanaPort"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPort")
     def attr_port(self) -> ros_cdk_core.IResolvable:
         '''Attribute Port:  Instance connection port.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPort"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPublicDomain")
     def attr_public_domain(self) -> ros_cdk_core.IResolvable:
         '''Attribute PublicDomain: Instance public connection domain.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPublicDomain"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrStatus")
     def attr_status(self) -> ros_cdk_core.IResolvable:
         '''Attribute Status: The Elasticsearch instance status.
 
         Includes active, activating, inactive. Some operations are denied when status is not active.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrStatus"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVersion")
     def attr_version(self) -> ros_cdk_core.IResolvable:
         '''Attribute Version: Elasticsearch version.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVersion"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVSwitchId")
     def attr_v_switch_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute VSwitchId: The ID of VSwitch.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVSwitchId"))
 
 
 @jsii.data_type(
@@ -139,32 +147,32 @@
         "zone_id": "zoneId",
     },
 )
 class InstanceProps:
     def __init__(
         self,
         *,
-        data_node: typing.Union["RosInstance.DataNodeProperty", ros_cdk_core.IResolvable],
+        data_node: typing.Union[typing.Union["RosInstance.DataNodeProperty", typing.Dict[str, typing.Any]], ros_cdk_core.IResolvable],
         password: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         version: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         v_switch_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         description: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         enable_kibana_private: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         enable_kibana_public: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         enable_public: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         instance_charge_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        kibana_node: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosInstance.KibanaNodeProperty"]] = None,
+        kibana_node: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosInstance.KibanaNodeProperty", typing.Dict[str, typing.Any]]]] = None,
         kibana_whitelist: typing.Optional[typing.Union[typing.Sequence[typing.Any], ros_cdk_core.IResolvable]] = None,
-        master_node: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosInstance.MasterNodeProperty"]] = None,
+        master_node: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosInstance.MasterNodeProperty", typing.Dict[str, typing.Any]]]] = None,
         period: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         private_whitelist: typing.Optional[typing.Union[typing.Sequence[typing.Any], ros_cdk_core.IResolvable]] = None,
         public_whitelist: typing.Optional[typing.Union[typing.Sequence[typing.Any], ros_cdk_core.IResolvable]] = None,
         resource_group_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        tags: typing.Optional[typing.Sequence["RosInstance.TagsProperty"]] = None,
-        yml_config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosInstance.YMLConfigProperty"]] = None,
+        tags: typing.Optional[typing.Sequence[typing.Union["RosInstance.TagsProperty", typing.Dict[str, typing.Any]]]] = None,
+        yml_config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosInstance.YMLConfigProperty", typing.Dict[str, typing.Any]]]] = None,
         zone_count: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         zone_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::ElasticSearch::Instance``.
 
         :param data_node: Property dataNode: The Elasticsearch cluster's data node setting.
         :param password: Property password: The password of the instance. The password can be 8 to 32 characters in length and must contain three of the following conditions: uppercase letters, lowercase letters, numbers, and special characters (!@#$%&*()_+-=).
@@ -183,14 +191,36 @@
         :param public_whitelist: Property publicWhitelist: Set the instance's IP whitelist in Internet. The AllocatePublicAddress should be true.
         :param resource_group_id: Property resourceGroupId: The ID of the resource group.
         :param tags: Property tags: Tags to attach to instance. Max support 20 tags to add during create instance. Each tag with two properties Key and Value, and Key is required.
         :param yml_config: Property ymlConfig: In the YML Configuration section of the Cluster Configuration page of your Alibaba Cloud Elasticsearch cluster, you can enable the Auto Indexing, Audit Log Indexing, or Watcher feature.
         :param zone_count: Property zoneCount: undefined.
         :param zone_id: Property zoneId: The zone id of elasticsearch.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(InstanceProps.__init__)
+            check_type(argname="argument data_node", value=data_node, expected_type=type_hints["data_node"])
+            check_type(argname="argument password", value=password, expected_type=type_hints["password"])
+            check_type(argname="argument version", value=version, expected_type=type_hints["version"])
+            check_type(argname="argument v_switch_id", value=v_switch_id, expected_type=type_hints["v_switch_id"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument enable_kibana_private", value=enable_kibana_private, expected_type=type_hints["enable_kibana_private"])
+            check_type(argname="argument enable_kibana_public", value=enable_kibana_public, expected_type=type_hints["enable_kibana_public"])
+            check_type(argname="argument enable_public", value=enable_public, expected_type=type_hints["enable_public"])
+            check_type(argname="argument instance_charge_type", value=instance_charge_type, expected_type=type_hints["instance_charge_type"])
+            check_type(argname="argument kibana_node", value=kibana_node, expected_type=type_hints["kibana_node"])
+            check_type(argname="argument kibana_whitelist", value=kibana_whitelist, expected_type=type_hints["kibana_whitelist"])
+            check_type(argname="argument master_node", value=master_node, expected_type=type_hints["master_node"])
+            check_type(argname="argument period", value=period, expected_type=type_hints["period"])
+            check_type(argname="argument private_whitelist", value=private_whitelist, expected_type=type_hints["private_whitelist"])
+            check_type(argname="argument public_whitelist", value=public_whitelist, expected_type=type_hints["public_whitelist"])
+            check_type(argname="argument resource_group_id", value=resource_group_id, expected_type=type_hints["resource_group_id"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
+            check_type(argname="argument yml_config", value=yml_config, expected_type=type_hints["yml_config"])
+            check_type(argname="argument zone_count", value=zone_count, expected_type=type_hints["zone_count"])
+            check_type(argname="argument zone_id", value=zone_id, expected_type=type_hints["zone_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "data_node": data_node,
             "password": password,
             "version": version,
             "v_switch_id": v_switch_id,
         }
         if description is not None:
@@ -425,419 +455,482 @@
 ):
     '''A ROS template type:  ``ALIYUN::ElasticSearch::Instance``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosInstanceProps",
+        props: typing.Union["RosInstanceProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::ElasticSearch::Instance``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosInstance.__init__)
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
+            type_hints = typing.get_type_hints(RosInstance._render_properties)
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
     @jsii.member(jsii_name="attrDomain")
     def attr_domain(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Domain: Instance connection domain (only VPC network access supported).
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDomain"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInstanceChargeType")
     def attr_instance_charge_type(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: InstanceChargeType: Instance charge type.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInstanceChargeType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInstanceId")
     def attr_instance_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: InstanceId: The ID of the Elasticsearch instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInstanceId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrKibanaDomain")
     def attr_kibana_domain(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: KibanaDomain: Kibana console domain (Internet access supported).
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrKibanaDomain"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrKibanaPort")
     def attr_kibana_port(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: KibanaPort: Kibana console port.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrKibanaPort"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPort")
     def attr_port(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Port:  Instance connection port.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPort"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPublicDomain")
     def attr_public_domain(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: PublicDomain: Instance public connection domain.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPublicDomain"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrStatus")
     def attr_status(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Status: The Elasticsearch instance status. Includes active, activating, inactive. Some operations are denied when status is not active.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrStatus"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVersion")
     def attr_version(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Version: Elasticsearch version.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVersion"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVSwitchId")
     def attr_v_switch_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: VSwitchId: The ID of VSwitch.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVSwitchId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dataNode")
     def data_node(
         self,
     ) -> typing.Union["RosInstance.DataNodeProperty", ros_cdk_core.IResolvable]:
         '''
         :Property: dataNode: The Elasticsearch cluster's data node setting.
         '''
         return typing.cast(typing.Union["RosInstance.DataNodeProperty", ros_cdk_core.IResolvable], jsii.get(self, "dataNode"))
 
     @data_node.setter
     def data_node(
         self,
         value: typing.Union["RosInstance.DataNodeProperty", ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "data_node").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dataNode", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="password")
     def password(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :: #$%&*()_+-=).
         :Property: password: The password of the instance. The password can be 8 to 32 characters in length and must contain three of the following conditions: uppercase letters, lowercase letters, numbers, and special characters (!
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "password"))
 
     @password.setter
     def password(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "password").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "password", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="version")
     def version(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: version: Elasticsearch version. Supported values: 5.5.3_with_X-Pack, 6.3_with_X-Pack, 6.7_with_X-Pack, 7.4_with_X-Pack, 6.8, 7.4, 7.7 and so on.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "version"))
 
     @version.setter
     def version(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "version").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "version", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vSwitchId")
     def v_switch_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: vSwitchId: The ID of VSwitch.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "vSwitchId"))
 
     @v_switch_id.setter
     def v_switch_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "v_switch_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "vSwitchId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="description")
     def description(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: description: The description of instance. It a string of 0 to 30 characters. It can contain numbers, letters, underscores, (_) and hyphens (-). It must start with a letter, a number or Chinese character.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "description"))
 
     @description.setter
     def description(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "description").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "description", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableKibanaPrivate")
     def enable_kibana_private(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property: enableKibanaPrivate: Enables or disables intranet access to Kibana.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "enableKibanaPrivate"))
 
     @enable_kibana_private.setter
     def enable_kibana_private(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "enable_kibana_private").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableKibanaPrivate", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableKibanaPublic")
     def enable_kibana_public(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property: enableKibanaPublic: Enables or disables Internet access to Kibana.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "enableKibanaPublic"))
 
     @enable_kibana_public.setter
     def enable_kibana_public(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "enable_kibana_public").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableKibanaPublic", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enablePublic")
     def enable_public(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property: enablePublic: Whether enable public access. If properties is true, will allocate public address.Default: false.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "enablePublic"))
 
     @enable_public.setter
     def enable_public(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "enable_public").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enablePublic", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="instanceChargeType")
     def instance_charge_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: instanceChargeType: Valid values are PrePaid, PostPaid, Default to PostPaid.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "instanceChargeType"))
 
     @instance_charge_type.setter
     def instance_charge_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "instance_charge_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "instanceChargeType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="kibanaNode")
     def kibana_node(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosInstance.KibanaNodeProperty"]]:
         '''
         :Property: kibanaNode: The dedicated kibana node setting.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosInstance.KibanaNodeProperty"]], jsii.get(self, "kibanaNode"))
 
     @kibana_node.setter
     def kibana_node(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosInstance.KibanaNodeProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "kibana_node").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "kibanaNode", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="kibanaWhitelist")
     def kibana_whitelist(
         self,
     ) -> typing.Optional[typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]]:
         '''
         :Property: kibanaWhitelist: Set the Kibana's IP whitelist in internet network.
         '''
         return typing.cast(typing.Optional[typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]], jsii.get(self, "kibanaWhitelist"))
 
     @kibana_whitelist.setter
     def kibana_whitelist(
         self,
         value: typing.Optional[typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "kibana_whitelist").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "kibanaWhitelist", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="masterNode")
     def master_node(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosInstance.MasterNodeProperty"]]:
         '''
         :Property: masterNode: The dedicated master node setting. If specified, dedicated master node will be created.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosInstance.MasterNodeProperty"]], jsii.get(self, "masterNode"))
 
     @master_node.setter
     def master_node(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosInstance.MasterNodeProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "master_node").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "masterNode", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="period")
     def period(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: period: The duration that you will buy Elasticsearch instance (in month). It is valid when instance_charge_type is PrePaid. Valid values: [1~9], 12, 24, 36. Default to 1.
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "period"))
 
     @period.setter
     def period(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "period").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "period", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="privateWhitelist")
     def private_whitelist(
         self,
     ) -> typing.Optional[typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]]:
         '''
         :Property: privateWhitelist: Set the instance's IP whitelist in VPC network.
         '''
         return typing.cast(typing.Optional[typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]], jsii.get(self, "privateWhitelist"))
 
     @private_whitelist.setter
     def private_whitelist(
         self,
         value: typing.Optional[typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "private_whitelist").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "privateWhitelist", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="publicWhitelist")
     def public_whitelist(
         self,
     ) -> typing.Optional[typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]]:
         '''
         :Property: publicWhitelist: Set the instance's IP whitelist in Internet. The AllocatePublicAddress should be true.
         '''
         return typing.cast(typing.Optional[typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]], jsii.get(self, "publicWhitelist"))
 
     @public_whitelist.setter
     def public_whitelist(
         self,
         value: typing.Optional[typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "public_whitelist").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "publicWhitelist", value)
 
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
+            type_hints = typing.get_type_hints(getattr(RosInstance, "resource_group_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "resourceGroupId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="tags")
     def tags(self) -> typing.Optional[typing.List["RosInstance.TagsProperty"]]:
         '''
         :Property: tags: Tags to attach to instance. Max support 20 tags to add during create instance. Each tag with two properties Key and Value, and Key is required.
         '''
         return typing.cast(typing.Optional[typing.List["RosInstance.TagsProperty"]], jsii.get(self, "tags"))
 
     @tags.setter
     def tags(
         self,
         value: typing.Optional[typing.List["RosInstance.TagsProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "tags").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "tags", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="ymlConfig")
     def yml_config(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosInstance.YMLConfigProperty"]]:
         '''
         :Property:
 
@@ -848,48 +941,57 @@
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosInstance.YMLConfigProperty"]], jsii.get(self, "ymlConfig"))
 
     @yml_config.setter
     def yml_config(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosInstance.YMLConfigProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "yml_config").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "ymlConfig", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="zoneCount")
     def zone_count(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: zoneCount: undefined
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "zoneCount"))
 
     @zone_count.setter
     def zone_count(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "zone_count").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "zoneCount", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="zoneId")
     def zone_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: zoneId: The zone id of elasticsearch.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "zoneId"))
 
     @zone_id.setter
     def zone_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "zone_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "zoneId", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-elasticsearch.RosInstance.DataNodeProperty",
         jsii_struct_bases=[],
         name_mapping={
             "amount": "amount",
@@ -915,14 +1017,22 @@
             :param amount: 
             :param disk_size: 
             :param disk_type: 
             :param spec: 
             :param disk_encryption: 
             :param performance_level: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosInstance.DataNodeProperty.__init__)
+                check_type(argname="argument amount", value=amount, expected_type=type_hints["amount"])
+                check_type(argname="argument disk_size", value=disk_size, expected_type=type_hints["disk_size"])
+                check_type(argname="argument disk_type", value=disk_type, expected_type=type_hints["disk_type"])
+                check_type(argname="argument spec", value=spec, expected_type=type_hints["spec"])
+                check_type(argname="argument disk_encryption", value=disk_encryption, expected_type=type_hints["disk_encryption"])
+                check_type(argname="argument performance_level", value=performance_level, expected_type=type_hints["performance_level"])
             self._values: typing.Dict[str, typing.Any] = {
                 "amount": amount,
                 "disk_size": disk_size,
                 "disk_type": disk_type,
                 "spec": spec,
             }
             if disk_encryption is not None:
@@ -1014,14 +1124,17 @@
             self,
             *,
             spec: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         ) -> None:
             '''
             :param spec: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosInstance.KibanaNodeProperty.__init__)
+                check_type(argname="argument spec", value=spec, expected_type=type_hints["spec"])
             self._values: typing.Dict[str, typing.Any] = {
                 "spec": spec,
             }
 
         @builtins.property
         def spec(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
             '''
@@ -1063,14 +1176,20 @@
         ) -> None:
             '''
             :param spec: 
             :param amount: 
             :param disk_size: 
             :param disk_type: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosInstance.MasterNodeProperty.__init__)
+                check_type(argname="argument spec", value=spec, expected_type=type_hints["spec"])
+                check_type(argname="argument amount", value=amount, expected_type=type_hints["amount"])
+                check_type(argname="argument disk_size", value=disk_size, expected_type=type_hints["disk_size"])
+                check_type(argname="argument disk_type", value=disk_type, expected_type=type_hints["disk_type"])
             self._values: typing.Dict[str, typing.Any] = {
                 "spec": spec,
             }
             if amount is not None:
                 self._values["amount"] = amount
             if disk_size is not None:
                 self._values["disk_size"] = disk_size
@@ -1139,14 +1258,18 @@
             key: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param key: 
             :param value: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosInstance.TagsProperty.__init__)
+                check_type(argname="argument key", value=key, expected_type=type_hints["key"])
+                check_type(argname="argument value", value=value, expected_type=type_hints["value"])
             self._values: typing.Dict[str, typing.Any] = {
                 "key": key,
             }
             if value is not None:
                 self._values["value"] = value
 
         @builtins.property
@@ -1203,14 +1326,21 @@
             '''
             :param audit_log: 
             :param create_index: 
             :param destructive_requires_name: 
             :param other_configs: 
             :param watcher: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosInstance.YMLConfigProperty.__init__)
+                check_type(argname="argument audit_log", value=audit_log, expected_type=type_hints["audit_log"])
+                check_type(argname="argument create_index", value=create_index, expected_type=type_hints["create_index"])
+                check_type(argname="argument destructive_requires_name", value=destructive_requires_name, expected_type=type_hints["destructive_requires_name"])
+                check_type(argname="argument other_configs", value=other_configs, expected_type=type_hints["other_configs"])
+                check_type(argname="argument watcher", value=watcher, expected_type=type_hints["watcher"])
             self._values: typing.Dict[str, typing.Any] = {}
             if audit_log is not None:
                 self._values["audit_log"] = audit_log
             if create_index is not None:
                 self._values["create_index"] = create_index
             if destructive_requires_name is not None:
                 self._values["destructive_requires_name"] = destructive_requires_name
@@ -1333,32 +1463,32 @@
         "zone_id": "zoneId",
     },
 )
 class RosInstanceProps:
     def __init__(
         self,
         *,
-        data_node: typing.Union[RosInstance.DataNodeProperty, ros_cdk_core.IResolvable],
+        data_node: typing.Union[typing.Union[RosInstance.DataNodeProperty, typing.Dict[str, typing.Any]], ros_cdk_core.IResolvable],
         password: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         version: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         v_switch_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         description: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         enable_kibana_private: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         enable_kibana_public: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         enable_public: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         instance_charge_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        kibana_node: typing.Optional[typing.Union[ros_cdk_core.IResolvable, RosInstance.KibanaNodeProperty]] = None,
+        kibana_node: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosInstance.KibanaNodeProperty, typing.Dict[str, typing.Any]]]] = None,
         kibana_whitelist: typing.Optional[typing.Union[typing.Sequence[typing.Any], ros_cdk_core.IResolvable]] = None,
-        master_node: typing.Optional[typing.Union[ros_cdk_core.IResolvable, RosInstance.MasterNodeProperty]] = None,
+        master_node: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosInstance.MasterNodeProperty, typing.Dict[str, typing.Any]]]] = None,
         period: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         private_whitelist: typing.Optional[typing.Union[typing.Sequence[typing.Any], ros_cdk_core.IResolvable]] = None,
         public_whitelist: typing.Optional[typing.Union[typing.Sequence[typing.Any], ros_cdk_core.IResolvable]] = None,
         resource_group_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        tags: typing.Optional[typing.Sequence[RosInstance.TagsProperty]] = None,
-        yml_config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, RosInstance.YMLConfigProperty]] = None,
+        tags: typing.Optional[typing.Sequence[typing.Union[RosInstance.TagsProperty, typing.Dict[str, typing.Any]]]] = None,
+        yml_config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosInstance.YMLConfigProperty, typing.Dict[str, typing.Any]]]] = None,
         zone_count: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         zone_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::ElasticSearch::Instance``.
 
         :param data_node: 
         :param password: 
@@ -1377,14 +1507,36 @@
         :param public_whitelist: 
         :param resource_group_id: 
         :param tags: 
         :param yml_config: 
         :param zone_count: 
         :param zone_id: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosInstanceProps.__init__)
+            check_type(argname="argument data_node", value=data_node, expected_type=type_hints["data_node"])
+            check_type(argname="argument password", value=password, expected_type=type_hints["password"])
+            check_type(argname="argument version", value=version, expected_type=type_hints["version"])
+            check_type(argname="argument v_switch_id", value=v_switch_id, expected_type=type_hints["v_switch_id"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument enable_kibana_private", value=enable_kibana_private, expected_type=type_hints["enable_kibana_private"])
+            check_type(argname="argument enable_kibana_public", value=enable_kibana_public, expected_type=type_hints["enable_kibana_public"])
+            check_type(argname="argument enable_public", value=enable_public, expected_type=type_hints["enable_public"])
+            check_type(argname="argument instance_charge_type", value=instance_charge_type, expected_type=type_hints["instance_charge_type"])
+            check_type(argname="argument kibana_node", value=kibana_node, expected_type=type_hints["kibana_node"])
+            check_type(argname="argument kibana_whitelist", value=kibana_whitelist, expected_type=type_hints["kibana_whitelist"])
+            check_type(argname="argument master_node", value=master_node, expected_type=type_hints["master_node"])
+            check_type(argname="argument period", value=period, expected_type=type_hints["period"])
+            check_type(argname="argument private_whitelist", value=private_whitelist, expected_type=type_hints["private_whitelist"])
+            check_type(argname="argument public_whitelist", value=public_whitelist, expected_type=type_hints["public_whitelist"])
+            check_type(argname="argument resource_group_id", value=resource_group_id, expected_type=type_hints["resource_group_id"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
+            check_type(argname="argument yml_config", value=yml_config, expected_type=type_hints["yml_config"])
+            check_type(argname="argument zone_count", value=zone_count, expected_type=type_hints["zone_count"])
+            check_type(argname="argument zone_id", value=zone_id, expected_type=type_hints["zone_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "data_node": data_node,
             "password": password,
             "version": version,
             "v_switch_id": v_switch_id,
         }
         if description is not None:
```

### Comparing `ros-cdk-elasticsearch-1.0.8/src/ros_cdk_elasticsearch.egg-info/PKG-INFO` & `ros-cdk-elasticsearch-1.0.9/src/ros_cdk_elasticsearch.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-elasticsearch
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS ELASTICSEARCH Construct Library
```

