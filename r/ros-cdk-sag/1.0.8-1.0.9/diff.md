# Comparing `tmp/ros-cdk-sag-1.0.8.tar.gz` & `tmp/ros-cdk-sag-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-sag-1.0.8.tar", last modified: Thu Jul 14 02:31:04 2022, max compression
+gzip compressed data, was "dist/ros-cdk-sag-1.0.9.tar", last modified: Fri Sep 23 12:28:25 2022, max compression
```

## Comparing `ros-cdk-sag-1.0.8.tar` & `ros-cdk-sag-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:31:04.000000 ros-cdk-sag-1.0.8/
--rw-r--r--   0 root         (0) root         (0)    10279 2022-07-14 02:31:04.000000 ros-cdk-sag-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2022-07-14 02:31:04.000000 ros-cdk-sag-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2022-07-14 02:31:04.000000 ros-cdk-sag-1.0.8/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1240 2022-07-14 02:31:04.000000 ros-cdk-sag-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      179 2022-07-14 02:31:04.000000 ros-cdk-sag-1.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)      106 2022-07-14 02:31:04.000000 ros-cdk-sag-1.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-07-14 02:31:04.000000 ros-cdk-sag-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1794 2022-07-14 02:31:04.000000 ros-cdk-sag-1.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:31:04.000000 ros-cdk-sag-1.0.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:31:04.000000 ros-cdk-sag-1.0.8/src/ros_cdk_sag/
--rw-r--r--   0 root         (0) root         (0)   286062 2022-07-14 02:31:04.000000 ros-cdk-sag-1.0.8/src/ros_cdk_sag/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:31:04.000000 ros-cdk-sag-1.0.8/src/ros_cdk_sag/_jsii/
--rw-r--r--   0 root         (0) root         (0)      370 2022-07-14 02:31:04.000000 ros-cdk-sag-1.0.8/src/ros_cdk_sag/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)   108548 2022-07-14 02:31:04.000000 ros-cdk-sag-1.0.8/src/ros_cdk_sag/_jsii/ros-cdk-sag@1.0.8.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:31:04.000000 ros-cdk-sag-1.0.8/src/ros_cdk_sag/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:31:04.000000 ros-cdk-sag-1.0.8/src/ros_cdk_sag.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1240 2022-07-14 02:31:04.000000 ros-cdk-sag-1.0.8/src/ros_cdk_sag.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      400 2022-07-14 02:31:04.000000 ros-cdk-sag-1.0.8/src/ros_cdk_sag.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:31:04.000000 ros-cdk-sag-1.0.8/src/ros_cdk_sag.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2022-07-14 02:31:04.000000 ros-cdk-sag-1.0.8/src/ros_cdk_sag.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2022-07-14 02:31:04.000000 ros-cdk-sag-1.0.8/src/ros_cdk_sag.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:28:25.000000 ros-cdk-sag-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)    10279 2022-09-23 12:28:25.000000 ros-cdk-sag-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-09-23 12:28:25.000000 ros-cdk-sag-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2022-09-23 12:28:25.000000 ros-cdk-sag-1.0.9/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1240 2022-09-23 12:28:25.000000 ros-cdk-sag-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      179 2022-09-23 12:28:25.000000 ros-cdk-sag-1.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      236 2022-09-23 12:28:25.000000 ros-cdk-sag-1.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-09-23 12:28:25.000000 ros-cdk-sag-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1823 2022-09-23 12:28:25.000000 ros-cdk-sag-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:28:25.000000 ros-cdk-sag-1.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:28:25.000000 ros-cdk-sag-1.0.9/src/ros_cdk_sag/
+-rw-r--r--   0 root         (0) root         (0)   349339 2022-09-23 12:28:25.000000 ros-cdk-sag-1.0.9/src/ros_cdk_sag/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:28:25.000000 ros-cdk-sag-1.0.9/src/ros_cdk_sag/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      404 2022-09-23 12:28:25.000000 ros-cdk-sag-1.0.9/src/ros_cdk_sag/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   108615 2022-09-23 12:28:25.000000 ros-cdk-sag-1.0.9/src/ros_cdk_sag/_jsii/ros-cdk-sag@1.0.9.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 12:28:25.000000 ros-cdk-sag-1.0.9/src/ros_cdk_sag/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:28:25.000000 ros-cdk-sag-1.0.9/src/ros_cdk_sag.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1240 2022-09-23 12:28:25.000000 ros-cdk-sag-1.0.9/src/ros_cdk_sag.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      400 2022-09-23 12:28:25.000000 ros-cdk-sag-1.0.9/src/ros_cdk_sag.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 12:28:25.000000 ros-cdk-sag-1.0.9/src/ros_cdk_sag.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2022-09-23 12:28:25.000000 ros-cdk-sag-1.0.9/src/ros_cdk_sag.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2022-09-23 12:28:25.000000 ros-cdk-sag-1.0.9/src/ros_cdk_sag.egg-info/top_level.txt
```

### Comparing `ros-cdk-sag-1.0.8/LICENSE` & `ros-cdk-sag-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-sag-1.0.8/PKG-INFO` & `ros-cdk-sag-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-sag
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS SAG Construct Library
```

### Comparing `ros-cdk-sag-1.0.8/setup.py` & `ros-cdk-sag-1.0.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-sag",
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
         "ros_cdk_sag",
         "ros_cdk_sag._jsii"
     ],
     "package_data": {
         "ros_cdk_sag._jsii": [
-            "ros-cdk-sag@1.0.8.jsii.tgz"
+            "ros-cdk-sag@1.0.9.jsii.tgz"
         ],
         "ros_cdk_sag": [
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

### Comparing `ros-cdk-sag-1.0.8/src/ros_cdk_sag/__init__.py` & `ros-cdk-sag-1.0.9/src/ros_cdk_sag/__init__.py`

 * *Files 24% similar despite different names*

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
 
 
 class ACLAssociation(
     ros_cdk_core.Resource,
@@ -29,28 +31,34 @@
 ):
     '''A ROS resource type:  ``ALIYUN::SAG::ACLAssociation``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "ACLAssociationProps",
+        props: typing.Union["ACLAssociationProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::SAG::ACLAssociation``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(ACLAssociation.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-sag.ACLAssociationProps",
     jsii_struct_bases=[],
     name_mapping={"acl_id": "aclId", "smart_ag_id": "smartAgId"},
@@ -63,14 +71,18 @@
         smart_ag_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
         '''Properties for defining a ``ALIYUN::SAG::ACLAssociation``.
 
         :param acl_id: Property aclId: Access control ID.
         :param smart_ag_id: Property smartAgId: An intelligent gateway instance that needs to bind access control.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(ACLAssociationProps.__init__)
+            check_type(argname="argument acl_id", value=acl_id, expected_type=type_hints["acl_id"])
+            check_type(argname="argument smart_ag_id", value=smart_ag_id, expected_type=type_hints["smart_ag_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "acl_id": acl_id,
             "smart_ag_id": smart_ag_id,
         }
 
     @builtins.property
     def acl_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
@@ -109,14 +121,17 @@
         *,
         name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
         '''Properties for defining a ``ALIYUN::SAG::ACL``.
 
         :param name: Property name: Access control name. The length is 2-128 characters. It must start with a letter or Chinese. It can contain numbers, periods (.), underscores (_) and dashes (-), but cannot start with http:// or https://.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(ACLProps.__init__)
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
         self._values: typing.Dict[str, typing.Any] = {
             "name": name,
         }
 
     @builtins.property
     def name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''Property name: Access control name.
@@ -146,31 +161,37 @@
 ):
     '''A ROS resource type:  ``ALIYUN::SAG::ACLRule``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "ACLRuleProps",
+        props: typing.Union["ACLRuleProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::SAG::ACLRule``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(ACLRule.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrAcrId")
     def attr_acr_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute AcrId: Access control rule ID.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAcrId"))
 
 
 @jsii.data_type(
@@ -225,14 +246,30 @@
         :param description: Property description: Rule description information, ranging from 1 to 512 characters.
         :param dpi_group_ids: Property dpiGroupIds: The ID of the application group. You can enter at most 100 application group IDs at a time. You can call the ListDpiGroups operation to query application group IDs and information about the applications.
         :param dpi_signature_ids: Property dpiSignatureIds: The ID of the application. You can enter at most 100 application IDs at a time. You can call the ListDpiSignatures operation to query application IDs and information about the applications.
         :param name: Property name: The name of the ACL rule. The name must be 2 to 100 characters in length, and can contain digits, underscores (_), and hyphens (-). It must start with a letter.
         :param priority: Property priority: Priority, ranging from 1 to 100. Default: 1
         :param type: Property type: The type of the ACL rule: Valid values: LAN: The ACL rule controls traffic of private IP addresses. This is the default value. WAN: The ACL rule controls traffic of public IP addresses.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(ACLRuleProps.__init__)
+            check_type(argname="argument acl_id", value=acl_id, expected_type=type_hints["acl_id"])
+            check_type(argname="argument dest_cidr", value=dest_cidr, expected_type=type_hints["dest_cidr"])
+            check_type(argname="argument dest_port_range", value=dest_port_range, expected_type=type_hints["dest_port_range"])
+            check_type(argname="argument direction", value=direction, expected_type=type_hints["direction"])
+            check_type(argname="argument ip_protocol", value=ip_protocol, expected_type=type_hints["ip_protocol"])
+            check_type(argname="argument policy", value=policy, expected_type=type_hints["policy"])
+            check_type(argname="argument source_cidr", value=source_cidr, expected_type=type_hints["source_cidr"])
+            check_type(argname="argument source_port_range", value=source_port_range, expected_type=type_hints["source_port_range"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument dpi_group_ids", value=dpi_group_ids, expected_type=type_hints["dpi_group_ids"])
+            check_type(argname="argument dpi_signature_ids", value=dpi_signature_ids, expected_type=type_hints["dpi_signature_ids"])
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+            check_type(argname="argument priority", value=priority, expected_type=type_hints["priority"])
+            check_type(argname="argument type", value=type, expected_type=type_hints["type"])
         self._values: typing.Dict[str, typing.Any] = {
             "acl_id": acl_id,
             "dest_cidr": dest_cidr,
             "dest_port_range": dest_port_range,
             "direction": direction,
             "ip_protocol": ip_protocol,
             "policy": policy,
@@ -397,31 +434,37 @@
 ):
     '''A ROS resource type:  ``ALIYUN::SAG::ACL``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: ACLProps,
+        props: typing.Union[ACLProps, typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::SAG::ACL``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(Acl.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrAclId")
     def attr_acl_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute AclId: Access control set ID.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAclId"))
 
 
 class App(
@@ -431,37 +474,43 @@
 ):
     '''A ROS resource type:  ``ALIYUN::SAG::App``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "AppProps",
+        props: typing.Union["AppProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::SAG::App``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(App.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrOrderId")
     def attr_order_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute OrderId: The ID of the order that you placed to subscribe to the SAG APP instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrOrderId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrSmartAgId")
     def attr_smart_ag_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute SmartAGId: The ID of the SAG APP instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrSmartAgId"))
 
 
 @jsii.data_type(
@@ -489,14 +538,21 @@
 
         :param auto_pay: Property autoPay: Specifies whether to automatically pay the bills of SAG APP instances. Default value: false. Valid values: true: automatically pays the bills of SAG APP instances. false: does not automatically pay the bills of SAG APP instances. If you set the parameter to false, after you call this operation, go to Billing Management of the SAG console to complete the payment, the instance can be created.
         :param data_plan: Property dataPlan: The quota of the traffic plan that the system allows each client account to use for free each month. Unit: GB. Set the value to 5. Note The system allows each client account to use 5 GB traffic plan for free.
         :param period: Property period: The subscription period of the SAG APP instance. Unit: months. Valid values: 1~9, 12, 24, and 36.
         :param user_count: Property userCount: The quota of client accounts for the SAG APP instance. Note The quota must be a positive multiple of 5, for example, 5, 10, and 15.
         :param charge_type: Property chargeType: The billing method of the SAG APP instance. Set the value to PREPAY. This value indicates that the SAG APP instance is a subscription resource.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(AppProps.__init__)
+            check_type(argname="argument auto_pay", value=auto_pay, expected_type=type_hints["auto_pay"])
+            check_type(argname="argument data_plan", value=data_plan, expected_type=type_hints["data_plan"])
+            check_type(argname="argument period", value=period, expected_type=type_hints["period"])
+            check_type(argname="argument user_count", value=user_count, expected_type=type_hints["user_count"])
+            check_type(argname="argument charge_type", value=charge_type, expected_type=type_hints["charge_type"])
         self._values: typing.Dict[str, typing.Any] = {
             "auto_pay": auto_pay,
             "data_plan": data_plan,
             "period": period,
             "user_count": user_count,
         }
         if charge_type is not None:
@@ -580,40 +636,46 @@
 ):
     '''A ROS resource type:  ``ALIYUN::SAG::AppUser``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "AppUserProps",
+        props: typing.Union["AppUserProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::SAG::AppUser``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(AppUser.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrSmartAgId")
     def attr_smart_ag_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute SmartAGId: The ID of the SAG APP instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrSmartAgId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrUserName")
     def attr_user_name(self) -> ros_cdk_core.IResolvable:
-        '''Attribute UserName: <heat.engine.properties.Schema object at 0x7f9b8661a510>.'''
+        '''Attribute UserName: <heat.engine.properties.Schema object at 0x7f9e467f45d0>.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrUserName"))
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-sag.AppUserProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -644,14 +706,23 @@
         :param smart_ag_id: Property smartAgId: The ID of the SAG APP instance.
         :param user_mail: Property userMail: The email address of the user. The username and password are sent to the specified email address.
         :param client_ip: Property clientIp: After this feature is enabled, you must specify the IP address of SAG APP. In this case, SAG APP connects to Alibaba Cloud through the specified IP address. Note The IP address must fall into the CIDR block of the private network. After this feature is disabled, an IP address within the CIDR block of the private network is assigned to SAG APP. Each connection to Alibaba Cloud uses a different IP address.
         :param disable: Property disable: Disable user or not.
         :param password: Property password: The password used to log on to SAG APP. For a client account, if you specify the username, you must also specify the password.
         :param user_name: Property userName: The username of the client account. Usernames of client accounts added to the same SAG APP instance must be unique. For a client account, if you specify the username, you must also specify the password.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(AppUserProps.__init__)
+            check_type(argname="argument bandwidth", value=bandwidth, expected_type=type_hints["bandwidth"])
+            check_type(argname="argument smart_ag_id", value=smart_ag_id, expected_type=type_hints["smart_ag_id"])
+            check_type(argname="argument user_mail", value=user_mail, expected_type=type_hints["user_mail"])
+            check_type(argname="argument client_ip", value=client_ip, expected_type=type_hints["client_ip"])
+            check_type(argname="argument disable", value=disable, expected_type=type_hints["disable"])
+            check_type(argname="argument password", value=password, expected_type=type_hints["password"])
+            check_type(argname="argument user_name", value=user_name, expected_type=type_hints["user_name"])
         self._values: typing.Dict[str, typing.Any] = {
             "bandwidth": bandwidth,
             "smart_ag_id": smart_ag_id,
             "user_mail": user_mail,
         }
         if client_ip is not None:
             self._values["client_ip"] = client_ip
@@ -757,31 +828,37 @@
 ):
     '''A ROS resource type:  ``ALIYUN::SAG::CloudConnectNetwork``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: typing.Optional["CloudConnectNetworkProps"] = None,
+        props: typing.Optional[typing.Union["CloudConnectNetworkProps", typing.Dict[str, typing.Any]]] = None,
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::SAG::CloudConnectNetwork``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(CloudConnectNetwork.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrCcnId")
     def attr_ccn_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute CcnId: The ID of the CCN instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrCcnId"))
 
 
 @jsii.data_type(
@@ -797,23 +874,29 @@
 class CloudConnectNetworkProps:
     def __init__(
         self,
         *,
         description: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         is_default: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         name: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        tags: typing.Optional[typing.Sequence["RosCloudConnectNetwork.TagsProperty"]] = None,
+        tags: typing.Optional[typing.Sequence[typing.Union["RosCloudConnectNetwork.TagsProperty", typing.Dict[str, typing.Any]]]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::SAG::CloudConnectNetwork``.
 
         :param description: Property description: The description of the CCN instance. The description can contain 2 to 256 characters. The description cannot start with http:// or https://.
         :param is_default: Property isDefault: Whether is created by system.
         :param name: Property name: The name of the CCN instance. The name can contain 2 to 128 characters including a-z, A-Z, 0-9, chinese, underlines, and hyphens. The name must start with an English letter, but cannot start with http:// or https://.
         :param tags: Property tags: Tags to attach to instance. Max support 20 tags to add during create instance. Each tag with two properties Key and Value, and Key is required.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(CloudConnectNetworkProps.__init__)
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument is_default", value=is_default, expected_type=type_hints["is_default"])
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
         self._values: typing.Dict[str, typing.Any] = {}
         if description is not None:
             self._values["description"] = description
         if is_default is not None:
             self._values["is_default"] = is_default
         if name is not None:
             self._values["name"] = name
@@ -880,37 +963,43 @@
 ):
     '''A ROS resource type:  ``ALIYUN::SAG::GrantCcnToCen``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "GrantCcnToCenProps",
+        props: typing.Union["GrantCcnToCenProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::SAG::GrantCcnToCen``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(GrantCcnToCen.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrCcnInstanceId")
     def attr_ccn_instance_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute CcnInstanceId: The ID of the CCN instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrCcnInstanceId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrCenInstanceId")
     def attr_cen_instance_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute CenInstanceId: The ID of the CEN instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrCenInstanceId"))
 
 
 @jsii.data_type(
@@ -932,14 +1021,19 @@
     ) -> None:
         '''Properties for defining a ``ALIYUN::SAG::GrantCcnToCen``.
 
         :param ccn_instance_id: Property ccnInstanceId: The ID of the CCN instance.
         :param cen_instance_id: Property cenInstanceId: The ID of the CEN instance.
         :param cen_uid: Property cenUid: The ID of the account to which the CEN instance belongs.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(GrantCcnToCenProps.__init__)
+            check_type(argname="argument ccn_instance_id", value=ccn_instance_id, expected_type=type_hints["ccn_instance_id"])
+            check_type(argname="argument cen_instance_id", value=cen_instance_id, expected_type=type_hints["cen_instance_id"])
+            check_type(argname="argument cen_uid", value=cen_uid, expected_type=type_hints["cen_uid"])
         self._values: typing.Dict[str, typing.Any] = {
             "ccn_instance_id": ccn_instance_id,
             "cen_instance_id": cen_instance_id,
             "cen_uid": cen_uid,
         }
 
     @builtins.property
@@ -982,31 +1076,37 @@
 ):
     '''A ROS resource type:  ``ALIYUN::SAG::Qos``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "QosProps",
+        props: typing.Union["QosProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::SAG::Qos``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(Qos.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrQosId")
     def attr_qos_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute QosId: The ID of the QoS policy.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrQosId"))
 
 
 class QosAssociation(
@@ -1016,37 +1116,43 @@
 ):
     '''A ROS resource type:  ``ALIYUN::SAG::QosAssociation``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "QosAssociationProps",
+        props: typing.Union["QosAssociationProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::SAG::QosAssociation``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(QosAssociation.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrQosId")
     def attr_qos_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute QosId: The ID of the QoS policy.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrQosId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrSmartAgId")
     def attr_smart_ag_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute SmartAGId: The ID of the SAG instance to which the QoS policy is to be applied.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrSmartAgId"))
 
 
 @jsii.data_type(
@@ -1062,14 +1168,18 @@
         smart_ag_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
         '''Properties for defining a ``ALIYUN::SAG::QosAssociation``.
 
         :param qos_id: Property qosId: The instance ID of the QoS policy.
         :param smart_ag_id: Property smartAgId: The ID of the SAG instance to which the QoS policy is to be applied.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(QosAssociationProps.__init__)
+            check_type(argname="argument qos_id", value=qos_id, expected_type=type_hints["qos_id"])
+            check_type(argname="argument smart_ag_id", value=smart_ag_id, expected_type=type_hints["smart_ag_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "qos_id": qos_id,
             "smart_ag_id": smart_ag_id,
         }
 
     @builtins.property
     def qos_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
@@ -1104,31 +1214,37 @@
 ):
     '''A ROS resource type:  ``ALIYUN::SAG::QosCar``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "QosCarProps",
+        props: typing.Union["QosCarProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::SAG::QosCar``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(QosCar.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrQosCarId")
     def attr_qos_car_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute QosCarId: The ID of the traffic throttling policy.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrQosCarId"))
 
 
 @jsii.data_type(
@@ -1171,14 +1287,26 @@
         :param max_bandwidth_abs: Property maxBandwidthAbs: The maximum bandwidth. This parameter is required when LimitType is set to Absolute.
         :param max_bandwidth_percent: Property maxBandwidthPercent: The maximum percentage that is based on the maximum upstream bandwidth of the SAG instance. This parameter is required when LimitType is set to Percent.
         :param min_bandwidth_abs: Property minBandwidthAbs: The minimum bandwidth. This parameter is required when LimitType is set to Absolute.
         :param min_bandwidth_percent: Property minBandwidthPercent: The minimum percentage that is based on the maximum upstream bandwidth of the SAG instance. This parameter is required when LimitType is set to Percent.
         :param name: Property name: The name of the traffic throttling policy. The name must be 2 to 128 characters in length, and can contain Chinese characters, letters, digits, periods (.), underscores (_), and hyphens (-).
         :param percent_source_type: Property percentSourceType: If the policy throttles traffic based on a specified bandwidth percentage, the following options are available: CcnBandwidth: Cloud Enterprise Network (CCN) bandwidth. InternetUpBandwidth: Internet upstream bandwidth.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(QosCarProps.__init__)
+            check_type(argname="argument limit_type", value=limit_type, expected_type=type_hints["limit_type"])
+            check_type(argname="argument priority", value=priority, expected_type=type_hints["priority"])
+            check_type(argname="argument qos_id", value=qos_id, expected_type=type_hints["qos_id"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument max_bandwidth_abs", value=max_bandwidth_abs, expected_type=type_hints["max_bandwidth_abs"])
+            check_type(argname="argument max_bandwidth_percent", value=max_bandwidth_percent, expected_type=type_hints["max_bandwidth_percent"])
+            check_type(argname="argument min_bandwidth_abs", value=min_bandwidth_abs, expected_type=type_hints["min_bandwidth_abs"])
+            check_type(argname="argument min_bandwidth_percent", value=min_bandwidth_percent, expected_type=type_hints["min_bandwidth_percent"])
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+            check_type(argname="argument percent_source_type", value=percent_source_type, expected_type=type_hints["percent_source_type"])
         self._values: typing.Dict[str, typing.Any] = {
             "limit_type": limit_type,
             "priority": priority,
             "qos_id": qos_id,
         }
         if description is not None:
             self._values["description"] = description
@@ -1321,31 +1449,37 @@
 ):
     '''A ROS resource type:  ``ALIYUN::SAG::QosPolicy``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "QosPolicyProps",
+        props: typing.Union["QosPolicyProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::SAG::QosPolicy``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(QosPolicy.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrQosPolicyId")
     def attr_qos_policy_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute QosPolicyId: The ID of the traffic classification rule.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrQosPolicyId"))
 
 
 @jsii.data_type(
@@ -1397,14 +1531,29 @@
         :param description: Property description: The description of the traffic classification rule. The description must be 1 to 512 characters in length and can contain letters, digits, underscores (_), and hyphens (-). It must start with a letter.
         :param dpi_group_ids: Property dpiGroupIds: The ID of the application group. You can enter at most 100 application group IDs at a time. You can call the ListDpiGroups operation to query application group IDs and information about the applications.
         :param dpi_signature_ids: Property dpiSignatureIds: The ID of the application. You can enter at most 100 application IDs at a time. You can call the ListDpiSignatures operation to query application IDs and information about the applications.
         :param end_time: Property endTime: The time when the traffic classification rule becomes invalid. Specify the time in the ISO 8601 standard in the YYYY-MM-DDThh:mm:ss+0800 format. The time must be in UTC+8.
         :param name: Property name: The name of the traffic classification rule. The name must be 2 to 100 characters in length, and can contain digits, underscores (_), and hyphens (-). It must start with a letter.
         :param start_time: Property startTime: The time when the traffic classification rule takes effect. Specify the time in the ISO 8601 standard in the YYYY-MM-DDThh:mm:ss+0800 format. The time must be in UTC+8.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(QosPolicyProps.__init__)
+            check_type(argname="argument dest_cidr", value=dest_cidr, expected_type=type_hints["dest_cidr"])
+            check_type(argname="argument dest_port_range", value=dest_port_range, expected_type=type_hints["dest_port_range"])
+            check_type(argname="argument ip_protocol", value=ip_protocol, expected_type=type_hints["ip_protocol"])
+            check_type(argname="argument priority", value=priority, expected_type=type_hints["priority"])
+            check_type(argname="argument qos_id", value=qos_id, expected_type=type_hints["qos_id"])
+            check_type(argname="argument source_cidr", value=source_cidr, expected_type=type_hints["source_cidr"])
+            check_type(argname="argument source_port_range", value=source_port_range, expected_type=type_hints["source_port_range"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument dpi_group_ids", value=dpi_group_ids, expected_type=type_hints["dpi_group_ids"])
+            check_type(argname="argument dpi_signature_ids", value=dpi_signature_ids, expected_type=type_hints["dpi_signature_ids"])
+            check_type(argname="argument end_time", value=end_time, expected_type=type_hints["end_time"])
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+            check_type(argname="argument start_time", value=start_time, expected_type=type_hints["start_time"])
         self._values: typing.Dict[str, typing.Any] = {
             "dest_cidr": dest_cidr,
             "dest_port_range": dest_port_range,
             "ip_protocol": ip_protocol,
             "priority": priority,
             "qos_id": qos_id,
             "source_cidr": source_cidr,
@@ -1593,14 +1742,18 @@
         qos_description: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::SAG::Qos``.
 
         :param qos_name: Property qosName: The name of the QoS policy. The name must be 2 to 100 characters in length and can contain letters, digits, periods (.), underscores (_), and hyphens (-). It must start with a letter.
         :param qos_description: Property qosDescription: The description of the QoS policy. The description must be 1 to 512 characters in length and can contain letters, digits, underscores (_), and hyphens (-). It must start with a letter.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(QosProps.__init__)
+            check_type(argname="argument qos_name", value=qos_name, expected_type=type_hints["qos_name"])
+            check_type(argname="argument qos_description", value=qos_description, expected_type=type_hints["qos_description"])
         self._values: typing.Dict[str, typing.Any] = {
             "qos_name": qos_name,
         }
         if qos_description is not None:
             self._values["qos_description"] = qos_description
 
     @builtins.property
@@ -1645,162 +1798,195 @@
 ):
     '''A ROS template type:  ``ALIYUN::SAG::ACL``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosACLProps",
+        props: typing.Union["RosACLProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::SAG::ACL``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosACL.__init__)
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
+            type_hints = typing.get_type_hints(RosACL._render_properties)
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
     @jsii.member(jsii_name="attrAclId")
     def attr_acl_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: AclId: Access control set ID.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAclId"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosACL, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="name")
     def name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         name: Access control name.
         The length is 2-128 characters. It must start with a letter or Chinese. It can contain numbers, periods (.), underscores (_) and dashes (-), but cannot start with http:// or https://.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "name"))
 
     @name.setter
     def name(self, value: typing.Union[builtins.str, ros_cdk_core.IResolvable]) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosACL, "name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "name", value)
 
 
 class RosACLAssociation(
     ros_cdk_core.RosResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@alicloud/ros-cdk-sag.RosACLAssociation",
 ):
     '''A ROS template type:  ``ALIYUN::SAG::ACLAssociation``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosACLAssociationProps",
+        props: typing.Union["RosACLAssociationProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::SAG::ACLAssociation``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosACLAssociation.__init__)
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
+            type_hints = typing.get_type_hints(RosACLAssociation._render_properties)
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
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="aclId")
     def acl_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: aclId: Access control ID.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "aclId"))
 
     @acl_id.setter
     def acl_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosACLAssociation, "acl_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "aclId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         '''A factory method that creates a new instance of this class from an object containing the properties of this ROS resource.'''
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosACLAssociation, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="smartAgId")
     def smart_ag_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: smartAgId: An intelligent gateway instance that needs to bind access control.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "smartAgId"))
 
     @smart_ag_id.setter
     def smart_ag_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosACLAssociation, "smart_ag_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "smartAgId", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-sag.RosACLAssociationProps",
     jsii_struct_bases=[],
     name_mapping={"acl_id": "aclId", "smart_ag_id": "smartAgId"},
@@ -1813,14 +1999,18 @@
         smart_ag_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
         '''Properties for defining a ``ALIYUN::SAG::ACLAssociation``.
 
         :param acl_id: 
         :param smart_ag_id: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosACLAssociationProps.__init__)
+            check_type(argname="argument acl_id", value=acl_id, expected_type=type_hints["acl_id"])
+            check_type(argname="argument smart_ag_id", value=smart_ag_id, expected_type=type_hints["smart_ag_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "acl_id": acl_id,
             "smart_ag_id": smart_ag_id,
         }
 
     @builtins.property
     def acl_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
@@ -1863,14 +2053,17 @@
         *,
         name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
         '''Properties for defining a ``ALIYUN::SAG::ACL``.
 
         :param name: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosACLProps.__init__)
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
         self._values: typing.Dict[str, typing.Any] = {
             "name": name,
         }
 
     @builtins.property
     def name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
@@ -1902,101 +2095,119 @@
 ):
     '''A ROS template type:  ``ALIYUN::SAG::ACLRule``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosACLRuleProps",
+        props: typing.Union["RosACLRuleProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::SAG::ACLRule``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosACLRule.__init__)
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
+            type_hints = typing.get_type_hints(RosACLRule._render_properties)
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
     @jsii.member(jsii_name="attrAcrId")
     def attr_acr_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: AcrId: Access control rule ID.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAcrId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="aclId")
     def acl_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: aclId: Access control ID.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "aclId"))
 
     @acl_id.setter
     def acl_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosACLRule, "acl_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "aclId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="destCidr")
     def dest_cidr(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: destCidr: Destination address, CIDR format and IP address range in IPv4 format.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "destCidr"))
 
     @dest_cidr.setter
     def dest_cidr(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosACLRule, "dest_cidr").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "destCidr", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="destPortRange")
     def dest_port_range(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: destPortRange: Destination port range, 80/80.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "destPortRange"))
 
     @dest_port_range.setter
     def dest_port_range(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosACLRule, "dest_port_range").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "destPortRange", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="direction")
     def direction(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         direction: Regular direction.
         Value: in|out
@@ -2004,103 +2215,124 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "direction"))
 
     @direction.setter
     def direction(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosACLRule, "direction").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "direction", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosACLRule, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="ipProtocol")
     def ip_protocol(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: ipProtocol: Protocol, not case sensitive.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "ipProtocol"))
 
     @ip_protocol.setter
     def ip_protocol(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosACLRule, "ip_protocol").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "ipProtocol", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="policy")
     def policy(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: policy: Access: accept|drop
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "policy"))
 
     @policy.setter
     def policy(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosACLRule, "policy").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "policy", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="sourceCidr")
     def source_cidr(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: sourceCidr: Source address, CIDR format and IP address range in IPv4 format.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "sourceCidr"))
 
     @source_cidr.setter
     def source_cidr(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosACLRule, "source_cidr").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "sourceCidr", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="sourcePortRange")
     def source_port_range(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: sourcePortRange: Source port range, 80/80.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "sourcePortRange"))
 
     @source_port_range.setter
     def source_port_range(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosACLRule, "source_port_range").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "sourcePortRange", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="description")
     def description(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: description: Rule description information, ranging from 1 to 512 characters.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "description"))
 
     @description.setter
     def description(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosACLRule, "description").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "description", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dpiGroupIds")
     def dpi_group_ids(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]]:
         '''
         :Property:
 
@@ -2111,17 +2343,20 @@
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]], jsii.get(self, "dpiGroupIds"))
 
     @dpi_group_ids.setter
     def dpi_group_ids(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosACLRule, "dpi_group_ids").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dpiGroupIds", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dpiSignatureIds")
     def dpi_signature_ids(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]]:
         '''
         :Property:
 
@@ -2132,17 +2367,20 @@
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]], jsii.get(self, "dpiSignatureIds"))
 
     @dpi_signature_ids.setter
     def dpi_signature_ids(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosACLRule, "dpi_signature_ids").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dpiSignatureIds", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="name")
     def name(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -2153,17 +2391,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "name"))
 
     @name.setter
     def name(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosACLRule, "name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "name", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="priority")
     def priority(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -2173,17 +2414,20 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "priority"))
 
     @priority.setter
     def priority(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosACLRule, "priority").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "priority", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="type")
     def type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -2194,14 +2438,17 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "type"))
 
     @type.setter
     def type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosACLRule, "type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "type", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-sag.RosACLRuleProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -2253,14 +2500,30 @@
         :param description: 
         :param dpi_group_ids: 
         :param dpi_signature_ids: 
         :param name: 
         :param priority: 
         :param type: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosACLRuleProps.__init__)
+            check_type(argname="argument acl_id", value=acl_id, expected_type=type_hints["acl_id"])
+            check_type(argname="argument dest_cidr", value=dest_cidr, expected_type=type_hints["dest_cidr"])
+            check_type(argname="argument dest_port_range", value=dest_port_range, expected_type=type_hints["dest_port_range"])
+            check_type(argname="argument direction", value=direction, expected_type=type_hints["direction"])
+            check_type(argname="argument ip_protocol", value=ip_protocol, expected_type=type_hints["ip_protocol"])
+            check_type(argname="argument policy", value=policy, expected_type=type_hints["policy"])
+            check_type(argname="argument source_cidr", value=source_cidr, expected_type=type_hints["source_cidr"])
+            check_type(argname="argument source_port_range", value=source_port_range, expected_type=type_hints["source_port_range"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument dpi_group_ids", value=dpi_group_ids, expected_type=type_hints["dpi_group_ids"])
+            check_type(argname="argument dpi_signature_ids", value=dpi_signature_ids, expected_type=type_hints["dpi_signature_ids"])
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+            check_type(argname="argument priority", value=priority, expected_type=type_hints["priority"])
+            check_type(argname="argument type", value=type, expected_type=type_hints["type"])
         self._values: typing.Dict[str, typing.Any] = {
             "acl_id": acl_id,
             "dest_cidr": dest_cidr,
             "dest_port_range": dest_port_range,
             "direction": direction,
             "ip_protocol": ip_protocol,
             "policy": policy,
@@ -2453,64 +2716,73 @@
 ):
     '''A ROS template type:  ``ALIYUN::SAG::App``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosAppProps",
+        props: typing.Union["RosAppProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::SAG::App``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosApp.__init__)
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
+            type_hints = typing.get_type_hints(RosApp._render_properties)
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
     @jsii.member(jsii_name="attrOrderId")
     def attr_order_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: OrderId: The ID of the order that you placed to subscribe to the SAG APP instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrOrderId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrSmartAgId")
     def attr_smart_ag_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: SmartAGId: The ID of the SAG APP instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrSmartAgId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="autoPay")
     def auto_pay(self) -> typing.Union[builtins.bool, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         autoPay: Specifies whether to automatically pay the bills of SAG APP instances. Default value:
         false. Valid values:
@@ -2522,17 +2794,20 @@
         return typing.cast(typing.Union[builtins.bool, ros_cdk_core.IResolvable], jsii.get(self, "autoPay"))
 
     @auto_pay.setter
     def auto_pay(
         self,
         value: typing.Union[builtins.bool, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosApp, "auto_pay").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "autoPay", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dataPlan")
     def data_plan(self) -> typing.Union[jsii.Number, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         dataPlan: The quota of the traffic plan that the system allows each client account to use for
         free each month. Unit: GB. Set the value to 5.
@@ -2541,26 +2816,32 @@
         return typing.cast(typing.Union[jsii.Number, ros_cdk_core.IResolvable], jsii.get(self, "dataPlan"))
 
     @data_plan.setter
     def data_plan(
         self,
         value: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosApp, "data_plan").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dataPlan", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosApp, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="period")
     def period(self) -> typing.Union[jsii.Number, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         period: The subscription period of the SAG APP instance. Unit: months.
         Valid values: 1~9, 12, 24, and 36.
@@ -2568,17 +2849,20 @@
         return typing.cast(typing.Union[jsii.Number, ros_cdk_core.IResolvable], jsii.get(self, "period"))
 
     @period.setter
     def period(
         self,
         value: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosApp, "period").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "period", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="userCount")
     def user_count(self) -> typing.Union[jsii.Number, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         userCount: The quota of client accounts for the SAG APP instance.
         Note The quota must be a positive multiple of 5, for example, 5, 10, and 15.
@@ -2586,17 +2870,20 @@
         return typing.cast(typing.Union[jsii.Number, ros_cdk_core.IResolvable], jsii.get(self, "userCount"))
 
     @user_count.setter
     def user_count(
         self,
         value: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosApp, "user_count").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "userCount", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="chargeType")
     def charge_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -2606,14 +2893,17 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "chargeType"))
 
     @charge_type.setter
     def charge_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosApp, "charge_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "chargeType", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-sag.RosAppProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -2638,14 +2928,21 @@
 
         :param auto_pay: 
         :param data_plan: 
         :param period: 
         :param user_count: 
         :param charge_type: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosAppProps.__init__)
+            check_type(argname="argument auto_pay", value=auto_pay, expected_type=type_hints["auto_pay"])
+            check_type(argname="argument data_plan", value=data_plan, expected_type=type_hints["data_plan"])
+            check_type(argname="argument period", value=period, expected_type=type_hints["period"])
+            check_type(argname="argument user_count", value=user_count, expected_type=type_hints["user_count"])
+            check_type(argname="argument charge_type", value=charge_type, expected_type=type_hints["charge_type"])
         self._values: typing.Dict[str, typing.Any] = {
             "auto_pay": auto_pay,
             "data_plan": data_plan,
             "period": period,
             "user_count": user_count,
         }
         if charge_type is not None:
@@ -2736,103 +3033,121 @@
 ):
     '''A ROS template type:  ``ALIYUN::SAG::AppUser``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosAppUserProps",
+        props: typing.Union["RosAppUserProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::SAG::AppUser``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosAppUser.__init__)
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
+            type_hints = typing.get_type_hints(RosAppUser._render_properties)
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
     @jsii.member(jsii_name="attrSmartAgId")
     def attr_smart_ag_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: SmartAGId: The ID of the SAG APP instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrSmartAgId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrUserName")
     def attr_user_name(self) -> ros_cdk_core.IResolvable:
         '''
-        :Attribute: UserName: <heat.engine.properties.Schema object at 0x7f9b8661a510>
+        :Attribute: UserName: <heat.engine.properties.Schema object at 0x7f9e467f45d0>
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrUserName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="bandwidth")
     def bandwidth(self) -> typing.Union[jsii.Number, ros_cdk_core.IResolvable]:
         '''
         :Property: bandwidth: The bandwidth. Unit: Kbit/s. Maximum bandwidth: 2,000 Kbit/s.
         '''
         return typing.cast(typing.Union[jsii.Number, ros_cdk_core.IResolvable], jsii.get(self, "bandwidth"))
 
     @bandwidth.setter
     def bandwidth(
         self,
         value: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAppUser, "bandwidth").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "bandwidth", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAppUser, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="smartAgId")
     def smart_ag_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: smartAgId: The ID of the SAG APP instance.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "smartAgId"))
 
     @smart_ag_id.setter
     def smart_ag_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAppUser, "smart_ag_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "smartAgId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="userMail")
     def user_mail(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         userMail: The email address of the user. The username and password are sent to the specified
         email address.
@@ -2840,17 +3155,20 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "userMail"))
 
     @user_mail.setter
     def user_mail(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAppUser, "user_mail").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "userMail", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="clientIp")
     def client_ip(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -2864,34 +3182,40 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "clientIp"))
 
     @client_ip.setter
     def client_ip(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAppUser, "client_ip").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "clientIp", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="disable")
     def disable(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property: disable: Disable user or not.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "disable"))
 
     @disable.setter
     def disable(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAppUser, "disable").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "disable", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="password")
     def password(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -2901,17 +3225,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "password"))
 
     @password.setter
     def password(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAppUser, "password").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "password", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="userName")
     def user_name(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -2922,14 +3249,17 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "userName"))
 
     @user_name.setter
     def user_name(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAppUser, "user_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "userName", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-sag.RosAppUserProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -2960,14 +3290,23 @@
         :param smart_ag_id: 
         :param user_mail: 
         :param client_ip: 
         :param disable: 
         :param password: 
         :param user_name: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosAppUserProps.__init__)
+            check_type(argname="argument bandwidth", value=bandwidth, expected_type=type_hints["bandwidth"])
+            check_type(argname="argument smart_ag_id", value=smart_ag_id, expected_type=type_hints["smart_ag_id"])
+            check_type(argname="argument user_mail", value=user_mail, expected_type=type_hints["user_mail"])
+            check_type(argname="argument client_ip", value=client_ip, expected_type=type_hints["client_ip"])
+            check_type(argname="argument disable", value=disable, expected_type=type_hints["disable"])
+            check_type(argname="argument password", value=password, expected_type=type_hints["password"])
+            check_type(argname="argument user_name", value=user_name, expected_type=type_hints["user_name"])
         self._values: typing.Dict[str, typing.Any] = {
             "bandwidth": bandwidth,
             "smart_ag_id": smart_ag_id,
             "user_mail": user_mail,
         }
         if client_ip is not None:
             self._values["client_ip"] = client_ip
@@ -3081,65 +3420,77 @@
 ):
     '''A ROS template type:  ``ALIYUN::SAG::CloudConnectNetwork``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosCloudConnectNetworkProps",
+        props: typing.Union["RosCloudConnectNetworkProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::SAG::CloudConnectNetwork``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosCloudConnectNetwork.__init__)
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
+            type_hints = typing.get_type_hints(RosCloudConnectNetwork._render_properties)
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
     @jsii.member(jsii_name="attrCcnId")
     def attr_ccn_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: CcnId: The ID of the CCN instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrCcnId"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosCloudConnectNetwork, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="description")
     def description(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -3149,34 +3500,40 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "description"))
 
     @description.setter
     def description(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCloudConnectNetwork, "description").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "description", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="isDefault")
     def is_default(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property: isDefault: Whether is created by system
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "isDefault"))
 
     @is_default.setter
     def is_default(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCloudConnectNetwork, "is_default").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "isDefault", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="name")
     def name(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -3186,31 +3543,37 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "name"))
 
     @name.setter
     def name(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCloudConnectNetwork, "name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "name", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="tags")
     def tags(
         self,
     ) -> typing.Optional[typing.List["RosCloudConnectNetwork.TagsProperty"]]:
         '''
         :Property: tags: Tags to attach to instance. Max support 20 tags to add during create instance. Each tag with two properties Key and Value, and Key is required.
         '''
         return typing.cast(typing.Optional[typing.List["RosCloudConnectNetwork.TagsProperty"]], jsii.get(self, "tags"))
 
     @tags.setter
     def tags(
         self,
         value: typing.Optional[typing.List["RosCloudConnectNetwork.TagsProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCloudConnectNetwork, "tags").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "tags", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-sag.RosCloudConnectNetwork.TagsProperty",
         jsii_struct_bases=[],
         name_mapping={"key": "key", "value": "value"},
     )
@@ -3221,14 +3584,18 @@
             key: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param key: 
             :param value: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosCloudConnectNetwork.TagsProperty.__init__)
+                check_type(argname="argument key", value=key, expected_type=type_hints["key"])
+                check_type(argname="argument value", value=value, expected_type=type_hints["value"])
             self._values: typing.Dict[str, typing.Any] = {
                 "key": key,
             }
             if value is not None:
                 self._values["value"] = value
 
         @builtins.property
@@ -3275,23 +3642,29 @@
 class RosCloudConnectNetworkProps:
     def __init__(
         self,
         *,
         description: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         is_default: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         name: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        tags: typing.Optional[typing.Sequence[RosCloudConnectNetwork.TagsProperty]] = None,
+        tags: typing.Optional[typing.Sequence[typing.Union[RosCloudConnectNetwork.TagsProperty, typing.Dict[str, typing.Any]]]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::SAG::CloudConnectNetwork``.
 
         :param description: 
         :param is_default: 
         :param name: 
         :param tags: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosCloudConnectNetworkProps.__init__)
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument is_default", value=is_default, expected_type=type_hints["is_default"])
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
         self._values: typing.Dict[str, typing.Any] = {}
         if description is not None:
             self._values["description"] = description
         if is_default is not None:
             self._values["is_default"] = is_default
         if name is not None:
             self._values["name"] = name
@@ -3361,115 +3734,136 @@
 ):
     '''A ROS template type:  ``ALIYUN::SAG::GrantCcnToCen``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosGrantCcnToCenProps",
+        props: typing.Union["RosGrantCcnToCenProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::SAG::GrantCcnToCen``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosGrantCcnToCen.__init__)
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
+            type_hints = typing.get_type_hints(RosGrantCcnToCen._render_properties)
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
     @jsii.member(jsii_name="attrCcnInstanceId")
     def attr_ccn_instance_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: CcnInstanceId: The ID of the CCN instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrCcnInstanceId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrCenInstanceId")
     def attr_cen_instance_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: CenInstanceId: The ID of the CEN instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrCenInstanceId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="ccnInstanceId")
     def ccn_instance_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: ccnInstanceId: The ID of the CCN instance.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "ccnInstanceId"))
 
     @ccn_instance_id.setter
     def ccn_instance_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosGrantCcnToCen, "ccn_instance_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "ccnInstanceId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="cenInstanceId")
     def cen_instance_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: cenInstanceId: The ID of the CEN instance.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "cenInstanceId"))
 
     @cen_instance_id.setter
     def cen_instance_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosGrantCcnToCen, "cen_instance_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "cenInstanceId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="cenUid")
     def cen_uid(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: cenUid: The ID of the account to which the CEN instance belongs.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "cenUid"))
 
     @cen_uid.setter
     def cen_uid(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosGrantCcnToCen, "cen_uid").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "cenUid", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosGrantCcnToCen, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-sag.RosGrantCcnToCenProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -3488,14 +3882,19 @@
     ) -> None:
         '''Properties for defining a ``ALIYUN::SAG::GrantCcnToCen``.
 
         :param ccn_instance_id: 
         :param cen_instance_id: 
         :param cen_uid: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosGrantCcnToCenProps.__init__)
+            check_type(argname="argument ccn_instance_id", value=ccn_instance_id, expected_type=type_hints["ccn_instance_id"])
+            check_type(argname="argument cen_instance_id", value=cen_instance_id, expected_type=type_hints["cen_instance_id"])
+            check_type(argname="argument cen_uid", value=cen_uid, expected_type=type_hints["cen_uid"])
         self._values: typing.Dict[str, typing.Any] = {
             "ccn_instance_id": ccn_instance_id,
             "cen_instance_id": cen_instance_id,
             "cen_uid": cen_uid,
         }
 
     @builtins.property
@@ -3544,65 +3943,77 @@
 ):
     '''A ROS template type:  ``ALIYUN::SAG::Qos``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosQosProps",
+        props: typing.Union["RosQosProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::SAG::Qos``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosQos.__init__)
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
+            type_hints = typing.get_type_hints(RosQos._render_properties)
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
     @jsii.member(jsii_name="attrQosId")
     def attr_qos_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: QosId: The ID of the QoS policy.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrQosId"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosQos, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="qosName")
     def qos_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         qosName: The name of the QoS policy.
         The name must be 2 to 100 characters in length and can contain letters, digits, periods
@@ -3611,17 +4022,20 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "qosName"))
 
     @qos_name.setter
     def qos_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosQos, "qos_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "qosName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="qosDescription")
     def qos_description(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -3632,114 +4046,135 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "qosDescription"))
 
     @qos_description.setter
     def qos_description(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosQos, "qos_description").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "qosDescription", value)
 
 
 class RosQosAssociation(
     ros_cdk_core.RosResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@alicloud/ros-cdk-sag.RosQosAssociation",
 ):
     '''A ROS template type:  ``ALIYUN::SAG::QosAssociation``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosQosAssociationProps",
+        props: typing.Union["RosQosAssociationProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::SAG::QosAssociation``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosQosAssociation.__init__)
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
+            type_hints = typing.get_type_hints(RosQosAssociation._render_properties)
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
     @jsii.member(jsii_name="attrQosId")
     def attr_qos_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: QosId: The ID of the QoS policy.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrQosId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrSmartAgId")
     def attr_smart_ag_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: SmartAGId: The ID of the SAG instance to which the QoS policy is to be applied.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrSmartAgId"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosQosAssociation, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="qosId")
     def qos_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: qosId: The instance ID of the QoS policy.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "qosId"))
 
     @qos_id.setter
     def qos_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosQosAssociation, "qos_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "qosId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="smartAgId")
     def smart_ag_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: smartAgId: The ID of the SAG instance to which the QoS policy is to be applied.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "smartAgId"))
 
     @smart_ag_id.setter
     def smart_ag_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosQosAssociation, "smart_ag_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "smartAgId", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-sag.RosQosAssociationProps",
     jsii_struct_bases=[],
     name_mapping={"qos_id": "qosId", "smart_ag_id": "smartAgId"},
@@ -3752,14 +4187,18 @@
         smart_ag_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
         '''Properties for defining a ``ALIYUN::SAG::QosAssociation``.
 
         :param qos_id: 
         :param smart_ag_id: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosQosAssociationProps.__init__)
+            check_type(argname="argument qos_id", value=qos_id, expected_type=type_hints["qos_id"])
+            check_type(argname="argument smart_ag_id", value=smart_ag_id, expected_type=type_hints["smart_ag_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "qos_id": qos_id,
             "smart_ag_id": smart_ag_id,
         }
 
     @builtins.property
     def qos_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
@@ -3798,65 +4237,77 @@
 ):
     '''A ROS template type:  ``ALIYUN::SAG::QosCar``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosQosCarProps",
+        props: typing.Union["RosQosCarProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::SAG::QosCar``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosQosCar.__init__)
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
+            type_hints = typing.get_type_hints(RosQosCar._render_properties)
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
     @jsii.member(jsii_name="attrQosCarId")
     def attr_qos_car_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: QosCarId: The ID of the traffic throttling policy.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrQosCarId"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosQosCar, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="limitType")
     def limit_type(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         limitType: The type of the traffic throttling policy. Valid values:
         Absolute: throttles traffic by a specific bandwidth range.
@@ -3865,17 +4316,20 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "limitType"))
 
     @limit_type.setter
     def limit_type(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosQosCar, "limit_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "limitType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="priority")
     def priority(self) -> typing.Union[jsii.Number, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         priority: The priority of the traffic throttling policy. A smaller value represents a higher
         priority. If policies are assigned the same priority, the one applied the earliest
@@ -3884,66 +4338,78 @@
         return typing.cast(typing.Union[jsii.Number, ros_cdk_core.IResolvable], jsii.get(self, "priority"))
 
     @priority.setter
     def priority(
         self,
         value: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosQosCar, "priority").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "priority", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="qosId")
     def qos_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: qosId: The ID of the QoS policy.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "qosId"))
 
     @qos_id.setter
     def qos_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosQosCar, "qos_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "qosId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="description")
     def description(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: description: The description of the traffic throttling policy.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "description"))
 
     @description.setter
     def description(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosQosCar, "description").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "description", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="maxBandwidthAbs")
     def max_bandwidth_abs(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: maxBandwidthAbs: The maximum bandwidth. This parameter is required when LimitType is set to Absolute.
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "maxBandwidthAbs"))
 
     @max_bandwidth_abs.setter
     def max_bandwidth_abs(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosQosCar, "max_bandwidth_abs").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "maxBandwidthAbs", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="maxBandwidthPercent")
     def max_bandwidth_percent(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -3954,34 +4420,40 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "maxBandwidthPercent"))
 
     @max_bandwidth_percent.setter
     def max_bandwidth_percent(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosQosCar, "max_bandwidth_percent").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "maxBandwidthPercent", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="minBandwidthAbs")
     def min_bandwidth_abs(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: minBandwidthAbs: The minimum bandwidth. This parameter is required when LimitType is set to Absolute.
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "minBandwidthAbs"))
 
     @min_bandwidth_abs.setter
     def min_bandwidth_abs(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosQosCar, "min_bandwidth_abs").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "minBandwidthAbs", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="minBandwidthPercent")
     def min_bandwidth_percent(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -3992,17 +4464,20 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "minBandwidthPercent"))
 
     @min_bandwidth_percent.setter
     def min_bandwidth_percent(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosQosCar, "min_bandwidth_percent").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "minBandwidthPercent", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="name")
     def name(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -4013,17 +4488,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "name"))
 
     @name.setter
     def name(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosQosCar, "name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "name", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="percentSourceType")
     def percent_source_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -4035,14 +4513,17 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "percentSourceType"))
 
     @percent_source_type.setter
     def percent_source_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosQosCar, "percent_source_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "percentSourceType", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-sag.RosQosCarProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -4082,14 +4563,26 @@
         :param max_bandwidth_abs: 
         :param max_bandwidth_percent: 
         :param min_bandwidth_abs: 
         :param min_bandwidth_percent: 
         :param name: 
         :param percent_source_type: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosQosCarProps.__init__)
+            check_type(argname="argument limit_type", value=limit_type, expected_type=type_hints["limit_type"])
+            check_type(argname="argument priority", value=priority, expected_type=type_hints["priority"])
+            check_type(argname="argument qos_id", value=qos_id, expected_type=type_hints["qos_id"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument max_bandwidth_abs", value=max_bandwidth_abs, expected_type=type_hints["max_bandwidth_abs"])
+            check_type(argname="argument max_bandwidth_percent", value=max_bandwidth_percent, expected_type=type_hints["max_bandwidth_percent"])
+            check_type(argname="argument min_bandwidth_abs", value=min_bandwidth_abs, expected_type=type_hints["min_bandwidth_abs"])
+            check_type(argname="argument min_bandwidth_percent", value=min_bandwidth_percent, expected_type=type_hints["min_bandwidth_percent"])
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+            check_type(argname="argument percent_source_type", value=percent_source_type, expected_type=type_hints["percent_source_type"])
         self._values: typing.Dict[str, typing.Any] = {
             "limit_type": limit_type,
             "priority": priority,
             "qos_id": qos_id,
         }
         if description is not None:
             self._values["description"] = description
@@ -4247,56 +4740,65 @@
 ):
     '''A ROS template type:  ``ALIYUN::SAG::QosPolicy``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosQosPolicyProps",
+        props: typing.Union["RosQosPolicyProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::SAG::QosPolicy``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosQosPolicy.__init__)
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
+            type_hints = typing.get_type_hints(RosQosPolicy._render_properties)
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
     @jsii.member(jsii_name="attrQosPolicyId")
     def attr_qos_policy_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: QosPolicyId: The ID of the traffic classification rule.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrQosPolicyId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="destCidr")
     def dest_cidr(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         destCidr: The range of the destination IP addresses.
         Specify the value of this parameter in CIDR notation. Example: 192.168.10.0/24.
@@ -4304,17 +4806,20 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "destCidr"))
 
     @dest_cidr.setter
     def dest_cidr(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosQosPolicy, "dest_cidr").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "destCidr", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="destPortRange")
     def dest_port_range(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         destPortRange: The range of destination ports.
         Valid values: 1 to 65535 and -1.
@@ -4326,26 +4831,32 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "destPortRange"))
 
     @dest_port_range.setter
     def dest_port_range(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosQosPolicy, "dest_port_range").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "destPortRange", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosQosPolicy, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="ipProtocol")
     def ip_protocol(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         ipProtocol: The type of the protocol that applies to the traffic classification rule.
         The supported protocols provided in this topic are for reference only. The actual
@@ -4354,17 +4865,20 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "ipProtocol"))
 
     @ip_protocol.setter
     def ip_protocol(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosQosPolicy, "ip_protocol").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "ipProtocol", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="priority")
     def priority(self) -> typing.Union[jsii.Number, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         priority: The priority of the traffic throttling policy to which the traffic classification
         rule belongs.
@@ -4372,32 +4886,38 @@
         return typing.cast(typing.Union[jsii.Number, ros_cdk_core.IResolvable], jsii.get(self, "priority"))
 
     @priority.setter
     def priority(
         self,
         value: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosQosPolicy, "priority").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "priority", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="qosId")
     def qos_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: qosId: The ID of the QoS policy.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "qosId"))
 
     @qos_id.setter
     def qos_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosQosPolicy, "qos_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "qosId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="sourceCidr")
     def source_cidr(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         sourceCidr: The range of the source IP addresses.
         Specify the value of this parameter in CIDR notation. Example: 192.168.1.0/24.
@@ -4405,17 +4925,20 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "sourceCidr"))
 
     @source_cidr.setter
     def source_cidr(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosQosPolicy, "source_cidr").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "sourceCidr", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="sourcePortRange")
     def source_port_range(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         sourcePortRange: The range of source ports.
         Valid values: 1 to 65535 and -1.
@@ -4427,17 +4950,20 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "sourcePortRange"))
 
     @source_port_range.setter
     def source_port_range(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosQosPolicy, "source_port_range").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "sourcePortRange", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="description")
     def description(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -4448,17 +4974,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "description"))
 
     @description.setter
     def description(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosQosPolicy, "description").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "description", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dpiGroupIds")
     def dpi_group_ids(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]]:
         '''
         :Property:
 
@@ -4469,17 +4998,20 @@
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]], jsii.get(self, "dpiGroupIds"))
 
     @dpi_group_ids.setter
     def dpi_group_ids(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosQosPolicy, "dpi_group_ids").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dpiGroupIds", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dpiSignatureIds")
     def dpi_signature_ids(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]]:
         '''
         :Property:
 
@@ -4490,17 +5022,20 @@
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]], jsii.get(self, "dpiSignatureIds"))
 
     @dpi_signature_ids.setter
     def dpi_signature_ids(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosQosPolicy, "dpi_signature_ids").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dpiSignatureIds", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="endTime")
     def end_time(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -4511,17 +5046,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "endTime"))
 
     @end_time.setter
     def end_time(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosQosPolicy, "end_time").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "endTime", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="name")
     def name(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -4532,17 +5070,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "name"))
 
     @name.setter
     def name(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosQosPolicy, "name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "name", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="startTime")
     def start_time(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -4553,14 +5094,17 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "startTime"))
 
     @start_time.setter
     def start_time(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosQosPolicy, "start_time").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "startTime", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-sag.RosQosPolicyProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -4609,14 +5153,29 @@
         :param description: 
         :param dpi_group_ids: 
         :param dpi_signature_ids: 
         :param end_time: 
         :param name: 
         :param start_time: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosQosPolicyProps.__init__)
+            check_type(argname="argument dest_cidr", value=dest_cidr, expected_type=type_hints["dest_cidr"])
+            check_type(argname="argument dest_port_range", value=dest_port_range, expected_type=type_hints["dest_port_range"])
+            check_type(argname="argument ip_protocol", value=ip_protocol, expected_type=type_hints["ip_protocol"])
+            check_type(argname="argument priority", value=priority, expected_type=type_hints["priority"])
+            check_type(argname="argument qos_id", value=qos_id, expected_type=type_hints["qos_id"])
+            check_type(argname="argument source_cidr", value=source_cidr, expected_type=type_hints["source_cidr"])
+            check_type(argname="argument source_port_range", value=source_port_range, expected_type=type_hints["source_port_range"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument dpi_group_ids", value=dpi_group_ids, expected_type=type_hints["dpi_group_ids"])
+            check_type(argname="argument dpi_signature_ids", value=dpi_signature_ids, expected_type=type_hints["dpi_signature_ids"])
+            check_type(argname="argument end_time", value=end_time, expected_type=type_hints["end_time"])
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+            check_type(argname="argument start_time", value=start_time, expected_type=type_hints["start_time"])
         self._values: typing.Dict[str, typing.Any] = {
             "dest_cidr": dest_cidr,
             "dest_port_range": dest_port_range,
             "ip_protocol": ip_protocol,
             "priority": priority,
             "qos_id": qos_id,
             "source_cidr": source_cidr,
@@ -4834,14 +5393,18 @@
         qos_description: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::SAG::Qos``.
 
         :param qos_name: 
         :param qos_description: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosQosProps.__init__)
+            check_type(argname="argument qos_name", value=qos_name, expected_type=type_hints["qos_name"])
+            check_type(argname="argument qos_description", value=qos_description, expected_type=type_hints["qos_description"])
         self._values: typing.Dict[str, typing.Any] = {
             "qos_name": qos_name,
         }
         if qos_description is not None:
             self._values["qos_description"] = qos_description
 
     @builtins.property
@@ -4890,92 +5453,110 @@
 ):
     '''A ROS template type:  ``ALIYUN::SAG::SerialNumberBinding``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosSerialNumberBindingProps",
+        props: typing.Union["RosSerialNumberBindingProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::SAG::SerialNumberBinding``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosSerialNumberBinding.__init__)
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
+            type_hints = typing.get_type_hints(RosSerialNumberBinding._render_properties)
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
     @jsii.member(jsii_name="attrSmartAgId")
     def attr_smart_ag_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: SmartAGId: The ID of the SAG instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrSmartAgId"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosSerialNumberBinding, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="serialNumber")
     def serial_number(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: serialNumber: The serial number (SN) of the SAG device.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "serialNumber"))
 
     @serial_number.setter
     def serial_number(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSerialNumberBinding, "serial_number").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "serialNumber", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="smartAgId")
     def smart_ag_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: smartAgId: The ID of the SAG instance.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "smartAgId"))
 
     @smart_ag_id.setter
     def smart_ag_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSerialNumberBinding, "smart_ag_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "smartAgId", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-sag.RosSerialNumberBindingProps",
     jsii_struct_bases=[],
     name_mapping={"serial_number": "serialNumber", "smart_ag_id": "smartAgId"},
@@ -4988,14 +5569,18 @@
         smart_ag_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
         '''Properties for defining a ``ALIYUN::SAG::SerialNumberBinding``.
 
         :param serial_number: 
         :param smart_ag_id: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosSerialNumberBindingProps.__init__)
+            check_type(argname="argument serial_number", value=serial_number, expected_type=type_hints["serial_number"])
+            check_type(argname="argument smart_ag_id", value=smart_ag_id, expected_type=type_hints["smart_ag_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "serial_number": serial_number,
             "smart_ag_id": smart_ag_id,
         }
 
     @builtins.property
     def serial_number(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
@@ -5034,79 +5619,91 @@
 ):
     '''A ROS template type:  ``ALIYUN::SAG::SmartAccessGateway``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosSmartAccessGatewayProps",
+        props: typing.Union["RosSmartAccessGatewayProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::SAG::SmartAccessGateway``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosSmartAccessGateway.__init__)
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
+            type_hints = typing.get_type_hints(RosSmartAccessGateway._render_properties)
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
     @jsii.member(jsii_name="attrOrderId")
     def attr_order_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: OrderId: The ID of the order.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrOrderId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrSmartAgId")
     def attr_smart_ag_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: SmartAGId: The ID of the SAG instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrSmartAgId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="buyerMessage")
     def buyer_message(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: buyerMessage: The remarks left by the buyer.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "buyerMessage"))
 
     @buyer_message.setter
     def buyer_message(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSmartAccessGateway, "buyer_message").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "buyerMessage", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="chargeType")
     def charge_type(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         chargeType: The billing method of the SAG instance.
         Set the value to PREPAY, which specifies the subscription billing method.
@@ -5114,26 +5711,32 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "chargeType"))
 
     @charge_type.setter
     def charge_type(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSmartAccessGateway, "charge_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "chargeType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSmartAccessGateway, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="hardWareSpec")
     def hard_ware_spec(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         hardWareSpec: The type of the SAG instance. Valid values:
         sag-100wm
@@ -5143,17 +5746,20 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "hardWareSpec"))
 
     @hard_ware_spec.setter
     def hard_ware_spec(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSmartAccessGateway, "hard_ware_spec").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "hardWareSpec", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="haType")
     def ha_type(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         haType: The deployment mode. Valid values:
         no_backup: You buy only one SAG device to connect private networks to Alibaba Cloud.
@@ -5169,17 +5775,20 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "haType"))
 
     @ha_type.setter
     def ha_type(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSmartAccessGateway, "ha_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "haType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="maxBandWidth")
     def max_band_width(self) -> typing.Union[jsii.Number, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         maxBandWidth: The bandwidth of the SAG instance.
         If you want to create an SAG CPE instance and the model is sag-100wm, valid values of this parameter are 2 to 50. Unit: Mbit/s.
@@ -5189,17 +5798,20 @@
         return typing.cast(typing.Union[jsii.Number, ros_cdk_core.IResolvable], jsii.get(self, "maxBandWidth"))
 
     @max_band_width.setter
     def max_band_width(
         self,
         value: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSmartAccessGateway, "max_band_width").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "maxBandWidth", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="period")
     def period(self) -> typing.Union[jsii.Number, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         period: The subscription period of the SAG instance. Unit: months.
         Valid values: 1 to 9, 12, 24, and 36.
@@ -5207,184 +5819,220 @@
         return typing.cast(typing.Union[jsii.Number, ros_cdk_core.IResolvable], jsii.get(self, "period"))
 
     @period.setter
     def period(
         self,
         value: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSmartAccessGateway, "period").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "period", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="receiverAddress")
     def receiver_address(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: receiverAddress: The detailed address of the recipient.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "receiverAddress"))
 
     @receiver_address.setter
     def receiver_address(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSmartAccessGateway, "receiver_address").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "receiverAddress", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="receiverCity")
     def receiver_city(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: receiverCity: The city of the recipient address.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "receiverCity"))
 
     @receiver_city.setter
     def receiver_city(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSmartAccessGateway, "receiver_city").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "receiverCity", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="receiverCountry")
     def receiver_country(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: receiverCountry: The country of the recipient address.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "receiverCountry"))
 
     @receiver_country.setter
     def receiver_country(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSmartAccessGateway, "receiver_country").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "receiverCountry", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="receiverDistrict")
     def receiver_district(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: receiverDistrict: The district of the recipient address.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "receiverDistrict"))
 
     @receiver_district.setter
     def receiver_district(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSmartAccessGateway, "receiver_district").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "receiverDistrict", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="receiverEmail")
     def receiver_email(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: receiverEmail: The email address of the recipient.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "receiverEmail"))
 
     @receiver_email.setter
     def receiver_email(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSmartAccessGateway, "receiver_email").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "receiverEmail", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="receiverMobile")
     def receiver_mobile(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: receiverMobile: The mobile phone number of the recipient.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "receiverMobile"))
 
     @receiver_mobile.setter
     def receiver_mobile(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSmartAccessGateway, "receiver_mobile").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "receiverMobile", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="receiverName")
     def receiver_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: receiverName: The name of the recipient.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "receiverName"))
 
     @receiver_name.setter
     def receiver_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSmartAccessGateway, "receiver_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "receiverName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="receiverState")
     def receiver_state(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: receiverState: The province of the recipient address.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "receiverState"))
 
     @receiver_state.setter
     def receiver_state(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSmartAccessGateway, "receiver_state").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "receiverState", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="receiverTown")
     def receiver_town(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: receiverTown: The town of the recipient address.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "receiverTown"))
 
     @receiver_town.setter
     def receiver_town(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSmartAccessGateway, "receiver_town").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "receiverTown", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="receiverZip")
     def receiver_zip(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: receiverZip: The postcode of the recipient address.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "receiverZip"))
 
     @receiver_zip.setter
     def receiver_zip(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSmartAccessGateway, "receiver_zip").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "receiverZip", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="activate")
     def activate(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property: activate: Activate SAG or not. Default is False
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "activate"))
 
     @activate.setter
     def activate(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSmartAccessGateway, "activate").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "activate", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="alreadyHaveSag")
     def already_have_sag(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -5395,17 +6043,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "alreadyHaveSag"))
 
     @already_have_sag.setter
     def already_have_sag(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSmartAccessGateway, "already_have_sag").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "alreadyHaveSag", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="autoPay")
     def auto_pay(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -5419,17 +6070,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "autoPay"))
 
     @auto_pay.setter
     def auto_pay(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSmartAccessGateway, "auto_pay").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "autoPay", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="cidrBlock")
     def cidr_block(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -5442,17 +6096,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "cidrBlock"))
 
     @cidr_block.setter
     def cidr_block(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSmartAccessGateway, "cidr_block").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "cidrBlock", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="description")
     def description(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -5463,17 +6120,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "description"))
 
     @description.setter
     def description(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSmartAccessGateway, "description").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "description", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="name")
     def name(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -5484,34 +6144,40 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "name"))
 
     @name.setter
     def name(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSmartAccessGateway, "name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "name", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="receiverPhone")
     def receiver_phone(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: receiverPhone: The landline phone number of the recipient.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "receiverPhone"))
 
     @receiver_phone.setter
     def receiver_phone(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSmartAccessGateway, "receiver_phone").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "receiverPhone", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="routingStrategy")
     def routing_strategy(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -5522,17 +6188,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "routingStrategy"))
 
     @routing_strategy.setter
     def routing_strategy(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSmartAccessGateway, "routing_strategy").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "routingStrategy", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="securityLockThreshold")
     def security_lock_threshold(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -5543,106 +6212,127 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "securityLockThreshold"))
 
     @security_lock_threshold.setter
     def security_lock_threshold(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSmartAccessGateway, "security_lock_threshold").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "securityLockThreshold", value)
 
 
 class RosSmartAccessGatewayBinding(
     ros_cdk_core.RosResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@alicloud/ros-cdk-sag.RosSmartAccessGatewayBinding",
 ):
     '''A ROS template type:  ``ALIYUN::SAG::SmartAccessGatewayBinding``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosSmartAccessGatewayBindingProps",
+        props: typing.Union["RosSmartAccessGatewayBindingProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::SAG::SmartAccessGatewayBinding``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosSmartAccessGatewayBinding.__init__)
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
+            type_hints = typing.get_type_hints(RosSmartAccessGatewayBinding._render_properties)
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
     @jsii.member(jsii_name="attrSmartAgId")
     def attr_smart_ag_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: SmartAGId: The ID of the Smart Access Gateway instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrSmartAgId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="ccnId")
     def ccn_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: ccnId: The ID of the CCN instance to bind.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "ccnId"))
 
     @ccn_id.setter
     def ccn_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSmartAccessGatewayBinding, "ccn_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "ccnId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSmartAccessGatewayBinding, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="smartAgId")
     def smart_ag_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: smartAgId: The ID of the Smart Access Gateway instance.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "smartAgId"))
 
     @smart_ag_id.setter
     def smart_ag_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSmartAccessGatewayBinding, "smart_ag_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "smartAgId", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-sag.RosSmartAccessGatewayBindingProps",
     jsii_struct_bases=[],
     name_mapping={"ccn_id": "ccnId", "smart_ag_id": "smartAgId"},
@@ -5655,14 +6345,18 @@
         smart_ag_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
         '''Properties for defining a ``ALIYUN::SAG::SmartAccessGatewayBinding``.
 
         :param ccn_id: 
         :param smart_ag_id: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosSmartAccessGatewayBindingProps.__init__)
+            check_type(argname="argument ccn_id", value=ccn_id, expected_type=type_hints["ccn_id"])
+            check_type(argname="argument smart_ag_id", value=smart_ag_id, expected_type=type_hints["smart_ag_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "ccn_id": ccn_id,
             "smart_ag_id": smart_ag_id,
         }
 
     @builtins.property
     def ccn_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
@@ -5779,14 +6473,41 @@
         :param cidr_block: 
         :param description: 
         :param name: 
         :param receiver_phone: 
         :param routing_strategy: 
         :param security_lock_threshold: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosSmartAccessGatewayProps.__init__)
+            check_type(argname="argument buyer_message", value=buyer_message, expected_type=type_hints["buyer_message"])
+            check_type(argname="argument charge_type", value=charge_type, expected_type=type_hints["charge_type"])
+            check_type(argname="argument hard_ware_spec", value=hard_ware_spec, expected_type=type_hints["hard_ware_spec"])
+            check_type(argname="argument ha_type", value=ha_type, expected_type=type_hints["ha_type"])
+            check_type(argname="argument max_band_width", value=max_band_width, expected_type=type_hints["max_band_width"])
+            check_type(argname="argument period", value=period, expected_type=type_hints["period"])
+            check_type(argname="argument receiver_address", value=receiver_address, expected_type=type_hints["receiver_address"])
+            check_type(argname="argument receiver_city", value=receiver_city, expected_type=type_hints["receiver_city"])
+            check_type(argname="argument receiver_country", value=receiver_country, expected_type=type_hints["receiver_country"])
+            check_type(argname="argument receiver_district", value=receiver_district, expected_type=type_hints["receiver_district"])
+            check_type(argname="argument receiver_email", value=receiver_email, expected_type=type_hints["receiver_email"])
+            check_type(argname="argument receiver_mobile", value=receiver_mobile, expected_type=type_hints["receiver_mobile"])
+            check_type(argname="argument receiver_name", value=receiver_name, expected_type=type_hints["receiver_name"])
+            check_type(argname="argument receiver_state", value=receiver_state, expected_type=type_hints["receiver_state"])
+            check_type(argname="argument receiver_town", value=receiver_town, expected_type=type_hints["receiver_town"])
+            check_type(argname="argument receiver_zip", value=receiver_zip, expected_type=type_hints["receiver_zip"])
+            check_type(argname="argument activate", value=activate, expected_type=type_hints["activate"])
+            check_type(argname="argument already_have_sag", value=already_have_sag, expected_type=type_hints["already_have_sag"])
+            check_type(argname="argument auto_pay", value=auto_pay, expected_type=type_hints["auto_pay"])
+            check_type(argname="argument cidr_block", value=cidr_block, expected_type=type_hints["cidr_block"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+            check_type(argname="argument receiver_phone", value=receiver_phone, expected_type=type_hints["receiver_phone"])
+            check_type(argname="argument routing_strategy", value=routing_strategy, expected_type=type_hints["routing_strategy"])
+            check_type(argname="argument security_lock_threshold", value=security_lock_threshold, expected_type=type_hints["security_lock_threshold"])
         self._values: typing.Dict[str, typing.Any] = {
             "buyer_message": buyer_message,
             "charge_type": charge_type,
             "hard_ware_spec": hard_ware_spec,
             "ha_type": ha_type,
             "max_band_width": max_band_width,
             "period": period,
@@ -6133,31 +6854,37 @@
 ):
     '''A ROS resource type:  ``ALIYUN::SAG::SerialNumberBinding``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "SerialNumberBindingProps",
+        props: typing.Union["SerialNumberBindingProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::SAG::SerialNumberBinding``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(SerialNumberBinding.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrSmartAgId")
     def attr_smart_ag_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute SmartAGId: The ID of the SAG instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrSmartAgId"))
 
 
 @jsii.data_type(
@@ -6173,14 +6900,18 @@
         smart_ag_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
         '''Properties for defining a ``ALIYUN::SAG::SerialNumberBinding``.
 
         :param serial_number: Property serialNumber: The serial number (SN) of the SAG device.
         :param smart_ag_id: Property smartAgId: The ID of the SAG instance.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(SerialNumberBindingProps.__init__)
+            check_type(argname="argument serial_number", value=serial_number, expected_type=type_hints["serial_number"])
+            check_type(argname="argument smart_ag_id", value=smart_ag_id, expected_type=type_hints["smart_ag_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "serial_number": serial_number,
             "smart_ag_id": smart_ag_id,
         }
 
     @builtins.property
     def serial_number(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
@@ -6215,37 +6946,43 @@
 ):
     '''A ROS resource type:  ``ALIYUN::SAG::SmartAccessGateway``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "SmartAccessGatewayProps",
+        props: typing.Union["SmartAccessGatewayProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::SAG::SmartAccessGateway``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(SmartAccessGateway.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrOrderId")
     def attr_order_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute OrderId: The ID of the order.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrOrderId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrSmartAgId")
     def attr_smart_ag_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute SmartAGId: The ID of the SAG instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrSmartAgId"))
 
 
 class SmartAccessGatewayBinding(
@@ -6255,31 +6992,37 @@
 ):
     '''A ROS resource type:  ``ALIYUN::SAG::SmartAccessGatewayBinding``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "SmartAccessGatewayBindingProps",
+        props: typing.Union["SmartAccessGatewayBindingProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::SAG::SmartAccessGatewayBinding``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(SmartAccessGatewayBinding.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrSmartAgId")
     def attr_smart_ag_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute SmartAGId: The ID of the Smart Access Gateway instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrSmartAgId"))
 
 
 @jsii.data_type(
@@ -6295,14 +7038,18 @@
         smart_ag_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
         '''Properties for defining a ``ALIYUN::SAG::SmartAccessGatewayBinding``.
 
         :param ccn_id: Property ccnId: The ID of the CCN instance to bind.
         :param smart_ag_id: Property smartAgId: The ID of the Smart Access Gateway instance.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(SmartAccessGatewayBindingProps.__init__)
+            check_type(argname="argument ccn_id", value=ccn_id, expected_type=type_hints["ccn_id"])
+            check_type(argname="argument smart_ag_id", value=smart_ag_id, expected_type=type_hints["smart_ag_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "ccn_id": ccn_id,
             "smart_ag_id": smart_ag_id,
         }
 
     @builtins.property
     def ccn_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
@@ -6415,14 +7162,41 @@
         :param cidr_block: Property cidrBlock: The CIDR blocks of terminals in the private network. Make sure that the CIDR blocks do not overlap with each other. If the LAN port of the SAG device dynamically assigns IP addresses, IP addresses within the first CIDR block are assigned to terminals that have the Dynamic Host Configuration Protocol (DHCP) enabled.
         :param description: Property description: The description of the SAG instance. The description must be 2 to 256 characters in length, and can contain digits, periods (.), underscores (_), and hyphens (-). It must start with a letter.
         :param name: Property name: The name of the SAG instance. The name must be 2 to 128 characters in length and can contain digits, periods (.), underscores (_), and hyphens (-). It must start with a letter.
         :param receiver_phone: Property receiverPhone: The landline phone number of the recipient.
         :param routing_strategy: Property routingStrategy: The policy to advertise routes from the private network to Alibaba Cloud. static: static routing. dynamic: dynamic routing.
         :param security_lock_threshold: Property securityLockThreshold: The time that a disconnected SAG device remain locked. The time must be no shorter than zero second. Unit: second.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(SmartAccessGatewayProps.__init__)
+            check_type(argname="argument buyer_message", value=buyer_message, expected_type=type_hints["buyer_message"])
+            check_type(argname="argument charge_type", value=charge_type, expected_type=type_hints["charge_type"])
+            check_type(argname="argument hard_ware_spec", value=hard_ware_spec, expected_type=type_hints["hard_ware_spec"])
+            check_type(argname="argument ha_type", value=ha_type, expected_type=type_hints["ha_type"])
+            check_type(argname="argument max_band_width", value=max_band_width, expected_type=type_hints["max_band_width"])
+            check_type(argname="argument period", value=period, expected_type=type_hints["period"])
+            check_type(argname="argument receiver_address", value=receiver_address, expected_type=type_hints["receiver_address"])
+            check_type(argname="argument receiver_city", value=receiver_city, expected_type=type_hints["receiver_city"])
+            check_type(argname="argument receiver_country", value=receiver_country, expected_type=type_hints["receiver_country"])
+            check_type(argname="argument receiver_district", value=receiver_district, expected_type=type_hints["receiver_district"])
+            check_type(argname="argument receiver_email", value=receiver_email, expected_type=type_hints["receiver_email"])
+            check_type(argname="argument receiver_mobile", value=receiver_mobile, expected_type=type_hints["receiver_mobile"])
+            check_type(argname="argument receiver_name", value=receiver_name, expected_type=type_hints["receiver_name"])
+            check_type(argname="argument receiver_state", value=receiver_state, expected_type=type_hints["receiver_state"])
+            check_type(argname="argument receiver_town", value=receiver_town, expected_type=type_hints["receiver_town"])
+            check_type(argname="argument receiver_zip", value=receiver_zip, expected_type=type_hints["receiver_zip"])
+            check_type(argname="argument activate", value=activate, expected_type=type_hints["activate"])
+            check_type(argname="argument already_have_sag", value=already_have_sag, expected_type=type_hints["already_have_sag"])
+            check_type(argname="argument auto_pay", value=auto_pay, expected_type=type_hints["auto_pay"])
+            check_type(argname="argument cidr_block", value=cidr_block, expected_type=type_hints["cidr_block"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+            check_type(argname="argument receiver_phone", value=receiver_phone, expected_type=type_hints["receiver_phone"])
+            check_type(argname="argument routing_strategy", value=routing_strategy, expected_type=type_hints["routing_strategy"])
+            check_type(argname="argument security_lock_threshold", value=security_lock_threshold, expected_type=type_hints["security_lock_threshold"])
         self._values: typing.Dict[str, typing.Any] = {
             "buyer_message": buyer_message,
             "charge_type": charge_type,
             "hard_ware_spec": hard_ware_spec,
             "ha_type": ha_type,
             "max_band_width": max_band_width,
             "period": period,
```

### Comparing `ros-cdk-sag-1.0.8/src/ros_cdk_sag.egg-info/PKG-INFO` & `ros-cdk-sag-1.0.9/src/ros_cdk_sag.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-sag
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS SAG Construct Library
```

