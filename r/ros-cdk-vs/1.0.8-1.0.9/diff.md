# Comparing `tmp/ros-cdk-vs-1.0.8.tar.gz` & `tmp/ros-cdk-vs-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-vs-1.0.8.tar", last modified: Thu Jul 14 02:15:12 2022, max compression
+gzip compressed data, was "dist/ros-cdk-vs-1.0.9.tar", last modified: Fri Sep 23 12:19:47 2022, max compression
```

## Comparing `ros-cdk-vs-1.0.8.tar` & `ros-cdk-vs-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:15:12.000000 ros-cdk-vs-1.0.8/
--rw-r--r--   0 root         (0) root         (0)    10279 2022-07-14 02:15:12.000000 ros-cdk-vs-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2022-07-14 02:15:12.000000 ros-cdk-vs-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2022-07-14 02:15:12.000000 ros-cdk-vs-1.0.8/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1236 2022-07-14 02:15:12.000000 ros-cdk-vs-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      176 2022-07-14 02:15:12.000000 ros-cdk-vs-1.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)      106 2022-07-14 02:15:12.000000 ros-cdk-vs-1.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-07-14 02:15:12.000000 ros-cdk-vs-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1788 2022-07-14 02:15:12.000000 ros-cdk-vs-1.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:15:12.000000 ros-cdk-vs-1.0.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:15:12.000000 ros-cdk-vs-1.0.8/src/ros_cdk_vs/
--rw-r--r--   0 root         (0) root         (0)    27772 2022-07-14 02:15:12.000000 ros-cdk-vs-1.0.8/src/ros_cdk_vs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:15:12.000000 ros-cdk-vs-1.0.8/src/ros_cdk_vs/_jsii/
--rw-r--r--   0 root         (0) root         (0)      368 2022-07-14 02:15:12.000000 ros-cdk-vs-1.0.8/src/ros_cdk_vs/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32799 2022-07-14 02:15:12.000000 ros-cdk-vs-1.0.8/src/ros_cdk_vs/_jsii/ros-cdk-vs@1.0.8.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:15:12.000000 ros-cdk-vs-1.0.8/src/ros_cdk_vs/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:15:12.000000 ros-cdk-vs-1.0.8/src/ros_cdk_vs.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1236 2022-07-14 02:15:12.000000 ros-cdk-vs-1.0.8/src/ros_cdk_vs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      390 2022-07-14 02:15:12.000000 ros-cdk-vs-1.0.8/src/ros_cdk_vs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:15:12.000000 ros-cdk-vs-1.0.8/src/ros_cdk_vs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2022-07-14 02:15:12.000000 ros-cdk-vs-1.0.8/src/ros_cdk_vs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2022-07-14 02:15:12.000000 ros-cdk-vs-1.0.8/src/ros_cdk_vs.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:19:47.000000 ros-cdk-vs-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)    10279 2022-09-23 12:19:47.000000 ros-cdk-vs-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-09-23 12:19:47.000000 ros-cdk-vs-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2022-09-23 12:19:47.000000 ros-cdk-vs-1.0.9/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1236 2022-09-23 12:19:47.000000 ros-cdk-vs-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      176 2022-09-23 12:19:47.000000 ros-cdk-vs-1.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      236 2022-09-23 12:19:47.000000 ros-cdk-vs-1.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-09-23 12:19:47.000000 ros-cdk-vs-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1817 2022-09-23 12:19:47.000000 ros-cdk-vs-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:19:47.000000 ros-cdk-vs-1.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:19:47.000000 ros-cdk-vs-1.0.9/src/ros_cdk_vs/
+-rw-r--r--   0 root         (0) root         (0)    33739 2022-09-23 12:19:47.000000 ros-cdk-vs-1.0.9/src/ros_cdk_vs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:19:47.000000 ros-cdk-vs-1.0.9/src/ros_cdk_vs/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      402 2022-09-23 12:19:47.000000 ros-cdk-vs-1.0.9/src/ros_cdk_vs/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    32863 2022-09-23 12:19:47.000000 ros-cdk-vs-1.0.9/src/ros_cdk_vs/_jsii/ros-cdk-vs@1.0.9.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 12:19:47.000000 ros-cdk-vs-1.0.9/src/ros_cdk_vs/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:19:47.000000 ros-cdk-vs-1.0.9/src/ros_cdk_vs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1236 2022-09-23 12:19:47.000000 ros-cdk-vs-1.0.9/src/ros_cdk_vs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      390 2022-09-23 12:19:47.000000 ros-cdk-vs-1.0.9/src/ros_cdk_vs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 12:19:47.000000 ros-cdk-vs-1.0.9/src/ros_cdk_vs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2022-09-23 12:19:47.000000 ros-cdk-vs-1.0.9/src/ros_cdk_vs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2022-09-23 12:19:47.000000 ros-cdk-vs-1.0.9/src/ros_cdk_vs.egg-info/top_level.txt
```

### Comparing `ros-cdk-vs-1.0.8/LICENSE` & `ros-cdk-vs-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-vs-1.0.8/PKG-INFO` & `ros-cdk-vs-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-vs
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS VS Construct Library
```

### Comparing `ros-cdk-vs-1.0.8/setup.py` & `ros-cdk-vs-1.0.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-vs",
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
         "ros_cdk_vs",
         "ros_cdk_vs._jsii"
     ],
     "package_data": {
         "ros_cdk_vs._jsii": [
-            "ros-cdk-vs@1.0.8.jsii.tgz"
+            "ros-cdk-vs@1.0.9.jsii.tgz"
         ],
         "ros_cdk_vs": [
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

### Comparing `ros-cdk-vs-1.0.8/src/ros_cdk_vs/__init__.py` & `ros-cdk-vs-1.0.9/src/ros_cdk_vs/__init__.py`

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
 
 
 class Group(
     ros_cdk_core.Resource,
@@ -29,58 +31,64 @@
 ):
     '''A ROS resource type:  ``ALIYUN::VS::Group``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "GroupProps",
+        props: typing.Union["GroupProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::VS::Group``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(Group.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrGbId")
     def attr_gb_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute GbId: GB ID space provided.
 
         (Applies only to access the space marked States)
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrGbId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrGbIp")
     def attr_gb_ip(self) -> ros_cdk_core.IResolvable:
         '''Attribute GbIp: GB signaling server address space provided.
 
         (Applies only to access the space marked States)
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrGbIp"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrGbPort")
     def attr_gb_port(self) -> ros_cdk_core.IResolvable:
         '''Attribute GbPort: GB Port space provided.
 
         (Applies only to access the space marked States)
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrGbPort"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrId")
     def attr_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute Id: Space ID.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrId"))
 
 
 @jsii.data_type(
@@ -126,14 +134,27 @@
         :param region: Property region: Space belongs to the region, as a service center.
         :param app: Property app: Application name space used, the default live.
         :param callback: Property callback: Updating the space callback device / flow state.
         :param description: Property description: Space description.
         :param enabled: Property enabled: Space is enabled.
         :param lazy_pull: Property lazyPull: Whether to enable on-demand pull flow, default false.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(GroupProps.__init__)
+            check_type(argname="argument in_protocol", value=in_protocol, expected_type=type_hints["in_protocol"])
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+            check_type(argname="argument out_protocol", value=out_protocol, expected_type=type_hints["out_protocol"])
+            check_type(argname="argument play_domain", value=play_domain, expected_type=type_hints["play_domain"])
+            check_type(argname="argument push_domain", value=push_domain, expected_type=type_hints["push_domain"])
+            check_type(argname="argument region", value=region, expected_type=type_hints["region"])
+            check_type(argname="argument app", value=app, expected_type=type_hints["app"])
+            check_type(argname="argument callback", value=callback, expected_type=type_hints["callback"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument enabled", value=enabled, expected_type=type_hints["enabled"])
+            check_type(argname="argument lazy_pull", value=lazy_pull, expected_type=type_hints["lazy_pull"])
         self._values: typing.Dict[str, typing.Any] = {
             "in_protocol": in_protocol,
             "name": name,
             "out_protocol": out_protocol,
             "play_domain": play_domain,
             "push_domain": push_domain,
             "region": region,
@@ -259,89 +280,101 @@
 ):
     '''A ROS template type:  ``ALIYUN::VS::Group``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosGroupProps",
+        props: typing.Union["RosGroupProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::VS::Group``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosGroup.__init__)
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
+            type_hints = typing.get_type_hints(RosGroup._render_properties)
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
     @jsii.member(jsii_name="attrGbId")
     def attr_gb_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: GbId: GB ID space provided. (Applies only to access the space marked States)
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrGbId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrGbIp")
     def attr_gb_ip(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: GbIp: GB signaling server address space provided. (Applies only to access the space marked States)
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrGbIp"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrGbPort")
     def attr_gb_port(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: GbPort: GB Port space provided. (Applies only to access the space marked States)
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrGbPort"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrId")
     def attr_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Id: Space ID.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrId"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosGroup, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="inProtocol")
     def in_protocol(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         inProtocol: Access protocol used by the space.
         Value: gb28181, rtmp
@@ -349,29 +382,35 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "inProtocol"))
 
     @in_protocol.setter
     def in_protocol(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosGroup, "in_protocol").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "inProtocol", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="name")
     def name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: name: Space name.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "name"))
 
     @name.setter
     def name(self, value: typing.Union[builtins.str, ros_cdk_core.IResolvable]) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosGroup, "name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "name", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="outProtocol")
     def out_protocol(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         outProtocol: Play protocol used by the space, multivalued separated by commas.
         Value: flv, hls, rtmp
@@ -379,144 +418,171 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "outProtocol"))
 
     @out_protocol.setter
     def out_protocol(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosGroup, "out_protocol").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "outProtocol", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="playDomain")
     def play_domain(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: playDomain: Use of the domain name space broadcast stream.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "playDomain"))
 
     @play_domain.setter
     def play_domain(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosGroup, "play_domain").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "playDomain", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="pushDomain")
     def push_domain(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: pushDomain: Plug flow domain name space to use. (Only access to the space rtmp)
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "pushDomain"))
 
     @push_domain.setter
     def push_domain(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosGroup, "push_domain").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "pushDomain", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="region")
     def region(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: region: Space belongs to the region, as a service center.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "region"))
 
     @region.setter
     def region(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosGroup, "region").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "region", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="app")
     def app(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: app: Application name space used, the default live.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "app"))
 
     @app.setter
     def app(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosGroup, "app").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "app", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="callback")
     def callback(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: callback: Updating the space callback device / flow state
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "callback"))
 
     @callback.setter
     def callback(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosGroup, "callback").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "callback", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="description")
     def description(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: description: Space description.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "description"))
 
     @description.setter
     def description(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosGroup, "description").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "description", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enabled")
     def enabled(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property: enabled: Space is enabled.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "enabled"))
 
     @enabled.setter
     def enabled(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosGroup, "enabled").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enabled", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="lazyPull")
     def lazy_pull(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property: lazyPull: Whether to enable on-demand pull flow, default false
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "lazyPull"))
 
     @lazy_pull.setter
     def lazy_pull(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosGroup, "lazy_pull").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "lazyPull", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-vs.RosGroupProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -559,14 +625,27 @@
         :param region: 
         :param app: 
         :param callback: 
         :param description: 
         :param enabled: 
         :param lazy_pull: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosGroupProps.__init__)
+            check_type(argname="argument in_protocol", value=in_protocol, expected_type=type_hints["in_protocol"])
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+            check_type(argname="argument out_protocol", value=out_protocol, expected_type=type_hints["out_protocol"])
+            check_type(argname="argument play_domain", value=play_domain, expected_type=type_hints["play_domain"])
+            check_type(argname="argument push_domain", value=push_domain, expected_type=type_hints["push_domain"])
+            check_type(argname="argument region", value=region, expected_type=type_hints["region"])
+            check_type(argname="argument app", value=app, expected_type=type_hints["app"])
+            check_type(argname="argument callback", value=callback, expected_type=type_hints["callback"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument enabled", value=enabled, expected_type=type_hints["enabled"])
+            check_type(argname="argument lazy_pull", value=lazy_pull, expected_type=type_hints["lazy_pull"])
         self._values: typing.Dict[str, typing.Any] = {
             "in_protocol": in_protocol,
             "name": name,
             "out_protocol": out_protocol,
             "play_domain": play_domain,
             "push_domain": push_domain,
             "region": region,
```

### Comparing `ros-cdk-vs-1.0.8/src/ros_cdk_vs.egg-info/PKG-INFO` & `ros-cdk-vs-1.0.9/src/ros_cdk_vs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-vs
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS VS Construct Library
```

