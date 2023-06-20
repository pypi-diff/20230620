# Comparing `tmp/ros-cdk-cloudphone-1.0.8.tar.gz` & `tmp/ros-cdk-cloudphone-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-cloudphone-1.0.8.tar", last modified: Thu Jul 14 02:25:48 2022, max compression
+gzip compressed data, was "dist/ros-cdk-cloudphone-1.0.9.tar", last modified: Fri Sep 23 11:00:12 2022, max compression
```

## Comparing `ros-cdk-cloudphone-1.0.8.tar` & `ros-cdk-cloudphone-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:25:48.000000 ros-cdk-cloudphone-1.0.8/
--rw-r--r--   0 root         (0) root         (0)    10279 2022-07-14 02:25:48.000000 ros-cdk-cloudphone-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2022-07-14 02:25:48.000000 ros-cdk-cloudphone-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2022-07-14 02:25:48.000000 ros-cdk-cloudphone-1.0.8/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1268 2022-07-14 02:25:48.000000 ros-cdk-cloudphone-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      200 2022-07-14 02:25:48.000000 ros-cdk-cloudphone-1.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)      106 2022-07-14 02:25:48.000000 ros-cdk-cloudphone-1.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-07-14 02:25:48.000000 ros-cdk-cloudphone-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1836 2022-07-14 02:25:48.000000 ros-cdk-cloudphone-1.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:25:48.000000 ros-cdk-cloudphone-1.0.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:25:48.000000 ros-cdk-cloudphone-1.0.8/src/ros_cdk_cloudphone/
--rw-r--r--   0 root         (0) root         (0)    45200 2022-07-14 02:25:48.000000 ros-cdk-cloudphone-1.0.8/src/ros_cdk_cloudphone/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:25:48.000000 ros-cdk-cloudphone-1.0.8/src/ros_cdk_cloudphone/_jsii/
--rw-r--r--   0 root         (0) root         (0)      397 2022-07-14 02:25:48.000000 ros-cdk-cloudphone-1.0.8/src/ros_cdk_cloudphone/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    39001 2022-07-14 02:25:48.000000 ros-cdk-cloudphone-1.0.8/src/ros_cdk_cloudphone/_jsii/ros-cdk-cloudphone@1.0.8.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:25:48.000000 ros-cdk-cloudphone-1.0.8/src/ros_cdk_cloudphone/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:25:48.000000 ros-cdk-cloudphone-1.0.8/src/ros_cdk_cloudphone.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1268 2022-07-14 02:25:48.000000 ros-cdk-cloudphone-1.0.8/src/ros_cdk_cloudphone.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      470 2022-07-14 02:25:48.000000 ros-cdk-cloudphone-1.0.8/src/ros_cdk_cloudphone.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:25:48.000000 ros-cdk-cloudphone-1.0.8/src/ros_cdk_cloudphone.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2022-07-14 02:25:48.000000 ros-cdk-cloudphone-1.0.8/src/ros_cdk_cloudphone.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2022-07-14 02:25:48.000000 ros-cdk-cloudphone-1.0.8/src/ros_cdk_cloudphone.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:00:12.000000 ros-cdk-cloudphone-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)    10279 2022-09-23 11:00:11.000000 ros-cdk-cloudphone-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-09-23 11:00:11.000000 ros-cdk-cloudphone-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2022-09-23 11:00:11.000000 ros-cdk-cloudphone-1.0.9/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1268 2022-09-23 11:00:12.000000 ros-cdk-cloudphone-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      200 2022-09-23 11:00:11.000000 ros-cdk-cloudphone-1.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      236 2022-09-23 11:00:11.000000 ros-cdk-cloudphone-1.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-09-23 11:00:12.000000 ros-cdk-cloudphone-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1865 2022-09-23 11:00:11.000000 ros-cdk-cloudphone-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:00:12.000000 ros-cdk-cloudphone-1.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:00:12.000000 ros-cdk-cloudphone-1.0.9/src/ros_cdk_cloudphone/
+-rw-r--r--   0 root         (0) root         (0)    53974 2022-09-23 11:00:11.000000 ros-cdk-cloudphone-1.0.9/src/ros_cdk_cloudphone/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:00:12.000000 ros-cdk-cloudphone-1.0.9/src/ros_cdk_cloudphone/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      431 2022-09-23 11:00:11.000000 ros-cdk-cloudphone-1.0.9/src/ros_cdk_cloudphone/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    39776 2022-09-23 11:00:11.000000 ros-cdk-cloudphone-1.0.9/src/ros_cdk_cloudphone/_jsii/ros-cdk-cloudphone@1.0.9.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 11:00:11.000000 ros-cdk-cloudphone-1.0.9/src/ros_cdk_cloudphone/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:00:12.000000 ros-cdk-cloudphone-1.0.9/src/ros_cdk_cloudphone.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1268 2022-09-23 11:00:12.000000 ros-cdk-cloudphone-1.0.9/src/ros_cdk_cloudphone.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      470 2022-09-23 11:00:12.000000 ros-cdk-cloudphone-1.0.9/src/ros_cdk_cloudphone.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 11:00:12.000000 ros-cdk-cloudphone-1.0.9/src/ros_cdk_cloudphone.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2022-09-23 11:00:12.000000 ros-cdk-cloudphone-1.0.9/src/ros_cdk_cloudphone.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2022-09-23 11:00:12.000000 ros-cdk-cloudphone-1.0.9/src/ros_cdk_cloudphone.egg-info/top_level.txt
```

### Comparing `ros-cdk-cloudphone-1.0.8/LICENSE` & `ros-cdk-cloudphone-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-cloudphone-1.0.8/PKG-INFO` & `ros-cdk-cloudphone-1.0.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-cloudphone
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS CLOUDPHONE Construct Library
```

### Comparing `ros-cdk-cloudphone-1.0.8/setup.py` & `ros-cdk-cloudphone-1.0.9/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-cloudphone",
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
         "ros_cdk_cloudphone",
         "ros_cdk_cloudphone._jsii"
     ],
     "package_data": {
         "ros_cdk_cloudphone._jsii": [
-            "ros-cdk-cloudphone@1.0.8.jsii.tgz"
+            "ros-cdk-cloudphone@1.0.9.jsii.tgz"
         ],
         "ros_cdk_cloudphone": [
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

### Comparing `ros-cdk-cloudphone-1.0.8/src/ros_cdk_cloudphone/__init__.py` & `ros-cdk-cloudphone-1.0.9/src/ros_cdk_cloudphone/__init__.py`

 * *Files 20% similar despite different names*

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
 
 
 class InstanceGroup(
     ros_cdk_core.Resource,
@@ -29,43 +31,49 @@
 ):
     '''A ROS resource type:  ``ALIYUN::CloudPhone::InstanceGroup``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "InstanceGroupProps",
+        props: typing.Union["InstanceGroupProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::CloudPhone::InstanceGroup``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(InstanceGroup.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInstanceIds")
     def attr_instance_ids(self) -> ros_cdk_core.IResolvable:
         '''Attribute InstanceIds: instance ids.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInstanceIds"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrOrderId")
     def attr_order_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute OrderId: oder id.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrOrderId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTradePrice")
     def attr_trade_price(self) -> ros_cdk_core.IResolvable:
         '''Attribute TradePrice: price.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTradePrice"))
 
 
 @jsii.data_type(
@@ -104,15 +112,15 @@
         charge_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         description: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         eip_bandwidth: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         instance_name: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         key_pair_name: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         period: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         resolution: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        tag: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, ros_cdk_core.RosTag]]]] = None,
+        tag: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[ros_cdk_core.RosTag, typing.Dict[str, typing.Any]]]]]] = None,
         vnc_password: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::CloudPhone::InstanceGroup``.
 
         :param image_id: Property imageId: The image id.
         :param instance_type: Property instanceType: instance type.
         :param security_group_id: Property securityGroupId: Security group to create ecs instance. For classic instance need the security group not belong to VPC, for VPC instance, please make sure the security group belong to specified VPC.
@@ -126,14 +134,32 @@
         :param instance_name: Property instanceName: "Display name of the instance, [2, 128] English or Chinese characters, must start with a letter or Chinese in size, can contain numbers, "_" or ".", "-".
         :param key_pair_name: Property keyPairName: Cloud phone instance key pair name. The cloud phone key can be imported through the ImportKeyPair interface.
         :param period: Property period: Prepaid time period. While PeriodUnit is month, it could be 1, 2, 3, 6. While PeriodUnit is year, it could be from 1 to 5Default value is 1.
         :param resolution: Property resolution: You can use the DescribeInstanceTypes interface to query the list of resolutions supported by the current specification and select an appropriate resolution.
         :param tag: Property tag: Tags to attach to instance. Max support 20 tags to add during create instance. Each tag with two properties Key and Value, and Key is required.
         :param vnc_password: Property vncPassword: Cloud phone VNC password. The password must be six characters long, and must contain only uppercase, lowercase English letters and Arabic numerals.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(InstanceGroupProps.__init__)
+            check_type(argname="argument image_id", value=image_id, expected_type=type_hints["image_id"])
+            check_type(argname="argument instance_type", value=instance_type, expected_type=type_hints["instance_type"])
+            check_type(argname="argument security_group_id", value=security_group_id, expected_type=type_hints["security_group_id"])
+            check_type(argname="argument v_switch_id", value=v_switch_id, expected_type=type_hints["v_switch_id"])
+            check_type(argname="argument amount", value=amount, expected_type=type_hints["amount"])
+            check_type(argname="argument auto_pay", value=auto_pay, expected_type=type_hints["auto_pay"])
+            check_type(argname="argument auto_renew", value=auto_renew, expected_type=type_hints["auto_renew"])
+            check_type(argname="argument charge_type", value=charge_type, expected_type=type_hints["charge_type"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument eip_bandwidth", value=eip_bandwidth, expected_type=type_hints["eip_bandwidth"])
+            check_type(argname="argument instance_name", value=instance_name, expected_type=type_hints["instance_name"])
+            check_type(argname="argument key_pair_name", value=key_pair_name, expected_type=type_hints["key_pair_name"])
+            check_type(argname="argument period", value=period, expected_type=type_hints["period"])
+            check_type(argname="argument resolution", value=resolution, expected_type=type_hints["resolution"])
+            check_type(argname="argument tag", value=tag, expected_type=type_hints["tag"])
+            check_type(argname="argument vnc_password", value=vnc_password, expected_type=type_hints["vnc_password"])
         self._values: typing.Dict[str, typing.Any] = {
             "image_id": image_id,
             "instance_type": instance_type,
             "security_group_id": security_group_id,
             "v_switch_id": v_switch_id,
         }
         if amount is not None:
@@ -335,141 +361,165 @@
 ):
     '''A ROS template type:  ``ALIYUN::CloudPhone::InstanceGroup``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosInstanceGroupProps",
+        props: typing.Union["RosInstanceGroupProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::CloudPhone::InstanceGroup``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosInstanceGroup.__init__)
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
+            type_hints = typing.get_type_hints(RosInstanceGroup._render_properties)
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
         :Attribute: InstanceIds: instance ids
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInstanceIds"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrOrderId")
     def attr_order_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: OrderId: oder id
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrOrderId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTradePrice")
     def attr_trade_price(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: TradePrice: price
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTradePrice"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosInstanceGroup, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="imageId")
     def image_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: imageId: The image id
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "imageId"))
 
     @image_id.setter
     def image_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstanceGroup, "image_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "imageId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="instanceType")
     def instance_type(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: instanceType: instance type
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "instanceType"))
 
     @instance_type.setter
     def instance_type(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstanceGroup, "instance_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "instanceType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="securityGroupId")
     def security_group_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: securityGroupId: Security group to create ecs instance. For classic instance need the security group not belong to VPC, for VPC instance, please make sure the security group belong to specified VPC.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "securityGroupId"))
 
     @security_group_id.setter
     def security_group_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstanceGroup, "security_group_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "securityGroupId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vSwitchId")
     def v_switch_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: vSwitchId: vswitch id
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "vSwitchId"))
 
     @v_switch_id.setter
     def v_switch_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstanceGroup, "v_switch_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "vSwitchId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="amount")
     def amount(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -479,34 +529,40 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "amount"))
 
     @amount.setter
     def amount(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstanceGroup, "amount").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "amount", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="autoPay")
     def auto_pay(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property: autoPay: Whether to pay automatically, the default is true
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "autoPay"))
 
     @auto_pay.setter
     def auto_pay(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstanceGroup, "auto_pay").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "autoPay", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="autoRenew")
     def auto_renew(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -518,34 +574,40 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "autoRenew"))
 
     @auto_renew.setter
     def auto_renew(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstanceGroup, "auto_renew").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "autoRenew", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="chargeType")
     def charge_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: chargeType: Instance internet access charge type.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "chargeType"))
 
     @charge_type.setter
     def charge_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstanceGroup, "charge_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "chargeType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="description")
     def description(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -555,17 +617,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "description"))
 
     @description.setter
     def description(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstanceGroup, "description").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "description", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="eipBandwidth")
     def eip_bandwidth(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -578,17 +643,20 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "eipBandwidth"))
 
     @eip_bandwidth.setter
     def eip_bandwidth(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstanceGroup, "eip_bandwidth").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "eipBandwidth", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="instanceName")
     def instance_name(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -598,17 +666,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "instanceName"))
 
     @instance_name.setter
     def instance_name(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstanceGroup, "instance_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "instanceName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="keyPairName")
     def key_pair_name(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -618,17 +689,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "keyPairName"))
 
     @key_pair_name.setter
     def key_pair_name(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstanceGroup, "key_pair_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "keyPairName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="period")
     def period(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -638,17 +712,20 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "period"))
 
     @period.setter
     def period(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstanceGroup, "period").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "period", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="resolution")
     def resolution(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -658,34 +735,40 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "resolution"))
 
     @resolution.setter
     def resolution(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstanceGroup, "resolution").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "resolution", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="tag")
     def tag(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, ros_cdk_core.RosTag]]]]:
         '''
         :Property: tag: Tags to attach to instance. Max support 20 tags to add during create instance. Each tag with two properties Key and Value, and Key is required.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, ros_cdk_core.RosTag]]]], jsii.get(self, "tag"))
 
     @tag.setter
     def tag(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, ros_cdk_core.RosTag]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstanceGroup, "tag").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "tag", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vncPassword")
     def vnc_password(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -696,14 +779,17 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "vncPassword"))
 
     @vnc_password.setter
     def vnc_password(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstanceGroup, "vnc_password").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "vncPassword", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-cloudphone.RosInstanceGroup.TagProperty",
         jsii_struct_bases=[],
         name_mapping={"key": "key", "value": "value"},
     )
@@ -714,14 +800,18 @@
             key: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param key: 
             :param value: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosInstanceGroup.TagProperty.__init__)
+                check_type(argname="argument key", value=key, expected_type=type_hints["key"])
+                check_type(argname="argument value", value=value, expected_type=type_hints["value"])
             self._values: typing.Dict[str, typing.Any] = {
                 "key": key,
             }
             if value is not None:
                 self._values["value"] = value
 
         @builtins.property
@@ -791,15 +881,15 @@
         charge_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         description: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         eip_bandwidth: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         instance_name: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         key_pair_name: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         period: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         resolution: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        tag: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, ros_cdk_core.RosTag]]]] = None,
+        tag: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[ros_cdk_core.RosTag, typing.Dict[str, typing.Any]]]]]] = None,
         vnc_password: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::CloudPhone::InstanceGroup``.
 
         :param image_id: 
         :param instance_type: 
         :param security_group_id: 
@@ -813,14 +903,32 @@
         :param instance_name: 
         :param key_pair_name: 
         :param period: 
         :param resolution: 
         :param tag: 
         :param vnc_password: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosInstanceGroupProps.__init__)
+            check_type(argname="argument image_id", value=image_id, expected_type=type_hints["image_id"])
+            check_type(argname="argument instance_type", value=instance_type, expected_type=type_hints["instance_type"])
+            check_type(argname="argument security_group_id", value=security_group_id, expected_type=type_hints["security_group_id"])
+            check_type(argname="argument v_switch_id", value=v_switch_id, expected_type=type_hints["v_switch_id"])
+            check_type(argname="argument amount", value=amount, expected_type=type_hints["amount"])
+            check_type(argname="argument auto_pay", value=auto_pay, expected_type=type_hints["auto_pay"])
+            check_type(argname="argument auto_renew", value=auto_renew, expected_type=type_hints["auto_renew"])
+            check_type(argname="argument charge_type", value=charge_type, expected_type=type_hints["charge_type"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument eip_bandwidth", value=eip_bandwidth, expected_type=type_hints["eip_bandwidth"])
+            check_type(argname="argument instance_name", value=instance_name, expected_type=type_hints["instance_name"])
+            check_type(argname="argument key_pair_name", value=key_pair_name, expected_type=type_hints["key_pair_name"])
+            check_type(argname="argument period", value=period, expected_type=type_hints["period"])
+            check_type(argname="argument resolution", value=resolution, expected_type=type_hints["resolution"])
+            check_type(argname="argument tag", value=tag, expected_type=type_hints["tag"])
+            check_type(argname="argument vnc_password", value=vnc_password, expected_type=type_hints["vnc_password"])
         self._values: typing.Dict[str, typing.Any] = {
             "image_id": image_id,
             "instance_type": instance_type,
             "security_group_id": security_group_id,
             "v_switch_id": v_switch_id,
         }
         if amount is not None:
```

### Comparing `ros-cdk-cloudphone-1.0.8/src/ros_cdk_cloudphone.egg-info/PKG-INFO` & `ros-cdk-cloudphone-1.0.9/src/ros_cdk_cloudphone.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-cloudphone
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS CLOUDPHONE Construct Library
```

