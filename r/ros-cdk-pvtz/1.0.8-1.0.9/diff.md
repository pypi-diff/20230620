# Comparing `tmp/ros-cdk-pvtz-1.0.8.tar.gz` & `tmp/ros-cdk-pvtz-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-pvtz-1.0.8.tar", last modified: Thu Jul 14 02:39:44 2022, max compression
+gzip compressed data, was "dist/ros-cdk-pvtz-1.0.9.tar", last modified: Fri Sep 23 10:50:19 2022, max compression
```

## Comparing `ros-cdk-pvtz-1.0.8.tar` & `ros-cdk-pvtz-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:39:44.000000 ros-cdk-pvtz-1.0.8/
--rw-r--r--   0 root         (0) root         (0)    10279 2022-07-14 02:39:44.000000 ros-cdk-pvtz-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2022-07-14 02:39:44.000000 ros-cdk-pvtz-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2022-07-14 02:39:44.000000 ros-cdk-pvtz-1.0.8/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1244 2022-07-14 02:39:44.000000 ros-cdk-pvtz-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      182 2022-07-14 02:39:44.000000 ros-cdk-pvtz-1.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)      106 2022-07-14 02:39:44.000000 ros-cdk-pvtz-1.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-07-14 02:39:44.000000 ros-cdk-pvtz-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1800 2022-07-14 02:39:44.000000 ros-cdk-pvtz-1.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:39:44.000000 ros-cdk-pvtz-1.0.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:39:44.000000 ros-cdk-pvtz-1.0.8/src/ros_cdk_pvtz/
--rw-r--r--   0 root         (0) root         (0)    73629 2022-07-14 02:39:44.000000 ros-cdk-pvtz-1.0.8/src/ros_cdk_pvtz/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:39:44.000000 ros-cdk-pvtz-1.0.8/src/ros_cdk_pvtz/_jsii/
--rw-r--r--   0 root         (0) root         (0)      372 2022-07-14 02:39:44.000000 ros-cdk-pvtz-1.0.8/src/ros_cdk_pvtz/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    51085 2022-07-14 02:39:44.000000 ros-cdk-pvtz-1.0.8/src/ros_cdk_pvtz/_jsii/ros-cdk-pvtz@1.0.8.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:39:44.000000 ros-cdk-pvtz-1.0.8/src/ros_cdk_pvtz/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:39:44.000000 ros-cdk-pvtz-1.0.8/src/ros_cdk_pvtz.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1244 2022-07-14 02:39:44.000000 ros-cdk-pvtz-1.0.8/src/ros_cdk_pvtz.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      410 2022-07-14 02:39:44.000000 ros-cdk-pvtz-1.0.8/src/ros_cdk_pvtz.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:39:44.000000 ros-cdk-pvtz-1.0.8/src/ros_cdk_pvtz.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2022-07-14 02:39:44.000000 ros-cdk-pvtz-1.0.8/src/ros_cdk_pvtz.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2022-07-14 02:39:44.000000 ros-cdk-pvtz-1.0.8/src/ros_cdk_pvtz.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 10:50:19.000000 ros-cdk-pvtz-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)    10279 2022-09-23 10:50:19.000000 ros-cdk-pvtz-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-09-23 10:50:19.000000 ros-cdk-pvtz-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2022-09-23 10:50:19.000000 ros-cdk-pvtz-1.0.9/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1244 2022-09-23 10:50:19.000000 ros-cdk-pvtz-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      182 2022-09-23 10:50:19.000000 ros-cdk-pvtz-1.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      236 2022-09-23 10:50:19.000000 ros-cdk-pvtz-1.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-09-23 10:50:19.000000 ros-cdk-pvtz-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1829 2022-09-23 10:50:19.000000 ros-cdk-pvtz-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 10:50:19.000000 ros-cdk-pvtz-1.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 10:50:19.000000 ros-cdk-pvtz-1.0.9/src/ros_cdk_pvtz/
+-rw-r--r--   0 root         (0) root         (0)    90130 2022-09-23 10:50:19.000000 ros-cdk-pvtz-1.0.9/src/ros_cdk_pvtz/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 10:50:19.000000 ros-cdk-pvtz-1.0.9/src/ros_cdk_pvtz/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      406 2022-09-23 10:50:19.000000 ros-cdk-pvtz-1.0.9/src/ros_cdk_pvtz/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    51142 2022-09-23 10:50:19.000000 ros-cdk-pvtz-1.0.9/src/ros_cdk_pvtz/_jsii/ros-cdk-pvtz@1.0.9.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 10:50:19.000000 ros-cdk-pvtz-1.0.9/src/ros_cdk_pvtz/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 10:50:19.000000 ros-cdk-pvtz-1.0.9/src/ros_cdk_pvtz.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1244 2022-09-23 10:50:19.000000 ros-cdk-pvtz-1.0.9/src/ros_cdk_pvtz.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      410 2022-09-23 10:50:19.000000 ros-cdk-pvtz-1.0.9/src/ros_cdk_pvtz.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 10:50:19.000000 ros-cdk-pvtz-1.0.9/src/ros_cdk_pvtz.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2022-09-23 10:50:19.000000 ros-cdk-pvtz-1.0.9/src/ros_cdk_pvtz.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2022-09-23 10:50:19.000000 ros-cdk-pvtz-1.0.9/src/ros_cdk_pvtz.egg-info/top_level.txt
```

### Comparing `ros-cdk-pvtz-1.0.8/LICENSE` & `ros-cdk-pvtz-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-pvtz-1.0.8/PKG-INFO` & `ros-cdk-pvtz-1.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-pvtz
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS PVTZ Construct Library
```

### Comparing `ros-cdk-pvtz-1.0.8/setup.py` & `ros-cdk-pvtz-1.0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-pvtz",
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
         "ros_cdk_pvtz",
         "ros_cdk_pvtz._jsii"
     ],
     "package_data": {
         "ros_cdk_pvtz._jsii": [
-            "ros-cdk-pvtz@1.0.8.jsii.tgz"
+            "ros-cdk-pvtz@1.0.9.jsii.tgz"
         ],
         "ros_cdk_pvtz": [
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

### Comparing `ros-cdk-pvtz-1.0.8/src/ros_cdk_pvtz/__init__.py` & `ros-cdk-pvtz-1.0.9/src/ros_cdk_pvtz/__init__.py`

 * *Files 18% similar despite different names*

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
 
 
 class RosUserVpcAuthorization(
     ros_cdk_core.RosResource,
@@ -29,90 +31,105 @@
 ):
     '''A ROS template type:  ``ALIYUN::PVTZ::UserVpcAuthorization``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosUserVpcAuthorizationProps",
+        props: typing.Union["RosUserVpcAuthorizationProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::PVTZ::UserVpcAuthorization``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosUserVpcAuthorization.__init__)
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
+            type_hints = typing.get_type_hints(RosUserVpcAuthorization._render_properties)
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
     @jsii.member(jsii_name="attrAuthorizedUserId")
     def attr_authorized_user_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: AuthorizedUserId: The account ID of the user who authorizes the resource.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAuthorizedUserId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrAuthType")
     def attr_auth_type(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: AuthType: Authorization type.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAuthType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="authorizedUserId")
     def authorized_user_id(
         self,
     ) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: authorizedUserId: The account ID of the user who authorizes the resource.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "authorizedUserId"))
 
     @authorized_user_id.setter
     def authorized_user_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosUserVpcAuthorization, "authorized_user_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "authorizedUserId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosUserVpcAuthorization, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="authChannel")
     def auth_channel(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -123,65 +140,77 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "authChannel"))
 
     @auth_channel.setter
     def auth_channel(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosUserVpcAuthorization, "auth_channel").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "authChannel", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="authCode")
     def auth_code(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: authCode: Verification code, if AuthChannel takes "AUTH_CODE" or is empty, it is mandatory.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "authCode"))
 
     @auth_code.setter
     def auth_code(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosUserVpcAuthorization, "auth_code").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "authCode", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="authType")
     def auth_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: authType: Authorization type.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "authType"))
 
     @auth_type.setter
     def auth_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosUserVpcAuthorization, "auth_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "authType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="ignoreDeletionForbidden")
     def ignore_deletion_forbidden(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property: ignoreDeletionForbidden: Whether to ignore following deletion forbidden errors when deleting:- UserAuth.DeleteForbidden.ZoneVpcExists
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "ignoreDeletionForbidden"))
 
     @ignore_deletion_forbidden.setter
     def ignore_deletion_forbidden(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosUserVpcAuthorization, "ignore_deletion_forbidden").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "ignoreDeletionForbidden", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-pvtz.RosUserVpcAuthorizationProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -206,14 +235,21 @@
 
         :param authorized_user_id: 
         :param auth_channel: 
         :param auth_code: 
         :param auth_type: 
         :param ignore_deletion_forbidden: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosUserVpcAuthorizationProps.__init__)
+            check_type(argname="argument authorized_user_id", value=authorized_user_id, expected_type=type_hints["authorized_user_id"])
+            check_type(argname="argument auth_channel", value=auth_channel, expected_type=type_hints["auth_channel"])
+            check_type(argname="argument auth_code", value=auth_code, expected_type=type_hints["auth_code"])
+            check_type(argname="argument auth_type", value=auth_type, expected_type=type_hints["auth_type"])
+            check_type(argname="argument ignore_deletion_forbidden", value=ignore_deletion_forbidden, expected_type=type_hints["ignore_deletion_forbidden"])
         self._values: typing.Dict[str, typing.Any] = {
             "authorized_user_id": authorized_user_id,
         }
         if auth_channel is not None:
             self._values["auth_channel"] = auth_channel
         if auth_code is not None:
             self._values["auth_code"] = auth_code
@@ -296,121 +332,139 @@
 ):
     '''A ROS template type:  ``ALIYUN::PVTZ::Zone``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosZoneProps",
+        props: typing.Union["RosZoneProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::PVTZ::Zone``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosZone.__init__)
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
+            type_hints = typing.get_type_hints(RosZone._render_properties)
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
     @jsii.member(jsii_name="attrZoneId")
     def attr_zone_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ZoneId: Zone ID.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrZoneId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrZoneName")
     def attr_zone_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ZoneName: Zone name.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrZoneName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrZoneTag")
     def attr_zone_tag(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ZoneTag: Zone label.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrZoneTag"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrZoneType")
     def attr_zone_type(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ZoneType: Zone type.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrZoneType"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosZone, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="zoneName")
     def zone_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: zoneName: Zone name
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "zoneName"))
 
     @zone_name.setter
     def zone_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosZone, "zone_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "zoneName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="ignoredStackTagKeys")
     def ignored_stack_tag_keys(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]]:
         '''
         :Property: ignoredStackTagKeys: Stack tag keys to ignore
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]], jsii.get(self, "ignoredStackTagKeys"))
 
     @ignored_stack_tag_keys.setter
     def ignored_stack_tag_keys(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosZone, "ignored_stack_tag_keys").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "ignoredStackTagKeys", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="proxyPattern")
     def proxy_pattern(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -421,94 +475,112 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "proxyPattern"))
 
     @proxy_pattern.setter
     def proxy_pattern(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosZone, "proxy_pattern").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "proxyPattern", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="remark")
     def remark(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: remark: 50 characters at most. It can only contain numbers, Chinese, English and special characters: "_-,.，。".
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "remark"))
 
     @remark.setter
     def remark(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosZone, "remark").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "remark", value)
 
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
+            type_hints = typing.get_type_hints(getattr(RosZone, "resource_group_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "resourceGroupId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="tags")
     def tags(self) -> typing.Optional[typing.List["RosZone.TagsProperty"]]:
         '''
         :Property: tags: Tags to attach to instance. Max support 20 tags to add during create instance. Each tag with two properties Key and Value, and Key is required.
         '''
         return typing.cast(typing.Optional[typing.List["RosZone.TagsProperty"]], jsii.get(self, "tags"))
 
     @tags.setter
     def tags(self, value: typing.Optional[typing.List["RosZone.TagsProperty"]]) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosZone, "tags").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "tags", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="zoneTag")
     def zone_tag(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: zoneTag: Zone label. It will be ignored when ZoneType is AUTH_ZONE.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "zoneTag"))
 
     @zone_tag.setter
     def zone_tag(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosZone, "zone_tag").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "zoneTag", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="zoneType")
     def zone_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: zoneType: Zone type. For instance: AUTH_ZONE, CLOUD_PRODUCT_ZONE.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "zoneType"))
 
     @zone_type.setter
     def zone_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosZone, "zone_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "zoneType", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-pvtz.RosZone.TagsProperty",
         jsii_struct_bases=[],
         name_mapping={"key": "key", "value": "value"},
     )
@@ -519,14 +591,18 @@
             key: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param key: 
             :param value: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosZone.TagsProperty.__init__)
+                check_type(argname="argument key", value=key, expected_type=type_hints["key"])
+                check_type(argname="argument value", value=value, expected_type=type_hints["value"])
             self._values: typing.Dict[str, typing.Any] = {
                 "key": key,
             }
             if value is not None:
                 self._values["value"] = value
 
         @builtins.property
@@ -579,29 +655,39 @@
         self,
         *,
         zone_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         ignored_stack_tag_keys: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]] = None,
         proxy_pattern: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         remark: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         resource_group_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        tags: typing.Optional[typing.Sequence[RosZone.TagsProperty]] = None,
+        tags: typing.Optional[typing.Sequence[typing.Union[RosZone.TagsProperty, typing.Dict[str, typing.Any]]]] = None,
         zone_tag: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         zone_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::PVTZ::Zone``.
 
         :param zone_name: 
         :param ignored_stack_tag_keys: 
         :param proxy_pattern: 
         :param remark: 
         :param resource_group_id: 
         :param tags: 
         :param zone_tag: 
         :param zone_type: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosZoneProps.__init__)
+            check_type(argname="argument zone_name", value=zone_name, expected_type=type_hints["zone_name"])
+            check_type(argname="argument ignored_stack_tag_keys", value=ignored_stack_tag_keys, expected_type=type_hints["ignored_stack_tag_keys"])
+            check_type(argname="argument proxy_pattern", value=proxy_pattern, expected_type=type_hints["proxy_pattern"])
+            check_type(argname="argument remark", value=remark, expected_type=type_hints["remark"])
+            check_type(argname="argument resource_group_id", value=resource_group_id, expected_type=type_hints["resource_group_id"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
+            check_type(argname="argument zone_tag", value=zone_tag, expected_type=type_hints["zone_tag"])
+            check_type(argname="argument zone_type", value=zone_type, expected_type=type_hints["zone_type"])
         self._values: typing.Dict[str, typing.Any] = {
             "zone_name": zone_name,
         }
         if ignored_stack_tag_keys is not None:
             self._values["ignored_stack_tag_keys"] = ignored_stack_tag_keys
         if proxy_pattern is not None:
             self._values["proxy_pattern"] = proxy_pattern
@@ -716,182 +802,215 @@
 ):
     '''A ROS template type:  ``ALIYUN::PVTZ::ZoneRecord``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosZoneRecordProps",
+        props: typing.Union["RosZoneRecordProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::PVTZ::ZoneRecord``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosZoneRecord.__init__)
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
+            type_hints = typing.get_type_hints(RosZoneRecord._render_properties)
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
     @jsii.member(jsii_name="attrRecord")
     def attr_record(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Record: Record data.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrRecord"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrRecordId")
     def attr_record_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: RecordId: Parsing record Id
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrRecordId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrZoneId")
     def attr_zone_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ZoneId: Zone ID.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrZoneId"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosZoneRecord, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rr")
     def rr(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :: " instead of empty
         :Property: rr: Host record, if you want to resolve
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "rr"))
 
     @rr.setter
     def rr(self, value: typing.Union[builtins.str, ros_cdk_core.IResolvable]) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosZoneRecord, "rr").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "rr", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="status")
     def status(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: status: Allowed values: [ENABLE, DISABLE]
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "status"))
 
     @status.setter
     def status(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosZoneRecord, "status").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "status", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="type")
     def type(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: type: Analyze record type, currently only supports A, AAAA, CNAME, TXT, MX, PTR, SRV
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "type"))
 
     @type.setter
     def type(self, value: typing.Union[builtins.str, ros_cdk_core.IResolvable]) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosZoneRecord, "type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "type", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="value")
     def value(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: value: Record value
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "value"))
 
     @value.setter
     def value(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosZoneRecord, "value").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "value", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="zoneId")
     def zone_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: zoneId: Zone Id
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "zoneId"))
 
     @zone_id.setter
     def zone_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosZoneRecord, "zone_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "zoneId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="priority")
     def priority(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: priority: MX record priority, value range [1,99]. Default to 10.
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "priority"))
 
     @priority.setter
     def priority(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosZoneRecord, "priority").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "priority", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="ttl")
     def ttl(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: ttl: Survival time, default is 60
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "ttl"))
 
     @ttl.setter
     def ttl(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosZoneRecord, "ttl").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "ttl", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-pvtz.RosZoneRecordProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -922,14 +1041,23 @@
         :param status: 
         :param type: 
         :param value: 
         :param zone_id: 
         :param priority: 
         :param ttl: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosZoneRecordProps.__init__)
+            check_type(argname="argument rr", value=rr, expected_type=type_hints["rr"])
+            check_type(argname="argument status", value=status, expected_type=type_hints["status"])
+            check_type(argname="argument type", value=type, expected_type=type_hints["type"])
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+            check_type(argname="argument zone_id", value=zone_id, expected_type=type_hints["zone_id"])
+            check_type(argname="argument priority", value=priority, expected_type=type_hints["priority"])
+            check_type(argname="argument ttl", value=ttl, expected_type=type_hints["ttl"])
         self._values: typing.Dict[str, typing.Any] = {
             "rr": rr,
             "status": status,
             "type": type,
             "value": value,
             "zone_id": zone_id,
         }
@@ -1023,102 +1151,120 @@
 ):
     '''A ROS template type:  ``ALIYUN::PVTZ::ZoneVpcBinder``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosZoneVpcBinderProps",
+        props: typing.Union["RosZoneVpcBinderProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::PVTZ::ZoneVpcBinder``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosZoneVpcBinder.__init__)
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
+            type_hints = typing.get_type_hints(RosZoneVpcBinder._render_properties)
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
     @jsii.member(jsii_name="attrVpcs")
     def attr_vpcs(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Vpcs: Vpc list
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVpcs"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrZoneId")
     def attr_zone_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ZoneId: Zone Id
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrZoneId"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosZoneVpcBinder, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vpcs")
     def vpcs(
         self,
     ) -> typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosZoneVpcBinder.VpcsProperty"]]]:
         '''
         :Property: vpcs:
         '''
         return typing.cast(typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosZoneVpcBinder.VpcsProperty"]]], jsii.get(self, "vpcs"))
 
     @vpcs.setter
     def vpcs(
         self,
         value: typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosZoneVpcBinder.VpcsProperty"]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosZoneVpcBinder, "vpcs").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "vpcs", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="zoneId")
     def zone_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: zoneId: Zone Id
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "zoneId"))
 
     @zone_id.setter
     def zone_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosZoneVpcBinder, "zone_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "zoneId", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-pvtz.RosZoneVpcBinder.VpcsProperty",
         jsii_struct_bases=[],
         name_mapping={"region_id": "regionId", "vpc_id": "vpcId"},
     )
@@ -1129,14 +1275,18 @@
             region_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             vpc_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         ) -> None:
             '''
             :param region_id: 
             :param vpc_id: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosZoneVpcBinder.VpcsProperty.__init__)
+                check_type(argname="argument region_id", value=region_id, expected_type=type_hints["region_id"])
+                check_type(argname="argument vpc_id", value=vpc_id, expected_type=type_hints["vpc_id"])
             self._values: typing.Dict[str, typing.Any] = {
                 "region_id": region_id,
                 "vpc_id": vpc_id,
             }
 
         @builtins.property
         def region_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
@@ -1173,22 +1323,26 @@
     jsii_struct_bases=[],
     name_mapping={"vpcs": "vpcs", "zone_id": "zoneId"},
 )
 class RosZoneVpcBinderProps:
     def __init__(
         self,
         *,
-        vpcs: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosZoneVpcBinder.VpcsProperty]]],
+        vpcs: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosZoneVpcBinder.VpcsProperty, typing.Dict[str, typing.Any]]]]],
         zone_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
         '''Properties for defining a ``ALIYUN::PVTZ::ZoneVpcBinder``.
 
         :param vpcs: 
         :param zone_id: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosZoneVpcBinderProps.__init__)
+            check_type(argname="argument vpcs", value=vpcs, expected_type=type_hints["vpcs"])
+            check_type(argname="argument zone_id", value=zone_id, expected_type=type_hints["zone_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "vpcs": vpcs,
             "zone_id": zone_id,
         }
 
     @builtins.property
     def vpcs(
@@ -1229,37 +1383,43 @@
 ):
     '''A ROS resource type:  ``ALIYUN::PVTZ::UserVpcAuthorization``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "UserVpcAuthorizationProps",
+        props: typing.Union["UserVpcAuthorizationProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::PVTZ::UserVpcAuthorization``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(UserVpcAuthorization.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrAuthorizedUserId")
     def attr_authorized_user_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute AuthorizedUserId: The account ID of the user who authorizes the resource.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAuthorizedUserId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrAuthType")
     def attr_auth_type(self) -> ros_cdk_core.IResolvable:
         '''Attribute AuthType: Authorization type.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAuthType"))
 
 
 @jsii.data_type(
@@ -1287,14 +1447,21 @@
 
         :param authorized_user_id: Property authorizedUserId: The account ID of the user who authorizes the resource.
         :param auth_channel: Property authChannel: Authorization channel. Valid values: AUTH_CODE: Verification code authorization, to verify whether the verification code passed in by AuthCode is correct. RESOURCE_DIRECTORY: Resource directory authorization, verify whether the AuthorizedUserId and the current account have resource directory credit.When it is empty, it is the same as AUTH_CODE, that is, verification code authorization.
         :param auth_code: Property authCode: Verification code, if AuthChannel takes "AUTH_CODE" or is empty, it is mandatory.
         :param auth_type: Property authType: Authorization type.
         :param ignore_deletion_forbidden: Property ignoreDeletionForbidden: Whether to ignore following deletion forbidden errors when deleting:- UserAuth.DeleteForbidden.ZoneVpcExists.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(UserVpcAuthorizationProps.__init__)
+            check_type(argname="argument authorized_user_id", value=authorized_user_id, expected_type=type_hints["authorized_user_id"])
+            check_type(argname="argument auth_channel", value=auth_channel, expected_type=type_hints["auth_channel"])
+            check_type(argname="argument auth_code", value=auth_code, expected_type=type_hints["auth_code"])
+            check_type(argname="argument auth_type", value=auth_type, expected_type=type_hints["auth_type"])
+            check_type(argname="argument ignore_deletion_forbidden", value=ignore_deletion_forbidden, expected_type=type_hints["ignore_deletion_forbidden"])
         self._values: typing.Dict[str, typing.Any] = {
             "authorized_user_id": authorized_user_id,
         }
         if auth_channel is not None:
             self._values["auth_channel"] = auth_channel
         if auth_code is not None:
             self._values["auth_code"] = auth_code
@@ -1368,49 +1535,55 @@
 ):
     '''A ROS resource type:  ``ALIYUN::PVTZ::Zone``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "ZoneProps",
+        props: typing.Union["ZoneProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::PVTZ::Zone``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(Zone.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrZoneId")
     def attr_zone_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute ZoneId: Zone ID.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrZoneId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrZoneName")
     def attr_zone_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute ZoneName: Zone name.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrZoneName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrZoneTag")
     def attr_zone_tag(self) -> ros_cdk_core.IResolvable:
         '''Attribute ZoneTag: Zone label.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrZoneTag"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrZoneType")
     def attr_zone_type(self) -> ros_cdk_core.IResolvable:
         '''Attribute ZoneType: Zone type.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrZoneType"))
 
 
 @jsii.data_type(
@@ -1432,29 +1605,39 @@
         self,
         *,
         zone_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         ignored_stack_tag_keys: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]] = None,
         proxy_pattern: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         remark: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         resource_group_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        tags: typing.Optional[typing.Sequence[RosZone.TagsProperty]] = None,
+        tags: typing.Optional[typing.Sequence[typing.Union[RosZone.TagsProperty, typing.Dict[str, typing.Any]]]] = None,
         zone_tag: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         zone_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::PVTZ::Zone``.
 
         :param zone_name: Property zoneName: Zone name.
         :param ignored_stack_tag_keys: Property ignoredStackTagKeys: Stack tag keys to ignore.
         :param proxy_pattern: Property proxyPattern: ZONE: completely hijack the entire zone. RECORD: Incomplete hijacking, recursive resolution agent. Default to ZONE.
         :param remark: Property remark: 50 characters at most. It can only contain numbers, Chinese, English and special characters: "_-,.，。".
         :param resource_group_id: Property resourceGroupId: Resource group id.
         :param tags: Property tags: Tags to attach to instance. Max support 20 tags to add during create instance. Each tag with two properties Key and Value, and Key is required.
         :param zone_tag: Property zoneTag: Zone label. It will be ignored when ZoneType is AUTH_ZONE.
         :param zone_type: Property zoneType: Zone type. For instance: AUTH_ZONE, CLOUD_PRODUCT_ZONE.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(ZoneProps.__init__)
+            check_type(argname="argument zone_name", value=zone_name, expected_type=type_hints["zone_name"])
+            check_type(argname="argument ignored_stack_tag_keys", value=ignored_stack_tag_keys, expected_type=type_hints["ignored_stack_tag_keys"])
+            check_type(argname="argument proxy_pattern", value=proxy_pattern, expected_type=type_hints["proxy_pattern"])
+            check_type(argname="argument remark", value=remark, expected_type=type_hints["remark"])
+            check_type(argname="argument resource_group_id", value=resource_group_id, expected_type=type_hints["resource_group_id"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
+            check_type(argname="argument zone_tag", value=zone_tag, expected_type=type_hints["zone_tag"])
+            check_type(argname="argument zone_type", value=zone_type, expected_type=type_hints["zone_type"])
         self._values: typing.Dict[str, typing.Any] = {
             "zone_name": zone_name,
         }
         if ignored_stack_tag_keys is not None:
             self._values["ignored_stack_tag_keys"] = ignored_stack_tag_keys
         if proxy_pattern is not None:
             self._values["proxy_pattern"] = proxy_pattern
@@ -1565,43 +1748,49 @@
 ):
     '''A ROS resource type:  ``ALIYUN::PVTZ::ZoneRecord``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "ZoneRecordProps",
+        props: typing.Union["ZoneRecordProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::PVTZ::ZoneRecord``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(ZoneRecord.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrRecord")
     def attr_record(self) -> ros_cdk_core.IResolvable:
         '''Attribute Record: Record data.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrRecord"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrRecordId")
     def attr_record_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute RecordId: Parsing record Id.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrRecordId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrZoneId")
     def attr_zone_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute ZoneId: Zone ID.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrZoneId"))
 
 
 @jsii.data_type(
@@ -1635,14 +1824,23 @@
         :param status: Property status: Allowed values: [ENABLE, DISABLE].
         :param type: Property type: Analyze record type, currently only supports A, AAAA, CNAME, TXT, MX, PTR, SRV.
         :param value: Property value: Record value.
         :param zone_id: Property zoneId: Zone Id.
         :param priority: Property priority: MX record priority, value range [1,99]. Default to 10.
         :param ttl: Property ttl: Survival time, default is 60.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(ZoneRecordProps.__init__)
+            check_type(argname="argument rr", value=rr, expected_type=type_hints["rr"])
+            check_type(argname="argument status", value=status, expected_type=type_hints["status"])
+            check_type(argname="argument type", value=type, expected_type=type_hints["type"])
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+            check_type(argname="argument zone_id", value=zone_id, expected_type=type_hints["zone_id"])
+            check_type(argname="argument priority", value=priority, expected_type=type_hints["priority"])
+            check_type(argname="argument ttl", value=ttl, expected_type=type_hints["ttl"])
         self._values: typing.Dict[str, typing.Any] = {
             "rr": rr,
             "status": status,
             "type": type,
             "value": value,
             "zone_id": zone_id,
         }
@@ -1724,37 +1922,43 @@
 ):
     '''A ROS resource type:  ``ALIYUN::PVTZ::ZoneVpcBinder``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "ZoneVpcBinderProps",
+        props: typing.Union["ZoneVpcBinderProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::PVTZ::ZoneVpcBinder``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(ZoneVpcBinder.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVpcs")
     def attr_vpcs(self) -> ros_cdk_core.IResolvable:
         '''Attribute Vpcs: Vpc list.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVpcs"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrZoneId")
     def attr_zone_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute ZoneId: Zone Id.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrZoneId"))
 
 
 @jsii.data_type(
@@ -1762,22 +1966,26 @@
     jsii_struct_bases=[],
     name_mapping={"vpcs": "vpcs", "zone_id": "zoneId"},
 )
 class ZoneVpcBinderProps:
     def __init__(
         self,
         *,
-        vpcs: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosZoneVpcBinder.VpcsProperty]]],
+        vpcs: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosZoneVpcBinder.VpcsProperty, typing.Dict[str, typing.Any]]]]],
         zone_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
         '''Properties for defining a ``ALIYUN::PVTZ::ZoneVpcBinder``.
 
         :param vpcs: Property vpcs:.
         :param zone_id: Property zoneId: Zone Id.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(ZoneVpcBinderProps.__init__)
+            check_type(argname="argument vpcs", value=vpcs, expected_type=type_hints["vpcs"])
+            check_type(argname="argument zone_id", value=zone_id, expected_type=type_hints["zone_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "vpcs": vpcs,
             "zone_id": zone_id,
         }
 
     @builtins.property
     def vpcs(
```

### Comparing `ros-cdk-pvtz-1.0.8/src/ros_cdk_pvtz.egg-info/PKG-INFO` & `ros-cdk-pvtz-1.0.9/src/ros_cdk_pvtz.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-pvtz
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS PVTZ Construct Library
```

