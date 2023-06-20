# Comparing `tmp/ros-cdk-memcache-1.0.8.tar.gz` & `tmp/ros-cdk-memcache-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-memcache-1.0.8.tar", last modified: Thu Jul 14 02:31:53 2022, max compression
+gzip compressed data, was "dist/ros-cdk-memcache-1.0.9.tar", last modified: Fri Sep 23 12:22:48 2022, max compression
```

## Comparing `ros-cdk-memcache-1.0.8.tar` & `ros-cdk-memcache-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:31:53.000000 ros-cdk-memcache-1.0.8/
--rw-r--r--   0 root         (0) root         (0)    10279 2022-07-14 02:31:53.000000 ros-cdk-memcache-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2022-07-14 02:31:53.000000 ros-cdk-memcache-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2022-07-14 02:31:53.000000 ros-cdk-memcache-1.0.8/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1260 2022-07-14 02:31:53.000000 ros-cdk-memcache-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      194 2022-07-14 02:31:53.000000 ros-cdk-memcache-1.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)      106 2022-07-14 02:31:53.000000 ros-cdk-memcache-1.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-07-14 02:31:53.000000 ros-cdk-memcache-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1824 2022-07-14 02:31:53.000000 ros-cdk-memcache-1.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:31:53.000000 ros-cdk-memcache-1.0.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:31:53.000000 ros-cdk-memcache-1.0.8/src/ros_cdk_memcache/
--rw-r--r--   0 root         (0) root         (0)    73531 2022-07-14 02:31:53.000000 ros-cdk-memcache-1.0.8/src/ros_cdk_memcache/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:31:53.000000 ros-cdk-memcache-1.0.8/src/ros_cdk_memcache/_jsii/
--rw-r--r--   0 root         (0) root         (0)      393 2022-07-14 02:31:53.000000 ros-cdk-memcache-1.0.8/src/ros_cdk_memcache/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    49093 2022-07-14 02:31:53.000000 ros-cdk-memcache-1.0.8/src/ros_cdk_memcache/_jsii/ros-cdk-memcache@1.0.8.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:31:53.000000 ros-cdk-memcache-1.0.8/src/ros_cdk_memcache/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:31:53.000000 ros-cdk-memcache-1.0.8/src/ros_cdk_memcache.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1260 2022-07-14 02:31:53.000000 ros-cdk-memcache-1.0.8/src/ros_cdk_memcache.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      450 2022-07-14 02:31:53.000000 ros-cdk-memcache-1.0.8/src/ros_cdk_memcache.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:31:53.000000 ros-cdk-memcache-1.0.8/src/ros_cdk_memcache.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2022-07-14 02:31:53.000000 ros-cdk-memcache-1.0.8/src/ros_cdk_memcache.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2022-07-14 02:31:53.000000 ros-cdk-memcache-1.0.8/src/ros_cdk_memcache.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:22:48.000000 ros-cdk-memcache-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)    10279 2022-09-23 12:22:48.000000 ros-cdk-memcache-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-09-23 12:22:48.000000 ros-cdk-memcache-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2022-09-23 12:22:48.000000 ros-cdk-memcache-1.0.9/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1260 2022-09-23 12:22:48.000000 ros-cdk-memcache-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      194 2022-09-23 12:22:48.000000 ros-cdk-memcache-1.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      236 2022-09-23 12:22:48.000000 ros-cdk-memcache-1.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-09-23 12:22:48.000000 ros-cdk-memcache-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1853 2022-09-23 12:22:48.000000 ros-cdk-memcache-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:22:48.000000 ros-cdk-memcache-1.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:22:48.000000 ros-cdk-memcache-1.0.9/src/ros_cdk_memcache/
+-rw-r--r--   0 root         (0) root         (0)    87260 2022-09-23 12:22:48.000000 ros-cdk-memcache-1.0.9/src/ros_cdk_memcache/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:22:48.000000 ros-cdk-memcache-1.0.9/src/ros_cdk_memcache/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      427 2022-09-23 12:22:48.000000 ros-cdk-memcache-1.0.9/src/ros_cdk_memcache/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    49159 2022-09-23 12:22:48.000000 ros-cdk-memcache-1.0.9/src/ros_cdk_memcache/_jsii/ros-cdk-memcache@1.0.9.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 12:22:48.000000 ros-cdk-memcache-1.0.9/src/ros_cdk_memcache/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:22:48.000000 ros-cdk-memcache-1.0.9/src/ros_cdk_memcache.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1260 2022-09-23 12:22:48.000000 ros-cdk-memcache-1.0.9/src/ros_cdk_memcache.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      450 2022-09-23 12:22:48.000000 ros-cdk-memcache-1.0.9/src/ros_cdk_memcache.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 12:22:48.000000 ros-cdk-memcache-1.0.9/src/ros_cdk_memcache.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2022-09-23 12:22:48.000000 ros-cdk-memcache-1.0.9/src/ros_cdk_memcache.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2022-09-23 12:22:48.000000 ros-cdk-memcache-1.0.9/src/ros_cdk_memcache.egg-info/top_level.txt
```

### Comparing `ros-cdk-memcache-1.0.8/LICENSE` & `ros-cdk-memcache-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-memcache-1.0.8/PKG-INFO` & `ros-cdk-memcache-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-memcache
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS MEMCACHE Construct Library
```

### Comparing `ros-cdk-memcache-1.0.8/setup.py` & `ros-cdk-memcache-1.0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-memcache",
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
         "ros_cdk_memcache",
         "ros_cdk_memcache._jsii"
     ],
     "package_data": {
         "ros_cdk_memcache._jsii": [
-            "ros-cdk-memcache@1.0.8.jsii.tgz"
+            "ros-cdk-memcache@1.0.9.jsii.tgz"
         ],
         "ros_cdk_memcache": [
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

### Comparing `ros-cdk-memcache-1.0.8/src/ros_cdk_memcache/__init__.py` & `ros-cdk-memcache-1.0.9/src/ros_cdk_memcache/__init__.py`

 * *Files 10% similar despite different names*

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
@@ -29,55 +31,61 @@
 ):
     '''A ROS resource type:  ``ALIYUN::Memcache::Instance``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: typing.Optional["InstanceProps"] = None,
+        props: typing.Optional[typing.Union["InstanceProps", typing.Dict[str, typing.Any]]] = None,
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::Memcache::Instance``.
 
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
     @jsii.member(jsii_name="attrConnectionDomain")
     def attr_connection_domain(self) -> ros_cdk_core.IResolvable:
         '''Attribute ConnectionDomain: The internal endpoint of the instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrConnectionDomain"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInstanceId")
     def attr_instance_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute InstanceId: The globally unique identifier (GUID) of the instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInstanceId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInstanceName")
     def attr_instance_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute InstanceName: The name of the instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInstanceName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPort")
     def attr_port(self) -> ros_cdk_core.IResolvable:
         '''Attribute Port: Port of created instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPort"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrQps")
     def attr_qps(self) -> ros_cdk_core.IResolvable:
         '''Attribute QPS: QPS.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrQps"))
 
 
 @jsii.data_type(
@@ -108,15 +116,15 @@
 class InstanceProps:
     def __init__(
         self,
         *,
         auto_renew: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         auto_renew_period: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         auto_use_coupon: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        backup_policy: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosInstance.BackupPolicyProperty"]] = None,
+        backup_policy: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosInstance.BackupPolicyProperty", typing.Dict[str, typing.Any]]]] = None,
         capacity: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         charge_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         config: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         coupon_no: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         instance_class: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         instance_name: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         network_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
@@ -147,14 +155,35 @@
         :param private_ip_address: Property privateIpAddress: The internal IP address of the instance. Note The internal IP address must be located in the Classless Inter-Domain Routing (CIDR) block of the VSwitch to which the instance belongs.
         :param resource_group_id: Property resourceGroupId: Resource group ID.
         :param vpc_id: Property vpcId: The ID of the VPC.
         :param vpc_password_free: Property vpcPasswordFree: Specifies whether to enable password free for access within the VPC. If set to: - true: enables password free. - false: disables password free.
         :param v_switch_id: Property vSwitchId: The ID of the VSwitch.
         :param zone_id: Property zoneId: The ID of the zone in which the instance is created. You can call the DescribeRegions operation to query the latest region list.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(InstanceProps.__init__)
+            check_type(argname="argument auto_renew", value=auto_renew, expected_type=type_hints["auto_renew"])
+            check_type(argname="argument auto_renew_period", value=auto_renew_period, expected_type=type_hints["auto_renew_period"])
+            check_type(argname="argument auto_use_coupon", value=auto_use_coupon, expected_type=type_hints["auto_use_coupon"])
+            check_type(argname="argument backup_policy", value=backup_policy, expected_type=type_hints["backup_policy"])
+            check_type(argname="argument capacity", value=capacity, expected_type=type_hints["capacity"])
+            check_type(argname="argument charge_type", value=charge_type, expected_type=type_hints["charge_type"])
+            check_type(argname="argument config", value=config, expected_type=type_hints["config"])
+            check_type(argname="argument coupon_no", value=coupon_no, expected_type=type_hints["coupon_no"])
+            check_type(argname="argument instance_class", value=instance_class, expected_type=type_hints["instance_class"])
+            check_type(argname="argument instance_name", value=instance_name, expected_type=type_hints["instance_name"])
+            check_type(argname="argument network_type", value=network_type, expected_type=type_hints["network_type"])
+            check_type(argname="argument password", value=password, expected_type=type_hints["password"])
+            check_type(argname="argument period", value=period, expected_type=type_hints["period"])
+            check_type(argname="argument private_ip_address", value=private_ip_address, expected_type=type_hints["private_ip_address"])
+            check_type(argname="argument resource_group_id", value=resource_group_id, expected_type=type_hints["resource_group_id"])
+            check_type(argname="argument vpc_id", value=vpc_id, expected_type=type_hints["vpc_id"])
+            check_type(argname="argument vpc_password_free", value=vpc_password_free, expected_type=type_hints["vpc_password_free"])
+            check_type(argname="argument v_switch_id", value=v_switch_id, expected_type=type_hints["v_switch_id"])
+            check_type(argname="argument zone_id", value=zone_id, expected_type=type_hints["zone_id"])
         self._values: typing.Dict[str, typing.Any] = {}
         if auto_renew is not None:
             self._values["auto_renew"] = auto_renew
         if auto_renew_period is not None:
             self._values["auto_renew_period"] = auto_renew_period
         if auto_use_coupon is not None:
             self._values["auto_use_coupon"] = auto_use_coupon
@@ -443,97 +472,109 @@
 ):
     '''A ROS template type:  ``ALIYUN::Memcache::Instance``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosInstanceProps",
+        props: typing.Union["RosInstanceProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::Memcache::Instance``.
 
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
     @jsii.member(jsii_name="attrConnectionDomain")
     def attr_connection_domain(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ConnectionDomain: The internal endpoint of the instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrConnectionDomain"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInstanceId")
     def attr_instance_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: InstanceId: The globally unique identifier (GUID) of the instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInstanceId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInstanceName")
     def attr_instance_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: InstanceName: The name of the instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInstanceName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPort")
     def attr_port(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Port: Port of created instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPort"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrQps")
     def attr_qps(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: QPS: QPS.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrQps"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosInstance, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="autoRenew")
     def auto_renew(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -545,17 +586,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "autoRenew"))
 
     @auto_renew.setter
     def auto_renew(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "auto_renew").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "autoRenew", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="autoRenewPeriod")
     def auto_renew_period(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -570,17 +614,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "autoRenewPeriod"))
 
     @auto_renew_period.setter
     def auto_renew_period(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "auto_renew_period").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "autoRenewPeriod", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="autoUseCoupon")
     def auto_use_coupon(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -592,34 +639,40 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "autoUseCoupon"))
 
     @auto_use_coupon.setter
     def auto_use_coupon(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "auto_use_coupon").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "autoUseCoupon", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="backupPolicy")
     def backup_policy(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosInstance.BackupPolicyProperty"]]:
         '''
         :Property: backupPolicy: Backup policy
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosInstance.BackupPolicyProperty"]], jsii.get(self, "backupPolicy"))
 
     @backup_policy.setter
     def backup_policy(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosInstance.BackupPolicyProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "backup_policy").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "backupPolicy", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="capacity")
     def capacity(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -630,17 +683,20 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "capacity"))
 
     @capacity.setter
     def capacity(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "capacity").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "capacity", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="chargeType")
     def charge_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -652,17 +708,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "chargeType"))
 
     @charge_type.setter
     def charge_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "charge_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "chargeType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="config")
     def config(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -672,34 +731,40 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "config"))
 
     @config.setter
     def config(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "config").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "config", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="couponNo")
     def coupon_no(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: couponNo: The coupon number. Default value: youhuiquan_promotion_option_id_for_blank.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "couponNo"))
 
     @coupon_no.setter
     def coupon_no(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "coupon_no").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "couponNo", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="instanceClass")
     def instance_class(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -710,17 +775,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "instanceClass"))
 
     @instance_class.setter
     def instance_class(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "instance_class").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "instanceClass", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="instanceName")
     def instance_name(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         ::
 
@@ -734,17 +802,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "instanceName"))
 
     @instance_name.setter
     def instance_name(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "instance_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "instanceName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="networkType")
     def network_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -756,17 +827,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "networkType"))
 
     @network_type.setter
     def network_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "network_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "networkType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="password")
     def password(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         ::
 
@@ -782,17 +856,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "password"))
 
     @password.setter
     def password(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "password").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "password", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="period")
     def period(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -804,17 +881,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "period"))
 
     @period.setter
     def period(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "period").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "period", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="privateIpAddress")
     def private_ip_address(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -825,51 +905,60 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "privateIpAddress"))
 
     @private_ip_address.setter
     def private_ip_address(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "private_ip_address").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "privateIpAddress", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="resourceGroupId")
     def resource_group_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: resourceGroupId: Resource group ID.
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
     @jsii.member(jsii_name="vpcId")
     def vpc_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: vpcId: The ID of the VPC.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "vpcId"))
 
     @vpc_id.setter
     def vpc_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "vpc_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "vpcId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vpcPasswordFree")
     def vpc_password_free(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -881,48 +970,57 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "vpcPasswordFree"))
 
     @vpc_password_free.setter
     def vpc_password_free(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "vpc_password_free").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "vpcPasswordFree", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vSwitchId")
     def v_switch_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: vSwitchId: The ID of the VSwitch.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "vSwitchId"))
 
     @v_switch_id.setter
     def v_switch_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "v_switch_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "vSwitchId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="zoneId")
     def zone_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: zoneId: The ID of the zone in which the instance is created. You can call the DescribeRegions operation to query the latest region list.
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
         jsii_type="@alicloud/ros-cdk-memcache.RosInstance.BackupPolicyProperty",
         jsii_struct_bases=[],
         name_mapping={
             "preferred_backup_period": "preferredBackupPeriod",
@@ -939,14 +1037,19 @@
             enable_backup_log: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param preferred_backup_period: 
             :param preferred_backup_time: 
             :param enable_backup_log: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosInstance.BackupPolicyProperty.__init__)
+                check_type(argname="argument preferred_backup_period", value=preferred_backup_period, expected_type=type_hints["preferred_backup_period"])
+                check_type(argname="argument preferred_backup_time", value=preferred_backup_time, expected_type=type_hints["preferred_backup_time"])
+                check_type(argname="argument enable_backup_log", value=enable_backup_log, expected_type=type_hints["enable_backup_log"])
             self._values: typing.Dict[str, typing.Any] = {
                 "preferred_backup_period": preferred_backup_period,
                 "preferred_backup_time": preferred_backup_time,
             }
             if enable_backup_log is not None:
                 self._values["enable_backup_log"] = enable_backup_log
 
@@ -1026,15 +1129,15 @@
 class RosInstanceProps:
     def __init__(
         self,
         *,
         auto_renew: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         auto_renew_period: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         auto_use_coupon: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        backup_policy: typing.Optional[typing.Union[ros_cdk_core.IResolvable, RosInstance.BackupPolicyProperty]] = None,
+        backup_policy: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosInstance.BackupPolicyProperty, typing.Dict[str, typing.Any]]]] = None,
         capacity: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         charge_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         config: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         coupon_no: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         instance_class: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         instance_name: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         network_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
@@ -1065,14 +1168,35 @@
         :param private_ip_address: 
         :param resource_group_id: 
         :param vpc_id: 
         :param vpc_password_free: 
         :param v_switch_id: 
         :param zone_id: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosInstanceProps.__init__)
+            check_type(argname="argument auto_renew", value=auto_renew, expected_type=type_hints["auto_renew"])
+            check_type(argname="argument auto_renew_period", value=auto_renew_period, expected_type=type_hints["auto_renew_period"])
+            check_type(argname="argument auto_use_coupon", value=auto_use_coupon, expected_type=type_hints["auto_use_coupon"])
+            check_type(argname="argument backup_policy", value=backup_policy, expected_type=type_hints["backup_policy"])
+            check_type(argname="argument capacity", value=capacity, expected_type=type_hints["capacity"])
+            check_type(argname="argument charge_type", value=charge_type, expected_type=type_hints["charge_type"])
+            check_type(argname="argument config", value=config, expected_type=type_hints["config"])
+            check_type(argname="argument coupon_no", value=coupon_no, expected_type=type_hints["coupon_no"])
+            check_type(argname="argument instance_class", value=instance_class, expected_type=type_hints["instance_class"])
+            check_type(argname="argument instance_name", value=instance_name, expected_type=type_hints["instance_name"])
+            check_type(argname="argument network_type", value=network_type, expected_type=type_hints["network_type"])
+            check_type(argname="argument password", value=password, expected_type=type_hints["password"])
+            check_type(argname="argument period", value=period, expected_type=type_hints["period"])
+            check_type(argname="argument private_ip_address", value=private_ip_address, expected_type=type_hints["private_ip_address"])
+            check_type(argname="argument resource_group_id", value=resource_group_id, expected_type=type_hints["resource_group_id"])
+            check_type(argname="argument vpc_id", value=vpc_id, expected_type=type_hints["vpc_id"])
+            check_type(argname="argument vpc_password_free", value=vpc_password_free, expected_type=type_hints["vpc_password_free"])
+            check_type(argname="argument v_switch_id", value=v_switch_id, expected_type=type_hints["v_switch_id"])
+            check_type(argname="argument zone_id", value=zone_id, expected_type=type_hints["zone_id"])
         self._values: typing.Dict[str, typing.Any] = {}
         if auto_renew is not None:
             self._values["auto_renew"] = auto_renew
         if auto_renew_period is not None:
             self._values["auto_renew_period"] = auto_renew_period
         if auto_use_coupon is not None:
             self._values["auto_use_coupon"] = auto_use_coupon
@@ -1387,142 +1511,166 @@
 ):
     '''A ROS template type:  ``ALIYUN::Memcache::Whitelist``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosWhitelistProps",
+        props: typing.Union["RosWhitelistProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::Memcache::Whitelist``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosWhitelist.__init__)
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
+            type_hints = typing.get_type_hints(RosWhitelist._render_properties)
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
     @jsii.member(jsii_name="attrSecurityIpGroupAttribute")
     def attr_security_ip_group_attribute(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: SecurityIpGroupAttribute: The default is empty. For distinguishing between different attribute values, the console will not display the value of hidden whitelist packet.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrSecurityIpGroupAttribute"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrSecurityIpGroupName")
     def attr_security_ip_group_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: SecurityIpGroupName: Whitelist group
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrSecurityIpGroupName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrSecurityIps")
     def attr_security_ips(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: SecurityIps: IP address whitelist to be modified
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrSecurityIps"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosWhitelist, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="instanceId")
     def instance_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: instanceId: Instance ID (globally unique)
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "instanceId"))
 
     @instance_id.setter
     def instance_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosWhitelist, "instance_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "instanceId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="securityIps")
     def security_ips(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: securityIps: IP address whitelist to be modified
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "securityIps"))
 
     @security_ips.setter
     def security_ips(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosWhitelist, "security_ips").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "securityIps", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="securityIpGroupAttribute")
     def security_ip_group_attribute(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: securityIpGroupAttribute: The default is empty. For distinguishing between different attribute values, the console will not display the value of hidden whitelist packet.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "securityIpGroupAttribute"))
 
     @security_ip_group_attribute.setter
     def security_ip_group_attribute(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosWhitelist, "security_ip_group_attribute").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "securityIpGroupAttribute", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="securityIpGroupName")
     def security_ip_group_name(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: securityIpGroupName: Whitelist group
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "securityIpGroupName"))
 
     @security_ip_group_name.setter
     def security_ip_group_name(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosWhitelist, "security_ip_group_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "securityIpGroupName", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-memcache.RosWhitelistProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -1544,14 +1692,20 @@
         '''Properties for defining a ``ALIYUN::Memcache::Whitelist``.
 
         :param instance_id: 
         :param security_ips: 
         :param security_ip_group_attribute: 
         :param security_ip_group_name: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosWhitelistProps.__init__)
+            check_type(argname="argument instance_id", value=instance_id, expected_type=type_hints["instance_id"])
+            check_type(argname="argument security_ips", value=security_ips, expected_type=type_hints["security_ips"])
+            check_type(argname="argument security_ip_group_attribute", value=security_ip_group_attribute, expected_type=type_hints["security_ip_group_attribute"])
+            check_type(argname="argument security_ip_group_name", value=security_ip_group_name, expected_type=type_hints["security_ip_group_name"])
         self._values: typing.Dict[str, typing.Any] = {
             "instance_id": instance_id,
             "security_ips": security_ips,
         }
         if security_ip_group_attribute is not None:
             self._values["security_ip_group_attribute"] = security_ip_group_attribute
         if security_ip_group_name is not None:
@@ -1614,46 +1768,52 @@
 ):
     '''A ROS resource type:  ``ALIYUN::Memcache::Whitelist``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "WhitelistProps",
+        props: typing.Union["WhitelistProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::Memcache::Whitelist``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(Whitelist.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrSecurityIpGroupAttribute")
     def attr_security_ip_group_attribute(self) -> ros_cdk_core.IResolvable:
         '''Attribute SecurityIpGroupAttribute: The default is empty.
 
         For distinguishing between different attribute values, the console will not display the value of hidden whitelist packet.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrSecurityIpGroupAttribute"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrSecurityIpGroupName")
     def attr_security_ip_group_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute SecurityIpGroupName: Whitelist group.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrSecurityIpGroupName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrSecurityIps")
     def attr_security_ips(self) -> ros_cdk_core.IResolvable:
         '''Attribute SecurityIps: IP address whitelist to be modified.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrSecurityIps"))
 
 
 @jsii.data_type(
@@ -1678,14 +1838,20 @@
         '''Properties for defining a ``ALIYUN::Memcache::Whitelist``.
 
         :param instance_id: Property instanceId: Instance ID (globally unique).
         :param security_ips: Property securityIps: IP address whitelist to be modified.
         :param security_ip_group_attribute: Property securityIpGroupAttribute: The default is empty. For distinguishing between different attribute values, the console will not display the value of hidden whitelist packet.
         :param security_ip_group_name: Property securityIpGroupName: Whitelist group.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(WhitelistProps.__init__)
+            check_type(argname="argument instance_id", value=instance_id, expected_type=type_hints["instance_id"])
+            check_type(argname="argument security_ips", value=security_ips, expected_type=type_hints["security_ips"])
+            check_type(argname="argument security_ip_group_attribute", value=security_ip_group_attribute, expected_type=type_hints["security_ip_group_attribute"])
+            check_type(argname="argument security_ip_group_name", value=security_ip_group_name, expected_type=type_hints["security_ip_group_name"])
         self._values: typing.Dict[str, typing.Any] = {
             "instance_id": instance_id,
             "security_ips": security_ips,
         }
         if security_ip_group_attribute is not None:
             self._values["security_ip_group_attribute"] = security_ip_group_attribute
         if security_ip_group_name is not None:
```

### Comparing `ros-cdk-memcache-1.0.8/src/ros_cdk_memcache.egg-info/PKG-INFO` & `ros-cdk-memcache-1.0.9/src/ros_cdk_memcache.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-memcache
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS MEMCACHE Construct Library
```

