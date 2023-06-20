# Comparing `tmp/ros-cdk-iot-1.0.8.tar.gz` & `tmp/ros-cdk-iot-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-iot-1.0.8.tar", last modified: Thu Jul 14 02:16:08 2022, max compression
+gzip compressed data, was "dist/ros-cdk-iot-1.0.9.tar", last modified: Fri Sep 23 11:54:25 2022, max compression
```

## Comparing `ros-cdk-iot-1.0.8.tar` & `ros-cdk-iot-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:16:08.000000 ros-cdk-iot-1.0.8/
--rw-r--r--   0 root         (0) root         (0)    10279 2022-07-14 02:16:08.000000 ros-cdk-iot-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2022-07-14 02:16:08.000000 ros-cdk-iot-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2022-07-14 02:16:08.000000 ros-cdk-iot-1.0.8/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1240 2022-07-14 02:16:08.000000 ros-cdk-iot-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      179 2022-07-14 02:16:08.000000 ros-cdk-iot-1.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)      106 2022-07-14 02:16:08.000000 ros-cdk-iot-1.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-07-14 02:16:08.000000 ros-cdk-iot-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1794 2022-07-14 02:16:08.000000 ros-cdk-iot-1.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:16:08.000000 ros-cdk-iot-1.0.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:16:08.000000 ros-cdk-iot-1.0.8/src/ros_cdk_iot/
--rw-r--r--   0 root         (0) root         (0)   178741 2022-07-14 02:16:08.000000 ros-cdk-iot-1.0.8/src/ros_cdk_iot/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:16:08.000000 ros-cdk-iot-1.0.8/src/ros_cdk_iot/_jsii/
--rw-r--r--   0 root         (0) root         (0)      370 2022-07-14 02:16:08.000000 ros-cdk-iot-1.0.8/src/ros_cdk_iot/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    85044 2022-07-14 02:16:08.000000 ros-cdk-iot-1.0.8/src/ros_cdk_iot/_jsii/ros-cdk-iot@1.0.8.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:16:08.000000 ros-cdk-iot-1.0.8/src/ros_cdk_iot/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:16:08.000000 ros-cdk-iot-1.0.8/src/ros_cdk_iot.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1240 2022-07-14 02:16:08.000000 ros-cdk-iot-1.0.8/src/ros_cdk_iot.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      400 2022-07-14 02:16:08.000000 ros-cdk-iot-1.0.8/src/ros_cdk_iot.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:16:08.000000 ros-cdk-iot-1.0.8/src/ros_cdk_iot.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2022-07-14 02:16:08.000000 ros-cdk-iot-1.0.8/src/ros_cdk_iot.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2022-07-14 02:16:08.000000 ros-cdk-iot-1.0.8/src/ros_cdk_iot.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:54:25.000000 ros-cdk-iot-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)    10279 2022-09-23 11:54:25.000000 ros-cdk-iot-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-09-23 11:54:25.000000 ros-cdk-iot-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2022-09-23 11:54:25.000000 ros-cdk-iot-1.0.9/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1240 2022-09-23 11:54:25.000000 ros-cdk-iot-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      179 2022-09-23 11:54:25.000000 ros-cdk-iot-1.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      236 2022-09-23 11:54:25.000000 ros-cdk-iot-1.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-09-23 11:54:25.000000 ros-cdk-iot-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1823 2022-09-23 11:54:25.000000 ros-cdk-iot-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:54:25.000000 ros-cdk-iot-1.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:54:25.000000 ros-cdk-iot-1.0.9/src/ros_cdk_iot/
+-rw-r--r--   0 root         (0) root         (0)   208372 2022-09-23 11:54:25.000000 ros-cdk-iot-1.0.9/src/ros_cdk_iot/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:54:25.000000 ros-cdk-iot-1.0.9/src/ros_cdk_iot/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      404 2022-09-23 11:54:25.000000 ros-cdk-iot-1.0.9/src/ros_cdk_iot/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    85125 2022-09-23 11:54:25.000000 ros-cdk-iot-1.0.9/src/ros_cdk_iot/_jsii/ros-cdk-iot@1.0.9.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 11:54:25.000000 ros-cdk-iot-1.0.9/src/ros_cdk_iot/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:54:25.000000 ros-cdk-iot-1.0.9/src/ros_cdk_iot.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1240 2022-09-23 11:54:25.000000 ros-cdk-iot-1.0.9/src/ros_cdk_iot.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      400 2022-09-23 11:54:25.000000 ros-cdk-iot-1.0.9/src/ros_cdk_iot.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 11:54:25.000000 ros-cdk-iot-1.0.9/src/ros_cdk_iot.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2022-09-23 11:54:25.000000 ros-cdk-iot-1.0.9/src/ros_cdk_iot.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2022-09-23 11:54:25.000000 ros-cdk-iot-1.0.9/src/ros_cdk_iot.egg-info/top_level.txt
```

### Comparing `ros-cdk-iot-1.0.8/LICENSE` & `ros-cdk-iot-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-iot-1.0.8/PKG-INFO` & `ros-cdk-iot-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-iot
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS IOT Construct Library
```

### Comparing `ros-cdk-iot-1.0.8/setup.py` & `ros-cdk-iot-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-iot",
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
         "ros_cdk_iot",
         "ros_cdk_iot._jsii"
     ],
     "package_data": {
         "ros_cdk_iot._jsii": [
-            "ros-cdk-iot@1.0.8.jsii.tgz"
+            "ros-cdk-iot@1.0.9.jsii.tgz"
         ],
         "ros_cdk_iot": [
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

### Comparing `ros-cdk-iot-1.0.8/src/ros_cdk_iot/__init__.py` & `ros-cdk-iot-1.0.9/src/ros_cdk_iot/__init__.py`

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
 
 
 class Device(
     ros_cdk_core.Resource,
@@ -29,82 +31,88 @@
 ):
     '''A ROS resource type:  ``ALIYUN::IOT::Device``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "DeviceProps",
+        props: typing.Union["DeviceProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::IOT::Device``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(Device.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDeviceName")
     def attr_device_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute DeviceName: Device name.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDeviceName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDeviceSecret")
     def attr_device_secret(self) -> ros_cdk_core.IResolvable:
         '''Attribute DeviceSecret: Device key.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDeviceSecret"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrIotId")
     def attr_iot_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute IotId: Things internet device ID issued for the device, as the unique identifier of the device.
 
         Description Keep, do not leak.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrIotId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrIotInstanceId")
     def attr_iot_instance_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute IotInstanceId: IOT instance ID.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrIotInstanceId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrIpAddress")
     def attr_ip_address(self) -> ros_cdk_core.IResolvable:
         '''Attribute IpAddress: IP address.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrIpAddress"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrNickName")
     def attr_nick_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute NickName: Nick name.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrNickName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrNodeType")
     def attr_node_type(self) -> ros_cdk_core.IResolvable:
         '''Attribute NodeType: Node type.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrNodeType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrProductKey")
     def attr_product_key(self) -> ros_cdk_core.IResolvable:
         '''Attribute ProductKey: Product key.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrProductKey"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrProductName")
     def attr_product_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute ProductName: Product name.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrProductName"))
 
 
 class DeviceGroup(
@@ -114,37 +122,43 @@
 ):
     '''A ROS resource type:  ``ALIYUN::IOT::DeviceGroup``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "DeviceGroupProps",
+        props: typing.Union["DeviceGroupProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::IOT::DeviceGroup``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(DeviceGroup.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrGroupId")
     def attr_group_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute GroupId: Packet, ID, System for the globally unique identifier generated packet.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrGroupId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrIotInstanceId")
     def attr_iot_instance_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute IotInstanceId: IOT instance ID.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrIotInstanceId"))
 
 
 @jsii.data_type(
@@ -169,14 +183,20 @@
         '''Properties for defining a ``ALIYUN::IOT::DeviceGroup``.
 
         :param group_name: Property groupName: The name of the group. The name can contain Chinese characters, English letters, digits, and underscores (_). The length must be 4 to 30 characters (a Chinese character counts as two characters).
         :param group_desc: Property groupDesc: The description of the group. You can enter a description with up to 100 characters.
         :param iot_instance_id: Property iotInstanceId: Public instance does not pass this parameter; instance that you need to buy the incoming instance ID.
         :param super_group_id: Property superGroupId: The ID of the parent group. If you want to create a first-level group, do not enter this parameter.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(DeviceGroupProps.__init__)
+            check_type(argname="argument group_name", value=group_name, expected_type=type_hints["group_name"])
+            check_type(argname="argument group_desc", value=group_desc, expected_type=type_hints["group_desc"])
+            check_type(argname="argument iot_instance_id", value=iot_instance_id, expected_type=type_hints["iot_instance_id"])
+            check_type(argname="argument super_group_id", value=super_group_id, expected_type=type_hints["super_group_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "group_name": group_name,
         }
         if group_desc is not None:
             self._values["group_desc"] = group_desc
         if iot_instance_id is not None:
             self._values["iot_instance_id"] = iot_instance_id
@@ -266,14 +286,22 @@
         :param product_key: Property productKey: The identifier of the product to which the device to be registered belongs.
         :param dev_eui: Property devEui: DevEUI LoRaWAN equipment. When you create a LoRaWAN devices, this will pass.
         :param device_name: Property deviceName: The name of the device that you want to register. The device name must consist of 4 to 32 characters, including English letters, digits, and special characters, for example, hyphens (-), underscores (_), at signs (@), periods (.) , and colons (:). DeviceName is used with ProductKey to identify a specified device. Note If you do not specify this parameter, the system will generate a name for the device.
         :param iot_instance_id: Property iotInstanceId: Public instance does not pass this parameter; instance that you need to buy the incoming instance ID.
         :param nickname: Property nickname: Add a nickname for the device. A nickname can be 4-64 characters in length, and can contain Chinese characters, English letters, numbers and underscores (_). A Chinese character counts as two characters.
         :param pin_code: Property pinCode: PIN Code LoRaWAN device for checking the legitimacy of DevEUI. When you create a LoRaWAN devices, this will pass.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(DeviceProps.__init__)
+            check_type(argname="argument product_key", value=product_key, expected_type=type_hints["product_key"])
+            check_type(argname="argument dev_eui", value=dev_eui, expected_type=type_hints["dev_eui"])
+            check_type(argname="argument device_name", value=device_name, expected_type=type_hints["device_name"])
+            check_type(argname="argument iot_instance_id", value=iot_instance_id, expected_type=type_hints["iot_instance_id"])
+            check_type(argname="argument nickname", value=nickname, expected_type=type_hints["nickname"])
+            check_type(argname="argument pin_code", value=pin_code, expected_type=type_hints["pin_code"])
         self._values: typing.Dict[str, typing.Any] = {
             "product_key": product_key,
         }
         if dev_eui is not None:
             self._values["dev_eui"] = dev_eui
         if device_name is not None:
             self._values["device_name"] = device_name
@@ -371,37 +399,43 @@
 ):
     '''A ROS resource type:  ``ALIYUN::IOT::Product``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "ProductProps",
+        props: typing.Union["ProductProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::IOT::Product``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(Product.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrIotInstanceId")
     def attr_iot_instance_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute IotInstanceId: IOT instance ID.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrIotInstanceId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrProductKey")
     def attr_product_key(self) -> ros_cdk_core.IResolvable:
         '''Attribute ProductKey: The globally unique identifier of the product issued by IoT Platform.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrProductKey"))
 
 
 @jsii.data_type(
@@ -456,14 +490,30 @@
         :param iot_instance_id: Property iotInstanceId: Public instance does not pass this parameter; instance that you need to buy the incoming instance ID.
         :param join_permission_id: Property joinPermissionId: LoRaWAN network credential ID. When networking mode NetType chosen LORA, the necessary parameters. Please call QueryLoRaJoinPermissions query JoinPermissionId network credentials LoRaWAN under your account. If you do not LoRaWAN network credentials, visit the network management platform to create things together.
         :param net_type: Property netType: Networking mode. Set this parameter only if you are creating a product whose devices directly connect to IoT Platform. Options: WIFI CELLULAR ETHERNET OTHER The default value is WIFI.
         :param protocol_type: Property protocolType: The protocol that devices of this product use to connect to gateways. Set this parameter only if you are creating a product whose devices will be connected to gateways. Options: modbus: Modbus. opc-ua: OPC UA. customize: Customized protocol. ble: BLE. zigbee: ZigBee.
         :param publish_auto: Property publishAuto: Whether to automatically model publication after the product is created. true: publishing. false: not released. This parameter is not passed, the default value true.
         :param resource_group_id: Property resourceGroupId: Resource group ID (group ID to view the resource in the resource management console), specify the product is classified as a resource group. If this parameter is passed, the product will be classified as a default resource group.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(ProductProps.__init__)
+            check_type(argname="argument node_type", value=node_type, expected_type=type_hints["node_type"])
+            check_type(argname="argument product_name", value=product_name, expected_type=type_hints["product_name"])
+            check_type(argname="argument aliyun_commodity_code", value=aliyun_commodity_code, expected_type=type_hints["aliyun_commodity_code"])
+            check_type(argname="argument auth_type", value=auth_type, expected_type=type_hints["auth_type"])
+            check_type(argname="argument category_key", value=category_key, expected_type=type_hints["category_key"])
+            check_type(argname="argument data_format", value=data_format, expected_type=type_hints["data_format"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument id2", value=id2, expected_type=type_hints["id2"])
+            check_type(argname="argument iot_instance_id", value=iot_instance_id, expected_type=type_hints["iot_instance_id"])
+            check_type(argname="argument join_permission_id", value=join_permission_id, expected_type=type_hints["join_permission_id"])
+            check_type(argname="argument net_type", value=net_type, expected_type=type_hints["net_type"])
+            check_type(argname="argument protocol_type", value=protocol_type, expected_type=type_hints["protocol_type"])
+            check_type(argname="argument publish_auto", value=publish_auto, expected_type=type_hints["publish_auto"])
+            check_type(argname="argument resource_group_id", value=resource_group_id, expected_type=type_hints["resource_group_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "node_type": node_type,
             "product_name": product_name,
         }
         if aliyun_commodity_code is not None:
             self._values["aliyun_commodity_code"] = aliyun_commodity_code
         if auth_type is not None:
@@ -706,31 +756,37 @@
 ):
     '''A ROS resource type:  ``ALIYUN::IOT::ProductTopic``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "ProductTopicProps",
+        props: typing.Union["ProductTopicProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::IOT::ProductTopic``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(ProductTopic.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTopicId")
     def attr_topic_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute TopicId: Topic ID.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTopicId"))
 
 
 @jsii.data_type(
@@ -758,14 +814,21 @@
 
         :param operation: Property operation: Operation permissions of devices on the topic category. Value options: SUB: Subscribe. Devices can subscribe to the topics of this category. PUB: Publish. Devices can publish messages using the topics of this category. ALL: Subscribe and publish. Devices can subscribe to and publish messages to the topics of this category.
         :param product_key: Property productKey: The unique identifier of the product for which you want to create a topic category.
         :param topic_short_name: Property topicShortName: The custom category hierarchy in the topic category. By default, a topic category contains two system defined category hierarchies: productKey and ${deviceName}. Forward slashes (/) are used to delimit the topic hierarchies. The format of a topic category is productKey/${deviceName}/topicShortName. Note The name of each category hierarchy can contain English letters, digits, and underscores (_), and cannot be empty.
         :param desc: Property desc: The description of the topic category. You can enter a description with up to 100 characters.
         :param iot_instance_id: Property iotInstanceId: Instance ID you purchased. Public instances do not need pass this property.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(ProductTopicProps.__init__)
+            check_type(argname="argument operation", value=operation, expected_type=type_hints["operation"])
+            check_type(argname="argument product_key", value=product_key, expected_type=type_hints["product_key"])
+            check_type(argname="argument topic_short_name", value=topic_short_name, expected_type=type_hints["topic_short_name"])
+            check_type(argname="argument desc", value=desc, expected_type=type_hints["desc"])
+            check_type(argname="argument iot_instance_id", value=iot_instance_id, expected_type=type_hints["iot_instance_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "operation": operation,
             "product_key": product_key,
             "topic_short_name": topic_short_name,
         }
         if desc is not None:
             self._values["desc"] = desc
@@ -844,147 +907,162 @@
 ):
     '''A ROS template type:  ``ALIYUN::IOT::Device``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosDeviceProps",
+        props: typing.Union["RosDeviceProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::IOT::Device``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosDevice.__init__)
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
+            type_hints = typing.get_type_hints(RosDevice._render_properties)
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
     @jsii.member(jsii_name="attrDeviceName")
     def attr_device_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: DeviceName: Device name.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDeviceName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDeviceSecret")
     def attr_device_secret(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: DeviceSecret: Device key.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDeviceSecret"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrIotId")
     def attr_iot_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute:
 
         IotId: Things internet device ID issued for the device, as the unique identifier of the device.
         Description Keep, do not leak.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrIotId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrIotInstanceId")
     def attr_iot_instance_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: IotInstanceId: IOT instance ID.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrIotInstanceId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrIpAddress")
     def attr_ip_address(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: IpAddress: IP address.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrIpAddress"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrNickName")
     def attr_nick_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: NickName: Nick name.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrNickName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrNodeType")
     def attr_node_type(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: NodeType: Node type.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrNodeType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrProductKey")
     def attr_product_key(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ProductKey: Product key.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrProductKey"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrProductName")
     def attr_product_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ProductName: Product name.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrProductName"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosDevice, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="productKey")
     def product_key(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: productKey: The identifier of the product to which the device to be registered belongs.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "productKey"))
 
     @product_key.setter
     def product_key(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDevice, "product_key").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "productKey", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="devEui")
     def dev_eui(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -994,17 +1072,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "devEui"))
 
     @dev_eui.setter
     def dev_eui(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDevice, "dev_eui").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "devEui", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="deviceName")
     def device_name(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         ::
 
@@ -1020,34 +1101,40 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "deviceName"))
 
     @device_name.setter
     def device_name(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDevice, "device_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "deviceName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="iotInstanceId")
     def iot_instance_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: iotInstanceId: Public instance does not pass this parameter; instance that you need to buy the incoming instance ID.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "iotInstanceId"))
 
     @iot_instance_id.setter
     def iot_instance_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDevice, "iot_instance_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "iotInstanceId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="nickname")
     def nickname(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -1058,17 +1145,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "nickname"))
 
     @nickname.setter
     def nickname(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDevice, "nickname").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "nickname", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="pinCode")
     def pin_code(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -1078,136 +1168,160 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "pinCode"))
 
     @pin_code.setter
     def pin_code(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDevice, "pin_code").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "pinCode", value)
 
 
 class RosDeviceGroup(
     ros_cdk_core.RosResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@alicloud/ros-cdk-iot.RosDeviceGroup",
 ):
     '''A ROS template type:  ``ALIYUN::IOT::DeviceGroup``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosDeviceGroupProps",
+        props: typing.Union["RosDeviceGroupProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::IOT::DeviceGroup``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosDeviceGroup.__init__)
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
+            type_hints = typing.get_type_hints(RosDeviceGroup._render_properties)
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
     @jsii.member(jsii_name="attrGroupId")
     def attr_group_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: GroupId: Packet, ID, System for the globally unique identifier generated packet.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrGroupId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrIotInstanceId")
     def attr_iot_instance_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: IotInstanceId: IOT instance ID.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrIotInstanceId"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosDeviceGroup, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="groupName")
     def group_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: groupName: The name of the group. The name can contain Chinese characters, English letters, digits, and underscores (_). The length must be 4 to 30 characters (a Chinese character counts as two characters).
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "groupName"))
 
     @group_name.setter
     def group_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDeviceGroup, "group_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "groupName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="groupDesc")
     def group_desc(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: groupDesc: The description of the group. You can enter a description with up to 100 characters.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "groupDesc"))
 
     @group_desc.setter
     def group_desc(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDeviceGroup, "group_desc").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "groupDesc", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="iotInstanceId")
     def iot_instance_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: iotInstanceId: Public instance does not pass this parameter; instance that you need to buy the incoming instance ID.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "iotInstanceId"))
 
     @iot_instance_id.setter
     def iot_instance_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDeviceGroup, "iot_instance_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "iotInstanceId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="superGroupId")
     def super_group_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -1217,14 +1331,17 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "superGroupId"))
 
     @super_group_id.setter
     def super_group_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDeviceGroup, "super_group_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "superGroupId", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-iot.RosDeviceGroupProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -1246,14 +1363,20 @@
         '''Properties for defining a ``ALIYUN::IOT::DeviceGroup``.
 
         :param group_name: 
         :param group_desc: 
         :param iot_instance_id: 
         :param super_group_id: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosDeviceGroupProps.__init__)
+            check_type(argname="argument group_name", value=group_name, expected_type=type_hints["group_name"])
+            check_type(argname="argument group_desc", value=group_desc, expected_type=type_hints["group_desc"])
+            check_type(argname="argument iot_instance_id", value=iot_instance_id, expected_type=type_hints["iot_instance_id"])
+            check_type(argname="argument super_group_id", value=super_group_id, expected_type=type_hints["super_group_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "group_name": group_name,
         }
         if group_desc is not None:
             self._values["group_desc"] = group_desc
         if iot_instance_id is not None:
             self._values["iot_instance_id"] = iot_instance_id
@@ -1342,14 +1465,22 @@
         :param product_key: 
         :param dev_eui: 
         :param device_name: 
         :param iot_instance_id: 
         :param nickname: 
         :param pin_code: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosDeviceProps.__init__)
+            check_type(argname="argument product_key", value=product_key, expected_type=type_hints["product_key"])
+            check_type(argname="argument dev_eui", value=dev_eui, expected_type=type_hints["dev_eui"])
+            check_type(argname="argument device_name", value=device_name, expected_type=type_hints["device_name"])
+            check_type(argname="argument iot_instance_id", value=iot_instance_id, expected_type=type_hints["iot_instance_id"])
+            check_type(argname="argument nickname", value=nickname, expected_type=type_hints["nickname"])
+            check_type(argname="argument pin_code", value=pin_code, expected_type=type_hints["pin_code"])
         self._values: typing.Dict[str, typing.Any] = {
             "product_key": product_key,
         }
         if dev_eui is not None:
             self._values["dev_eui"] = dev_eui
         if device_name is not None:
             self._values["device_name"] = device_name
@@ -1457,73 +1588,85 @@
 ):
     '''A ROS template type:  ``ALIYUN::IOT::Product``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosProductProps",
+        props: typing.Union["RosProductProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::IOT::Product``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosProduct.__init__)
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
+            type_hints = typing.get_type_hints(RosProduct._render_properties)
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
     @jsii.member(jsii_name="attrIotInstanceId")
     def attr_iot_instance_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: IotInstanceId: IOT instance ID.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrIotInstanceId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrProductKey")
     def attr_product_key(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ProductKey: The globally unique identifier of the product issued by IoT Platform.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrProductKey"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosProduct, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="nodeType")
     def node_type(self) -> typing.Union[jsii.Number, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         nodeType: The node type of the product. Values:
         0: Device. A device cannot be mounted with sub-devices. It can connect to IoT Platform
@@ -1535,17 +1678,20 @@
         return typing.cast(typing.Union[jsii.Number, ros_cdk_core.IResolvable], jsii.get(self, "nodeType"))
 
     @node_type.setter
     def node_type(
         self,
         value: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosProduct, "node_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "nodeType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="productName")
     def product_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         productName: The name of the product. A product name can be 4 to 30 characters in length and can
         contain Chinese characters, English letters, digits, and underscores (_).
@@ -1554,17 +1700,20 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "productName"))
 
     @product_name.setter
     def product_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosProduct, "product_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "productName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="aliyunCommodityCode")
     def aliyun_commodity_code(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -1577,17 +1726,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "aliyunCommodityCode"))
 
     @aliyun_commodity_code.setter
     def aliyun_commodity_code(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosProduct, "aliyun_commodity_code").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "aliyunCommodityCode", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="authType")
     def auth_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -1602,17 +1754,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "authType"))
 
     @auth_type.setter
     def auth_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosProduct, "auth_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "authType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="categoryKey")
     def category_key(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -1622,17 +1777,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "categoryKey"))
 
     @category_key.setter
     def category_key(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosProduct, "category_key").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "categoryKey", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dataFormat")
     def data_format(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -1645,17 +1803,20 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "dataFormat"))
 
     @data_format.setter
     def data_format(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosProduct, "data_format").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dataFormat", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="description")
     def description(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -1665,17 +1826,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "description"))
 
     @description.setter
     def description(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosProduct, "description").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "description", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="id2")
     def id2(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -1691,34 +1855,40 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "id2"))
 
     @id2.setter
     def id2(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosProduct, "id2").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "id2", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="iotInstanceId")
     def iot_instance_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: iotInstanceId: Public instance does not pass this parameter; instance that you need to buy the incoming instance ID.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "iotInstanceId"))
 
     @iot_instance_id.setter
     def iot_instance_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosProduct, "iot_instance_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "iotInstanceId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="joinPermissionId")
     def join_permission_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -1729,17 +1899,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "joinPermissionId"))
 
     @join_permission_id.setter
     def join_permission_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosProduct, "join_permission_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "joinPermissionId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="netType")
     def net_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -1756,17 +1929,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "netType"))
 
     @net_type.setter
     def net_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosProduct, "net_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "netType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="protocolType")
     def protocol_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -1783,17 +1959,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "protocolType"))
 
     @protocol_type.setter
     def protocol_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosProduct, "protocol_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "protocolType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="publishAuto")
     def publish_auto(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -1805,17 +1984,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "publishAuto"))
 
     @publish_auto.setter
     def publish_auto(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosProduct, "publish_auto").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "publishAuto", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="resourceGroupId")
     def resource_group_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -1825,14 +2007,17 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "resourceGroupId"))
 
     @resource_group_id.setter
     def resource_group_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosProduct, "resource_group_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "resourceGroupId", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-iot.RosProductProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -1884,14 +2069,30 @@
         :param iot_instance_id: 
         :param join_permission_id: 
         :param net_type: 
         :param protocol_type: 
         :param publish_auto: 
         :param resource_group_id: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosProductProps.__init__)
+            check_type(argname="argument node_type", value=node_type, expected_type=type_hints["node_type"])
+            check_type(argname="argument product_name", value=product_name, expected_type=type_hints["product_name"])
+            check_type(argname="argument aliyun_commodity_code", value=aliyun_commodity_code, expected_type=type_hints["aliyun_commodity_code"])
+            check_type(argname="argument auth_type", value=auth_type, expected_type=type_hints["auth_type"])
+            check_type(argname="argument category_key", value=category_key, expected_type=type_hints["category_key"])
+            check_type(argname="argument data_format", value=data_format, expected_type=type_hints["data_format"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument id2", value=id2, expected_type=type_hints["id2"])
+            check_type(argname="argument iot_instance_id", value=iot_instance_id, expected_type=type_hints["iot_instance_id"])
+            check_type(argname="argument join_permission_id", value=join_permission_id, expected_type=type_hints["join_permission_id"])
+            check_type(argname="argument net_type", value=net_type, expected_type=type_hints["net_type"])
+            check_type(argname="argument protocol_type", value=protocol_type, expected_type=type_hints["protocol_type"])
+            check_type(argname="argument publish_auto", value=publish_auto, expected_type=type_hints["publish_auto"])
+            check_type(argname="argument resource_group_id", value=resource_group_id, expected_type=type_hints["resource_group_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "node_type": node_type,
             "product_name": product_name,
         }
         if aliyun_commodity_code is not None:
             self._values["aliyun_commodity_code"] = aliyun_commodity_code
         if auth_type is not None:
@@ -2152,65 +2353,77 @@
 ):
     '''A ROS template type:  ``ALIYUN::IOT::ProductTopic``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosProductTopicProps",
+        props: typing.Union["RosProductTopicProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::IOT::ProductTopic``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosProductTopic.__init__)
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
+            type_hints = typing.get_type_hints(RosProductTopic._render_properties)
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
     @jsii.member(jsii_name="attrTopicId")
     def attr_topic_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: TopicId: Topic ID
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTopicId"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosProductTopic, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="operation")
     def operation(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         operation: Operation permissions of devices on the topic category. Value options:
         SUB: Subscribe. Devices can subscribe to the topics of this category.
@@ -2220,32 +2433,38 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "operation"))
 
     @operation.setter
     def operation(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosProductTopic, "operation").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "operation", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="productKey")
     def product_key(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: productKey: The unique identifier of the product for which you want to create a topic category.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "productKey"))
 
     @product_key.setter
     def product_key(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosProductTopic, "product_key").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "productKey", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="topicShortName")
     def topic_short_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         topicShortName: The custom category hierarchy in the topic category. By default, a topic category contains two system defined category hierarchies: productKey and ${deviceName}. Forward slashes (/) are used to delimit the topic hierarchies. The format of a topic category is productKey/${deviceName}/topicShortName.
         Note The name of each category hierarchy can contain English letters, digits, and underscores (_), and cannot be empty.
@@ -2253,48 +2472,57 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "topicShortName"))
 
     @topic_short_name.setter
     def topic_short_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosProductTopic, "topic_short_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "topicShortName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="desc")
     def desc(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: desc: The description of the topic category. You can enter a description with up to 100 characters.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "desc"))
 
     @desc.setter
     def desc(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosProductTopic, "desc").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "desc", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="iotInstanceId")
     def iot_instance_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: iotInstanceId: Instance ID you purchased. Public instances do not need pass this property.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "iotInstanceId"))
 
     @iot_instance_id.setter
     def iot_instance_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosProductTopic, "iot_instance_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "iotInstanceId", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-iot.RosProductTopicProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -2319,14 +2547,21 @@
 
         :param operation: 
         :param product_key: 
         :param topic_short_name: 
         :param desc: 
         :param iot_instance_id: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosProductTopicProps.__init__)
+            check_type(argname="argument operation", value=operation, expected_type=type_hints["operation"])
+            check_type(argname="argument product_key", value=product_key, expected_type=type_hints["product_key"])
+            check_type(argname="argument topic_short_name", value=topic_short_name, expected_type=type_hints["topic_short_name"])
+            check_type(argname="argument desc", value=desc, expected_type=type_hints["desc"])
+            check_type(argname="argument iot_instance_id", value=iot_instance_id, expected_type=type_hints["iot_instance_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "operation": operation,
             "product_key": product_key,
             "topic_short_name": topic_short_name,
         }
         if desc is not None:
             self._values["desc"] = desc
@@ -2407,89 +2642,104 @@
 ):
     '''A ROS template type:  ``ALIYUN::IOT::Rule``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosRuleProps",
+        props: typing.Union["RosRuleProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::IOT::Rule``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosRule.__init__)
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
+            type_hints = typing.get_type_hints(RosRule._render_properties)
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
     @jsii.member(jsii_name="attrActionId")
     def attr_action_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ActionId: The ID of the rule action.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrActionId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrRuleId")
     def attr_rule_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: RuleId: The ID of the rule.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrRuleId"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosRule, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="name")
     def name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         name: The name of the rule. The name must be 1 to 30 characters in length and can contain
         English letters, digits, underscores (_), and hyphens (-). Chinese language is also
         supported. Each Chinese symbol occupies 2 characters.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "name"))
 
     @name.setter
     def name(self, value: typing.Union[builtins.str, ros_cdk_core.IResolvable]) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosRule, "name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "name", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dataType")
     def data_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -2504,17 +2754,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "dataType"))
 
     @data_type.setter
     def data_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosRule, "data_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dataType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="iotInstanceId")
     def iot_instance_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -2524,34 +2777,40 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "iotInstanceId"))
 
     @iot_instance_id.setter
     def iot_instance_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosRule, "iot_instance_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "iotInstanceId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="productKey")
     def product_key(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: productKey: The ProductKey of the product to which the rule applies.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "productKey"))
 
     @product_key.setter
     def product_key(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosRule, "product_key").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "productKey", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="resourceGroupId")
     def resource_group_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -2563,34 +2822,40 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "resourceGroupId"))
 
     @resource_group_id.setter
     def resource_group_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosRule, "resource_group_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "resourceGroupId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="ruleAction")
     def rule_action(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosRule.RuleActionProperty"]]]]:
         '''
         :Property: ruleAction:
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosRule.RuleActionProperty"]]]], jsii.get(self, "ruleAction"))
 
     @rule_action.setter
     def rule_action(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosRule.RuleActionProperty"]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosRule, "rule_action").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "ruleAction", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="ruleDesc")
     def rule_desc(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -2600,17 +2865,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "ruleDesc"))
 
     @rule_desc.setter
     def rule_desc(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosRule, "rule_desc").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "ruleDesc", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="select")
     def select(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -2620,17 +2888,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "select"))
 
     @select.setter
     def select(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosRule, "select").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "select", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="shortTopic")
     def short_topic(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -2666,34 +2937,40 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "shortTopic"))
 
     @short_topic.setter
     def short_topic(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosRule, "short_topic").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "shortTopic", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="startRule")
     def start_rule(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property: startRule: Start the rule. The rule at least contains one rule action with normal data forward.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "startRule"))
 
     @start_rule.setter
     def start_rule(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosRule, "start_rule").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "startRule", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="topicType")
     def topic_type(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -2704,17 +2981,20 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "topicType"))
 
     @topic_type.setter
     def topic_type(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosRule, "topic_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "topicType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="where")
     def where(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -2724,14 +3004,17 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "where"))
 
     @where.setter
     def where(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosRule, "where").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "where", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-iot.RosRule.RuleActionProperty",
         jsii_struct_bases=[],
         name_mapping={
             "configuration": "configuration",
@@ -2748,14 +3031,19 @@
             error_action_flag: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param configuration: 
             :param type: 
             :param error_action_flag: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosRule.RuleActionProperty.__init__)
+                check_type(argname="argument configuration", value=configuration, expected_type=type_hints["configuration"])
+                check_type(argname="argument type", value=type, expected_type=type_hints["type"])
+                check_type(argname="argument error_action_flag", value=error_action_flag, expected_type=type_hints["error_action_flag"])
             self._values: typing.Dict[str, typing.Any] = {
                 "configuration": configuration,
                 "type": type,
             }
             if error_action_flag is not None:
                 self._values["error_action_flag"] = error_action_flag
 
@@ -2834,56 +3122,65 @@
 ):
     '''A ROS template type:  ``ALIYUN::IOT::RuleAction``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosRuleActionProps",
+        props: typing.Union["RosRuleActionProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::IOT::RuleAction``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosRuleAction.__init__)
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
+            type_hints = typing.get_type_hints(RosRuleAction._render_properties)
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
     @jsii.member(jsii_name="attrActionId")
     def attr_action_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ActionId: The ID of the rule action.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrActionId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="configuration")
     def configuration(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         configuration: The configurations of the rule action. You must specify a JSON string. The configurations
         for different types of rule actions are different. For more information about required
@@ -2892,26 +3189,32 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "configuration"))
 
     @configuration.setter
     def configuration(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosRuleAction, "configuration").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "configuration", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosRuleAction, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="ruleId")
     def rule_id(self) -> typing.Union[jsii.Number, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         ruleId: The ID of the rule for which you want to create an action. You can use either of the
         following methods to view the rule ID: 1. Log on to the IoT Platform console and choose Rules>Data Forwarding. 2. Call the ListRule operation.
@@ -2919,17 +3222,20 @@
         return typing.cast(typing.Union[jsii.Number, ros_cdk_core.IResolvable], jsii.get(self, "ruleId"))
 
     @rule_id.setter
     def rule_id(
         self,
         value: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosRuleAction, "rule_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "ruleId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="type")
     def type(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         type: The type of the rule action. Valid values:
         MNS: forwards data in the topics that have been processed by the rule engine to Message
@@ -2947,17 +3253,20 @@
         on regions. For more information about the regions and destination cloud services
         that are supported by the rule engine, see Regions and zones.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "type"))
 
     @type.setter
     def type(self, value: typing.Union[builtins.str, ros_cdk_core.IResolvable]) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosRuleAction, "type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "type", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="errorActionFlag")
     def error_action_flag(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -2972,17 +3281,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "errorActionFlag"))
 
     @error_action_flag.setter
     def error_action_flag(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosRuleAction, "error_action_flag").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "errorActionFlag", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="iotInstanceId")
     def iot_instance_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -2992,14 +3304,17 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "iotInstanceId"))
 
     @iot_instance_id.setter
     def iot_instance_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosRuleAction, "iot_instance_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "iotInstanceId", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-iot.RosRuleActionProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -3024,14 +3339,21 @@
 
         :param configuration: 
         :param rule_id: 
         :param type: 
         :param error_action_flag: 
         :param iot_instance_id: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosRuleActionProps.__init__)
+            check_type(argname="argument configuration", value=configuration, expected_type=type_hints["configuration"])
+            check_type(argname="argument rule_id", value=rule_id, expected_type=type_hints["rule_id"])
+            check_type(argname="argument type", value=type, expected_type=type_hints["type"])
+            check_type(argname="argument error_action_flag", value=error_action_flag, expected_type=type_hints["error_action_flag"])
+            check_type(argname="argument iot_instance_id", value=iot_instance_id, expected_type=type_hints["iot_instance_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "configuration": configuration,
             "rule_id": rule_id,
             "type": type,
         }
         if error_action_flag is not None:
             self._values["error_action_flag"] = error_action_flag
@@ -3154,15 +3476,15 @@
         self,
         *,
         name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         data_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         iot_instance_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         product_key: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         resource_group_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        rule_action: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosRule.RuleActionProperty]]]] = None,
+        rule_action: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosRule.RuleActionProperty, typing.Dict[str, typing.Any]]]]]] = None,
         rule_desc: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         select: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         short_topic: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         start_rule: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         topic_type: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         where: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
     ) -> None:
@@ -3177,14 +3499,28 @@
         :param rule_desc: 
         :param select: 
         :param short_topic: 
         :param start_rule: 
         :param topic_type: 
         :param where: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosRuleProps.__init__)
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+            check_type(argname="argument data_type", value=data_type, expected_type=type_hints["data_type"])
+            check_type(argname="argument iot_instance_id", value=iot_instance_id, expected_type=type_hints["iot_instance_id"])
+            check_type(argname="argument product_key", value=product_key, expected_type=type_hints["product_key"])
+            check_type(argname="argument resource_group_id", value=resource_group_id, expected_type=type_hints["resource_group_id"])
+            check_type(argname="argument rule_action", value=rule_action, expected_type=type_hints["rule_action"])
+            check_type(argname="argument rule_desc", value=rule_desc, expected_type=type_hints["rule_desc"])
+            check_type(argname="argument select", value=select, expected_type=type_hints["select"])
+            check_type(argname="argument short_topic", value=short_topic, expected_type=type_hints["short_topic"])
+            check_type(argname="argument start_rule", value=start_rule, expected_type=type_hints["start_rule"])
+            check_type(argname="argument topic_type", value=topic_type, expected_type=type_hints["topic_type"])
+            check_type(argname="argument where", value=where, expected_type=type_hints["where"])
         self._values: typing.Dict[str, typing.Any] = {
             "name": name,
         }
         if data_type is not None:
             self._values["data_type"] = data_type
         if iot_instance_id is not None:
             self._values["iot_instance_id"] = iot_instance_id
@@ -3407,37 +3743,43 @@
 ):
     '''A ROS resource type:  ``ALIYUN::IOT::Rule``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RuleProps",
+        props: typing.Union["RuleProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::IOT::Rule``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(Rule.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrActionId")
     def attr_action_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute ActionId: The ID of the rule action.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrActionId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrRuleId")
     def attr_rule_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute RuleId: The ID of the rule.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrRuleId"))
 
 
 class RuleAction(
@@ -3447,31 +3789,37 @@
 ):
     '''A ROS resource type:  ``ALIYUN::IOT::RuleAction``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RuleActionProps",
+        props: typing.Union["RuleActionProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::IOT::RuleAction``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RuleAction.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrActionId")
     def attr_action_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute ActionId: The ID of the rule action.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrActionId"))
 
 
 @jsii.data_type(
@@ -3499,14 +3847,21 @@
 
         :param configuration: Property configuration: The configurations of the rule action. You must specify a JSON string. The configurations for different types of rule actions are different. For more information about required syntax and examples, see the following tables.
         :param rule_id: Property ruleId: The ID of the rule for which you want to create an action. You can use either of the following methods to view the rule ID: 1. Log on to the IoT Platform console and choose Rules>Data Forwarding. 2. Call the ListRule operation.
         :param type: Property type: The type of the rule action. Valid values: MNS: forwards data in the topics that have been processed by the rule engine to Message Service (MNS) for message transmission. FC: forwards data in the topics that have been processed by the rule engine to Function Compute for event computing. REPUBLISH: forwards data in the topics that have been processed by the rule engine to another IoT Platform topic. AMQP: forwards data to AMQP consumer groups. OTS: forwards data in the topics that have been processed by the rule engine to Table Store for NoSQL data storage. Note Rules of the binary data format (the DataType parameter is set toBINARY) do not support forwarding data to Table Store. Destination Alibaba Cloud services that are supported by the rule engine vary based on regions. For more information about the regions and destination cloud services that are supported by the rule engine, see Regions and zones.
         :param error_action_flag: Property errorActionFlag: Indicates whether the rule action forwarded error operation data. Error operation data indicates that the rule engine failed to forward data from the IoT Platform topic to the destination cloud service. A data forwarding failure indicates that forwarding retries also failed. Valid values: true: forwards error operation data. false: forwards normal data instead of error operation data. Default value: false.
         :param iot_instance_id: Property iotInstanceId: The ID of the instance. This parameter is not required for public instances. However, the parameter is required for the instances that you have purchased.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RuleActionProps.__init__)
+            check_type(argname="argument configuration", value=configuration, expected_type=type_hints["configuration"])
+            check_type(argname="argument rule_id", value=rule_id, expected_type=type_hints["rule_id"])
+            check_type(argname="argument type", value=type, expected_type=type_hints["type"])
+            check_type(argname="argument error_action_flag", value=error_action_flag, expected_type=type_hints["error_action_flag"])
+            check_type(argname="argument iot_instance_id", value=iot_instance_id, expected_type=type_hints["iot_instance_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "configuration": configuration,
             "rule_id": rule_id,
             "type": type,
         }
         if error_action_flag is not None:
             self._values["error_action_flag"] = error_action_flag
@@ -3624,15 +3979,15 @@
         self,
         *,
         name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         data_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         iot_instance_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         product_key: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         resource_group_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        rule_action: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosRule.RuleActionProperty]]]] = None,
+        rule_action: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosRule.RuleActionProperty, typing.Dict[str, typing.Any]]]]]] = None,
         rule_desc: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         select: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         short_topic: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         start_rule: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         topic_type: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         where: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
     ) -> None:
@@ -3647,14 +4002,28 @@
         :param rule_desc: Property ruleDesc: The description of the rule. The description can be up to 100 characters in length. Each Chinese symbol occupies 1 characters.
         :param select: Property select: The SQL SELECT statement that you want to execute. For more information, seeSQL expressions. Note Specify the fields that follow the Select keyword for this parameter. For example, if the Select statement is Select a,b,c, specify a,b,c for this parameter.
         :param short_topic: Property shortTopic: The topic to which this rule is applied. Syntax: ${deviceName}/topicShortName. ${deviceName}specifies the name of the device, and topicShortNamespecifies the custom name of the topic. Basic communication topics or Thing Specification Language (TSL)-based communication topics. Syntax: ${deviceName}/topicShortName. You can replace ${deviceName} with the + wildcard. The wildcard indicates that the topic applies to all devices under the product. Valid values of topicShortName: /thing/event/property/post: submits the property data of a device. /thing/event/${tsl.event.identifier}/post: submits the event data of a device.${tsl.event.identifier} specifies the identifier of an event in the TSL. /thing/lifecycle: submits device lifecycle changes. /thing/downlink/reply/message: sends a response to a request from IoT Platform. /thing/list/found: submits the data when a gateway detects a new sub-device. /thing/topo/lifecycle: submits device topology changes. /thing/event/property/history/post: submits historical property data of a device. /thing/event/${tsl.event.identifier}/post: submits the historical event data of a device.${tsl.event.identifier}specifies the identifier of an event in the TSL. /ota/upgrade: submits OTA update status. /ota/version/post: submits OTA module versions. /thing/deviceinfo/update: submits device tag changes. /edge/driver/${driver_id}/point_post: submits pass-through data from Link IoT Edge.${driver_id} specifies the ID of the driver that a device uses to access Link IoT Edge. ${packageId}/${jobId}/ota/job/status: submits the status of OTA update batches. This topic is a basic communication topic. ${packageId}specifies the ID of the firmware. ${jobId}specifies the ID of the update batch. Custom topics. Example:${deviceName}/user/get. You can call theQueryProductTopicoperation to view all custom topics of the product. When you specify a custom topic, you can use the + and # wildcards. You can replace ${deviceName} with the+ wildcard. The wildcard indicates that the topic applies to all devices under the product. You can replace the fields that follow ${deviceName} with /user/#. The # wildcard indicates that the topic applies whatever values are specified for the fields that follow/user. For more information about how to use wildcards, see Wildcards in topics. Topic that is used to submit device status changes: ${deviceName}. You can use the+wildcard. In this case, the status changes of all devices under the product are submitted.
         :param start_rule: Property startRule: Start the rule. The rule at least contains one rule action with normal data forward.
         :param topic_type: Property topicType: 0: The topic is a basic communication topic or TSL-based communication topic. 1: The topic is a custom topic. 2: The topic is used to submit device status changes. Syntax: /as/mqtt/status/${productKey}/${deviceName}.
         :param where: Property where: The condition that is used to trigger the rule. For more information, seeSQL expressions. Note Specify the fields that follow theWherekeyword for this parameter. For example, if the Where statement is Where a>10, specify a>10 for this parameter.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RuleProps.__init__)
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+            check_type(argname="argument data_type", value=data_type, expected_type=type_hints["data_type"])
+            check_type(argname="argument iot_instance_id", value=iot_instance_id, expected_type=type_hints["iot_instance_id"])
+            check_type(argname="argument product_key", value=product_key, expected_type=type_hints["product_key"])
+            check_type(argname="argument resource_group_id", value=resource_group_id, expected_type=type_hints["resource_group_id"])
+            check_type(argname="argument rule_action", value=rule_action, expected_type=type_hints["rule_action"])
+            check_type(argname="argument rule_desc", value=rule_desc, expected_type=type_hints["rule_desc"])
+            check_type(argname="argument select", value=select, expected_type=type_hints["select"])
+            check_type(argname="argument short_topic", value=short_topic, expected_type=type_hints["short_topic"])
+            check_type(argname="argument start_rule", value=start_rule, expected_type=type_hints["start_rule"])
+            check_type(argname="argument topic_type", value=topic_type, expected_type=type_hints["topic_type"])
+            check_type(argname="argument where", value=where, expected_type=type_hints["where"])
         self._values: typing.Dict[str, typing.Any] = {
             "name": name,
         }
         if data_type is not None:
             self._values["data_type"] = data_type
         if iot_instance_id is not None:
             self._values["iot_instance_id"] = iot_instance_id
```

### Comparing `ros-cdk-iot-1.0.8/src/ros_cdk_iot.egg-info/PKG-INFO` & `ros-cdk-iot-1.0.9/src/ros_cdk_iot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-iot
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS IOT Construct Library
```

