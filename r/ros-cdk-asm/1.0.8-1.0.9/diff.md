# Comparing `tmp/ros-cdk-asm-1.0.8.tar.gz` & `tmp/ros-cdk-asm-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-asm-1.0.8.tar", last modified: Thu Jul 14 02:34:24 2022, max compression
+gzip compressed data, was "dist/ros-cdk-asm-1.0.9.tar", last modified: Fri Sep 23 10:46:44 2022, max compression
```

## Comparing `ros-cdk-asm-1.0.8.tar` & `ros-cdk-asm-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:34:24.000000 ros-cdk-asm-1.0.8/
--rw-r--r--   0 root         (0) root         (0)    10279 2022-07-14 02:34:23.000000 ros-cdk-asm-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2022-07-14 02:34:23.000000 ros-cdk-asm-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2022-07-14 02:34:23.000000 ros-cdk-asm-1.0.8/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1240 2022-07-14 02:34:24.000000 ros-cdk-asm-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      179 2022-07-14 02:34:23.000000 ros-cdk-asm-1.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)      106 2022-07-14 02:34:23.000000 ros-cdk-asm-1.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-07-14 02:34:24.000000 ros-cdk-asm-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1794 2022-07-14 02:34:23.000000 ros-cdk-asm-1.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:34:24.000000 ros-cdk-asm-1.0.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:34:24.000000 ros-cdk-asm-1.0.8/src/ros_cdk_asm/
--rw-r--r--   0 root         (0) root         (0)    54126 2022-07-14 02:34:23.000000 ros-cdk-asm-1.0.8/src/ros_cdk_asm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:34:24.000000 ros-cdk-asm-1.0.8/src/ros_cdk_asm/_jsii/
--rw-r--r--   0 root         (0) root         (0)      370 2022-07-14 02:34:23.000000 ros-cdk-asm-1.0.8/src/ros_cdk_asm/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    39956 2022-07-14 02:34:23.000000 ros-cdk-asm-1.0.8/src/ros_cdk_asm/_jsii/ros-cdk-asm@1.0.8.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:34:23.000000 ros-cdk-asm-1.0.8/src/ros_cdk_asm/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:34:24.000000 ros-cdk-asm-1.0.8/src/ros_cdk_asm.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1240 2022-07-14 02:34:24.000000 ros-cdk-asm-1.0.8/src/ros_cdk_asm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      400 2022-07-14 02:34:24.000000 ros-cdk-asm-1.0.8/src/ros_cdk_asm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:34:24.000000 ros-cdk-asm-1.0.8/src/ros_cdk_asm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2022-07-14 02:34:24.000000 ros-cdk-asm-1.0.8/src/ros_cdk_asm.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2022-07-14 02:34:24.000000 ros-cdk-asm-1.0.8/src/ros_cdk_asm.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 10:46:44.000000 ros-cdk-asm-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)    10279 2022-09-23 10:46:44.000000 ros-cdk-asm-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-09-23 10:46:44.000000 ros-cdk-asm-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2022-09-23 10:46:44.000000 ros-cdk-asm-1.0.9/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1240 2022-09-23 10:46:44.000000 ros-cdk-asm-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      179 2022-09-23 10:46:44.000000 ros-cdk-asm-1.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      236 2022-09-23 10:46:44.000000 ros-cdk-asm-1.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-09-23 10:46:44.000000 ros-cdk-asm-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1823 2022-09-23 10:46:44.000000 ros-cdk-asm-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 10:46:44.000000 ros-cdk-asm-1.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 10:46:44.000000 ros-cdk-asm-1.0.9/src/ros_cdk_asm/
+-rw-r--r--   0 root         (0) root         (0)    65099 2022-09-23 10:46:44.000000 ros-cdk-asm-1.0.9/src/ros_cdk_asm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 10:46:44.000000 ros-cdk-asm-1.0.9/src/ros_cdk_asm/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      404 2022-09-23 10:46:44.000000 ros-cdk-asm-1.0.9/src/ros_cdk_asm/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    40018 2022-09-23 10:46:44.000000 ros-cdk-asm-1.0.9/src/ros_cdk_asm/_jsii/ros-cdk-asm@1.0.9.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 10:46:44.000000 ros-cdk-asm-1.0.9/src/ros_cdk_asm/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 10:46:44.000000 ros-cdk-asm-1.0.9/src/ros_cdk_asm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1240 2022-09-23 10:46:44.000000 ros-cdk-asm-1.0.9/src/ros_cdk_asm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      400 2022-09-23 10:46:44.000000 ros-cdk-asm-1.0.9/src/ros_cdk_asm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 10:46:44.000000 ros-cdk-asm-1.0.9/src/ros_cdk_asm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2022-09-23 10:46:44.000000 ros-cdk-asm-1.0.9/src/ros_cdk_asm.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2022-09-23 10:46:44.000000 ros-cdk-asm-1.0.9/src/ros_cdk_asm.egg-info/top_level.txt
```

### Comparing `ros-cdk-asm-1.0.8/LICENSE` & `ros-cdk-asm-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-asm-1.0.8/PKG-INFO` & `ros-cdk-asm-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-asm
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS ASM Construct Library
```

### Comparing `ros-cdk-asm-1.0.8/setup.py` & `ros-cdk-asm-1.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-asm",
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
         "ros_cdk_asm",
         "ros_cdk_asm._jsii"
     ],
     "package_data": {
         "ros_cdk_asm._jsii": [
-            "ros-cdk-asm@1.0.8.jsii.tgz"
+            "ros-cdk-asm@1.0.9.jsii.tgz"
         ],
         "ros_cdk_asm": [
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

### Comparing `ros-cdk-asm-1.0.8/src/ros_cdk_asm/__init__.py` & `ros-cdk-asm-1.0.9/src/ros_cdk_asm/__init__.py`

 * *Files 25% similar despite different names*

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
 
 
 class RosServiceMesh(
     ros_cdk_core.RosResource,
@@ -29,97 +31,115 @@
 ):
     '''A ROS template type:  ``ALIYUN::ASM::ServiceMesh``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosServiceMeshProps",
+        props: typing.Union["RosServiceMeshProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::ASM::ServiceMesh``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosServiceMesh.__init__)
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
+            type_hints = typing.get_type_hints(RosServiceMesh._render_properties)
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
     @jsii.member(jsii_name="attrServiceMeshId")
     def attr_service_mesh_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ServiceMeshId: The ID of the ASM instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrServiceMeshId"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosServiceMesh, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vpcId")
     def vpc_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: vpcId: The ID of the virtual private cloud (VPC).
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "vpcId"))
 
     @vpc_id.setter
     def vpc_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosServiceMesh, "vpc_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "vpcId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vSwitches")
     def v_switches(
         self,
     ) -> typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]:
         '''
         :Property: vSwitches: The ID of the vSwitch, eg: ["vsw-xzegf5dndkbf4m6eg****"]
         '''
         return typing.cast(typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable], jsii.get(self, "vSwitches"))
 
     @v_switches.setter
     def v_switches(
         self,
         value: typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosServiceMesh, "v_switches").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "vSwitches", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="apiServerPublicEip")
     def api_server_public_eip(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -131,17 +151,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "apiServerPublicEip"))
 
     @api_server_public_eip.setter
     def api_server_public_eip(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosServiceMesh, "api_server_public_eip").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "apiServerPublicEip", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="auditProject")
     def audit_project(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -151,34 +174,40 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "auditProject"))
 
     @audit_project.setter
     def audit_project(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosServiceMesh, "audit_project").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "auditProject", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="customizedZipkin")
     def customized_zipkin(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property: customizedZipkin: Specifies whether to use a user-created Zipkin system.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "customizedZipkin"))
 
     @customized_zipkin.setter
     def customized_zipkin(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosServiceMesh, "customized_zipkin").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "customizedZipkin", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableAudit")
     def enable_audit(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -189,17 +218,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "enableAudit"))
 
     @enable_audit.setter
     def enable_audit(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosServiceMesh, "enable_audit").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableAudit", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="includeIpRanges")
     def include_ip_ranges(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -209,34 +241,40 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "includeIpRanges"))
 
     @include_ip_ranges.setter
     def include_ip_ranges(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosServiceMesh, "include_ip_ranges").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "includeIpRanges", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="istioVersion")
     def istio_version(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: istioVersion: The Istio version of the ASM instance.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "istioVersion"))
 
     @istio_version.setter
     def istio_version(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosServiceMesh, "istio_version").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "istioVersion", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="localityLoadBalancing")
     def locality_load_balancing(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -246,68 +284,80 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "localityLoadBalancing"))
 
     @locality_load_balancing.setter
     def locality_load_balancing(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosServiceMesh, "locality_load_balancing").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "localityLoadBalancing", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="name")
     def name(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: name: The name of the ASM instance.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "name"))
 
     @name.setter
     def name(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosServiceMesh, "name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "name", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="opa")
     def opa(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosServiceMesh.OPAProperty"]]:
         '''
         :Property: opa: OPA settings.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosServiceMesh.OPAProperty"]], jsii.get(self, "opa"))
 
     @opa.setter
     def opa(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosServiceMesh.OPAProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosServiceMesh, "opa").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "opa", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="outboundTrafficPolicy")
     def outbound_traffic_policy(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: outboundTrafficPolicy: The outbound traffic policy of the ASM instance.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "outboundTrafficPolicy"))
 
     @outbound_traffic_policy.setter
     def outbound_traffic_policy(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosServiceMesh, "outbound_traffic_policy").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "outboundTrafficPolicy", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="pilotPublicEip")
     def pilot_public_eip(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -319,68 +369,80 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "pilotPublicEip"))
 
     @pilot_public_eip.setter
     def pilot_public_eip(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosServiceMesh, "pilot_public_eip").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "pilotPublicEip", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="proxy")
     def proxy(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosServiceMesh.ProxyProperty"]]:
         '''
         :Property: proxy: Proxy settings.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosServiceMesh.ProxyProperty"]], jsii.get(self, "proxy"))
 
     @proxy.setter
     def proxy(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosServiceMesh.ProxyProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosServiceMesh, "proxy").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "proxy", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="telemetry")
     def telemetry(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property: telemetry: Specifies whether to enable Prometheus monitoring. We recommend that you use Application Real-Time Monitoring Service (ARMS).
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "telemetry"))
 
     @telemetry.setter
     def telemetry(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosServiceMesh, "telemetry").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "telemetry", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="traceSampling")
     def trace_sampling(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: traceSampling: The sampling percentage of tracing.
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "traceSampling"))
 
     @trace_sampling.setter
     def trace_sampling(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosServiceMesh, "trace_sampling").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "traceSampling", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="tracing")
     def tracing(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -391,14 +453,17 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "tracing"))
 
     @tracing.setter
     def tracing(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosServiceMesh, "tracing").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "tracing", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-asm.RosServiceMesh.OPAProperty",
         jsii_struct_bases=[],
         name_mapping={
             "opa_limit_cpu": "opaLimitCpu",
@@ -424,14 +489,22 @@
             :param opa_limit_cpu: 
             :param opa_limit_memory: 
             :param opa_log_level: 
             :param opa_request_cpu: 
             :param opa_request_memory: 
             :param open_agent_policy: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosServiceMesh.OPAProperty.__init__)
+                check_type(argname="argument opa_limit_cpu", value=opa_limit_cpu, expected_type=type_hints["opa_limit_cpu"])
+                check_type(argname="argument opa_limit_memory", value=opa_limit_memory, expected_type=type_hints["opa_limit_memory"])
+                check_type(argname="argument opa_log_level", value=opa_log_level, expected_type=type_hints["opa_log_level"])
+                check_type(argname="argument opa_request_cpu", value=opa_request_cpu, expected_type=type_hints["opa_request_cpu"])
+                check_type(argname="argument opa_request_memory", value=opa_request_memory, expected_type=type_hints["opa_request_memory"])
+                check_type(argname="argument open_agent_policy", value=open_agent_policy, expected_type=type_hints["open_agent_policy"])
             self._values: typing.Dict[str, typing.Any] = {}
             if opa_limit_cpu is not None:
                 self._values["opa_limit_cpu"] = opa_limit_cpu
             if opa_limit_memory is not None:
                 self._values["opa_limit_memory"] = opa_limit_memory
             if opa_log_level is not None:
                 self._values["opa_log_level"] = opa_log_level
@@ -540,14 +613,21 @@
             '''
             :param cluster_domain: 
             :param proxy_limit_cpu: 
             :param proxy_limit_memory: 
             :param proxy_request_cpu: 
             :param proxy_request_memory: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosServiceMesh.ProxyProperty.__init__)
+                check_type(argname="argument cluster_domain", value=cluster_domain, expected_type=type_hints["cluster_domain"])
+                check_type(argname="argument proxy_limit_cpu", value=proxy_limit_cpu, expected_type=type_hints["proxy_limit_cpu"])
+                check_type(argname="argument proxy_limit_memory", value=proxy_limit_memory, expected_type=type_hints["proxy_limit_memory"])
+                check_type(argname="argument proxy_request_cpu", value=proxy_request_cpu, expected_type=type_hints["proxy_request_cpu"])
+                check_type(argname="argument proxy_request_memory", value=proxy_request_memory, expected_type=type_hints["proxy_request_memory"])
             self._values: typing.Dict[str, typing.Any] = {}
             if cluster_domain is not None:
                 self._values["cluster_domain"] = cluster_domain
             if proxy_limit_cpu is not None:
                 self._values["proxy_limit_cpu"] = proxy_limit_cpu
             if proxy_limit_memory is not None:
                 self._values["proxy_limit_memory"] = proxy_limit_memory
@@ -651,18 +731,18 @@
         audit_project: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         customized_zipkin: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         enable_audit: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         include_ip_ranges: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         istio_version: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         locality_load_balancing: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         name: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        opa: typing.Optional[typing.Union[ros_cdk_core.IResolvable, RosServiceMesh.OPAProperty]] = None,
+        opa: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosServiceMesh.OPAProperty, typing.Dict[str, typing.Any]]]] = None,
         outbound_traffic_policy: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         pilot_public_eip: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
-        proxy: typing.Optional[typing.Union[ros_cdk_core.IResolvable, RosServiceMesh.ProxyProperty]] = None,
+        proxy: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosServiceMesh.ProxyProperty, typing.Dict[str, typing.Any]]]] = None,
         telemetry: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         trace_sampling: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         tracing: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::ASM::ServiceMesh``.
 
         :param vpc_id: 
@@ -679,14 +759,33 @@
         :param outbound_traffic_policy: 
         :param pilot_public_eip: 
         :param proxy: 
         :param telemetry: 
         :param trace_sampling: 
         :param tracing: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosServiceMeshProps.__init__)
+            check_type(argname="argument vpc_id", value=vpc_id, expected_type=type_hints["vpc_id"])
+            check_type(argname="argument v_switches", value=v_switches, expected_type=type_hints["v_switches"])
+            check_type(argname="argument api_server_public_eip", value=api_server_public_eip, expected_type=type_hints["api_server_public_eip"])
+            check_type(argname="argument audit_project", value=audit_project, expected_type=type_hints["audit_project"])
+            check_type(argname="argument customized_zipkin", value=customized_zipkin, expected_type=type_hints["customized_zipkin"])
+            check_type(argname="argument enable_audit", value=enable_audit, expected_type=type_hints["enable_audit"])
+            check_type(argname="argument include_ip_ranges", value=include_ip_ranges, expected_type=type_hints["include_ip_ranges"])
+            check_type(argname="argument istio_version", value=istio_version, expected_type=type_hints["istio_version"])
+            check_type(argname="argument locality_load_balancing", value=locality_load_balancing, expected_type=type_hints["locality_load_balancing"])
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+            check_type(argname="argument opa", value=opa, expected_type=type_hints["opa"])
+            check_type(argname="argument outbound_traffic_policy", value=outbound_traffic_policy, expected_type=type_hints["outbound_traffic_policy"])
+            check_type(argname="argument pilot_public_eip", value=pilot_public_eip, expected_type=type_hints["pilot_public_eip"])
+            check_type(argname="argument proxy", value=proxy, expected_type=type_hints["proxy"])
+            check_type(argname="argument telemetry", value=telemetry, expected_type=type_hints["telemetry"])
+            check_type(argname="argument trace_sampling", value=trace_sampling, expected_type=type_hints["trace_sampling"])
+            check_type(argname="argument tracing", value=tracing, expected_type=type_hints["tracing"])
         self._values: typing.Dict[str, typing.Any] = {
             "vpc_id": vpc_id,
             "v_switches": v_switches,
         }
         if api_server_public_eip is not None:
             self._values["api_server_public_eip"] = api_server_public_eip
         if audit_project is not None:
@@ -934,31 +1033,37 @@
 ):
     '''A ROS resource type:  ``ALIYUN::ASM::ServiceMesh``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "ServiceMeshProps",
+        props: typing.Union["ServiceMeshProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::ASM::ServiceMesh``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(ServiceMesh.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrServiceMeshId")
     def attr_service_mesh_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute ServiceMeshId: The ID of the ASM instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrServiceMeshId"))
 
 
 @jsii.data_type(
@@ -994,18 +1099,18 @@
         audit_project: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         customized_zipkin: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         enable_audit: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         include_ip_ranges: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         istio_version: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         locality_load_balancing: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         name: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        opa: typing.Optional[typing.Union[ros_cdk_core.IResolvable, RosServiceMesh.OPAProperty]] = None,
+        opa: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosServiceMesh.OPAProperty, typing.Dict[str, typing.Any]]]] = None,
         outbound_traffic_policy: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         pilot_public_eip: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
-        proxy: typing.Optional[typing.Union[ros_cdk_core.IResolvable, RosServiceMesh.ProxyProperty]] = None,
+        proxy: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosServiceMesh.ProxyProperty, typing.Dict[str, typing.Any]]]] = None,
         telemetry: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         trace_sampling: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         tracing: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::ASM::ServiceMesh``.
 
         :param vpc_id: Property vpcId: The ID of the virtual private cloud (VPC).
@@ -1022,14 +1127,33 @@
         :param outbound_traffic_policy: Property outboundTrafficPolicy: The outbound traffic policy of the ASM instance.
         :param pilot_public_eip: Property pilotPublicEip: Specifies whether to expose Istio Pilot to the Internet. Valid values: true and false. Default value: false. If you do not set this parameter, only clusters in the same VPC as the ASM instance can access Istio Pilot of the instance.
         :param proxy: Property proxy: Proxy settings.
         :param telemetry: Property telemetry: Specifies whether to enable Prometheus monitoring. We recommend that you use Application Real-Time Monitoring Service (ARMS).
         :param trace_sampling: Property traceSampling: The sampling percentage of tracing.
         :param tracing: Property tracing: Specifies whether to enable the tracing feature. To enable this feature, make sure that you have activated Alibaba Cloud Tracing Analysis. Valid values: true and false. Default value: false.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(ServiceMeshProps.__init__)
+            check_type(argname="argument vpc_id", value=vpc_id, expected_type=type_hints["vpc_id"])
+            check_type(argname="argument v_switches", value=v_switches, expected_type=type_hints["v_switches"])
+            check_type(argname="argument api_server_public_eip", value=api_server_public_eip, expected_type=type_hints["api_server_public_eip"])
+            check_type(argname="argument audit_project", value=audit_project, expected_type=type_hints["audit_project"])
+            check_type(argname="argument customized_zipkin", value=customized_zipkin, expected_type=type_hints["customized_zipkin"])
+            check_type(argname="argument enable_audit", value=enable_audit, expected_type=type_hints["enable_audit"])
+            check_type(argname="argument include_ip_ranges", value=include_ip_ranges, expected_type=type_hints["include_ip_ranges"])
+            check_type(argname="argument istio_version", value=istio_version, expected_type=type_hints["istio_version"])
+            check_type(argname="argument locality_load_balancing", value=locality_load_balancing, expected_type=type_hints["locality_load_balancing"])
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+            check_type(argname="argument opa", value=opa, expected_type=type_hints["opa"])
+            check_type(argname="argument outbound_traffic_policy", value=outbound_traffic_policy, expected_type=type_hints["outbound_traffic_policy"])
+            check_type(argname="argument pilot_public_eip", value=pilot_public_eip, expected_type=type_hints["pilot_public_eip"])
+            check_type(argname="argument proxy", value=proxy, expected_type=type_hints["proxy"])
+            check_type(argname="argument telemetry", value=telemetry, expected_type=type_hints["telemetry"])
+            check_type(argname="argument trace_sampling", value=trace_sampling, expected_type=type_hints["trace_sampling"])
+            check_type(argname="argument tracing", value=tracing, expected_type=type_hints["tracing"])
         self._values: typing.Dict[str, typing.Any] = {
             "vpc_id": vpc_id,
             "v_switches": v_switches,
         }
         if api_server_public_eip is not None:
             self._values["api_server_public_eip"] = api_server_public_eip
         if audit_project is not None:
```

### Comparing `ros-cdk-asm-1.0.8/src/ros_cdk_asm.egg-info/PKG-INFO` & `ros-cdk-asm-1.0.9/src/ros_cdk_asm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-asm
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS ASM Construct Library
```

