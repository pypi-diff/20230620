# Comparing `tmp/ros-cdk-mps-1.0.8.tar.gz` & `tmp/ros-cdk-mps-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-mps-1.0.8.tar", last modified: Thu Jul 14 02:34:28 2022, max compression
+gzip compressed data, was "dist/ros-cdk-mps-1.0.9.tar", last modified: Fri Sep 23 11:23:55 2022, max compression
```

## Comparing `ros-cdk-mps-1.0.8.tar` & `ros-cdk-mps-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:34:28.000000 ros-cdk-mps-1.0.8/
--rw-r--r--   0 root         (0) root         (0)    10279 2022-07-14 02:34:28.000000 ros-cdk-mps-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2022-07-14 02:34:28.000000 ros-cdk-mps-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2022-07-14 02:34:28.000000 ros-cdk-mps-1.0.8/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1240 2022-07-14 02:34:28.000000 ros-cdk-mps-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      179 2022-07-14 02:34:28.000000 ros-cdk-mps-1.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)      106 2022-07-14 02:34:28.000000 ros-cdk-mps-1.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-07-14 02:34:28.000000 ros-cdk-mps-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1794 2022-07-14 02:34:28.000000 ros-cdk-mps-1.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:34:28.000000 ros-cdk-mps-1.0.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:34:28.000000 ros-cdk-mps-1.0.8/src/ros_cdk_mps/
--rw-r--r--   0 root         (0) root         (0)    22332 2022-07-14 02:34:28.000000 ros-cdk-mps-1.0.8/src/ros_cdk_mps/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:34:28.000000 ros-cdk-mps-1.0.8/src/ros_cdk_mps/_jsii/
--rw-r--r--   0 root         (0) root         (0)      370 2022-07-14 02:34:28.000000 ros-cdk-mps-1.0.8/src/ros_cdk_mps/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    33182 2022-07-14 02:34:28.000000 ros-cdk-mps-1.0.8/src/ros_cdk_mps/_jsii/ros-cdk-mps@1.0.8.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:34:28.000000 ros-cdk-mps-1.0.8/src/ros_cdk_mps/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:34:28.000000 ros-cdk-mps-1.0.8/src/ros_cdk_mps.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1240 2022-07-14 02:34:28.000000 ros-cdk-mps-1.0.8/src/ros_cdk_mps.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      400 2022-07-14 02:34:28.000000 ros-cdk-mps-1.0.8/src/ros_cdk_mps.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:34:28.000000 ros-cdk-mps-1.0.8/src/ros_cdk_mps.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2022-07-14 02:34:28.000000 ros-cdk-mps-1.0.8/src/ros_cdk_mps.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2022-07-14 02:34:28.000000 ros-cdk-mps-1.0.8/src/ros_cdk_mps.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:23:55.000000 ros-cdk-mps-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)    10279 2022-09-23 11:23:55.000000 ros-cdk-mps-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-09-23 11:23:55.000000 ros-cdk-mps-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2022-09-23 11:23:55.000000 ros-cdk-mps-1.0.9/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1240 2022-09-23 11:23:55.000000 ros-cdk-mps-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      179 2022-09-23 11:23:55.000000 ros-cdk-mps-1.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      236 2022-09-23 11:23:55.000000 ros-cdk-mps-1.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-09-23 11:23:55.000000 ros-cdk-mps-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1823 2022-09-23 11:23:55.000000 ros-cdk-mps-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:23:55.000000 ros-cdk-mps-1.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:23:55.000000 ros-cdk-mps-1.0.9/src/ros_cdk_mps/
+-rw-r--r--   0 root         (0) root         (0)    26844 2022-09-23 11:23:55.000000 ros-cdk-mps-1.0.9/src/ros_cdk_mps/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:23:55.000000 ros-cdk-mps-1.0.9/src/ros_cdk_mps/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      404 2022-09-23 11:23:55.000000 ros-cdk-mps-1.0.9/src/ros_cdk_mps/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    33247 2022-09-23 11:23:55.000000 ros-cdk-mps-1.0.9/src/ros_cdk_mps/_jsii/ros-cdk-mps@1.0.9.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 11:23:55.000000 ros-cdk-mps-1.0.9/src/ros_cdk_mps/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:23:55.000000 ros-cdk-mps-1.0.9/src/ros_cdk_mps.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1240 2022-09-23 11:23:55.000000 ros-cdk-mps-1.0.9/src/ros_cdk_mps.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      400 2022-09-23 11:23:55.000000 ros-cdk-mps-1.0.9/src/ros_cdk_mps.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 11:23:55.000000 ros-cdk-mps-1.0.9/src/ros_cdk_mps.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2022-09-23 11:23:55.000000 ros-cdk-mps-1.0.9/src/ros_cdk_mps.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2022-09-23 11:23:55.000000 ros-cdk-mps-1.0.9/src/ros_cdk_mps.egg-info/top_level.txt
```

### Comparing `ros-cdk-mps-1.0.8/LICENSE` & `ros-cdk-mps-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-mps-1.0.8/PKG-INFO` & `ros-cdk-mps-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-mps
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS MPS Construct Library
```

### Comparing `ros-cdk-mps-1.0.8/setup.py` & `ros-cdk-mps-1.0.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-mps",
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
         "ros_cdk_mps",
         "ros_cdk_mps._jsii"
     ],
     "package_data": {
         "ros_cdk_mps._jsii": [
-            "ros-cdk-mps@1.0.8.jsii.tgz"
+            "ros-cdk-mps@1.0.9.jsii.tgz"
         ],
         "ros_cdk_mps": [
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

### Comparing `ros-cdk-mps-1.0.8/src/ros_cdk_mps/__init__.py` & `ros-cdk-mps-1.0.9/src/ros_cdk_mps/__init__.py`

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
 
 
 class Pipeline(
     ros_cdk_core.Resource,
@@ -29,31 +31,37 @@
 ):
     '''A ROS resource type:  ``ALIYUN::MPS::Pipeline``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "PipelineProps",
+        props: typing.Union["PipelineProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::MPS::Pipeline``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(Pipeline.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPipelineId")
     def attr_pipeline_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute PipelineId: The ID of the MPS queue.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPipelineId"))
 
 
 @jsii.data_type(
@@ -69,29 +77,37 @@
     },
 )
 class PipelineProps:
     def __init__(
         self,
         *,
         name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
-        notify_config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosPipeline.NotifyConfigProperty"]] = None,
+        notify_config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosPipeline.NotifyConfigProperty", typing.Dict[str, typing.Any]]]] = None,
         role: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         speed: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         speed_level: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         state: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::MPS::Pipeline``.
 
         :param name: Property name: The new name of the MPS queue. The value can contain letters, digits, and special characters such as hyphens (-) and can be up to 128 bytes in size. The value cannot start with a special character.
         :param notify_config: Property notifyConfig: The Message Service (MNS) configuration, such as the information about the MNS queue or topic. For more information, see NotifyConfig.
         :param role: Property role: The role that is assigned to the current RAM user. To obtain the role, you can log on to the RAM console and choose Identities > Roles in the left-side navigation pane.
         :param speed: Property speed: Pipe type. Value: Boost: Double-speed transcoding Standard: ordinary pipe NarrowBandHDV2: Narrowband HD 2.0 AIVideoCover: Smart Screenshots AIVideoTag: video tag (supports regions Shanghai, Beijing, Hangzhou). Default: Standard.
         :param speed_level: Property speedLevel: Speed level.
         :param state: Property state: The new state of the MPS queue. Active: The MPS queue is active. Jobs in the MPS queue can be scheduled and run by MPS. Paused: The MPS queue is paused. Jobs in the MPS queue cannot be scheduled or run by MPS, and all jobs remain in the Submitted state. Jobs that are running will not be affected.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(PipelineProps.__init__)
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+            check_type(argname="argument notify_config", value=notify_config, expected_type=type_hints["notify_config"])
+            check_type(argname="argument role", value=role, expected_type=type_hints["role"])
+            check_type(argname="argument speed", value=speed, expected_type=type_hints["speed"])
+            check_type(argname="argument speed_level", value=speed_level, expected_type=type_hints["speed_level"])
+            check_type(argname="argument state", value=state, expected_type=type_hints["state"])
         self._values: typing.Dict[str, typing.Any] = {
             "name": name,
         }
         if notify_config is not None:
             self._values["notify_config"] = notify_config
         if role is not None:
             self._values["role"] = role
@@ -192,81 +208,96 @@
 ):
     '''A ROS template type:  ``ALIYUN::MPS::Pipeline``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosPipelineProps",
+        props: typing.Union["RosPipelineProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::MPS::Pipeline``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosPipeline.__init__)
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
+            type_hints = typing.get_type_hints(RosPipeline._render_properties)
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
     @jsii.member(jsii_name="attrPipelineId")
     def attr_pipeline_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: PipelineId: The ID of the MPS queue.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPipelineId"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosPipeline, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="name")
     def name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         name: The new name of the MPS queue. The value can contain letters, digits, and special
         characters such as hyphens (-) and can be up to 128 bytes in size. The value cannot
         start with a special character.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "name"))
 
     @name.setter
     def name(self, value: typing.Union[builtins.str, ros_cdk_core.IResolvable]) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPipeline, "name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "name", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="notifyConfig")
     def notify_config(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosPipeline.NotifyConfigProperty"]]:
         '''
         :Property:
 
@@ -276,34 +307,40 @@
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosPipeline.NotifyConfigProperty"]], jsii.get(self, "notifyConfig"))
 
     @notify_config.setter
     def notify_config(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosPipeline.NotifyConfigProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPipeline, "notify_config").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "notifyConfig", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="role")
     def role(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: role: The role that is assigned to the current RAM user. To obtain the role, you can log on to the RAM console and choose Identities > Roles in the left-side navigation pane.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "role"))
 
     @role.setter
     def role(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPipeline, "role").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "role", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="speed")
     def speed(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -318,34 +355,40 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "speed"))
 
     @speed.setter
     def speed(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPipeline, "speed").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "speed", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="speedLevel")
     def speed_level(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: speedLevel: Speed level.
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "speedLevel"))
 
     @speed_level.setter
     def speed_level(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPipeline, "speed_level").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "speedLevel", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="state")
     def state(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -356,14 +399,17 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "state"))
 
     @state.setter
     def state(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPipeline, "state").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "state", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-mps.RosPipeline.NotifyConfigProperty",
         jsii_struct_bases=[],
         name_mapping={"queue_name": "queueName", "topic": "topic"},
     )
@@ -374,14 +420,18 @@
             queue_name: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
             topic: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param queue_name: 
             :param topic: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosPipeline.NotifyConfigProperty.__init__)
+                check_type(argname="argument queue_name", value=queue_name, expected_type=type_hints["queue_name"])
+                check_type(argname="argument topic", value=topic, expected_type=type_hints["topic"])
             self._values: typing.Dict[str, typing.Any] = {}
             if queue_name is not None:
                 self._values["queue_name"] = queue_name
             if topic is not None:
                 self._values["topic"] = topic
 
         @builtins.property
@@ -429,29 +479,37 @@
     },
 )
 class RosPipelineProps:
     def __init__(
         self,
         *,
         name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
-        notify_config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, RosPipeline.NotifyConfigProperty]] = None,
+        notify_config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosPipeline.NotifyConfigProperty, typing.Dict[str, typing.Any]]]] = None,
         role: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         speed: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         speed_level: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         state: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::MPS::Pipeline``.
 
         :param name: 
         :param notify_config: 
         :param role: 
         :param speed: 
         :param speed_level: 
         :param state: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosPipelineProps.__init__)
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+            check_type(argname="argument notify_config", value=notify_config, expected_type=type_hints["notify_config"])
+            check_type(argname="argument role", value=role, expected_type=type_hints["role"])
+            check_type(argname="argument speed", value=speed, expected_type=type_hints["speed"])
+            check_type(argname="argument speed_level", value=speed_level, expected_type=type_hints["speed_level"])
+            check_type(argname="argument state", value=state, expected_type=type_hints["state"])
         self._values: typing.Dict[str, typing.Any] = {
             "name": name,
         }
         if notify_config is not None:
             self._values["notify_config"] = notify_config
         if role is not None:
             self._values["role"] = role
```

### Comparing `ros-cdk-mps-1.0.8/src/ros_cdk_mps.egg-info/PKG-INFO` & `ros-cdk-mps-1.0.9/src/ros_cdk_mps.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-mps
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS MPS Construct Library
```

