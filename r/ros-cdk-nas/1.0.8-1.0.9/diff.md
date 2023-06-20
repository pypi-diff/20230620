# Comparing `tmp/ros-cdk-nas-1.0.8.tar.gz` & `tmp/ros-cdk-nas-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-nas-1.0.8.tar", last modified: Thu Jul 14 02:17:39 2022, max compression
+gzip compressed data, was "dist/ros-cdk-nas-1.0.9.tar", last modified: Fri Sep 23 10:54:47 2022, max compression
```

## Comparing `ros-cdk-nas-1.0.8.tar` & `ros-cdk-nas-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:17:39.000000 ros-cdk-nas-1.0.8/
--rw-r--r--   0 root         (0) root         (0)    10279 2022-07-14 02:17:38.000000 ros-cdk-nas-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2022-07-14 02:17:38.000000 ros-cdk-nas-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2022-07-14 02:17:38.000000 ros-cdk-nas-1.0.8/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1240 2022-07-14 02:17:39.000000 ros-cdk-nas-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      179 2022-07-14 02:17:38.000000 ros-cdk-nas-1.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)      106 2022-07-14 02:17:38.000000 ros-cdk-nas-1.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-07-14 02:17:39.000000 ros-cdk-nas-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1794 2022-07-14 02:17:38.000000 ros-cdk-nas-1.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:17:39.000000 ros-cdk-nas-1.0.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:17:39.000000 ros-cdk-nas-1.0.8/src/ros_cdk_nas/
--rw-r--r--   0 root         (0) root         (0)    82526 2022-07-14 02:17:38.000000 ros-cdk-nas-1.0.8/src/ros_cdk_nas/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:17:39.000000 ros-cdk-nas-1.0.8/src/ros_cdk_nas/_jsii/
--rw-r--r--   0 root         (0) root         (0)      370 2022-07-14 02:17:38.000000 ros-cdk-nas-1.0.8/src/ros_cdk_nas/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    52226 2022-07-14 02:17:38.000000 ros-cdk-nas-1.0.8/src/ros_cdk_nas/_jsii/ros-cdk-nas@1.0.8.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:17:38.000000 ros-cdk-nas-1.0.8/src/ros_cdk_nas/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:17:39.000000 ros-cdk-nas-1.0.8/src/ros_cdk_nas.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1240 2022-07-14 02:17:39.000000 ros-cdk-nas-1.0.8/src/ros_cdk_nas.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      400 2022-07-14 02:17:39.000000 ros-cdk-nas-1.0.8/src/ros_cdk_nas.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:17:39.000000 ros-cdk-nas-1.0.8/src/ros_cdk_nas.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2022-07-14 02:17:39.000000 ros-cdk-nas-1.0.8/src/ros_cdk_nas.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2022-07-14 02:17:39.000000 ros-cdk-nas-1.0.8/src/ros_cdk_nas.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 10:54:47.000000 ros-cdk-nas-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)    10279 2022-09-23 10:54:46.000000 ros-cdk-nas-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-09-23 10:54:46.000000 ros-cdk-nas-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2022-09-23 10:54:46.000000 ros-cdk-nas-1.0.9/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1240 2022-09-23 10:54:47.000000 ros-cdk-nas-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      179 2022-09-23 10:54:46.000000 ros-cdk-nas-1.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      236 2022-09-23 10:54:46.000000 ros-cdk-nas-1.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-09-23 10:54:47.000000 ros-cdk-nas-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1823 2022-09-23 10:54:46.000000 ros-cdk-nas-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 10:54:47.000000 ros-cdk-nas-1.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 10:54:47.000000 ros-cdk-nas-1.0.9/src/ros_cdk_nas/
+-rw-r--r--   0 root         (0) root         (0)   102152 2022-09-23 10:54:46.000000 ros-cdk-nas-1.0.9/src/ros_cdk_nas/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 10:54:47.000000 ros-cdk-nas-1.0.9/src/ros_cdk_nas/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      404 2022-09-23 10:54:46.000000 ros-cdk-nas-1.0.9/src/ros_cdk_nas/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    52285 2022-09-23 10:54:46.000000 ros-cdk-nas-1.0.9/src/ros_cdk_nas/_jsii/ros-cdk-nas@1.0.9.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 10:54:46.000000 ros-cdk-nas-1.0.9/src/ros_cdk_nas/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 10:54:47.000000 ros-cdk-nas-1.0.9/src/ros_cdk_nas.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1240 2022-09-23 10:54:46.000000 ros-cdk-nas-1.0.9/src/ros_cdk_nas.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      400 2022-09-23 10:54:46.000000 ros-cdk-nas-1.0.9/src/ros_cdk_nas.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 10:54:46.000000 ros-cdk-nas-1.0.9/src/ros_cdk_nas.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2022-09-23 10:54:46.000000 ros-cdk-nas-1.0.9/src/ros_cdk_nas.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2022-09-23 10:54:46.000000 ros-cdk-nas-1.0.9/src/ros_cdk_nas.egg-info/top_level.txt
```

### Comparing `ros-cdk-nas-1.0.8/LICENSE` & `ros-cdk-nas-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-nas-1.0.8/PKG-INFO` & `ros-cdk-nas-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-nas
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS NAS Construct Library
```

### Comparing `ros-cdk-nas-1.0.8/setup.py` & `ros-cdk-nas-1.0.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-nas",
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
         "ros_cdk_nas",
         "ros_cdk_nas._jsii"
     ],
     "package_data": {
         "ros_cdk_nas._jsii": [
-            "ros-cdk-nas@1.0.8.jsii.tgz"
+            "ros-cdk-nas@1.0.9.jsii.tgz"
         ],
         "ros_cdk_nas": [
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

### Comparing `ros-cdk-nas-1.0.8/src/ros_cdk_nas/__init__.py` & `ros-cdk-nas-1.0.9/src/ros_cdk_nas/__init__.py`

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
 
 
 class AccessGroup(
     ros_cdk_core.Resource,
@@ -29,31 +31,37 @@
 ):
     '''A ROS resource type:  ``ALIYUN::NAS::AccessGroup``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "AccessGroupProps",
+        props: typing.Union["AccessGroupProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::NAS::AccessGroup``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(AccessGroup.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrAccessGroupName")
     def attr_access_group_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute AccessGroupName: Permission group name.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAccessGroupName"))
 
 
 @jsii.data_type(
@@ -75,14 +83,19 @@
     ) -> None:
         '''Properties for defining a ``ALIYUN::NAS::AccessGroup``.
 
         :param access_group_name: Property accessGroupName: Permission group name.
         :param access_group_type: Property accessGroupType: Permission group type, including the Vpc and Classic types.
         :param description: Property description: Permission group description. It is the same as the permission group name by default.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(AccessGroupProps.__init__)
+            check_type(argname="argument access_group_name", value=access_group_name, expected_type=type_hints["access_group_name"])
+            check_type(argname="argument access_group_type", value=access_group_type, expected_type=type_hints["access_group_type"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
         self._values: typing.Dict[str, typing.Any] = {
             "access_group_name": access_group_name,
             "access_group_type": access_group_type,
         }
         if description is not None:
             self._values["description"] = description
 
@@ -130,31 +143,37 @@
 ):
     '''A ROS resource type:  ``ALIYUN::NAS::AccessRule``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "AccessRuleProps",
+        props: typing.Union["AccessRuleProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::NAS::AccessRule``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(AccessRule.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrAccessRuleId")
     def attr_access_rule_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute AccessRuleId: Rule serial number.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAccessRuleId"))
 
 
 @jsii.data_type(
@@ -182,14 +201,21 @@
 
         :param access_group_name: Property accessGroupName: Permission group name.
         :param source_cidr_ip: Property sourceCidrIp: Address or address segment.
         :param priority: Property priority: Priority level. Range: 1-100. Default value: 1
         :param rw_access_type: Property rwAccessType: Read-write permission type: RDWR (default), RDONLY.
         :param user_access_type: Property userAccessType: User permission type: no_squash (default), root_squash, all_squash.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(AccessRuleProps.__init__)
+            check_type(argname="argument access_group_name", value=access_group_name, expected_type=type_hints["access_group_name"])
+            check_type(argname="argument source_cidr_ip", value=source_cidr_ip, expected_type=type_hints["source_cidr_ip"])
+            check_type(argname="argument priority", value=priority, expected_type=type_hints["priority"])
+            check_type(argname="argument rw_access_type", value=rw_access_type, expected_type=type_hints["rw_access_type"])
+            check_type(argname="argument user_access_type", value=user_access_type, expected_type=type_hints["user_access_type"])
         self._values: typing.Dict[str, typing.Any] = {
             "access_group_name": access_group_name,
             "source_cidr_ip": source_cidr_ip,
         }
         if priority is not None:
             self._values["priority"] = priority
         if rw_access_type is not None:
@@ -257,31 +283,37 @@
 ):
     '''A ROS resource type:  ``ALIYUN::NAS::FileSystem``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "FileSystemProps",
+        props: typing.Union["FileSystemProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::NAS::FileSystem``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(FileSystem.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrFileSystemId")
     def attr_file_system_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute FileSystemId: ID of the file system created.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrFileSystemId"))
 
 
 @jsii.data_type(
@@ -316,15 +348,15 @@
         charge_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         deletion_force: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         description: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         duration: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         encrypt_type: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         file_system_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         snapshot_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        tags: typing.Optional[typing.Sequence["RosFileSystem.TagsProperty"]] = None,
+        tags: typing.Optional[typing.Sequence[typing.Union["RosFileSystem.TagsProperty", typing.Dict[str, typing.Any]]]] = None,
         vpc_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         v_switch_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         zone_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::NAS::FileSystem``.
 
         :param protocol_type: Property protocolType: Type of protocol used. Currently includes the NFS type and the SMB type
@@ -339,14 +371,31 @@
         :param file_system_type: Property fileSystemType: File system type. Allowed values: standard, extreme, cpfs
         :param snapshot_id: Property snapshotId: Snapshot ID.
         :param tags: Property tags: Tags to attach to filesystem. Max support 20 tags to add during create filesystem. Each tag with two properties Key and Value, and Key is required.
         :param vpc_id: Property vpcId: Vpc ID.
         :param v_switch_id: Property vSwitchId: VSwitch ID.
         :param zone_id: Property zoneId: Zone ID.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(FileSystemProps.__init__)
+            check_type(argname="argument protocol_type", value=protocol_type, expected_type=type_hints["protocol_type"])
+            check_type(argname="argument storage_type", value=storage_type, expected_type=type_hints["storage_type"])
+            check_type(argname="argument bandwidth", value=bandwidth, expected_type=type_hints["bandwidth"])
+            check_type(argname="argument capacity", value=capacity, expected_type=type_hints["capacity"])
+            check_type(argname="argument charge_type", value=charge_type, expected_type=type_hints["charge_type"])
+            check_type(argname="argument deletion_force", value=deletion_force, expected_type=type_hints["deletion_force"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument duration", value=duration, expected_type=type_hints["duration"])
+            check_type(argname="argument encrypt_type", value=encrypt_type, expected_type=type_hints["encrypt_type"])
+            check_type(argname="argument file_system_type", value=file_system_type, expected_type=type_hints["file_system_type"])
+            check_type(argname="argument snapshot_id", value=snapshot_id, expected_type=type_hints["snapshot_id"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
+            check_type(argname="argument vpc_id", value=vpc_id, expected_type=type_hints["vpc_id"])
+            check_type(argname="argument v_switch_id", value=v_switch_id, expected_type=type_hints["v_switch_id"])
+            check_type(argname="argument zone_id", value=zone_id, expected_type=type_hints["zone_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "protocol_type": protocol_type,
             "storage_type": storage_type,
         }
         if bandwidth is not None:
             self._values["bandwidth"] = bandwidth
         if capacity is not None:
@@ -539,31 +588,37 @@
 ):
     '''A ROS resource type:  ``ALIYUN::NAS::MountTarget``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "MountTargetProps",
+        props: typing.Union["MountTargetProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::NAS::MountTarget``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(MountTarget.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrMountTargetDomain")
     def attr_mount_target_domain(self) -> ros_cdk_core.IResolvable:
         '''Attribute MountTargetDomain: Mount point domain name.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrMountTargetDomain"))
 
 
 @jsii.data_type(
@@ -594,14 +649,22 @@
         :param access_group_name: Property accessGroupName: Permission group name. Default to DEFAULT_VPC_GROUP_NAME.
         :param file_system_id: Property fileSystemId: File system ID.
         :param network_type: Property networkType: Network type, including Vpc and Classic networks.
         :param status: Property status: Status, including Active and Inactive.
         :param vpc_id: Property vpcId: VPC network ID.
         :param v_switch_id: Property vSwitchId: VSwitch ID.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(MountTargetProps.__init__)
+            check_type(argname="argument access_group_name", value=access_group_name, expected_type=type_hints["access_group_name"])
+            check_type(argname="argument file_system_id", value=file_system_id, expected_type=type_hints["file_system_id"])
+            check_type(argname="argument network_type", value=network_type, expected_type=type_hints["network_type"])
+            check_type(argname="argument status", value=status, expected_type=type_hints["status"])
+            check_type(argname="argument vpc_id", value=vpc_id, expected_type=type_hints["vpc_id"])
+            check_type(argname="argument v_switch_id", value=v_switch_id, expected_type=type_hints["v_switch_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "access_group_name": access_group_name,
             "file_system_id": file_system_id,
             "network_type": network_type,
         }
         if status is not None:
             self._values["status"] = status
@@ -677,109 +740,130 @@
 ):
     '''A ROS template type:  ``ALIYUN::NAS::AccessGroup``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosAccessGroupProps",
+        props: typing.Union["RosAccessGroupProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::NAS::AccessGroup``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosAccessGroup.__init__)
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
+            type_hints = typing.get_type_hints(RosAccessGroup._render_properties)
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
     @jsii.member(jsii_name="attrAccessGroupName")
     def attr_access_group_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: AccessGroupName: Permission group name
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAccessGroupName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="accessGroupName")
     def access_group_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: accessGroupName: Permission group name
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "accessGroupName"))
 
     @access_group_name.setter
     def access_group_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAccessGroup, "access_group_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "accessGroupName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="accessGroupType")
     def access_group_type(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: accessGroupType: Permission group type, including the Vpc and Classic types
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "accessGroupType"))
 
     @access_group_type.setter
     def access_group_type(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAccessGroup, "access_group_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "accessGroupType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAccessGroup, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="description")
     def description(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: description: Permission group description. It is the same as the permission group name by default.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "description"))
 
     @description.setter
     def description(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAccessGroup, "description").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "description", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-nas.RosAccessGroupProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -798,14 +882,19 @@
     ) -> None:
         '''Properties for defining a ``ALIYUN::NAS::AccessGroup``.
 
         :param access_group_name: 
         :param access_group_type: 
         :param description: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosAccessGroupProps.__init__)
+            check_type(argname="argument access_group_name", value=access_group_name, expected_type=type_hints["access_group_name"])
+            check_type(argname="argument access_group_type", value=access_group_type, expected_type=type_hints["access_group_type"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
         self._values: typing.Dict[str, typing.Any] = {
             "access_group_name": access_group_name,
             "access_group_type": access_group_type,
         }
         if description is not None:
             self._values["description"] = description
 
@@ -856,143 +945,170 @@
 ):
     '''A ROS template type:  ``ALIYUN::NAS::AccessRule``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosAccessRuleProps",
+        props: typing.Union["RosAccessRuleProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::NAS::AccessRule``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosAccessRule.__init__)
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
+            type_hints = typing.get_type_hints(RosAccessRule._render_properties)
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
     @jsii.member(jsii_name="attrAccessRuleId")
     def attr_access_rule_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: AccessRuleId: Rule serial number
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAccessRuleId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="accessGroupName")
     def access_group_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: accessGroupName: Permission group name
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "accessGroupName"))
 
     @access_group_name.setter
     def access_group_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAccessRule, "access_group_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "accessGroupName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAccessRule, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="sourceCidrIp")
     def source_cidr_ip(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: sourceCidrIp: Address or address segment
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "sourceCidrIp"))
 
     @source_cidr_ip.setter
     def source_cidr_ip(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAccessRule, "source_cidr_ip").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "sourceCidrIp", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="priority")
     def priority(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: priority: Priority level. Range: 1-100. Default value: 1
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "priority"))
 
     @priority.setter
     def priority(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAccessRule, "priority").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "priority", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rwAccessType")
     def rw_access_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: rwAccessType: Read-write permission type: RDWR (default), RDONLY
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "rwAccessType"))
 
     @rw_access_type.setter
     def rw_access_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAccessRule, "rw_access_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "rwAccessType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="userAccessType")
     def user_access_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: userAccessType: User permission type: no_squash (default), root_squash, all_squash
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "userAccessType"))
 
     @user_access_type.setter
     def user_access_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAccessRule, "user_access_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "userAccessType", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-nas.RosAccessRuleProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -1017,14 +1133,21 @@
 
         :param access_group_name: 
         :param source_cidr_ip: 
         :param priority: 
         :param rw_access_type: 
         :param user_access_type: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosAccessRuleProps.__init__)
+            check_type(argname="argument access_group_name", value=access_group_name, expected_type=type_hints["access_group_name"])
+            check_type(argname="argument source_cidr_ip", value=source_cidr_ip, expected_type=type_hints["source_cidr_ip"])
+            check_type(argname="argument priority", value=priority, expected_type=type_hints["priority"])
+            check_type(argname="argument rw_access_type", value=rw_access_type, expected_type=type_hints["rw_access_type"])
+            check_type(argname="argument user_access_type", value=user_access_type, expected_type=type_hints["user_access_type"])
         self._values: typing.Dict[str, typing.Any] = {
             "access_group_name": access_group_name,
             "source_cidr_ip": source_cidr_ip,
         }
         if priority is not None:
             self._values["priority"] = priority
         if rw_access_type is not None:
@@ -1099,129 +1222,153 @@
 ):
     '''A ROS template type:  ``ALIYUN::NAS::FileSystem``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosFileSystemProps",
+        props: typing.Union["RosFileSystemProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::NAS::FileSystem``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosFileSystem.__init__)
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
+            type_hints = typing.get_type_hints(RosFileSystem._render_properties)
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
     @jsii.member(jsii_name="attrFileSystemId")
     def attr_file_system_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: FileSystemId: ID of the file system created
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrFileSystemId"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosFileSystem, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="protocolType")
     def protocol_type(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: protocolType: Type of protocol used. Currently includes the NFS type and the SMB type
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "protocolType"))
 
     @protocol_type.setter
     def protocol_type(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosFileSystem, "protocol_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "protocolType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="storageType")
     def storage_type(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: storageType: The file system type. Currently includes the Performance type and the Capacity type
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "storageType"))
 
     @storage_type.setter
     def storage_type(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosFileSystem, "storage_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "storageType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="bandwidth")
     def bandwidth(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: bandwidth: Maximum file system throughput, unit is MB/s. Required and valid only when FileSystemType=cpfs.
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "bandwidth"))
 
     @bandwidth.setter
     def bandwidth(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosFileSystem, "bandwidth").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "bandwidth", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="capacity")
     def capacity(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: capacity: File system capacity, the unit is GB. Required and valid when FileSystemType=extreme or cpfs.
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "capacity"))
 
     @capacity.setter
     def capacity(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosFileSystem, "capacity").fset)
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
 
@@ -1232,51 +1379,60 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "chargeType"))
 
     @charge_type.setter
     def charge_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosFileSystem, "charge_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "chargeType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="deletionForce")
     def deletion_force(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property: deletionForce: Whether delete all mount targets on the file system and then delete file system. Default is false
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "deletionForce"))
 
     @deletion_force.setter
     def deletion_force(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosFileSystem, "deletion_force").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "deletionForce", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="description")
     def description(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: description: File system description (space characters are not allowed)
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "description"))
 
     @description.setter
     def description(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosFileSystem, "description").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "description", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="duration")
     def duration(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -1286,17 +1442,20 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "duration"))
 
     @duration.setter
     def duration(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosFileSystem, "duration").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "duration", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="encryptType")
     def encrypt_type(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -1307,114 +1466,135 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "encryptType"))
 
     @encrypt_type.setter
     def encrypt_type(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosFileSystem, "encrypt_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "encryptType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="fileSystemType")
     def file_system_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: fileSystemType: File system type. Allowed values: standard, extreme, cpfs
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "fileSystemType"))
 
     @file_system_type.setter
     def file_system_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosFileSystem, "file_system_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "fileSystemType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="snapshotId")
     def snapshot_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: snapshotId: Snapshot ID.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "snapshotId"))
 
     @snapshot_id.setter
     def snapshot_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosFileSystem, "snapshot_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "snapshotId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="tags")
     def tags(self) -> typing.Optional[typing.List["RosFileSystem.TagsProperty"]]:
         '''
         :Property: tags: Tags to attach to filesystem. Max support 20 tags to add during create filesystem. Each tag with two properties Key and Value, and Key is required.
         '''
         return typing.cast(typing.Optional[typing.List["RosFileSystem.TagsProperty"]], jsii.get(self, "tags"))
 
     @tags.setter
     def tags(
         self,
         value: typing.Optional[typing.List["RosFileSystem.TagsProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosFileSystem, "tags").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "tags", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vpcId")
     def vpc_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: vpcId: Vpc ID.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "vpcId"))
 
     @vpc_id.setter
     def vpc_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosFileSystem, "vpc_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "vpcId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vSwitchId")
     def v_switch_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: vSwitchId: VSwitch ID.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "vSwitchId"))
 
     @v_switch_id.setter
     def v_switch_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosFileSystem, "v_switch_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "vSwitchId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="zoneId")
     def zone_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: zoneId: Zone ID.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "zoneId"))
 
     @zone_id.setter
     def zone_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosFileSystem, "zone_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "zoneId", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-nas.RosFileSystem.TagsProperty",
         jsii_struct_bases=[],
         name_mapping={"key": "key", "value": "value"},
     )
@@ -1425,14 +1605,18 @@
             key: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param key: 
             :param value: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosFileSystem.TagsProperty.__init__)
+                check_type(argname="argument key", value=key, expected_type=type_hints["key"])
+                check_type(argname="argument value", value=value, expected_type=type_hints["value"])
             self._values: typing.Dict[str, typing.Any] = {
                 "key": key,
             }
             if value is not None:
                 self._values["value"] = value
 
         @builtins.property
@@ -1498,15 +1682,15 @@
         charge_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         deletion_force: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         description: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         duration: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         encrypt_type: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         file_system_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         snapshot_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        tags: typing.Optional[typing.Sequence[RosFileSystem.TagsProperty]] = None,
+        tags: typing.Optional[typing.Sequence[typing.Union[RosFileSystem.TagsProperty, typing.Dict[str, typing.Any]]]] = None,
         vpc_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         v_switch_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         zone_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::NAS::FileSystem``.
 
         :param protocol_type: 
@@ -1521,14 +1705,31 @@
         :param file_system_type: 
         :param snapshot_id: 
         :param tags: 
         :param vpc_id: 
         :param v_switch_id: 
         :param zone_id: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosFileSystemProps.__init__)
+            check_type(argname="argument protocol_type", value=protocol_type, expected_type=type_hints["protocol_type"])
+            check_type(argname="argument storage_type", value=storage_type, expected_type=type_hints["storage_type"])
+            check_type(argname="argument bandwidth", value=bandwidth, expected_type=type_hints["bandwidth"])
+            check_type(argname="argument capacity", value=capacity, expected_type=type_hints["capacity"])
+            check_type(argname="argument charge_type", value=charge_type, expected_type=type_hints["charge_type"])
+            check_type(argname="argument deletion_force", value=deletion_force, expected_type=type_hints["deletion_force"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument duration", value=duration, expected_type=type_hints["duration"])
+            check_type(argname="argument encrypt_type", value=encrypt_type, expected_type=type_hints["encrypt_type"])
+            check_type(argname="argument file_system_type", value=file_system_type, expected_type=type_hints["file_system_type"])
+            check_type(argname="argument snapshot_id", value=snapshot_id, expected_type=type_hints["snapshot_id"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
+            check_type(argname="argument vpc_id", value=vpc_id, expected_type=type_hints["vpc_id"])
+            check_type(argname="argument v_switch_id", value=v_switch_id, expected_type=type_hints["v_switch_id"])
+            check_type(argname="argument zone_id", value=zone_id, expected_type=type_hints["zone_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "protocol_type": protocol_type,
             "storage_type": storage_type,
         }
         if bandwidth is not None:
             self._values["bandwidth"] = bandwidth
         if capacity is not None:
@@ -1732,158 +1933,188 @@
 ):
     '''A ROS template type:  ``ALIYUN::NAS::MountTarget``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosMountTargetProps",
+        props: typing.Union["RosMountTargetProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::NAS::MountTarget``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosMountTarget.__init__)
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
+            type_hints = typing.get_type_hints(RosMountTarget._render_properties)
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
     @jsii.member(jsii_name="attrMountTargetDomain")
     def attr_mount_target_domain(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: MountTargetDomain: Mount point domain name
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrMountTargetDomain"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="accessGroupName")
     def access_group_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: accessGroupName: Permission group name. Default to DEFAULT_VPC_GROUP_NAME.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "accessGroupName"))
 
     @access_group_name.setter
     def access_group_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosMountTarget, "access_group_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "accessGroupName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosMountTarget, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="fileSystemId")
     def file_system_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: fileSystemId: File system ID
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "fileSystemId"))
 
     @file_system_id.setter
     def file_system_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosMountTarget, "file_system_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "fileSystemId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="networkType")
     def network_type(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: networkType: Network type, including Vpc and Classic networks.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "networkType"))
 
     @network_type.setter
     def network_type(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosMountTarget, "network_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "networkType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="status")
     def status(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: status: Status, including Active and Inactive
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "status"))
 
     @status.setter
     def status(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosMountTarget, "status").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "status", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vpcId")
     def vpc_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: vpcId: VPC network ID
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "vpcId"))
 
     @vpc_id.setter
     def vpc_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosMountTarget, "vpc_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "vpcId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vSwitchId")
     def v_switch_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: vSwitchId: VSwitch ID.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "vSwitchId"))
 
     @v_switch_id.setter
     def v_switch_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosMountTarget, "v_switch_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "vSwitchId", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-nas.RosMountTargetProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -1911,14 +2142,22 @@
         :param access_group_name: 
         :param file_system_id: 
         :param network_type: 
         :param status: 
         :param vpc_id: 
         :param v_switch_id: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosMountTargetProps.__init__)
+            check_type(argname="argument access_group_name", value=access_group_name, expected_type=type_hints["access_group_name"])
+            check_type(argname="argument file_system_id", value=file_system_id, expected_type=type_hints["file_system_id"])
+            check_type(argname="argument network_type", value=network_type, expected_type=type_hints["network_type"])
+            check_type(argname="argument status", value=status, expected_type=type_hints["status"])
+            check_type(argname="argument vpc_id", value=vpc_id, expected_type=type_hints["vpc_id"])
+            check_type(argname="argument v_switch_id", value=v_switch_id, expected_type=type_hints["v_switch_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "access_group_name": access_group_name,
             "file_system_id": file_system_id,
             "network_type": network_type,
         }
         if status is not None:
             self._values["status"] = status
```

### Comparing `ros-cdk-nas-1.0.8/src/ros_cdk_nas.egg-info/PKG-INFO` & `ros-cdk-nas-1.0.9/src/ros_cdk_nas.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-nas
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS NAS Construct Library
```

