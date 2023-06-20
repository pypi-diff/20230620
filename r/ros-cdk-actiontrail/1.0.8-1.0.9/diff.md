# Comparing `tmp/ros-cdk-actiontrail-1.0.8.tar.gz` & `tmp/ros-cdk-actiontrail-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-actiontrail-1.0.8.tar", last modified: Thu Jul 14 02:42:34 2022, max compression
+gzip compressed data, was "dist/ros-cdk-actiontrail-1.0.9.tar", last modified: Fri Sep 23 11:39:34 2022, max compression
```

## Comparing `ros-cdk-actiontrail-1.0.8.tar` & `ros-cdk-actiontrail-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:42:34.000000 ros-cdk-actiontrail-1.0.8/
--rw-r--r--   0 root         (0) root         (0)    10279 2022-07-14 02:42:34.000000 ros-cdk-actiontrail-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2022-07-14 02:42:34.000000 ros-cdk-actiontrail-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2022-07-14 02:42:34.000000 ros-cdk-actiontrail-1.0.8/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1272 2022-07-14 02:42:34.000000 ros-cdk-actiontrail-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      203 2022-07-14 02:42:34.000000 ros-cdk-actiontrail-1.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)      106 2022-07-14 02:42:34.000000 ros-cdk-actiontrail-1.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-07-14 02:42:34.000000 ros-cdk-actiontrail-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1842 2022-07-14 02:42:34.000000 ros-cdk-actiontrail-1.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:42:34.000000 ros-cdk-actiontrail-1.0.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:42:34.000000 ros-cdk-actiontrail-1.0.8/src/ros_cdk_actiontrail/
--rw-r--r--   0 root         (0) root         (0)    31579 2022-07-14 02:42:34.000000 ros-cdk-actiontrail-1.0.8/src/ros_cdk_actiontrail/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:42:34.000000 ros-cdk-actiontrail-1.0.8/src/ros_cdk_actiontrail/_jsii/
--rw-r--r--   0 root         (0) root         (0)      399 2022-07-14 02:42:34.000000 ros-cdk-actiontrail-1.0.8/src/ros_cdk_actiontrail/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    35571 2022-07-14 02:42:34.000000 ros-cdk-actiontrail-1.0.8/src/ros_cdk_actiontrail/_jsii/ros-cdk-actiontrail@1.0.8.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:42:34.000000 ros-cdk-actiontrail-1.0.8/src/ros_cdk_actiontrail/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:42:34.000000 ros-cdk-actiontrail-1.0.8/src/ros_cdk_actiontrail.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1272 2022-07-14 02:42:34.000000 ros-cdk-actiontrail-1.0.8/src/ros_cdk_actiontrail.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      480 2022-07-14 02:42:34.000000 ros-cdk-actiontrail-1.0.8/src/ros_cdk_actiontrail.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:42:34.000000 ros-cdk-actiontrail-1.0.8/src/ros_cdk_actiontrail.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2022-07-14 02:42:34.000000 ros-cdk-actiontrail-1.0.8/src/ros_cdk_actiontrail.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2022-07-14 02:42:34.000000 ros-cdk-actiontrail-1.0.8/src/ros_cdk_actiontrail.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:39:34.000000 ros-cdk-actiontrail-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)    10279 2022-09-23 11:39:33.000000 ros-cdk-actiontrail-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-09-23 11:39:33.000000 ros-cdk-actiontrail-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2022-09-23 11:39:33.000000 ros-cdk-actiontrail-1.0.9/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1272 2022-09-23 11:39:34.000000 ros-cdk-actiontrail-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      203 2022-09-23 11:39:33.000000 ros-cdk-actiontrail-1.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      236 2022-09-23 11:39:33.000000 ros-cdk-actiontrail-1.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-09-23 11:39:34.000000 ros-cdk-actiontrail-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1871 2022-09-23 11:39:33.000000 ros-cdk-actiontrail-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:39:34.000000 ros-cdk-actiontrail-1.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:39:34.000000 ros-cdk-actiontrail-1.0.9/src/ros_cdk_actiontrail/
+-rw-r--r--   0 root         (0) root         (0)    38587 2022-09-23 11:39:33.000000 ros-cdk-actiontrail-1.0.9/src/ros_cdk_actiontrail/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:39:34.000000 ros-cdk-actiontrail-1.0.9/src/ros_cdk_actiontrail/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      433 2022-09-23 11:39:33.000000 ros-cdk-actiontrail-1.0.9/src/ros_cdk_actiontrail/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    35644 2022-09-23 11:39:33.000000 ros-cdk-actiontrail-1.0.9/src/ros_cdk_actiontrail/_jsii/ros-cdk-actiontrail@1.0.9.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 11:39:33.000000 ros-cdk-actiontrail-1.0.9/src/ros_cdk_actiontrail/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:39:34.000000 ros-cdk-actiontrail-1.0.9/src/ros_cdk_actiontrail.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1272 2022-09-23 11:39:34.000000 ros-cdk-actiontrail-1.0.9/src/ros_cdk_actiontrail.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      480 2022-09-23 11:39:34.000000 ros-cdk-actiontrail-1.0.9/src/ros_cdk_actiontrail.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 11:39:34.000000 ros-cdk-actiontrail-1.0.9/src/ros_cdk_actiontrail.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2022-09-23 11:39:34.000000 ros-cdk-actiontrail-1.0.9/src/ros_cdk_actiontrail.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2022-09-23 11:39:34.000000 ros-cdk-actiontrail-1.0.9/src/ros_cdk_actiontrail.egg-info/top_level.txt
```

### Comparing `ros-cdk-actiontrail-1.0.8/LICENSE` & `ros-cdk-actiontrail-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-actiontrail-1.0.8/PKG-INFO` & `ros-cdk-actiontrail-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-actiontrail
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS ACTIONTRAIL Construct Library
```

### Comparing `ros-cdk-actiontrail-1.0.8/setup.py` & `ros-cdk-actiontrail-1.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-actiontrail",
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
         "ros_cdk_actiontrail",
         "ros_cdk_actiontrail._jsii"
     ],
     "package_data": {
         "ros_cdk_actiontrail._jsii": [
-            "ros-cdk-actiontrail@1.0.8.jsii.tgz"
+            "ros-cdk-actiontrail@1.0.9.jsii.tgz"
         ],
         "ros_cdk_actiontrail": [
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

### Comparing `ros-cdk-actiontrail-1.0.8/src/ros_cdk_actiontrail/__init__.py` & `ros-cdk-actiontrail-1.0.9/src/ros_cdk_actiontrail/__init__.py`

 * *Files 15% similar despite different names*

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
 
 
 class RosTrail(
     ros_cdk_core.RosResource,
@@ -29,293 +31,344 @@
 ):
     '''A ROS template type:  ``ALIYUN::ACTIONTRAIL::Trail``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosTrailProps",
+        props: typing.Union["RosTrailProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::ACTIONTRAIL::Trail``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosTrail.__init__)
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
+            type_hints = typing.get_type_hints(RosTrail._render_properties)
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
     @jsii.member(jsii_name="attrName")
     def attr_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Name: The name of the trail to be created, which must be unique for an account.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrName"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosTrail, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="name")
     def name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: name: The name of the trail to be created, which must be unique for an account.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "name"))
 
     @name.setter
     def name(self, value: typing.Union[builtins.str, ros_cdk_core.IResolvable]) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTrail, "name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "name", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="ossBucketName")
     def oss_bucket_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: ossBucketName: The OSS bucket to which the trail delivers logs. Ensure that this is an existing OSS bucket.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "ossBucketName"))
 
     @oss_bucket_name.setter
     def oss_bucket_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTrail, "oss_bucket_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "ossBucketName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="roleName")
     def role_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: roleName: The RAM role in ActionTrail permitted by the user.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "roleName"))
 
     @role_name.setter
     def role_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTrail, "role_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "roleName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="eventRw")
     def event_rw(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: eventRw: Indicates whether the event is a read or a write event. Valid values: Read, Write, and All. Default value: Write.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "eventRw"))
 
     @event_rw.setter
     def event_rw(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTrail, "event_rw").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "eventRw", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="ossKeyPrefix")
     def oss_key_prefix(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: ossKeyPrefix: The prefix of the specified OSS bucket name. This parameter can be left empty.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "ossKeyPrefix"))
 
     @oss_key_prefix.setter
     def oss_key_prefix(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTrail, "oss_key_prefix").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "ossKeyPrefix", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="slsProjectArn")
     def sls_project_arn(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: slsProjectArn: The unique ARN of the Log Service project.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "slsProjectArn"))
 
     @sls_project_arn.setter
     def sls_project_arn(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTrail, "sls_project_arn").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "slsProjectArn", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="slsWriteRoleArn")
     def sls_write_role_arn(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: slsWriteRoleArn: The unique ARN of the Log Service role.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "slsWriteRoleArn"))
 
     @sls_write_role_arn.setter
     def sls_write_role_arn(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTrail, "sls_write_role_arn").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "slsWriteRoleArn", value)
 
 
 class RosTrailLogging(
     ros_cdk_core.RosResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@alicloud/ros-cdk-actiontrail.RosTrailLogging",
 ):
     '''A ROS template type:  ``ALIYUN::ACTIONTRAIL::TrailLogging``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosTrailLoggingProps",
+        props: typing.Union["RosTrailLoggingProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::ACTIONTRAIL::TrailLogging``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosTrailLogging.__init__)
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
+            type_hints = typing.get_type_hints(RosTrailLogging._render_properties)
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
     @jsii.member(jsii_name="attrIsLogging")
     def attr_is_logging(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: IsLogging: Indicates whether the trail is logging API invocations.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrIsLogging"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrLatestDeliveryError")
     def attr_latest_delivery_error(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: LatestDeliveryError: The last time an error occurred when the trail attempted to deliver log files.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrLatestDeliveryError"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrLatestDeliveryTime")
     def attr_latest_delivery_time(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: LatestDeliveryTime: The date and time of the last successful delivery of a log file.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrLatestDeliveryTime"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrStartLoggingTime")
     def attr_start_logging_time(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: StartLoggingTime: The most recent date and time when the user enables the trail.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrStartLoggingTime"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrStopLoggingTime")
     def attr_stop_logging_time(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: StopLoggingTime: The most recent date and time when the user disables the trail.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrStopLoggingTime"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enable")
     def enable(self) -> typing.Union[builtins.bool, ros_cdk_core.IResolvable]:
         '''
         :Property: enable: Whether to enable the trail logging.
         '''
         return typing.cast(typing.Union[builtins.bool, ros_cdk_core.IResolvable], jsii.get(self, "enable"))
 
     @enable.setter
     def enable(
         self,
         value: typing.Union[builtins.bool, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTrailLogging, "enable").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enable", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTrailLogging, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="name")
     def name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: name: The name of the trail to be enabled.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "name"))
 
     @name.setter
     def name(self, value: typing.Union[builtins.str, ros_cdk_core.IResolvable]) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTrailLogging, "name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "name", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-actiontrail.RosTrailLoggingProps",
     jsii_struct_bases=[],
     name_mapping={"enable": "enable", "name": "name"},
@@ -328,14 +381,18 @@
         name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
         '''Properties for defining a ``ALIYUN::ACTIONTRAIL::TrailLogging``.
 
         :param enable: 
         :param name: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosTrailLoggingProps.__init__)
+            check_type(argname="argument enable", value=enable, expected_type=type_hints["enable"])
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
         self._values: typing.Dict[str, typing.Any] = {
             "enable": enable,
             "name": name,
         }
 
     @builtins.property
     def enable(self) -> typing.Union[builtins.bool, ros_cdk_core.IResolvable]:
@@ -398,14 +455,23 @@
         :param oss_bucket_name: 
         :param role_name: 
         :param event_rw: 
         :param oss_key_prefix: 
         :param sls_project_arn: 
         :param sls_write_role_arn: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosTrailProps.__init__)
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+            check_type(argname="argument oss_bucket_name", value=oss_bucket_name, expected_type=type_hints["oss_bucket_name"])
+            check_type(argname="argument role_name", value=role_name, expected_type=type_hints["role_name"])
+            check_type(argname="argument event_rw", value=event_rw, expected_type=type_hints["event_rw"])
+            check_type(argname="argument oss_key_prefix", value=oss_key_prefix, expected_type=type_hints["oss_key_prefix"])
+            check_type(argname="argument sls_project_arn", value=sls_project_arn, expected_type=type_hints["sls_project_arn"])
+            check_type(argname="argument sls_write_role_arn", value=sls_write_role_arn, expected_type=type_hints["sls_write_role_arn"])
         self._values: typing.Dict[str, typing.Any] = {
             "name": name,
             "oss_bucket_name": oss_bucket_name,
             "role_name": role_name,
         }
         if event_rw is not None:
             self._values["event_rw"] = event_rw
@@ -502,31 +568,37 @@
 ):
     '''A ROS resource type:  ``ALIYUN::ACTIONTRAIL::Trail``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "TrailProps",
+        props: typing.Union["TrailProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::ACTIONTRAIL::Trail``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(Trail.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrName")
     def attr_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute Name: The name of the trail to be created, which must be unique for an account.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrName"))
 
 
 class TrailLogging(
@@ -536,55 +608,61 @@
 ):
     '''A ROS resource type:  ``ALIYUN::ACTIONTRAIL::TrailLogging``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "TrailLoggingProps",
+        props: typing.Union["TrailLoggingProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::ACTIONTRAIL::TrailLogging``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(TrailLogging.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrIsLogging")
     def attr_is_logging(self) -> ros_cdk_core.IResolvable:
         '''Attribute IsLogging: Indicates whether the trail is logging API invocations.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrIsLogging"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrLatestDeliveryError")
     def attr_latest_delivery_error(self) -> ros_cdk_core.IResolvable:
         '''Attribute LatestDeliveryError: The last time an error occurred when the trail attempted to deliver log files.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrLatestDeliveryError"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrLatestDeliveryTime")
     def attr_latest_delivery_time(self) -> ros_cdk_core.IResolvable:
         '''Attribute LatestDeliveryTime: The date and time of the last successful delivery of a log file.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrLatestDeliveryTime"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrStartLoggingTime")
     def attr_start_logging_time(self) -> ros_cdk_core.IResolvable:
         '''Attribute StartLoggingTime: The most recent date and time when the user enables the trail.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrStartLoggingTime"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrStopLoggingTime")
     def attr_stop_logging_time(self) -> ros_cdk_core.IResolvable:
         '''Attribute StopLoggingTime: The most recent date and time when the user disables the trail.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrStopLoggingTime"))
 
 
 @jsii.data_type(
@@ -600,14 +678,18 @@
         name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
         '''Properties for defining a ``ALIYUN::ACTIONTRAIL::TrailLogging``.
 
         :param enable: Property enable: Whether to enable the trail logging.
         :param name: Property name: The name of the trail to be enabled.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(TrailLoggingProps.__init__)
+            check_type(argname="argument enable", value=enable, expected_type=type_hints["enable"])
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
         self._values: typing.Dict[str, typing.Any] = {
             "enable": enable,
             "name": name,
         }
 
     @builtins.property
     def enable(self) -> typing.Union[builtins.bool, ros_cdk_core.IResolvable]:
@@ -666,14 +748,23 @@
         :param oss_bucket_name: Property ossBucketName: The OSS bucket to which the trail delivers logs. Ensure that this is an existing OSS bucket.
         :param role_name: Property roleName: The RAM role in ActionTrail permitted by the user.
         :param event_rw: Property eventRw: Indicates whether the event is a read or a write event. Valid values: Read, Write, and All. Default value: Write.
         :param oss_key_prefix: Property ossKeyPrefix: The prefix of the specified OSS bucket name. This parameter can be left empty.
         :param sls_project_arn: Property slsProjectArn: The unique ARN of the Log Service project.
         :param sls_write_role_arn: Property slsWriteRoleArn: The unique ARN of the Log Service role.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(TrailProps.__init__)
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+            check_type(argname="argument oss_bucket_name", value=oss_bucket_name, expected_type=type_hints["oss_bucket_name"])
+            check_type(argname="argument role_name", value=role_name, expected_type=type_hints["role_name"])
+            check_type(argname="argument event_rw", value=event_rw, expected_type=type_hints["event_rw"])
+            check_type(argname="argument oss_key_prefix", value=oss_key_prefix, expected_type=type_hints["oss_key_prefix"])
+            check_type(argname="argument sls_project_arn", value=sls_project_arn, expected_type=type_hints["sls_project_arn"])
+            check_type(argname="argument sls_write_role_arn", value=sls_write_role_arn, expected_type=type_hints["sls_write_role_arn"])
         self._values: typing.Dict[str, typing.Any] = {
             "name": name,
             "oss_bucket_name": oss_bucket_name,
             "role_name": role_name,
         }
         if event_rw is not None:
             self._values["event_rw"] = event_rw
```

### Comparing `ros-cdk-actiontrail-1.0.8/src/ros_cdk_actiontrail.egg-info/PKG-INFO` & `ros-cdk-actiontrail-1.0.9/src/ros_cdk_actiontrail.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-actiontrail
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS ACTIONTRAIL Construct Library
```

