# Comparing `tmp/ros-cdk-eci-1.0.8.tar.gz` & `tmp/ros-cdk-eci-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-eci-1.0.8.tar", last modified: Thu Jul 14 02:18:35 2022, max compression
+gzip compressed data, was "dist/ros-cdk-eci-1.0.9.tar", last modified: Fri Sep 23 12:17:27 2022, max compression
```

## Comparing `ros-cdk-eci-1.0.8.tar` & `ros-cdk-eci-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:18:35.000000 ros-cdk-eci-1.0.8/
--rw-r--r--   0 root         (0) root         (0)    10279 2022-07-14 02:18:34.000000 ros-cdk-eci-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2022-07-14 02:18:34.000000 ros-cdk-eci-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2022-07-14 02:18:34.000000 ros-cdk-eci-1.0.8/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1240 2022-07-14 02:18:35.000000 ros-cdk-eci-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      179 2022-07-14 02:18:34.000000 ros-cdk-eci-1.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)      106 2022-07-14 02:18:34.000000 ros-cdk-eci-1.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-07-14 02:18:35.000000 ros-cdk-eci-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1794 2022-07-14 02:18:34.000000 ros-cdk-eci-1.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:18:35.000000 ros-cdk-eci-1.0.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:18:35.000000 ros-cdk-eci-1.0.8/src/ros_cdk_eci/
--rw-r--r--   0 root         (0) root         (0)   190963 2022-07-14 02:18:34.000000 ros-cdk-eci-1.0.8/src/ros_cdk_eci/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:18:35.000000 ros-cdk-eci-1.0.8/src/ros_cdk_eci/_jsii/
--rw-r--r--   0 root         (0) root         (0)      370 2022-07-14 02:18:34.000000 ros-cdk-eci-1.0.8/src/ros_cdk_eci/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    82897 2022-07-14 02:18:34.000000 ros-cdk-eci-1.0.8/src/ros_cdk_eci/_jsii/ros-cdk-eci@1.0.8.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:18:34.000000 ros-cdk-eci-1.0.8/src/ros_cdk_eci/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:18:35.000000 ros-cdk-eci-1.0.8/src/ros_cdk_eci.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1240 2022-07-14 02:18:35.000000 ros-cdk-eci-1.0.8/src/ros_cdk_eci.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      400 2022-07-14 02:18:35.000000 ros-cdk-eci-1.0.8/src/ros_cdk_eci.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:18:35.000000 ros-cdk-eci-1.0.8/src/ros_cdk_eci.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2022-07-14 02:18:35.000000 ros-cdk-eci-1.0.8/src/ros_cdk_eci.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2022-07-14 02:18:35.000000 ros-cdk-eci-1.0.8/src/ros_cdk_eci.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:17:27.000000 ros-cdk-eci-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)    10279 2022-09-23 12:17:26.000000 ros-cdk-eci-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-09-23 12:17:26.000000 ros-cdk-eci-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2022-09-23 12:17:26.000000 ros-cdk-eci-1.0.9/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1240 2022-09-23 12:17:27.000000 ros-cdk-eci-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      179 2022-09-23 12:17:26.000000 ros-cdk-eci-1.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      236 2022-09-23 12:17:26.000000 ros-cdk-eci-1.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-09-23 12:17:27.000000 ros-cdk-eci-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1823 2022-09-23 12:17:26.000000 ros-cdk-eci-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:17:27.000000 ros-cdk-eci-1.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:17:27.000000 ros-cdk-eci-1.0.9/src/ros_cdk_eci/
+-rw-r--r--   0 root         (0) root         (0)   225328 2022-09-23 12:17:26.000000 ros-cdk-eci-1.0.9/src/ros_cdk_eci/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:17:27.000000 ros-cdk-eci-1.0.9/src/ros_cdk_eci/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      404 2022-09-23 12:17:26.000000 ros-cdk-eci-1.0.9/src/ros_cdk_eci/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    82956 2022-09-23 12:17:26.000000 ros-cdk-eci-1.0.9/src/ros_cdk_eci/_jsii/ros-cdk-eci@1.0.9.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 12:17:26.000000 ros-cdk-eci-1.0.9/src/ros_cdk_eci/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:17:27.000000 ros-cdk-eci-1.0.9/src/ros_cdk_eci.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1240 2022-09-23 12:17:27.000000 ros-cdk-eci-1.0.9/src/ros_cdk_eci.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      400 2022-09-23 12:17:27.000000 ros-cdk-eci-1.0.9/src/ros_cdk_eci.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 12:17:27.000000 ros-cdk-eci-1.0.9/src/ros_cdk_eci.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2022-09-23 12:17:27.000000 ros-cdk-eci-1.0.9/src/ros_cdk_eci.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2022-09-23 12:17:27.000000 ros-cdk-eci-1.0.9/src/ros_cdk_eci.egg-info/top_level.txt
```

### Comparing `ros-cdk-eci-1.0.8/LICENSE` & `ros-cdk-eci-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-eci-1.0.8/PKG-INFO` & `ros-cdk-eci-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-eci
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS ECI Construct Library
```

### Comparing `ros-cdk-eci-1.0.8/setup.py` & `ros-cdk-eci-1.0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-eci",
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
         "ros_cdk_eci",
         "ros_cdk_eci._jsii"
     ],
     "package_data": {
         "ros_cdk_eci._jsii": [
-            "ros-cdk-eci@1.0.8.jsii.tgz"
+            "ros-cdk-eci@1.0.9.jsii.tgz"
         ],
         "ros_cdk_eci": [
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

### Comparing `ros-cdk-eci-1.0.8/src/ros_cdk_eci/__init__.py` & `ros-cdk-eci-1.0.9/src/ros_cdk_eci/__init__.py`

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
 
 
 class ContainerGroup(
     ros_cdk_core.Resource,
@@ -29,91 +31,97 @@
 ):
     '''A ROS resource type:  ``ALIYUN::ECI::ContainerGroup``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "ContainerGroupProps",
+        props: typing.Union["ContainerGroupProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::ECI::ContainerGroup``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(ContainerGroup.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrContainerGroupId")
     def attr_container_group_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute ContainerGroupId: The ID of the container group.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrContainerGroupId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrContainerGroupName")
     def attr_container_group_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute ContainerGroupName: The name of the container group.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrContainerGroupName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrEniInstanceId")
     def attr_eni_instance_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute EniInstanceId: ENI instance ID.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrEniInstanceId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInternetIp")
     def attr_internet_ip(self) -> ros_cdk_core.IResolvable:
         '''Attribute InternetIp: Internet IP.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInternetIp"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrIntranetIp")
     def attr_intranet_ip(self) -> ros_cdk_core.IResolvable:
         '''Attribute IntranetIp: Intranet IP.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrIntranetIp"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrIpv6Address")
     def attr_ipv6_address(self) -> ros_cdk_core.IResolvable:
         '''Attribute Ipv6Address: Ipv6 address.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrIpv6Address"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrRegionId")
     def attr_region_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute RegionId: The ID of the region in which the instance resides.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrRegionId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrSecurityGroupId")
     def attr_security_group_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute SecurityGroupId: The ID of the security group to which the instance belongs.
 
         Instances in the same security group can access one another.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrSecurityGroupId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVSwitchId")
     def attr_v_switch_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute VSwitchId: The ID of the VSwitch.
 
         Currently, ECI instances can only be deployed in VPCs.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVSwitchId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrZoneId")
     def attr_zone_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute ZoneId: The ID of the zone in which the instance resides.
 
         If you leave the parameter blank, the system assigns a zone for you. The default value is blank.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrZoneId"))
@@ -153,41 +161,41 @@
         "zone_id": "zoneId",
     },
 )
 class ContainerGroupProps:
     def __init__(
         self,
         *,
-        container: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union["RosContainerGroup.ContainerProperty", ros_cdk_core.IResolvable]]],
+        container: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[typing.Union["RosContainerGroup.ContainerProperty", typing.Dict[str, typing.Any]], ros_cdk_core.IResolvable]]],
         container_group_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         security_group_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         v_switch_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
-        acr_registry_info: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosContainerGroup.AcrRegistryInfoProperty"]]]] = None,
+        acr_registry_info: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosContainerGroup.AcrRegistryInfoProperty", typing.Dict[str, typing.Any]]]]]] = None,
         active_deadline_seconds: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         auto_match_image_cache: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         cpu: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
-        dns_config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosContainerGroup.DnsConfigProperty"]] = None,
+        dns_config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosContainerGroup.DnsConfigProperty", typing.Dict[str, typing.Any]]]] = None,
         eip_instance_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        host_aliase: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosContainerGroup.HostAliaseProperty"]]]] = None,
-        image_registry_credential: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosContainerGroup.ImageRegistryCredentialProperty"]]]] = None,
+        host_aliase: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosContainerGroup.HostAliaseProperty", typing.Dict[str, typing.Any]]]]]] = None,
+        image_registry_credential: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosContainerGroup.ImageRegistryCredentialProperty", typing.Dict[str, typing.Any]]]]]] = None,
         image_snapshot_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        init_container: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosContainerGroup.InitContainerProperty"]]]] = None,
+        init_container: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosContainerGroup.InitContainerProperty", typing.Dict[str, typing.Any]]]]]] = None,
         instance_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ipv6_address_count: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         memory: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         ram_role_name: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         resource_group_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         restart_policy: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        security_context_sysctl: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosContainerGroup.SecurityContextSysctlProperty"]]]] = None,
+        security_context_sysctl: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosContainerGroup.SecurityContextSysctlProperty", typing.Dict[str, typing.Any]]]]]] = None,
         sls_enable: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         spot_price_limit: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         spot_strategy: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        tag: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, ros_cdk_core.RosTag]]]] = None,
+        tag: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[ros_cdk_core.RosTag, typing.Dict[str, typing.Any]]]]]] = None,
         termination_grace_period_seconds: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
-        volume: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosContainerGroup.VolumeProperty"]]]] = None,
+        volume: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosContainerGroup.VolumeProperty", typing.Dict[str, typing.Any]]]]]] = None,
         zone_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::ECI::ContainerGroup``.
 
         :param container: Property container: The containers that constitute the container group.
         :param container_group_name: Property containerGroupName: The name of the container group. The length is [2,128] English lowercase letters, numbers or hyphens (-), cannot begin or end with a hyphens.
         :param security_group_id: Property securityGroupId: The ID of the security group to which the instance belongs. Instances in the same security group can access one another.
@@ -213,14 +221,44 @@
         :param spot_price_limit: Property spotPriceLimit: Set the hourly maximum price of the instance. It supports a maximum of 3 decimal places. It takes effect when the value of the parameter SpotStrategy is SpotWithPriceLimit.
         :param spot_strategy: Property spotStrategy: Instance preemption strategy. Ranges: NoSpot (default): normal pay-as-you-go instances. SpotWithPriceLimit: Preemptive instance that sets a cap price. SpotAsPriceGo: The system automatically bids, following the current market actual price.
         :param tag: Property tag: The list of container group tags in the form of key/value pairs. You can define a maximum of 20 tags for each container group.
         :param termination_grace_period_seconds: Property terminationGracePeriodSeconds: The buffer time for the program to handle operations before it is stopped.
         :param volume: Property volume: The data volume. You can specify a maximum of 20 data volumes.
         :param zone_id: Property zoneId: The ID of the zone in which the instance resides. If you leave the parameter blank, the system assigns a zone for you. The default value is blank.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(ContainerGroupProps.__init__)
+            check_type(argname="argument container", value=container, expected_type=type_hints["container"])
+            check_type(argname="argument container_group_name", value=container_group_name, expected_type=type_hints["container_group_name"])
+            check_type(argname="argument security_group_id", value=security_group_id, expected_type=type_hints["security_group_id"])
+            check_type(argname="argument v_switch_id", value=v_switch_id, expected_type=type_hints["v_switch_id"])
+            check_type(argname="argument acr_registry_info", value=acr_registry_info, expected_type=type_hints["acr_registry_info"])
+            check_type(argname="argument active_deadline_seconds", value=active_deadline_seconds, expected_type=type_hints["active_deadline_seconds"])
+            check_type(argname="argument auto_match_image_cache", value=auto_match_image_cache, expected_type=type_hints["auto_match_image_cache"])
+            check_type(argname="argument cpu", value=cpu, expected_type=type_hints["cpu"])
+            check_type(argname="argument dns_config", value=dns_config, expected_type=type_hints["dns_config"])
+            check_type(argname="argument eip_instance_id", value=eip_instance_id, expected_type=type_hints["eip_instance_id"])
+            check_type(argname="argument host_aliase", value=host_aliase, expected_type=type_hints["host_aliase"])
+            check_type(argname="argument image_registry_credential", value=image_registry_credential, expected_type=type_hints["image_registry_credential"])
+            check_type(argname="argument image_snapshot_id", value=image_snapshot_id, expected_type=type_hints["image_snapshot_id"])
+            check_type(argname="argument init_container", value=init_container, expected_type=type_hints["init_container"])
+            check_type(argname="argument instance_type", value=instance_type, expected_type=type_hints["instance_type"])
+            check_type(argname="argument ipv6_address_count", value=ipv6_address_count, expected_type=type_hints["ipv6_address_count"])
+            check_type(argname="argument memory", value=memory, expected_type=type_hints["memory"])
+            check_type(argname="argument ram_role_name", value=ram_role_name, expected_type=type_hints["ram_role_name"])
+            check_type(argname="argument resource_group_id", value=resource_group_id, expected_type=type_hints["resource_group_id"])
+            check_type(argname="argument restart_policy", value=restart_policy, expected_type=type_hints["restart_policy"])
+            check_type(argname="argument security_context_sysctl", value=security_context_sysctl, expected_type=type_hints["security_context_sysctl"])
+            check_type(argname="argument sls_enable", value=sls_enable, expected_type=type_hints["sls_enable"])
+            check_type(argname="argument spot_price_limit", value=spot_price_limit, expected_type=type_hints["spot_price_limit"])
+            check_type(argname="argument spot_strategy", value=spot_strategy, expected_type=type_hints["spot_strategy"])
+            check_type(argname="argument tag", value=tag, expected_type=type_hints["tag"])
+            check_type(argname="argument termination_grace_period_seconds", value=termination_grace_period_seconds, expected_type=type_hints["termination_grace_period_seconds"])
+            check_type(argname="argument volume", value=volume, expected_type=type_hints["volume"])
+            check_type(argname="argument zone_id", value=zone_id, expected_type=type_hints["zone_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "container": container,
             "container_group_name": container_group_name,
             "security_group_id": security_group_id,
             "v_switch_id": v_switch_id,
         }
         if acr_registry_info is not None:
@@ -556,31 +594,37 @@
 ):
     '''A ROS resource type:  ``ALIYUN::ECI::ImageCache``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "ImageCacheProps",
+        props: typing.Union["ImageCacheProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::ECI::ImageCache``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(ImageCache.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrImageCacheId")
     def attr_image_cache_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute ImageCacheId: The ID of the image cache.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrImageCacheId"))
 
 
 @jsii.data_type(
@@ -614,14 +658,23 @@
         :param image_cache_name: Property imageCacheName: Image cache name.
         :param security_group_id: Property securityGroupId: Security group ID.
         :param v_switch_id: Property vSwitchId: VSwitch ID.
         :param eip_instance_id: Property eipInstanceId: If you want to pull the public network image, you need to configure the public network ip or configure the switch NAT gateway.
         :param image_registry_credential: Property imageRegistryCredential: Private image password. Alibaba Cloud ACR image can be left blank.
         :param resource_group_id: Property resourceGroupId: Resource group id.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(ImageCacheProps.__init__)
+            check_type(argname="argument image", value=image, expected_type=type_hints["image"])
+            check_type(argname="argument image_cache_name", value=image_cache_name, expected_type=type_hints["image_cache_name"])
+            check_type(argname="argument security_group_id", value=security_group_id, expected_type=type_hints["security_group_id"])
+            check_type(argname="argument v_switch_id", value=v_switch_id, expected_type=type_hints["v_switch_id"])
+            check_type(argname="argument eip_instance_id", value=eip_instance_id, expected_type=type_hints["eip_instance_id"])
+            check_type(argname="argument image_registry_credential", value=image_registry_credential, expected_type=type_hints["image_registry_credential"])
+            check_type(argname="argument resource_group_id", value=resource_group_id, expected_type=type_hints["resource_group_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "image": image,
             "image_cache_name": image_cache_name,
             "security_group_id": security_group_id,
             "v_switch_id": v_switch_id,
         }
         if eip_instance_id is not None:
@@ -707,145 +760,157 @@
 ):
     '''A ROS template type:  ``ALIYUN::ECI::ContainerGroup``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosContainerGroupProps",
+        props: typing.Union["RosContainerGroupProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::ECI::ContainerGroup``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosContainerGroup.__init__)
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
+            type_hints = typing.get_type_hints(RosContainerGroup._render_properties)
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
     @jsii.member(jsii_name="attrContainerGroupId")
     def attr_container_group_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ContainerGroupId: The ID of the container group.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrContainerGroupId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrContainerGroupName")
     def attr_container_group_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ContainerGroupName: The name of the container group.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrContainerGroupName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrEniInstanceId")
     def attr_eni_instance_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: EniInstanceId: ENI instance ID.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrEniInstanceId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInternetIp")
     def attr_internet_ip(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: InternetIp: Internet IP.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInternetIp"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrIntranetIp")
     def attr_intranet_ip(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: IntranetIp: Intranet IP.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrIntranetIp"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrIpv6Address")
     def attr_ipv6_address(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Ipv6Address: Ipv6 address.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrIpv6Address"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrRegionId")
     def attr_region_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: RegionId: The ID of the region in which the instance resides.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrRegionId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrSecurityGroupId")
     def attr_security_group_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: SecurityGroupId: The ID of the security group to which the instance belongs. Instances in the same security group can access one another.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrSecurityGroupId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVSwitchId")
     def attr_v_switch_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: VSwitchId: The ID of the VSwitch. Currently, ECI instances can only be deployed in VPCs.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVSwitchId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrZoneId")
     def attr_zone_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ZoneId: The ID of the zone in which the instance resides. If you leave the parameter blank, the system assigns a zone for you. The default value is blank.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrZoneId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="container")
     def container(
         self,
     ) -> typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union["RosContainerGroup.ContainerProperty", ros_cdk_core.IResolvable]]]:
         '''
         :Property: container: The containers that constitute the container group.
         '''
         return typing.cast(typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union["RosContainerGroup.ContainerProperty", ros_cdk_core.IResolvable]]], jsii.get(self, "container"))
 
     @container.setter
     def container(
         self,
         value: typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union["RosContainerGroup.ContainerProperty", ros_cdk_core.IResolvable]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosContainerGroup, "container").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "container", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="containerGroupName")
     def container_group_name(
         self,
     ) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
@@ -855,328 +920,388 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "containerGroupName"))
 
     @container_group_name.setter
     def container_group_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosContainerGroup, "container_group_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "containerGroupName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosContainerGroup, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="securityGroupId")
     def security_group_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: securityGroupId: The ID of the security group to which the instance belongs. Instances in the same security group can access one another.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "securityGroupId"))
 
     @security_group_id.setter
     def security_group_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosContainerGroup, "security_group_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "securityGroupId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vSwitchId")
     def v_switch_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: vSwitchId: The ID of the specified VSwitch. Currently, ECI instances can only be deployed in VPCs.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "vSwitchId"))
 
     @v_switch_id.setter
     def v_switch_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosContainerGroup, "v_switch_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "vSwitchId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="acrRegistryInfo")
     def acr_registry_info(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosContainerGroup.AcrRegistryInfoProperty"]]]]:
         '''
         :Property: acrRegistryInfo: Enterprise Edition access credential configuration information.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosContainerGroup.AcrRegistryInfoProperty"]]]], jsii.get(self, "acrRegistryInfo"))
 
     @acr_registry_info.setter
     def acr_registry_info(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosContainerGroup.AcrRegistryInfoProperty"]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosContainerGroup, "acr_registry_info").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "acrRegistryInfo", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="activeDeadlineSeconds")
     def active_deadline_seconds(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: activeDeadlineSeconds: The validity period in seconds.
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "activeDeadlineSeconds"))
 
     @active_deadline_seconds.setter
     def active_deadline_seconds(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosContainerGroup, "active_deadline_seconds").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "activeDeadlineSeconds", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="autoMatchImageCache")
     def auto_match_image_cache(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property: autoMatchImageCache: Specifies whether to automatically match the image cache.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "autoMatchImageCache"))
 
     @auto_match_image_cache.setter
     def auto_match_image_cache(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosContainerGroup, "auto_match_image_cache").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "autoMatchImageCache", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="cpu")
     def cpu(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: cpu: CPU size
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "cpu"))
 
     @cpu.setter
     def cpu(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosContainerGroup, "cpu").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "cpu", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dnsConfig")
     def dns_config(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosContainerGroup.DnsConfigProperty"]]:
         '''
         :Property: dnsConfig: The information about DNS configurations.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosContainerGroup.DnsConfigProperty"]], jsii.get(self, "dnsConfig"))
 
     @dns_config.setter
     def dns_config(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosContainerGroup.DnsConfigProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosContainerGroup, "dns_config").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dnsConfig", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="eipInstanceId")
     def eip_instance_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: eipInstanceId: Elastic IP ID
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "eipInstanceId"))
 
     @eip_instance_id.setter
     def eip_instance_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosContainerGroup, "eip_instance_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "eipInstanceId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="hostAliase")
     def host_aliase(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosContainerGroup.HostAliaseProperty"]]]]:
         '''
         :Property: hostAliase: Customize the hostname mapping of a container inside the pod
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosContainerGroup.HostAliaseProperty"]]]], jsii.get(self, "hostAliase"))
 
     @host_aliase.setter
     def host_aliase(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosContainerGroup.HostAliaseProperty"]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosContainerGroup, "host_aliase").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "hostAliase", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="imageRegistryCredential")
     def image_registry_credential(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosContainerGroup.ImageRegistryCredentialProperty"]]]]:
         '''
         :Property: imageRegistryCredential: The information that you need to log on to the container image repository, including the server address, username, and password.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosContainerGroup.ImageRegistryCredentialProperty"]]]], jsii.get(self, "imageRegistryCredential"))
 
     @image_registry_credential.setter
     def image_registry_credential(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosContainerGroup.ImageRegistryCredentialProperty"]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosContainerGroup, "image_registry_credential").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "imageRegistryCredential", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="imageSnapshotId")
     def image_snapshot_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: imageSnapshotId: Image cache ID or snapshot ID.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "imageSnapshotId"))
 
     @image_snapshot_id.setter
     def image_snapshot_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosContainerGroup, "image_snapshot_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "imageSnapshotId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="initContainer")
     def init_container(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosContainerGroup.InitContainerProperty"]]]]:
         '''
         :Property: initContainer: The containers that constitute the container group for initializing.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosContainerGroup.InitContainerProperty"]]]], jsii.get(self, "initContainer"))
 
     @init_container.setter
     def init_container(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosContainerGroup.InitContainerProperty"]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosContainerGroup, "init_container").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "initContainer", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="instanceType")
     def instance_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: instanceType: The type of the ECS instance.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "instanceType"))
 
     @instance_type.setter
     def instance_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosContainerGroup, "instance_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "instanceType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="ipv6AddressCount")
     def ipv6_address_count(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: ipv6AddressCount: The number of IPv6 addresses.
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "ipv6AddressCount"))
 
     @ipv6_address_count.setter
     def ipv6_address_count(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosContainerGroup, "ipv6_address_count").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "ipv6AddressCount", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="memory")
     def memory(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: memory: memory size
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "memory"))
 
     @memory.setter
     def memory(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosContainerGroup, "memory").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "memory", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="ramRoleName")
     def ram_role_name(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: ramRoleName: The RAM role that the container group assumes. ECI and ECS share the same RAM role.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "ramRoleName"))
 
     @ram_role_name.setter
     def ram_role_name(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosContainerGroup, "ram_role_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "ramRoleName", value)
 
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
+            type_hints = typing.get_type_hints(getattr(RosContainerGroup, "resource_group_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "resourceGroupId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="restartPolicy")
     def restart_policy(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: restartPolicy: The policy for restarting the instance. Default value: Always.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "restartPolicy"))
 
     @restart_policy.setter
     def restart_policy(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosContainerGroup, "restart_policy").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "restartPolicy", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="securityContextSysctl")
     def security_context_sysctl(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosContainerGroup.SecurityContextSysctlProperty"]]]]:
         '''
         :Property:
 
@@ -1188,51 +1313,60 @@
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosContainerGroup.SecurityContextSysctlProperty"]]]], jsii.get(self, "securityContextSysctl"))
 
     @security_context_sysctl.setter
     def security_context_sysctl(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosContainerGroup.SecurityContextSysctlProperty"]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosContainerGroup, "security_context_sysctl").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "securityContextSysctl", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="slsEnable")
     def sls_enable(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property: slsEnable: Enable user log collection. The default is False.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "slsEnable"))
 
     @sls_enable.setter
     def sls_enable(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosContainerGroup, "sls_enable").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "slsEnable", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="spotPriceLimit")
     def spot_price_limit(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: spotPriceLimit: Set the hourly maximum price of the instance. It supports a maximum of 3 decimal places. It takes effect when the value of the parameter SpotStrategy is SpotWithPriceLimit.
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "spotPriceLimit"))
 
     @spot_price_limit.setter
     def spot_price_limit(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosContainerGroup, "spot_price_limit").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "spotPriceLimit", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="spotStrategy")
     def spot_strategy(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -1245,82 +1379,97 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "spotStrategy"))
 
     @spot_strategy.setter
     def spot_strategy(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosContainerGroup, "spot_strategy").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "spotStrategy", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="tag")
     def tag(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, ros_cdk_core.RosTag]]]]:
         '''
         :Property: tag: The list of container group tags in the form of key/value pairs. You can define a maximum of 20 tags for each container group.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, ros_cdk_core.RosTag]]]], jsii.get(self, "tag"))
 
     @tag.setter
     def tag(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, ros_cdk_core.RosTag]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosContainerGroup, "tag").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "tag", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="terminationGracePeriodSeconds")
     def termination_grace_period_seconds(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: terminationGracePeriodSeconds: The buffer time for the program to handle operations before it is stopped.
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "terminationGracePeriodSeconds"))
 
     @termination_grace_period_seconds.setter
     def termination_grace_period_seconds(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosContainerGroup, "termination_grace_period_seconds").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "terminationGracePeriodSeconds", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="volume")
     def volume(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosContainerGroup.VolumeProperty"]]]]:
         '''
         :Property: volume: The data volume. You can specify a maximum of 20 data volumes.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosContainerGroup.VolumeProperty"]]]], jsii.get(self, "volume"))
 
     @volume.setter
     def volume(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosContainerGroup.VolumeProperty"]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosContainerGroup, "volume").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "volume", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="zoneId")
     def zone_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: zoneId: The ID of the zone in which the instance resides. If you leave the parameter blank, the system assigns a zone for you. The default value is blank.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "zoneId"))
 
     @zone_id.setter
     def zone_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosContainerGroup, "zone_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "zoneId", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-eci.RosContainerGroup.AcrRegistryInfoProperty",
         jsii_struct_bases=[],
         name_mapping={
             "instance_id": "instanceId",
@@ -1340,14 +1489,20 @@
         ) -> None:
             '''
             :param instance_id: 
             :param domain: 
             :param instance_name: 
             :param region_id: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosContainerGroup.AcrRegistryInfoProperty.__init__)
+                check_type(argname="argument instance_id", value=instance_id, expected_type=type_hints["instance_id"])
+                check_type(argname="argument domain", value=domain, expected_type=type_hints["domain"])
+                check_type(argname="argument instance_name", value=instance_name, expected_type=type_hints["instance_name"])
+                check_type(argname="argument region_id", value=region_id, expected_type=type_hints["region_id"])
             self._values: typing.Dict[str, typing.Any] = {
                 "instance_id": instance_id,
             }
             if domain is not None:
                 self._values["domain"] = domain
             if instance_name is not None:
                 self._values["instance_name"] = instance_name
@@ -1416,14 +1571,18 @@
             path: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             content: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param path: 
             :param content: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosContainerGroup.ConfigFileVolumeConfigFileToPathProperty.__init__)
+                check_type(argname="argument path", value=path, expected_type=type_hints["path"])
+                check_type(argname="argument content", value=content, expected_type=type_hints["content"])
             self._values: typing.Dict[str, typing.Any] = {
                 "path": path,
             }
             if content is not None:
                 self._values["content"] = content
 
         @builtins.property
@@ -1484,25 +1643,25 @@
             self,
             *,
             image: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             arg: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]] = None,
             command: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]] = None,
             cpu: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
-            environment_var: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosContainerGroup.EnvironmentVarProperty"]]]] = None,
+            environment_var: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosContainerGroup.EnvironmentVarProperty", typing.Dict[str, typing.Any]]]]]] = None,
             image_pull_policy: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-            liveness_probe: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosContainerGroup.LivenessProbeProperty"]] = None,
+            liveness_probe: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosContainerGroup.LivenessProbeProperty", typing.Dict[str, typing.Any]]]] = None,
             memory: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
-            port: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosContainerGroup.PortProperty"]]]] = None,
-            readiness_probe: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosContainerGroup.ReadinessProbeProperty"]] = None,
-            security_context: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosContainerGroup.SecurityContextProperty"]] = None,
+            port: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosContainerGroup.PortProperty", typing.Dict[str, typing.Any]]]]]] = None,
+            readiness_probe: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosContainerGroup.ReadinessProbeProperty", typing.Dict[str, typing.Any]]]] = None,
+            security_context: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosContainerGroup.SecurityContextProperty", typing.Dict[str, typing.Any]]]] = None,
             stdin: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
             stdin_once: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
             tty: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
-            volume_mount: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosContainerGroup.VolumeMountProperty"]]]] = None,
+            volume_mount: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosContainerGroup.VolumeMountProperty", typing.Dict[str, typing.Any]]]]]] = None,
             working_dir: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param image: 
             :param name: 
             :param arg: 
             :param command: 
@@ -1516,14 +1675,33 @@
             :param security_context: 
             :param stdin: 
             :param stdin_once: 
             :param tty: 
             :param volume_mount: 
             :param working_dir: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosContainerGroup.ContainerProperty.__init__)
+                check_type(argname="argument image", value=image, expected_type=type_hints["image"])
+                check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+                check_type(argname="argument arg", value=arg, expected_type=type_hints["arg"])
+                check_type(argname="argument command", value=command, expected_type=type_hints["command"])
+                check_type(argname="argument cpu", value=cpu, expected_type=type_hints["cpu"])
+                check_type(argname="argument environment_var", value=environment_var, expected_type=type_hints["environment_var"])
+                check_type(argname="argument image_pull_policy", value=image_pull_policy, expected_type=type_hints["image_pull_policy"])
+                check_type(argname="argument liveness_probe", value=liveness_probe, expected_type=type_hints["liveness_probe"])
+                check_type(argname="argument memory", value=memory, expected_type=type_hints["memory"])
+                check_type(argname="argument port", value=port, expected_type=type_hints["port"])
+                check_type(argname="argument readiness_probe", value=readiness_probe, expected_type=type_hints["readiness_probe"])
+                check_type(argname="argument security_context", value=security_context, expected_type=type_hints["security_context"])
+                check_type(argname="argument stdin", value=stdin, expected_type=type_hints["stdin"])
+                check_type(argname="argument stdin_once", value=stdin_once, expected_type=type_hints["stdin_once"])
+                check_type(argname="argument tty", value=tty, expected_type=type_hints["tty"])
+                check_type(argname="argument volume_mount", value=volume_mount, expected_type=type_hints["volume_mount"])
+                check_type(argname="argument working_dir", value=working_dir, expected_type=type_hints["working_dir"])
             self._values: typing.Dict[str, typing.Any] = {
                 "image": image,
                 "name": name,
             }
             if arg is not None:
                 self._values["arg"] = arg
             if command is not None:
@@ -1744,22 +1922,27 @@
         },
     )
     class DnsConfigProperty:
         def __init__(
             self,
             *,
             name_server: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]] = None,
-            option: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosContainerGroup.OptionProperty"]]]] = None,
+            option: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosContainerGroup.OptionProperty", typing.Dict[str, typing.Any]]]]]] = None,
             search: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]] = None,
         ) -> None:
             '''
             :param name_server: 
             :param option: 
             :param search: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosContainerGroup.DnsConfigProperty.__init__)
+                check_type(argname="argument name_server", value=name_server, expected_type=type_hints["name_server"])
+                check_type(argname="argument option", value=option, expected_type=type_hints["option"])
+                check_type(argname="argument search", value=search, expected_type=type_hints["search"])
             self._values: typing.Dict[str, typing.Any] = {}
             if name_server is not None:
                 self._values["name_server"] = name_server
             if option is not None:
                 self._values["option"] = option
             if search is not None:
                 self._values["search"] = search
@@ -1823,14 +2006,19 @@
             value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param field_ref_field_path: 
             :param key: 
             :param value: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosContainerGroup.EnvironmentVarProperty.__init__)
+                check_type(argname="argument field_ref_field_path", value=field_ref_field_path, expected_type=type_hints["field_ref_field_path"])
+                check_type(argname="argument key", value=key, expected_type=type_hints["key"])
+                check_type(argname="argument value", value=value, expected_type=type_hints["value"])
             self._values: typing.Dict[str, typing.Any] = {}
             if field_ref_field_path is not None:
                 self._values["field_ref_field_path"] = field_ref_field_path
             if key is not None:
                 self._values["key"] = key
             if value is not None:
                 self._values["value"] = value
@@ -1888,14 +2076,18 @@
             hostname: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]] = None,
             ip: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param hostname: 
             :param ip: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosContainerGroup.HostAliaseProperty.__init__)
+                check_type(argname="argument hostname", value=hostname, expected_type=type_hints["hostname"])
+                check_type(argname="argument ip", value=ip, expected_type=type_hints["ip"])
             self._values: typing.Dict[str, typing.Any] = {}
             if hostname is not None:
                 self._values["hostname"] = hostname
             if ip is not None:
                 self._values["ip"] = ip
 
         @builtins.property
@@ -1947,14 +2139,19 @@
             user_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         ) -> None:
             '''
             :param password: 
             :param server: 
             :param user_name: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosContainerGroup.ImageRegistryCredentialProperty.__init__)
+                check_type(argname="argument password", value=password, expected_type=type_hints["password"])
+                check_type(argname="argument server", value=server, expected_type=type_hints["server"])
+                check_type(argname="argument user_name", value=user_name, expected_type=type_hints["user_name"])
             self._values: typing.Dict[str, typing.Any] = {
                 "password": password,
                 "server": server,
                 "user_name": user_name,
             }
 
         @builtins.property
@@ -2013,14 +2210,19 @@
             value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param field_ref_field_path: 
             :param key: 
             :param value: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosContainerGroup.InitContainerEnvironmentVarProperty.__init__)
+                check_type(argname="argument field_ref_field_path", value=field_ref_field_path, expected_type=type_hints["field_ref_field_path"])
+                check_type(argname="argument key", value=key, expected_type=type_hints["key"])
+                check_type(argname="argument value", value=value, expected_type=type_hints["value"])
             self._values: typing.Dict[str, typing.Any] = {}
             if field_ref_field_path is not None:
                 self._values["field_ref_field_path"] = field_ref_field_path
             if key is not None:
                 self._values["key"] = key
             if value is not None:
                 self._values["value"] = value
@@ -2078,14 +2280,18 @@
             port: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
             protocol: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param port: 
             :param protocol: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosContainerGroup.InitContainerPortProperty.__init__)
+                check_type(argname="argument port", value=port, expected_type=type_hints["port"])
+                check_type(argname="argument protocol", value=protocol, expected_type=type_hints["protocol"])
             self._values: typing.Dict[str, typing.Any] = {}
             if port is not None:
                 self._values["port"] = port
             if protocol is not None:
                 self._values["protocol"] = protocol
 
         @builtins.property
@@ -2140,22 +2346,22 @@
     class InitContainerProperty:
         def __init__(
             self,
             *,
             arg: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]] = None,
             command: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]] = None,
             cpu: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
-            environment_var: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosContainerGroup.InitContainerEnvironmentVarProperty"]]]] = None,
+            environment_var: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosContainerGroup.InitContainerEnvironmentVarProperty", typing.Dict[str, typing.Any]]]]]] = None,
             image: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
             image_pull_policy: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
             memory: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
             name: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-            port: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosContainerGroup.InitContainerPortProperty"]]]] = None,
-            security_context: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosContainerGroup.InitContainerSecurityContextProperty"]] = None,
-            volume_mount: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosContainerGroup.InitContainerVolumeMountProperty"]]]] = None,
+            port: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosContainerGroup.InitContainerPortProperty", typing.Dict[str, typing.Any]]]]]] = None,
+            security_context: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosContainerGroup.InitContainerSecurityContextProperty", typing.Dict[str, typing.Any]]]] = None,
+            volume_mount: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosContainerGroup.InitContainerVolumeMountProperty", typing.Dict[str, typing.Any]]]]]] = None,
             working_dir: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param arg: 
             :param command: 
             :param cpu: 
             :param environment_var: 
@@ -2164,14 +2370,28 @@
             :param memory: 
             :param name: 
             :param port: 
             :param security_context: 
             :param volume_mount: 
             :param working_dir: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosContainerGroup.InitContainerProperty.__init__)
+                check_type(argname="argument arg", value=arg, expected_type=type_hints["arg"])
+                check_type(argname="argument command", value=command, expected_type=type_hints["command"])
+                check_type(argname="argument cpu", value=cpu, expected_type=type_hints["cpu"])
+                check_type(argname="argument environment_var", value=environment_var, expected_type=type_hints["environment_var"])
+                check_type(argname="argument image", value=image, expected_type=type_hints["image"])
+                check_type(argname="argument image_pull_policy", value=image_pull_policy, expected_type=type_hints["image_pull_policy"])
+                check_type(argname="argument memory", value=memory, expected_type=type_hints["memory"])
+                check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+                check_type(argname="argument port", value=port, expected_type=type_hints["port"])
+                check_type(argname="argument security_context", value=security_context, expected_type=type_hints["security_context"])
+                check_type(argname="argument volume_mount", value=volume_mount, expected_type=type_hints["volume_mount"])
+                check_type(argname="argument working_dir", value=working_dir, expected_type=type_hints["working_dir"])
             self._values: typing.Dict[str, typing.Any] = {}
             if arg is not None:
                 self._values["arg"] = arg
             if command is not None:
                 self._values["command"] = command
             if cpu is not None:
                 self._values["cpu"] = cpu
@@ -2343,14 +2563,19 @@
             run_as_user: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param capability_add: 
             :param read_only_root_filesystem: 
             :param run_as_user: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosContainerGroup.InitContainerSecurityContextProperty.__init__)
+                check_type(argname="argument capability_add", value=capability_add, expected_type=type_hints["capability_add"])
+                check_type(argname="argument read_only_root_filesystem", value=read_only_root_filesystem, expected_type=type_hints["read_only_root_filesystem"])
+                check_type(argname="argument run_as_user", value=run_as_user, expected_type=type_hints["run_as_user"])
             self._values: typing.Dict[str, typing.Any] = {}
             if capability_add is not None:
                 self._values["capability_add"] = capability_add
             if read_only_root_filesystem is not None:
                 self._values["read_only_root_filesystem"] = read_only_root_filesystem
             if run_as_user is not None:
                 self._values["run_as_user"] = run_as_user
@@ -2414,14 +2639,19 @@
             read_only: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param mount_path: 
             :param name: 
             :param read_only: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosContainerGroup.InitContainerVolumeMountProperty.__init__)
+                check_type(argname="argument mount_path", value=mount_path, expected_type=type_hints["mount_path"])
+                check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+                check_type(argname="argument read_only", value=read_only, expected_type=type_hints["read_only"])
             self._values: typing.Dict[str, typing.Any] = {}
             if mount_path is not None:
                 self._values["mount_path"] = mount_path
             if name is not None:
                 self._values["name"] = name
             if read_only is not None:
                 self._values["read_only"] = read_only
@@ -2506,14 +2736,26 @@
             :param http_get_scheme: 
             :param initial_delay_seconds: 
             :param period_seconds: 
             :param success_threshold: 
             :param tcp_socket_port: 
             :param timeout_seconds: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosContainerGroup.LivenessProbeProperty.__init__)
+                check_type(argname="argument exec_command", value=exec_command, expected_type=type_hints["exec_command"])
+                check_type(argname="argument failure_threshold", value=failure_threshold, expected_type=type_hints["failure_threshold"])
+                check_type(argname="argument http_get_path", value=http_get_path, expected_type=type_hints["http_get_path"])
+                check_type(argname="argument http_get_port", value=http_get_port, expected_type=type_hints["http_get_port"])
+                check_type(argname="argument http_get_scheme", value=http_get_scheme, expected_type=type_hints["http_get_scheme"])
+                check_type(argname="argument initial_delay_seconds", value=initial_delay_seconds, expected_type=type_hints["initial_delay_seconds"])
+                check_type(argname="argument period_seconds", value=period_seconds, expected_type=type_hints["period_seconds"])
+                check_type(argname="argument success_threshold", value=success_threshold, expected_type=type_hints["success_threshold"])
+                check_type(argname="argument tcp_socket_port", value=tcp_socket_port, expected_type=type_hints["tcp_socket_port"])
+                check_type(argname="argument timeout_seconds", value=timeout_seconds, expected_type=type_hints["timeout_seconds"])
             self._values: typing.Dict[str, typing.Any] = {}
             if exec_command is not None:
                 self._values["exec_command"] = exec_command
             if failure_threshold is not None:
                 self._values["failure_threshold"] = failure_threshold
             if http_get_path is not None:
                 self._values["http_get_path"] = http_get_path
@@ -2655,14 +2897,18 @@
             name: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
             value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param name: 
             :param value: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosContainerGroup.OptionProperty.__init__)
+                check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+                check_type(argname="argument value", value=value, expected_type=type_hints["value"])
             self._values: typing.Dict[str, typing.Any] = {}
             if name is not None:
                 self._values["name"] = name
             if value is not None:
                 self._values["value"] = value
 
         @builtins.property
@@ -2708,14 +2954,18 @@
             port: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
             protocol: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param port: 
             :param protocol: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosContainerGroup.PortProperty.__init__)
+                check_type(argname="argument port", value=port, expected_type=type_hints["port"])
+                check_type(argname="argument protocol", value=protocol, expected_type=type_hints["protocol"])
             self._values: typing.Dict[str, typing.Any] = {}
             if port is not None:
                 self._values["port"] = port
             if protocol is not None:
                 self._values["protocol"] = protocol
 
         @builtins.property
@@ -2788,14 +3038,26 @@
             :param http_get_scheme: 
             :param initial_delay_seconds: 
             :param period_seconds: 
             :param success_threshold: 
             :param tcp_socket_port: 
             :param timeout_seconds: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosContainerGroup.ReadinessProbeProperty.__init__)
+                check_type(argname="argument exec_command", value=exec_command, expected_type=type_hints["exec_command"])
+                check_type(argname="argument failure_threshold", value=failure_threshold, expected_type=type_hints["failure_threshold"])
+                check_type(argname="argument http_get_path", value=http_get_path, expected_type=type_hints["http_get_path"])
+                check_type(argname="argument http_get_port", value=http_get_port, expected_type=type_hints["http_get_port"])
+                check_type(argname="argument http_get_scheme", value=http_get_scheme, expected_type=type_hints["http_get_scheme"])
+                check_type(argname="argument initial_delay_seconds", value=initial_delay_seconds, expected_type=type_hints["initial_delay_seconds"])
+                check_type(argname="argument period_seconds", value=period_seconds, expected_type=type_hints["period_seconds"])
+                check_type(argname="argument success_threshold", value=success_threshold, expected_type=type_hints["success_threshold"])
+                check_type(argname="argument tcp_socket_port", value=tcp_socket_port, expected_type=type_hints["tcp_socket_port"])
+                check_type(argname="argument timeout_seconds", value=timeout_seconds, expected_type=type_hints["timeout_seconds"])
             self._values: typing.Dict[str, typing.Any] = {}
             if exec_command is not None:
                 self._values["exec_command"] = exec_command
             if failure_threshold is not None:
                 self._values["failure_threshold"] = failure_threshold
             if http_get_path is not None:
                 self._values["http_get_path"] = http_get_path
@@ -2943,14 +3205,19 @@
             run_as_user: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param capability_add: 
             :param read_only_root_filesystem: 
             :param run_as_user: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosContainerGroup.SecurityContextProperty.__init__)
+                check_type(argname="argument capability_add", value=capability_add, expected_type=type_hints["capability_add"])
+                check_type(argname="argument read_only_root_filesystem", value=read_only_root_filesystem, expected_type=type_hints["read_only_root_filesystem"])
+                check_type(argname="argument run_as_user", value=run_as_user, expected_type=type_hints["run_as_user"])
             self._values: typing.Dict[str, typing.Any] = {}
             if capability_add is not None:
                 self._values["capability_add"] = capability_add
             if read_only_root_filesystem is not None:
                 self._values["read_only_root_filesystem"] = read_only_root_filesystem
             if run_as_user is not None:
                 self._values["run_as_user"] = run_as_user
@@ -3008,14 +3275,18 @@
             name: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
             value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param name: 
             :param value: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosContainerGroup.SecurityContextSysctlProperty.__init__)
+                check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+                check_type(argname="argument value", value=value, expected_type=type_hints["value"])
             self._values: typing.Dict[str, typing.Any] = {}
             if name is not None:
                 self._values["name"] = name
             if value is not None:
                 self._values["value"] = value
 
         @builtins.property
@@ -3061,14 +3332,18 @@
             key: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param key: 
             :param value: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosContainerGroup.TagProperty.__init__)
+                check_type(argname="argument key", value=key, expected_type=type_hints["key"])
+                check_type(argname="argument value", value=value, expected_type=type_hints["value"])
             self._values: typing.Dict[str, typing.Any] = {
                 "key": key,
             }
             if value is not None:
                 self._values["value"] = value
 
         @builtins.property
@@ -3119,14 +3394,19 @@
             read_only: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param mount_path: 
             :param name: 
             :param read_only: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosContainerGroup.VolumeMountProperty.__init__)
+                check_type(argname="argument mount_path", value=mount_path, expected_type=type_hints["mount_path"])
+                check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+                check_type(argname="argument read_only", value=read_only, expected_type=type_hints["read_only"])
             self._values: typing.Dict[str, typing.Any] = {}
             if mount_path is not None:
                 self._values["mount_path"] = mount_path
             if name is not None:
                 self._values["name"] = name
             if read_only is not None:
                 self._values["read_only"] = read_only
@@ -3187,29 +3467,38 @@
     )
     class VolumeProperty:
         def __init__(
             self,
             *,
             name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             type: typing.Union[builtins.str, ros_cdk_core.IResolvable],
-            config_file_volume_config_file_to_path: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosContainerGroup.ConfigFileVolumeConfigFileToPathProperty"]]]] = None,
+            config_file_volume_config_file_to_path: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosContainerGroup.ConfigFileVolumeConfigFileToPathProperty", typing.Dict[str, typing.Any]]]]]] = None,
             empty_dir_volume_medium: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
             nfs_volume_path: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
             nfs_volume_read_only: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
             nfs_volume_server: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param name: 
             :param type: 
             :param config_file_volume_config_file_to_path: 
             :param empty_dir_volume_medium: 
             :param nfs_volume_path: 
             :param nfs_volume_read_only: 
             :param nfs_volume_server: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosContainerGroup.VolumeProperty.__init__)
+                check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+                check_type(argname="argument type", value=type, expected_type=type_hints["type"])
+                check_type(argname="argument config_file_volume_config_file_to_path", value=config_file_volume_config_file_to_path, expected_type=type_hints["config_file_volume_config_file_to_path"])
+                check_type(argname="argument empty_dir_volume_medium", value=empty_dir_volume_medium, expected_type=type_hints["empty_dir_volume_medium"])
+                check_type(argname="argument nfs_volume_path", value=nfs_volume_path, expected_type=type_hints["nfs_volume_path"])
+                check_type(argname="argument nfs_volume_read_only", value=nfs_volume_read_only, expected_type=type_hints["nfs_volume_read_only"])
+                check_type(argname="argument nfs_volume_server", value=nfs_volume_server, expected_type=type_hints["nfs_volume_server"])
             self._values: typing.Dict[str, typing.Any] = {
                 "name": name,
                 "type": type,
             }
             if config_file_volume_config_file_to_path is not None:
                 self._values["config_file_volume_config_file_to_path"] = config_file_volume_config_file_to_path
             if empty_dir_volume_medium is not None:
@@ -3335,41 +3624,41 @@
         "zone_id": "zoneId",
     },
 )
 class RosContainerGroupProps:
     def __init__(
         self,
         *,
-        container: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[RosContainerGroup.ContainerProperty, ros_cdk_core.IResolvable]]],
+        container: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[typing.Union[RosContainerGroup.ContainerProperty, typing.Dict[str, typing.Any]], ros_cdk_core.IResolvable]]],
         container_group_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         security_group_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         v_switch_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
-        acr_registry_info: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosContainerGroup.AcrRegistryInfoProperty]]]] = None,
+        acr_registry_info: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosContainerGroup.AcrRegistryInfoProperty, typing.Dict[str, typing.Any]]]]]] = None,
         active_deadline_seconds: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         auto_match_image_cache: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         cpu: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
-        dns_config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, RosContainerGroup.DnsConfigProperty]] = None,
+        dns_config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosContainerGroup.DnsConfigProperty, typing.Dict[str, typing.Any]]]] = None,
         eip_instance_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        host_aliase: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosContainerGroup.HostAliaseProperty]]]] = None,
-        image_registry_credential: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosContainerGroup.ImageRegistryCredentialProperty]]]] = None,
+        host_aliase: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosContainerGroup.HostAliaseProperty, typing.Dict[str, typing.Any]]]]]] = None,
+        image_registry_credential: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosContainerGroup.ImageRegistryCredentialProperty, typing.Dict[str, typing.Any]]]]]] = None,
         image_snapshot_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        init_container: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosContainerGroup.InitContainerProperty]]]] = None,
+        init_container: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosContainerGroup.InitContainerProperty, typing.Dict[str, typing.Any]]]]]] = None,
         instance_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ipv6_address_count: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         memory: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         ram_role_name: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         resource_group_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         restart_policy: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        security_context_sysctl: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosContainerGroup.SecurityContextSysctlProperty]]]] = None,
+        security_context_sysctl: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosContainerGroup.SecurityContextSysctlProperty, typing.Dict[str, typing.Any]]]]]] = None,
         sls_enable: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         spot_price_limit: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         spot_strategy: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        tag: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, ros_cdk_core.RosTag]]]] = None,
+        tag: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[ros_cdk_core.RosTag, typing.Dict[str, typing.Any]]]]]] = None,
         termination_grace_period_seconds: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
-        volume: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosContainerGroup.VolumeProperty]]]] = None,
+        volume: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosContainerGroup.VolumeProperty, typing.Dict[str, typing.Any]]]]]] = None,
         zone_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::ECI::ContainerGroup``.
 
         :param container: 
         :param container_group_name: 
         :param security_group_id: 
@@ -3395,14 +3684,44 @@
         :param spot_price_limit: 
         :param spot_strategy: 
         :param tag: 
         :param termination_grace_period_seconds: 
         :param volume: 
         :param zone_id: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosContainerGroupProps.__init__)
+            check_type(argname="argument container", value=container, expected_type=type_hints["container"])
+            check_type(argname="argument container_group_name", value=container_group_name, expected_type=type_hints["container_group_name"])
+            check_type(argname="argument security_group_id", value=security_group_id, expected_type=type_hints["security_group_id"])
+            check_type(argname="argument v_switch_id", value=v_switch_id, expected_type=type_hints["v_switch_id"])
+            check_type(argname="argument acr_registry_info", value=acr_registry_info, expected_type=type_hints["acr_registry_info"])
+            check_type(argname="argument active_deadline_seconds", value=active_deadline_seconds, expected_type=type_hints["active_deadline_seconds"])
+            check_type(argname="argument auto_match_image_cache", value=auto_match_image_cache, expected_type=type_hints["auto_match_image_cache"])
+            check_type(argname="argument cpu", value=cpu, expected_type=type_hints["cpu"])
+            check_type(argname="argument dns_config", value=dns_config, expected_type=type_hints["dns_config"])
+            check_type(argname="argument eip_instance_id", value=eip_instance_id, expected_type=type_hints["eip_instance_id"])
+            check_type(argname="argument host_aliase", value=host_aliase, expected_type=type_hints["host_aliase"])
+            check_type(argname="argument image_registry_credential", value=image_registry_credential, expected_type=type_hints["image_registry_credential"])
+            check_type(argname="argument image_snapshot_id", value=image_snapshot_id, expected_type=type_hints["image_snapshot_id"])
+            check_type(argname="argument init_container", value=init_container, expected_type=type_hints["init_container"])
+            check_type(argname="argument instance_type", value=instance_type, expected_type=type_hints["instance_type"])
+            check_type(argname="argument ipv6_address_count", value=ipv6_address_count, expected_type=type_hints["ipv6_address_count"])
+            check_type(argname="argument memory", value=memory, expected_type=type_hints["memory"])
+            check_type(argname="argument ram_role_name", value=ram_role_name, expected_type=type_hints["ram_role_name"])
+            check_type(argname="argument resource_group_id", value=resource_group_id, expected_type=type_hints["resource_group_id"])
+            check_type(argname="argument restart_policy", value=restart_policy, expected_type=type_hints["restart_policy"])
+            check_type(argname="argument security_context_sysctl", value=security_context_sysctl, expected_type=type_hints["security_context_sysctl"])
+            check_type(argname="argument sls_enable", value=sls_enable, expected_type=type_hints["sls_enable"])
+            check_type(argname="argument spot_price_limit", value=spot_price_limit, expected_type=type_hints["spot_price_limit"])
+            check_type(argname="argument spot_strategy", value=spot_strategy, expected_type=type_hints["spot_strategy"])
+            check_type(argname="argument tag", value=tag, expected_type=type_hints["tag"])
+            check_type(argname="argument termination_grace_period_seconds", value=termination_grace_period_seconds, expected_type=type_hints["termination_grace_period_seconds"])
+            check_type(argname="argument volume", value=volume, expected_type=type_hints["volume"])
+            check_type(argname="argument zone_id", value=zone_id, expected_type=type_hints["zone_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "container": container,
             "container_group_name": container_group_name,
             "security_group_id": security_group_id,
             "v_switch_id": v_switch_id,
         }
         if acr_registry_info is not None:
@@ -3767,175 +4086,208 @@
 ):
     '''A ROS template type:  ``ALIYUN::ECI::ImageCache``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosImageCacheProps",
+        props: typing.Union["RosImageCacheProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::ECI::ImageCache``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosImageCache.__init__)
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
+            type_hints = typing.get_type_hints(RosImageCache._render_properties)
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
     @jsii.member(jsii_name="attrImageCacheId")
     def attr_image_cache_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ImageCacheId: The ID of the image cache.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrImageCacheId"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosImageCache, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="image")
     def image(
         self,
     ) -> typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]:
         '''
         :Property: image: The image list to be cached.
         '''
         return typing.cast(typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]], jsii.get(self, "image"))
 
     @image.setter
     def image(
         self,
         value: typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosImageCache, "image").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "image", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="imageCacheName")
     def image_cache_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: imageCacheName: Image cache name.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "imageCacheName"))
 
     @image_cache_name.setter
     def image_cache_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosImageCache, "image_cache_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "imageCacheName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="securityGroupId")
     def security_group_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: securityGroupId: Security group ID.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "securityGroupId"))
 
     @security_group_id.setter
     def security_group_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosImageCache, "security_group_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "securityGroupId", value)
 
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
+            type_hints = typing.get_type_hints(getattr(RosImageCache, "v_switch_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "vSwitchId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="eipInstanceId")
     def eip_instance_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: eipInstanceId: If you want to pull the public network image, you need to configure the public network ip or configure the switch NAT gateway.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "eipInstanceId"))
 
     @eip_instance_id.setter
     def eip_instance_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosImageCache, "eip_instance_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "eipInstanceId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="imageRegistryCredential")
     def image_registry_credential(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]]:
         '''
         :Property: imageRegistryCredential: Private image password. Alibaba Cloud ACR image can be left blank.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]], jsii.get(self, "imageRegistryCredential"))
 
     @image_registry_credential.setter
     def image_registry_credential(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosImageCache, "image_registry_credential").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "imageRegistryCredential", value)
 
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
+            type_hints = typing.get_type_hints(getattr(RosImageCache, "resource_group_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "resourceGroupId", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-eci.RosImageCacheProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -3966,14 +4318,23 @@
         :param image_cache_name: 
         :param security_group_id: 
         :param v_switch_id: 
         :param eip_instance_id: 
         :param image_registry_credential: 
         :param resource_group_id: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosImageCacheProps.__init__)
+            check_type(argname="argument image", value=image, expected_type=type_hints["image"])
+            check_type(argname="argument image_cache_name", value=image_cache_name, expected_type=type_hints["image_cache_name"])
+            check_type(argname="argument security_group_id", value=security_group_id, expected_type=type_hints["security_group_id"])
+            check_type(argname="argument v_switch_id", value=v_switch_id, expected_type=type_hints["v_switch_id"])
+            check_type(argname="argument eip_instance_id", value=eip_instance_id, expected_type=type_hints["eip_instance_id"])
+            check_type(argname="argument image_registry_credential", value=image_registry_credential, expected_type=type_hints["image_registry_credential"])
+            check_type(argname="argument resource_group_id", value=resource_group_id, expected_type=type_hints["resource_group_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "image": image,
             "image_cache_name": image_cache_name,
             "security_group_id": security_group_id,
             "v_switch_id": v_switch_id,
         }
         if eip_instance_id is not None:
```

### Comparing `ros-cdk-eci-1.0.8/src/ros_cdk_eci.egg-info/PKG-INFO` & `ros-cdk-eci-1.0.9/src/ros_cdk_eci.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-eci
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS ECI Construct Library
```

