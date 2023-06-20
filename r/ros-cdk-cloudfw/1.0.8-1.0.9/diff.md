# Comparing `tmp/ros-cdk-cloudfw-1.0.8.tar.gz` & `tmp/ros-cdk-cloudfw-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-cloudfw-1.0.8.tar", last modified: Thu Jul 14 02:14:26 2022, max compression
+gzip compressed data, was "dist/ros-cdk-cloudfw-1.0.9.tar", last modified: Fri Sep 23 10:54:13 2022, max compression
```

## Comparing `ros-cdk-cloudfw-1.0.8.tar` & `ros-cdk-cloudfw-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:14:26.000000 ros-cdk-cloudfw-1.0.8/
--rw-r--r--   0 root         (0) root         (0)    10279 2022-07-14 02:14:26.000000 ros-cdk-cloudfw-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2022-07-14 02:14:26.000000 ros-cdk-cloudfw-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2022-07-14 02:14:26.000000 ros-cdk-cloudfw-1.0.8/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1256 2022-07-14 02:14:26.000000 ros-cdk-cloudfw-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      191 2022-07-14 02:14:26.000000 ros-cdk-cloudfw-1.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)      106 2022-07-14 02:14:26.000000 ros-cdk-cloudfw-1.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-07-14 02:14:26.000000 ros-cdk-cloudfw-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1818 2022-07-14 02:14:26.000000 ros-cdk-cloudfw-1.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:14:26.000000 ros-cdk-cloudfw-1.0.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:14:26.000000 ros-cdk-cloudfw-1.0.8/src/ros_cdk_cloudfw/
--rw-r--r--   0 root         (0) root         (0)   110201 2022-07-14 02:14:26.000000 ros-cdk-cloudfw-1.0.8/src/ros_cdk_cloudfw/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:14:26.000000 ros-cdk-cloudfw-1.0.8/src/ros_cdk_cloudfw/_jsii/
--rw-r--r--   0 root         (0) root         (0)      391 2022-07-14 02:14:26.000000 ros-cdk-cloudfw-1.0.8/src/ros_cdk_cloudfw/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    59372 2022-07-14 02:14:26.000000 ros-cdk-cloudfw-1.0.8/src/ros_cdk_cloudfw/_jsii/ros-cdk-cloudfw@1.0.8.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:14:26.000000 ros-cdk-cloudfw-1.0.8/src/ros_cdk_cloudfw/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:14:26.000000 ros-cdk-cloudfw-1.0.8/src/ros_cdk_cloudfw.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1256 2022-07-14 02:14:26.000000 ros-cdk-cloudfw-1.0.8/src/ros_cdk_cloudfw.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      440 2022-07-14 02:14:26.000000 ros-cdk-cloudfw-1.0.8/src/ros_cdk_cloudfw.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:14:26.000000 ros-cdk-cloudfw-1.0.8/src/ros_cdk_cloudfw.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2022-07-14 02:14:26.000000 ros-cdk-cloudfw-1.0.8/src/ros_cdk_cloudfw.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2022-07-14 02:14:26.000000 ros-cdk-cloudfw-1.0.8/src/ros_cdk_cloudfw.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 10:54:13.000000 ros-cdk-cloudfw-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)    10279 2022-09-23 10:54:13.000000 ros-cdk-cloudfw-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-09-23 10:54:13.000000 ros-cdk-cloudfw-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2022-09-23 10:54:13.000000 ros-cdk-cloudfw-1.0.9/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1256 2022-09-23 10:54:13.000000 ros-cdk-cloudfw-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      191 2022-09-23 10:54:13.000000 ros-cdk-cloudfw-1.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      236 2022-09-23 10:54:13.000000 ros-cdk-cloudfw-1.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-09-23 10:54:13.000000 ros-cdk-cloudfw-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1847 2022-09-23 10:54:13.000000 ros-cdk-cloudfw-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 10:54:13.000000 ros-cdk-cloudfw-1.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 10:54:13.000000 ros-cdk-cloudfw-1.0.9/src/ros_cdk_cloudfw/
+-rw-r--r--   0 root         (0) root         (0)   131676 2022-09-23 10:54:13.000000 ros-cdk-cloudfw-1.0.9/src/ros_cdk_cloudfw/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 10:54:13.000000 ros-cdk-cloudfw-1.0.9/src/ros_cdk_cloudfw/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      425 2022-09-23 10:54:13.000000 ros-cdk-cloudfw-1.0.9/src/ros_cdk_cloudfw/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    59439 2022-09-23 10:54:13.000000 ros-cdk-cloudfw-1.0.9/src/ros_cdk_cloudfw/_jsii/ros-cdk-cloudfw@1.0.9.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 10:54:13.000000 ros-cdk-cloudfw-1.0.9/src/ros_cdk_cloudfw/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 10:54:13.000000 ros-cdk-cloudfw-1.0.9/src/ros_cdk_cloudfw.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1256 2022-09-23 10:54:13.000000 ros-cdk-cloudfw-1.0.9/src/ros_cdk_cloudfw.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      440 2022-09-23 10:54:13.000000 ros-cdk-cloudfw-1.0.9/src/ros_cdk_cloudfw.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 10:54:13.000000 ros-cdk-cloudfw-1.0.9/src/ros_cdk_cloudfw.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2022-09-23 10:54:13.000000 ros-cdk-cloudfw-1.0.9/src/ros_cdk_cloudfw.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2022-09-23 10:54:13.000000 ros-cdk-cloudfw-1.0.9/src/ros_cdk_cloudfw.egg-info/top_level.txt
```

### Comparing `ros-cdk-cloudfw-1.0.8/LICENSE` & `ros-cdk-cloudfw-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-cloudfw-1.0.8/PKG-INFO` & `ros-cdk-cloudfw-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-cloudfw
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS CLOUDFW Construct Library
```

### Comparing `ros-cdk-cloudfw-1.0.8/setup.py` & `ros-cdk-cloudfw-1.0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-cloudfw",
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
         "ros_cdk_cloudfw",
         "ros_cdk_cloudfw._jsii"
     ],
     "package_data": {
         "ros_cdk_cloudfw._jsii": [
-            "ros-cdk-cloudfw@1.0.8.jsii.tgz"
+            "ros-cdk-cloudfw@1.0.9.jsii.tgz"
         ],
         "ros_cdk_cloudfw": [
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

### Comparing `ros-cdk-cloudfw-1.0.8/src/ros_cdk_cloudfw/__init__.py` & `ros-cdk-cloudfw-1.0.9/src/ros_cdk_cloudfw/__init__.py`

 * *Files 16% similar despite different names*

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
 
 
 class AddressBook(
     ros_cdk_core.Resource,
@@ -29,31 +31,37 @@
 ):
     '''A ROS resource type:  ``ALIYUN::CLOUDFW::AddressBook``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "AddressBookProps",
+        props: typing.Union["AddressBookProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::CLOUDFW::AddressBook``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(AddressBook.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrGroupUuid")
     def attr_group_uuid(self) -> ros_cdk_core.IResolvable:
         '''Attribute GroupUuid: After a successful return to the address book to add unique identification ID.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrGroupUuid"))
 
 
 @jsii.data_type(
@@ -76,28 +84,38 @@
         *,
         description: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         group_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         group_type: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         address_list: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         auto_add_tag_ecs: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         region_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        tag_list: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosAddressBook.TagListProperty"]]]] = None,
+        tag_list: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosAddressBook.TagListProperty", typing.Dict[str, typing.Any]]]]]] = None,
         tag_relation: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::CLOUDFW::AddressBook``.
 
         :param description: Property description: Address book description.
         :param group_name: Property groupName: Name Address book.
         :param group_type: Property groupType: Type the address book, the optional values ​​are: ip: IP Address Book domain: domain name address book port: Port Address Book tag: ECS label address book.
         :param address_list: Property addressList: Address list of the address book, between multiple addresses separated by commas. Note: When GroupType ip, it must be set to port or domain. When GroupType as ip, address list, fill in the IP address. For example: 1.2.3.4/32, 1.2.3.0/24 When GroupType for the port, the address list to fill in ports or port ranges. For example: 80, 100/200 When GroupType for the domain, the domain name to fill in the address list. For example: demo1.aliyun.com, demo2.aliyun.com
         :param auto_add_tag_ecs: Property autoAddTagEcs: Whether to automatically add new ECS public network IP matching tags to the address book. Default to false.
         :param region_id: Property regionId: Region ID. Default to cn-hangzhou.
         :param tag_list: Property tagList:.
         :param tag_relation: Property tagRelation: The relationship between the labels to be matched more ECS. and: the relationship between multiple labels "and" that matches both ECS IP public network more tags will be added to the address book. or: a plurality of inter-labeled "or" relationship, i.e., as long as a matching tag ECS ​​public IP address book will be added.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(AddressBookProps.__init__)
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument group_name", value=group_name, expected_type=type_hints["group_name"])
+            check_type(argname="argument group_type", value=group_type, expected_type=type_hints["group_type"])
+            check_type(argname="argument address_list", value=address_list, expected_type=type_hints["address_list"])
+            check_type(argname="argument auto_add_tag_ecs", value=auto_add_tag_ecs, expected_type=type_hints["auto_add_tag_ecs"])
+            check_type(argname="argument region_id", value=region_id, expected_type=type_hints["region_id"])
+            check_type(argname="argument tag_list", value=tag_list, expected_type=type_hints["tag_list"])
+            check_type(argname="argument tag_relation", value=tag_relation, expected_type=type_hints["tag_relation"])
         self._values: typing.Dict[str, typing.Any] = {
             "description": description,
             "group_name": group_name,
             "group_type": group_type,
         }
         if address_list is not None:
             self._values["address_list"] = address_list
@@ -206,31 +224,37 @@
 ):
     '''A ROS resource type:  ``ALIYUN::CLOUDFW::ControlPolicy``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "ControlPolicyProps",
+        props: typing.Union["ControlPolicyProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::CLOUDFW::ControlPolicy``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(ControlPolicy.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrAclUuid")
     def attr_acl_uuid(self) -> ros_cdk_core.IResolvable:
         '''Attribute AclUuid: Security access control ID that uniquely identifies the policy.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAclUuid"))
 
 
 @jsii.data_type(
@@ -285,14 +309,30 @@
         :param source: Property source: Security access control source address policy. When SourceType for the net, Source is the source CIDR. For example: 1.2.3.0/24 When SourceType as a group, Source name for the source address book. For example: db_group When SourceType as location, Source source region (specific region position encoder see below). For example, [ "BJ11", "ZB"]
         :param source_type: Property sourceType: Security access control source address type of policy. net: Source segment (CIDR) group: source address book location: the source area
         :param dest_port: Property destPort: Security access control policy access traffic destination port. Note When DestPortType to port, set the item.
         :param dest_port_group: Property destPortGroup: Security access control policy access traffic destination port address book name. Description DestPortType is group, set the item.
         :param dest_port_type: Property destPortType: Security access control policy access destination port traffic type. port: Port group: port address book
         :param region_id: Property regionId: Region ID. Default to cn-hangzhou.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(ControlPolicyProps.__init__)
+            check_type(argname="argument acl_action", value=acl_action, expected_type=type_hints["acl_action"])
+            check_type(argname="argument application_name", value=application_name, expected_type=type_hints["application_name"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument destination", value=destination, expected_type=type_hints["destination"])
+            check_type(argname="argument destination_type", value=destination_type, expected_type=type_hints["destination_type"])
+            check_type(argname="argument direction", value=direction, expected_type=type_hints["direction"])
+            check_type(argname="argument new_order", value=new_order, expected_type=type_hints["new_order"])
+            check_type(argname="argument proto", value=proto, expected_type=type_hints["proto"])
+            check_type(argname="argument source", value=source, expected_type=type_hints["source"])
+            check_type(argname="argument source_type", value=source_type, expected_type=type_hints["source_type"])
+            check_type(argname="argument dest_port", value=dest_port, expected_type=type_hints["dest_port"])
+            check_type(argname="argument dest_port_group", value=dest_port_group, expected_type=type_hints["dest_port_group"])
+            check_type(argname="argument dest_port_type", value=dest_port_type, expected_type=type_hints["dest_port_type"])
+            check_type(argname="argument region_id", value=region_id, expected_type=type_hints["region_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "acl_action": acl_action,
             "application_name": application_name,
             "description": description,
             "destination": destination,
             "destination_type": destination_type,
             "direction": direction,
@@ -487,95 +527,113 @@
 ):
     '''A ROS template type:  ``ALIYUN::CLOUDFW::AddressBook``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosAddressBookProps",
+        props: typing.Union["RosAddressBookProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::CLOUDFW::AddressBook``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosAddressBook.__init__)
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
+            type_hints = typing.get_type_hints(RosAddressBook._render_properties)
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
     @jsii.member(jsii_name="attrGroupUuid")
     def attr_group_uuid(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: GroupUuid: After a successful return to the address book to add unique identification ID.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrGroupUuid"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="description")
     def description(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: description: Address book description.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "description"))
 
     @description.setter
     def description(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAddressBook, "description").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "description", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAddressBook, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="groupName")
     def group_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: groupName: Name Address book.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "groupName"))
 
     @group_name.setter
     def group_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAddressBook, "group_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "groupName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="groupType")
     def group_type(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         groupType: Type the address book, the optional values ​​are:
         ip: IP Address Book
@@ -586,17 +644,20 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "groupType"))
 
     @group_type.setter
     def group_type(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAddressBook, "group_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "groupType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="addressList")
     def address_list(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -609,68 +670,80 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "addressList"))
 
     @address_list.setter
     def address_list(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAddressBook, "address_list").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "addressList", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="autoAddTagEcs")
     def auto_add_tag_ecs(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property: autoAddTagEcs: Whether to automatically add new ECS public network IP matching tags to the address book. Default to false.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "autoAddTagEcs"))
 
     @auto_add_tag_ecs.setter
     def auto_add_tag_ecs(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAddressBook, "auto_add_tag_ecs").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "autoAddTagEcs", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="regionId")
     def region_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: regionId: Region ID. Default to cn-hangzhou.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "regionId"))
 
     @region_id.setter
     def region_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAddressBook, "region_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "regionId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="tagList")
     def tag_list(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosAddressBook.TagListProperty"]]]]:
         '''
         :Property: tagList:
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosAddressBook.TagListProperty"]]]], jsii.get(self, "tagList"))
 
     @tag_list.setter
     def tag_list(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosAddressBook.TagListProperty"]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAddressBook, "tag_list").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "tagList", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="tagRelation")
     def tag_relation(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -681,14 +754,17 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "tagRelation"))
 
     @tag_relation.setter
     def tag_relation(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAddressBook, "tag_relation").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "tagRelation", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-cloudfw.RosAddressBook.TagListProperty",
         jsii_struct_bases=[],
         name_mapping={"tag_key": "tagKey", "tag_value": "tagValue"},
     )
@@ -699,14 +775,18 @@
             tag_key: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
             tag_value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param tag_key: 
             :param tag_value: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosAddressBook.TagListProperty.__init__)
+                check_type(argname="argument tag_key", value=tag_key, expected_type=type_hints["tag_key"])
+                check_type(argname="argument tag_value", value=tag_value, expected_type=type_hints["tag_value"])
             self._values: typing.Dict[str, typing.Any] = {}
             if tag_key is not None:
                 self._values["tag_key"] = tag_key
             if tag_value is not None:
                 self._values["tag_value"] = tag_value
 
         @builtins.property
@@ -761,28 +841,38 @@
         *,
         description: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         group_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         group_type: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         address_list: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         auto_add_tag_ecs: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         region_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        tag_list: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosAddressBook.TagListProperty]]]] = None,
+        tag_list: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosAddressBook.TagListProperty, typing.Dict[str, typing.Any]]]]]] = None,
         tag_relation: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::CLOUDFW::AddressBook``.
 
         :param description: 
         :param group_name: 
         :param group_type: 
         :param address_list: 
         :param auto_add_tag_ecs: 
         :param region_id: 
         :param tag_list: 
         :param tag_relation: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosAddressBookProps.__init__)
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument group_name", value=group_name, expected_type=type_hints["group_name"])
+            check_type(argname="argument group_type", value=group_type, expected_type=type_hints["group_type"])
+            check_type(argname="argument address_list", value=address_list, expected_type=type_hints["address_list"])
+            check_type(argname="argument auto_add_tag_ecs", value=auto_add_tag_ecs, expected_type=type_hints["auto_add_tag_ecs"])
+            check_type(argname="argument region_id", value=region_id, expected_type=type_hints["region_id"])
+            check_type(argname="argument tag_list", value=tag_list, expected_type=type_hints["tag_list"])
+            check_type(argname="argument tag_relation", value=tag_relation, expected_type=type_hints["tag_relation"])
         self._values: typing.Dict[str, typing.Any] = {
             "description": description,
             "group_name": group_name,
             "group_type": group_type,
         }
         if address_list is not None:
             self._values["address_list"] = address_list
@@ -907,56 +997,65 @@
 ):
     '''A ROS template type:  ``ALIYUN::CLOUDFW::ControlPolicy``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosControlPolicyProps",
+        props: typing.Union["RosControlPolicyProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::CLOUDFW::ControlPolicy``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosControlPolicy.__init__)
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
+            type_hints = typing.get_type_hints(RosControlPolicy._render_properties)
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
     @jsii.member(jsii_name="attrAclUuid")
     def attr_acl_uuid(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: AclUuid: Security access control ID that uniquely identifies the policy.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAclUuid"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="aclAction")
     def acl_action(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         aclAction: Traffic access control policy set by the cloud of a firewall.
         accept: Release
@@ -966,17 +1065,20 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "aclAction"))
 
     @acl_action.setter
     def acl_action(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosControlPolicy, "acl_action").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "aclAction", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="applicationName")
     def application_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         applicationName: Application types supported by the security policy.
         The following types of applications are supported: ANY, HTTP, HTTPS, MySQL, SMTP, SMTPS, RDP, VNC, SSH, Redis, MQTT, MongoDB, Memcache, SSL
@@ -985,32 +1087,38 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "applicationName"))
 
     @application_name.setter
     def application_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosControlPolicy, "application_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "applicationName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="description")
     def description(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: description: Security access control policy description information.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "description"))
 
     @description.setter
     def description(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosControlPolicy, "description").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "description", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="destination")
     def destination(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         destination: Security Access Control destination address policy.
         When DestinationType is net, Destination purpose CIDR. For example: 1.2.3.4/24
@@ -1021,17 +1129,20 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "destination"))
 
     @destination.setter
     def destination(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosControlPolicy, "destination").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "destination", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="destinationType")
     def destination_type(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         destinationType: Security Access Control destination address type of policy.
         net: Destination network segment (CIDR)
@@ -1042,17 +1153,20 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "destinationType"))
 
     @destination_type.setter
     def destination_type(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosControlPolicy, "destination_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "destinationType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="direction")
     def direction(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         direction: Security access control traffic direction policies.
         in: internal and external traffic access control
@@ -1061,26 +1175,32 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "direction"))
 
     @direction.setter
     def direction(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosControlPolicy, "direction").fset)
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
+            type_hints = typing.get_type_hints(getattr(RosControlPolicy, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="newOrder")
     def new_order(self) -> typing.Union[jsii.Number, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         newOrder: Security access control priority policy in force. Priority number increments sequentially from 1, lower the priority number, the higher the priority.
         Description -1 indicates the lowest priority.
@@ -1088,17 +1208,20 @@
         return typing.cast(typing.Union[jsii.Number, ros_cdk_core.IResolvable], jsii.get(self, "newOrder"))
 
     @new_order.setter
     def new_order(
         self,
         value: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosControlPolicy, "new_order").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "newOrder", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="proto")
     def proto(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         proto: The type of security protocol for traffic access in the security access control policy. Can be set to ANY when you are not sure of the specific protocol type.
         Allowed values: ANY, TCP, UDP, ICMP
@@ -1106,17 +1229,20 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "proto"))
 
     @proto.setter
     def proto(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosControlPolicy, "proto").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "proto", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="source")
     def source(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         source: Security access control source address policy.
         When SourceType for the net, Source is the source CIDR. For example: 1.2.3.0/24
@@ -1126,17 +1252,20 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "source"))
 
     @source.setter
     def source(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosControlPolicy, "source").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "source", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="sourceType")
     def source_type(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         sourceType: Security access control source address type of policy.
         net: Source segment (CIDR)
@@ -1146,17 +1275,20 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "sourceType"))
 
     @source_type.setter
     def source_type(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosControlPolicy, "source_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "sourceType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="destPort")
     def dest_port(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -1166,17 +1298,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "destPort"))
 
     @dest_port.setter
     def dest_port(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosControlPolicy, "dest_port").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "destPort", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="destPortGroup")
     def dest_port_group(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -1186,17 +1321,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "destPortGroup"))
 
     @dest_port_group.setter
     def dest_port_group(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosControlPolicy, "dest_port_group").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "destPortGroup", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="destPortType")
     def dest_port_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -1207,31 +1345,37 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "destPortType"))
 
     @dest_port_type.setter
     def dest_port_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosControlPolicy, "dest_port_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "destPortType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="regionId")
     def region_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: regionId: Region ID. Default to cn-hangzhou.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "regionId"))
 
     @region_id.setter
     def region_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosControlPolicy, "region_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "regionId", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-cloudfw.RosControlPolicyProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -1283,14 +1427,30 @@
         :param source: 
         :param source_type: 
         :param dest_port: 
         :param dest_port_group: 
         :param dest_port_type: 
         :param region_id: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosControlPolicyProps.__init__)
+            check_type(argname="argument acl_action", value=acl_action, expected_type=type_hints["acl_action"])
+            check_type(argname="argument application_name", value=application_name, expected_type=type_hints["application_name"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument destination", value=destination, expected_type=type_hints["destination"])
+            check_type(argname="argument destination_type", value=destination_type, expected_type=type_hints["destination_type"])
+            check_type(argname="argument direction", value=direction, expected_type=type_hints["direction"])
+            check_type(argname="argument new_order", value=new_order, expected_type=type_hints["new_order"])
+            check_type(argname="argument proto", value=proto, expected_type=type_hints["proto"])
+            check_type(argname="argument source", value=source, expected_type=type_hints["source"])
+            check_type(argname="argument source_type", value=source_type, expected_type=type_hints["source_type"])
+            check_type(argname="argument dest_port", value=dest_port, expected_type=type_hints["dest_port"])
+            check_type(argname="argument dest_port_group", value=dest_port_group, expected_type=type_hints["dest_port_group"])
+            check_type(argname="argument dest_port_type", value=dest_port_type, expected_type=type_hints["dest_port_type"])
+            check_type(argname="argument region_id", value=region_id, expected_type=type_hints["region_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "acl_action": acl_action,
             "application_name": application_name,
             "description": description,
             "destination": destination,
             "destination_type": destination_type,
             "direction": direction,
@@ -1508,56 +1668,65 @@
 ):
     '''A ROS template type:  ``ALIYUN::CLOUDFW::VpcFirewallControlPolicy``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosVpcFirewallControlPolicyProps",
+        props: typing.Union["RosVpcFirewallControlPolicyProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::CLOUDFW::VpcFirewallControlPolicy``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosVpcFirewallControlPolicy.__init__)
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
+            type_hints = typing.get_type_hints(RosVpcFirewallControlPolicy._render_properties)
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
     @jsii.member(jsii_name="attrAclUuid")
     def attr_acl_uuid(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: AclUuid: The unique ID of the access control policy.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAclUuid"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="aclAction")
     def acl_action(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         aclAction: The action that Cloud Firewall performs on the traffic. Valid values:
         accept: allows the traffic.
@@ -1567,17 +1736,20 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "aclAction"))
 
     @acl_action.setter
     def acl_action(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosVpcFirewallControlPolicy, "acl_action").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "aclAction", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="applicationName")
     def application_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         applicationName: The application type that the access control policy supports.
         Valid values:
@@ -1600,32 +1772,38 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "applicationName"))
 
     @application_name.setter
     def application_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosVpcFirewallControlPolicy, "application_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "applicationName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="description")
     def description(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: description: The description of the access control policy.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "description"))
 
     @description.setter
     def description(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosVpcFirewallControlPolicy, "description").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "description", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="destination")
     def destination(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         destination: The destination address in the access control policy.
         Set this parameter in the following way:
@@ -1639,17 +1817,20 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "destination"))
 
     @destination.setter
     def destination(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosVpcFirewallControlPolicy, "destination").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "destination", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="destinationType")
     def destination_type(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         destinationType: The type of the destination address in the access control policy. Valid values:
         net: CIDR block
@@ -1659,26 +1840,32 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "destinationType"))
 
     @destination_type.setter
     def destination_type(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosVpcFirewallControlPolicy, "destination_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "destinationType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosVpcFirewallControlPolicy, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="newOrder")
     def new_order(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         newOrder: The priority of the access control policy.
         The priority value starts from 1. A smaller priority value indicates a higher priority.
@@ -1687,32 +1874,38 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "newOrder"))
 
     @new_order.setter
     def new_order(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosVpcFirewallControlPolicy, "new_order").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "newOrder", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="proto")
     def proto(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: proto: The type of the security protocol in the access control policy.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "proto"))
 
     @proto.setter
     def proto(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosVpcFirewallControlPolicy, "proto").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "proto", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="source")
     def source(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         source: The source address in the access control policy.
         If the SourceType parameter is set to net, set the value to a CIDR block. Example: 10.2.3.0/24.
@@ -1721,17 +1914,20 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "source"))
 
     @source.setter
     def source(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosVpcFirewallControlPolicy, "source").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "source", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="sourceType")
     def source_type(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         sourceType: The type of the source address in the access control policy. Valid values:
         net: CIDR block
@@ -1740,17 +1936,20 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "sourceType"))
 
     @source_type.setter
     def source_type(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosVpcFirewallControlPolicy, "source_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "sourceType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vpcFirewallId")
     def vpc_firewall_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         vpcFirewallId: The ID of the policy group to which you want to add the access control policy.
         If the VPC firewall is used to protect CEN, set the value to the ID of the CEN instance
@@ -1762,17 +1961,20 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "vpcFirewallId"))
 
     @vpc_firewall_id.setter
     def vpc_firewall_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosVpcFirewallControlPolicy, "vpc_firewall_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "vpcFirewallId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="destPort")
     def dest_port(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -1782,17 +1984,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "destPort"))
 
     @dest_port.setter
     def dest_port(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosVpcFirewallControlPolicy, "dest_port").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "destPort", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="destPortGroup")
     def dest_port_group(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -1802,17 +2007,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "destPortGroup"))
 
     @dest_port_group.setter
     def dest_port_group(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosVpcFirewallControlPolicy, "dest_port_group").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "destPortGroup", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="destPortType")
     def dest_port_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -1823,17 +2031,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "destPortType"))
 
     @dest_port_type.setter
     def dest_port_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosVpcFirewallControlPolicy, "dest_port_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "destPortType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="lang")
     def lang(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -1844,31 +2055,37 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "lang"))
 
     @lang.setter
     def lang(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosVpcFirewallControlPolicy, "lang").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "lang", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="regionId")
     def region_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: regionId: Region ID. Default to cn-hangzhou.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "regionId"))
 
     @region_id.setter
     def region_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosVpcFirewallControlPolicy, "region_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "regionId", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-cloudfw.RosVpcFirewallControlPolicyProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -1923,14 +2140,31 @@
         :param vpc_firewall_id: 
         :param dest_port: 
         :param dest_port_group: 
         :param dest_port_type: 
         :param lang: 
         :param region_id: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosVpcFirewallControlPolicyProps.__init__)
+            check_type(argname="argument acl_action", value=acl_action, expected_type=type_hints["acl_action"])
+            check_type(argname="argument application_name", value=application_name, expected_type=type_hints["application_name"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument destination", value=destination, expected_type=type_hints["destination"])
+            check_type(argname="argument destination_type", value=destination_type, expected_type=type_hints["destination_type"])
+            check_type(argname="argument new_order", value=new_order, expected_type=type_hints["new_order"])
+            check_type(argname="argument proto", value=proto, expected_type=type_hints["proto"])
+            check_type(argname="argument source", value=source, expected_type=type_hints["source"])
+            check_type(argname="argument source_type", value=source_type, expected_type=type_hints["source_type"])
+            check_type(argname="argument vpc_firewall_id", value=vpc_firewall_id, expected_type=type_hints["vpc_firewall_id"])
+            check_type(argname="argument dest_port", value=dest_port, expected_type=type_hints["dest_port"])
+            check_type(argname="argument dest_port_group", value=dest_port_group, expected_type=type_hints["dest_port_group"])
+            check_type(argname="argument dest_port_type", value=dest_port_type, expected_type=type_hints["dest_port_type"])
+            check_type(argname="argument lang", value=lang, expected_type=type_hints["lang"])
+            check_type(argname="argument region_id", value=region_id, expected_type=type_hints["region_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "acl_action": acl_action,
             "application_name": application_name,
             "description": description,
             "destination": destination,
             "destination_type": destination_type,
             "new_order": new_order,
@@ -2179,31 +2413,37 @@
 ):
     '''A ROS resource type:  ``ALIYUN::CLOUDFW::VpcFirewallControlPolicy``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "VpcFirewallControlPolicyProps",
+        props: typing.Union["VpcFirewallControlPolicyProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::CLOUDFW::VpcFirewallControlPolicy``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(VpcFirewallControlPolicy.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrAclUuid")
     def attr_acl_uuid(self) -> ros_cdk_core.IResolvable:
         '''Attribute AclUuid: The unique ID of the access control policy.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAclUuid"))
 
 
 @jsii.data_type(
@@ -2261,14 +2501,31 @@
         :param vpc_firewall_id: Property vpcFirewallId: The ID of the policy group to which you want to add the access control policy. If the VPC firewall is used to protect CEN, set the value to the ID of the CEN instance that the VPC firewall protects. Example: cen-ervw5jbw1234*****. If the VPC firewall is used to protect Express Connect, set the value to the ID of the VPC firewall instance. Example: vfw-a42bbb748c91234*****. Note You can call the DescribeVpcFirewallAclGroupList operation to query the ID of the policy group.
         :param dest_port: Property destPort: The destination port in the access control policy. Note This parameter must be specified if the DestPortType parameter is set to port.
         :param dest_port_group: Property destPortGroup: The address book of destination ports in the access control policy. Note This parameter must be specified if the DestPortType parameter is set to group.
         :param dest_port_type: Property destPortType: The type of the destination port in the access control policy. Valid values: port: port group: address book
         :param lang: Property lang: The natural language of the request and response. Valid values: zh: Chinese en: English
         :param region_id: Property regionId: Region ID. Default to cn-hangzhou.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(VpcFirewallControlPolicyProps.__init__)
+            check_type(argname="argument acl_action", value=acl_action, expected_type=type_hints["acl_action"])
+            check_type(argname="argument application_name", value=application_name, expected_type=type_hints["application_name"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument destination", value=destination, expected_type=type_hints["destination"])
+            check_type(argname="argument destination_type", value=destination_type, expected_type=type_hints["destination_type"])
+            check_type(argname="argument new_order", value=new_order, expected_type=type_hints["new_order"])
+            check_type(argname="argument proto", value=proto, expected_type=type_hints["proto"])
+            check_type(argname="argument source", value=source, expected_type=type_hints["source"])
+            check_type(argname="argument source_type", value=source_type, expected_type=type_hints["source_type"])
+            check_type(argname="argument vpc_firewall_id", value=vpc_firewall_id, expected_type=type_hints["vpc_firewall_id"])
+            check_type(argname="argument dest_port", value=dest_port, expected_type=type_hints["dest_port"])
+            check_type(argname="argument dest_port_group", value=dest_port_group, expected_type=type_hints["dest_port_group"])
+            check_type(argname="argument dest_port_type", value=dest_port_type, expected_type=type_hints["dest_port_type"])
+            check_type(argname="argument lang", value=lang, expected_type=type_hints["lang"])
+            check_type(argname="argument region_id", value=region_id, expected_type=type_hints["region_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "acl_action": acl_action,
             "application_name": application_name,
             "description": description,
             "destination": destination,
             "destination_type": destination_type,
             "new_order": new_order,
```

### Comparing `ros-cdk-cloudfw-1.0.8/src/ros_cdk_cloudfw.egg-info/PKG-INFO` & `ros-cdk-cloudfw-1.0.9/src/ros_cdk_cloudfw.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-cloudfw
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS CLOUDFW Construct Library
```

