# Comparing `tmp/ros-cdk-fc-1.0.8.tar.gz` & `tmp/ros-cdk-fc-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-fc-1.0.8.tar", last modified: Thu Jul 14 02:32:46 2022, max compression
+gzip compressed data, was "dist/ros-cdk-fc-1.0.9.tar", last modified: Fri Sep 23 11:27:05 2022, max compression
```

## Comparing `ros-cdk-fc-1.0.8.tar` & `ros-cdk-fc-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:32:46.000000 ros-cdk-fc-1.0.8/
--rw-r--r--   0 root         (0) root         (0)    10279 2022-07-14 02:32:46.000000 ros-cdk-fc-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2022-07-14 02:32:46.000000 ros-cdk-fc-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2022-07-14 02:32:46.000000 ros-cdk-fc-1.0.8/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1236 2022-07-14 02:32:46.000000 ros-cdk-fc-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      176 2022-07-14 02:32:46.000000 ros-cdk-fc-1.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)      106 2022-07-14 02:32:46.000000 ros-cdk-fc-1.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-07-14 02:32:46.000000 ros-cdk-fc-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1788 2022-07-14 02:32:46.000000 ros-cdk-fc-1.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:32:46.000000 ros-cdk-fc-1.0.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:32:46.000000 ros-cdk-fc-1.0.8/src/ros_cdk_fc/
--rw-r--r--   0 root         (0) root         (0)   241214 2022-07-14 02:32:46.000000 ros-cdk-fc-1.0.8/src/ros_cdk_fc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:32:46.000000 ros-cdk-fc-1.0.8/src/ros_cdk_fc/_jsii/
--rw-r--r--   0 root         (0) root         (0)      368 2022-07-14 02:32:46.000000 ros-cdk-fc-1.0.8/src/ros_cdk_fc/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)   101605 2022-07-14 02:32:46.000000 ros-cdk-fc-1.0.8/src/ros_cdk_fc/_jsii/ros-cdk-fc@1.0.8.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:32:46.000000 ros-cdk-fc-1.0.8/src/ros_cdk_fc/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:32:46.000000 ros-cdk-fc-1.0.8/src/ros_cdk_fc.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1236 2022-07-14 02:32:46.000000 ros-cdk-fc-1.0.8/src/ros_cdk_fc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      390 2022-07-14 02:32:46.000000 ros-cdk-fc-1.0.8/src/ros_cdk_fc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:32:46.000000 ros-cdk-fc-1.0.8/src/ros_cdk_fc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2022-07-14 02:32:46.000000 ros-cdk-fc-1.0.8/src/ros_cdk_fc.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2022-07-14 02:32:46.000000 ros-cdk-fc-1.0.8/src/ros_cdk_fc.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:27:05.000000 ros-cdk-fc-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)    10279 2022-09-23 11:27:05.000000 ros-cdk-fc-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-09-23 11:27:05.000000 ros-cdk-fc-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2022-09-23 11:27:05.000000 ros-cdk-fc-1.0.9/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1236 2022-09-23 11:27:05.000000 ros-cdk-fc-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      176 2022-09-23 11:27:05.000000 ros-cdk-fc-1.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      236 2022-09-23 11:27:05.000000 ros-cdk-fc-1.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-09-23 11:27:05.000000 ros-cdk-fc-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1817 2022-09-23 11:27:05.000000 ros-cdk-fc-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:27:05.000000 ros-cdk-fc-1.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:27:05.000000 ros-cdk-fc-1.0.9/src/ros_cdk_fc/
+-rw-r--r--   0 root         (0) root         (0)   290508 2022-09-23 11:27:05.000000 ros-cdk-fc-1.0.9/src/ros_cdk_fc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:27:05.000000 ros-cdk-fc-1.0.9/src/ros_cdk_fc/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      402 2022-09-23 11:27:05.000000 ros-cdk-fc-1.0.9/src/ros_cdk_fc/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   101678 2022-09-23 11:27:05.000000 ros-cdk-fc-1.0.9/src/ros_cdk_fc/_jsii/ros-cdk-fc@1.0.9.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 11:27:05.000000 ros-cdk-fc-1.0.9/src/ros_cdk_fc/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:27:05.000000 ros-cdk-fc-1.0.9/src/ros_cdk_fc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1236 2022-09-23 11:27:05.000000 ros-cdk-fc-1.0.9/src/ros_cdk_fc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      390 2022-09-23 11:27:05.000000 ros-cdk-fc-1.0.9/src/ros_cdk_fc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 11:27:05.000000 ros-cdk-fc-1.0.9/src/ros_cdk_fc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2022-09-23 11:27:05.000000 ros-cdk-fc-1.0.9/src/ros_cdk_fc.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2022-09-23 11:27:05.000000 ros-cdk-fc-1.0.9/src/ros_cdk_fc.egg-info/top_level.txt
```

### Comparing `ros-cdk-fc-1.0.8/LICENSE` & `ros-cdk-fc-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-fc-1.0.8/PKG-INFO` & `ros-cdk-fc-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-fc
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS FC Construct Library
```

### Comparing `ros-cdk-fc-1.0.8/setup.py` & `ros-cdk-fc-1.0.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-fc",
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
         "ros_cdk_fc",
         "ros_cdk_fc._jsii"
     ],
     "package_data": {
         "ros_cdk_fc._jsii": [
-            "ros-cdk-fc@1.0.8.jsii.tgz"
+            "ros-cdk-fc@1.0.9.jsii.tgz"
         ],
         "ros_cdk_fc": [
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

### Comparing `ros-cdk-fc-1.0.8/src/ros_cdk_fc/__init__.py` & `ros-cdk-fc-1.0.9/src/ros_cdk_fc/__init__.py`

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
 
 
 class Alias(
     ros_cdk_core.Resource,
@@ -29,43 +31,49 @@
 ):
     '''A ROS resource type:  ``ALIYUN::FC::Alias``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "AliasProps",
+        props: typing.Union["AliasProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::FC::Alias``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(Alias.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrAliasName")
     def attr_alias_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute AliasName: The alias name.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAliasName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrServiceName")
     def attr_service_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute ServiceName: The service name.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrServiceName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVersionId")
     def attr_version_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute VersionId: The version ID.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVersionId"))
 
 
 @jsii.data_type(
@@ -96,14 +104,22 @@
         :param alias_name: Property aliasName: Alias name.
         :param service_name: Property serviceName: Service name.
         :param additional_version: Property additionalVersion: Additional version.
         :param additional_weight: Property additionalWeight: Traffic weight of additional version. From 0 to 100.
         :param description: Property description: Version description.
         :param version_id: Property versionId: Version ID.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(AliasProps.__init__)
+            check_type(argname="argument alias_name", value=alias_name, expected_type=type_hints["alias_name"])
+            check_type(argname="argument service_name", value=service_name, expected_type=type_hints["service_name"])
+            check_type(argname="argument additional_version", value=additional_version, expected_type=type_hints["additional_version"])
+            check_type(argname="argument additional_weight", value=additional_weight, expected_type=type_hints["additional_weight"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument version_id", value=version_id, expected_type=type_hints["version_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "alias_name": alias_name,
             "service_name": service_name,
         }
         if additional_version is not None:
             self._values["additional_version"] = additional_version
         if additional_weight is not None:
@@ -181,37 +197,43 @@
 ):
     '''A ROS resource type:  ``ALIYUN::FC::CustomDomain``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "CustomDomainProps",
+        props: typing.Union["CustomDomainProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::FC::CustomDomain``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(CustomDomain.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDomain")
     def attr_domain(self) -> ros_cdk_core.IResolvable:
         '''Attribute Domain: The domain with protocol.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDomain"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDomainName")
     def attr_domain_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute DomainName: The domain name.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDomainName"))
 
 
 @jsii.data_type(
@@ -228,25 +250,32 @@
 class CustomDomainProps:
     def __init__(
         self,
         *,
         domain_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         protocol: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         api_version: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        cert_config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosCustomDomain.CertConfigProperty"]] = None,
-        route_config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosCustomDomain.RouteConfigProperty"]] = None,
+        cert_config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosCustomDomain.CertConfigProperty", typing.Dict[str, typing.Any]]]] = None,
+        route_config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosCustomDomain.RouteConfigProperty", typing.Dict[str, typing.Any]]]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::FC::CustomDomain``.
 
         :param domain_name: Property domainName: domain name.
         :param protocol: Property protocol: HTTP or HTTP,HTTPS.
         :param api_version: Property apiVersion: api version.
         :param cert_config: Property certConfig: certificate info.
         :param route_config: Property routeConfig: Routing table: path to function mappingwhen a function is called with a custom domain name.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(CustomDomainProps.__init__)
+            check_type(argname="argument domain_name", value=domain_name, expected_type=type_hints["domain_name"])
+            check_type(argname="argument protocol", value=protocol, expected_type=type_hints["protocol"])
+            check_type(argname="argument api_version", value=api_version, expected_type=type_hints["api_version"])
+            check_type(argname="argument cert_config", value=cert_config, expected_type=type_hints["cert_config"])
+            check_type(argname="argument route_config", value=route_config, expected_type=type_hints["route_config"])
         self._values: typing.Dict[str, typing.Any] = {
             "domain_name": domain_name,
             "protocol": protocol,
         }
         if api_version is not None:
             self._values["api_version"] = api_version
         if cert_config is not None:
@@ -311,55 +340,61 @@
 ):
     '''A ROS resource type:  ``ALIYUN::FC::Function``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "FunctionProps",
+        props: typing.Union["FunctionProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::FC::Function``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(Function.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrArn")
     def attr_arn(self) -> ros_cdk_core.IResolvable:
         '''Attribute ARN: The ARN for ALIYUN::ROS::CustomResource.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrArn"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrFunctionId")
     def attr_function_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute FunctionId: The function ID.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrFunctionId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrFunctionName")
     def attr_function_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute FunctionName: The function name.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrFunctionName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrServiceId")
     def attr_service_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute ServiceId: The service ID.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrServiceId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrServiceName")
     def attr_service_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute ServiceName: The service name.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrServiceName"))
 
 
 class FunctionInvoker(
@@ -369,41 +404,47 @@
 ):
     '''A ROS resource type:  ``ALIYUN::FC::FunctionInvoker``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "FunctionInvokerProps",
+        props: typing.Union["FunctionInvokerProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::FC::FunctionInvoker``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(FunctionInvoker.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrResult")
     def attr_result(self) -> ros_cdk_core.IResolvable:
         '''Attribute Result: Depends on result type: NoResult: Async invoke has no result.
 
         Success: The response of the function. The response should be utf-8 encoded string, otherwise ROS will report an error. If the response is binary, encode it via base64 before it is returned.
         Failure: Error Message.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrResult"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrResultType")
     def attr_result_type(self) -> ros_cdk_core.IResolvable:
         '''Attribute ResultType: Result type: NoResult: Async invoke has no result.
 
         Success: Sync invoke succeeds.
         Failure: Sync invoke fails.
         '''
@@ -444,14 +485,24 @@
         :param async_: Property async: Invocation type, Sync or Async. Defaults to Sync.
         :param check_error: Property checkError: Whether check error for function invocation result. If set true and function invocation result has error, the resource creation will be regard as failed. Default is false
         :param event: Property event: This value is passed to function as utf-8 encoded string.It’s function’s responsibility to interpret the value. If the value needs to be binary, encode it via base64 before passing to this property.
         :param execute_version: Property executeVersion: If the property is not specified for creation and update, the function will not be invoked. The change of the property leads to the invoke of the function.
         :param qualifier: Property qualifier: service version, can be versionId or aliasName.
         :param service_region_id: Property serviceRegionId: Which region service belongs to.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(FunctionInvokerProps.__init__)
+            check_type(argname="argument function_name", value=function_name, expected_type=type_hints["function_name"])
+            check_type(argname="argument service_name", value=service_name, expected_type=type_hints["service_name"])
+            check_type(argname="argument async_", value=async_, expected_type=type_hints["async_"])
+            check_type(argname="argument check_error", value=check_error, expected_type=type_hints["check_error"])
+            check_type(argname="argument event", value=event, expected_type=type_hints["event"])
+            check_type(argname="argument execute_version", value=execute_version, expected_type=type_hints["execute_version"])
+            check_type(argname="argument qualifier", value=qualifier, expected_type=type_hints["qualifier"])
+            check_type(argname="argument service_region_id", value=service_region_id, expected_type=type_hints["service_region_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "function_name": function_name,
             "service_name": service_name,
         }
         if async_ is not None:
             self._values["async_"] = async_
         if check_error is not None:
@@ -575,18 +626,18 @@
     def __init__(
         self,
         *,
         function_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         handler: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         runtime: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         service_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
-        async_configuration: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosFunction.AsyncConfigurationProperty"]] = None,
+        async_configuration: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosFunction.AsyncConfigurationProperty", typing.Dict[str, typing.Any]]]] = None,
         ca_port: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
-        code: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosFunction.CodeProperty"]] = None,
-        custom_container_config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosFunction.CustomContainerConfigProperty"]] = None,
+        code: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosFunction.CodeProperty", typing.Dict[str, typing.Any]]]] = None,
+        custom_container_config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosFunction.CustomContainerConfigProperty", typing.Dict[str, typing.Any]]]] = None,
         description: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         environment_variables: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]]] = None,
         initialization_timeout: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         initializer: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         instance_concurrency: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         instance_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         memory_size: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
@@ -607,14 +658,32 @@
         :param initialization_timeout: Property initializationTimeout: the max execution time of the initializer, in second.
         :param initializer: Property initializer: the entry point of the initializer.
         :param instance_concurrency: Property instanceConcurrency: Function instance concurrency. Value can be between 1 to 100.
         :param instance_type: Property instanceType: Instance type. Value:e1: flexible instance. Memory size between 128 and 3072c1: performance instance. Memory size allow values are 4096, 8192, 16384 and 32768
         :param memory_size: Property memorySize: The amount of memory that’s used to run function, in MB. Function Compute uses this value to allocate CPU resources proportionally. Defaults to 128 MB. It can be multiple of 64 MB and between 128 MB and 3072 MB.
         :param timeout: Property timeout: The maximum time duration a function can run, in seconds. After which Function Compute terminates the execution. Defaults to 3 seconds, and can be between 1 to 600 seconds.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(FunctionProps.__init__)
+            check_type(argname="argument function_name", value=function_name, expected_type=type_hints["function_name"])
+            check_type(argname="argument handler", value=handler, expected_type=type_hints["handler"])
+            check_type(argname="argument runtime", value=runtime, expected_type=type_hints["runtime"])
+            check_type(argname="argument service_name", value=service_name, expected_type=type_hints["service_name"])
+            check_type(argname="argument async_configuration", value=async_configuration, expected_type=type_hints["async_configuration"])
+            check_type(argname="argument ca_port", value=ca_port, expected_type=type_hints["ca_port"])
+            check_type(argname="argument code", value=code, expected_type=type_hints["code"])
+            check_type(argname="argument custom_container_config", value=custom_container_config, expected_type=type_hints["custom_container_config"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument environment_variables", value=environment_variables, expected_type=type_hints["environment_variables"])
+            check_type(argname="argument initialization_timeout", value=initialization_timeout, expected_type=type_hints["initialization_timeout"])
+            check_type(argname="argument initializer", value=initializer, expected_type=type_hints["initializer"])
+            check_type(argname="argument instance_concurrency", value=instance_concurrency, expected_type=type_hints["instance_concurrency"])
+            check_type(argname="argument instance_type", value=instance_type, expected_type=type_hints["instance_type"])
+            check_type(argname="argument memory_size", value=memory_size, expected_type=type_hints["memory_size"])
+            check_type(argname="argument timeout", value=timeout, expected_type=type_hints["timeout"])
         self._values: typing.Dict[str, typing.Any] = {
             "function_name": function_name,
             "handler": handler,
             "runtime": runtime,
             "service_name": service_name,
         }
         if async_configuration is not None:
@@ -806,43 +875,49 @@
 ):
     '''A ROS resource type:  ``ALIYUN::FC::Layer``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "LayerProps",
+        props: typing.Union["LayerProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::FC::Layer``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(Layer.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrArn")
     def attr_arn(self) -> ros_cdk_core.IResolvable:
         '''Attribute Arn: The name of the layer resource.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrArn"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrLayerName")
     def attr_layer_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute LayerName: The name of layer.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrLayerName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVersion")
     def attr_version(self) -> ros_cdk_core.IResolvable:
         '''Attribute Version: The version of the layer resource.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVersion"))
 
 
 @jsii.data_type(
@@ -855,26 +930,32 @@
         "description": "description",
     },
 )
 class LayerProps:
     def __init__(
         self,
         *,
-        code: typing.Union[ros_cdk_core.IResolvable, "RosLayer.CodeProperty"],
+        code: typing.Union[ros_cdk_core.IResolvable, typing.Union["RosLayer.CodeProperty", typing.Dict[str, typing.Any]]],
         compatible_runtime: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]],
         layer_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         description: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::FC::Layer``.
 
         :param code: Property code: The code of layer.
         :param compatible_runtime: Property compatibleRuntime: The runtime environment supported by the layer. For example:nodejs12, nodejs10, nodejs8, nodejs6, python3, and python2.7
         :param layer_name: Property layerName: The name of layer.
         :param description: Property description: The description of the layer.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(LayerProps.__init__)
+            check_type(argname="argument code", value=code, expected_type=type_hints["code"])
+            check_type(argname="argument compatible_runtime", value=compatible_runtime, expected_type=type_hints["compatible_runtime"])
+            check_type(argname="argument layer_name", value=layer_name, expected_type=type_hints["layer_name"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
         self._values: typing.Dict[str, typing.Any] = {
             "code": code,
             "compatible_runtime": compatible_runtime,
             "layer_name": layer_name,
         }
         if description is not None:
             self._values["description"] = description
@@ -932,55 +1013,61 @@
 ):
     '''A ROS resource type:  ``ALIYUN::FC::ProvisionConfig``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "ProvisionConfigProps",
+        props: typing.Union["ProvisionConfigProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::FC::ProvisionConfig``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(ProvisionConfig.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrFunctionName")
     def attr_function_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute FunctionName: The function name.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrFunctionName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrQualifier")
     def attr_qualifier(self) -> ros_cdk_core.IResolvable:
         '''Attribute Qualifier: The service alias.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrQualifier"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrResource")
     def attr_resource(self) -> ros_cdk_core.IResolvable:
         '''Attribute Resource: The resource.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrResource"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrServiceName")
     def attr_service_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute ServiceName: The service name.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrServiceName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTarget")
     def attr_target(self) -> ros_cdk_core.IResolvable:
         '''Attribute Target: Number of provision.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTarget"))
 
 
 @jsii.data_type(
@@ -1005,14 +1092,20 @@
         '''Properties for defining a ``ALIYUN::FC::ProvisionConfig``.
 
         :param function_name: Property functionName: Function name.
         :param qualifier: Property qualifier: Service's alias. Example : "LATEST"
         :param service_name: Property serviceName: Service name.
         :param target: Property target: Number of provision.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(ProvisionConfigProps.__init__)
+            check_type(argname="argument function_name", value=function_name, expected_type=type_hints["function_name"])
+            check_type(argname="argument qualifier", value=qualifier, expected_type=type_hints["qualifier"])
+            check_type(argname="argument service_name", value=service_name, expected_type=type_hints["service_name"])
+            check_type(argname="argument target", value=target, expected_type=type_hints["target"])
         self._values: typing.Dict[str, typing.Any] = {
             "function_name": function_name,
             "qualifier": qualifier,
             "service_name": service_name,
             "target": target,
         }
 
@@ -1066,176 +1159,206 @@
 ):
     '''A ROS template type:  ``ALIYUN::FC::Alias``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosAliasProps",
+        props: typing.Union["RosAliasProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::FC::Alias``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosAlias.__init__)
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
+            type_hints = typing.get_type_hints(RosAlias._render_properties)
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
     @jsii.member(jsii_name="attrAliasName")
     def attr_alias_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: AliasName: The alias name
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAliasName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrServiceName")
     def attr_service_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ServiceName: The service name
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrServiceName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVersionId")
     def attr_version_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: VersionId: The version ID
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVersionId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="aliasName")
     def alias_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: aliasName: Alias name
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "aliasName"))
 
     @alias_name.setter
     def alias_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAlias, "alias_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "aliasName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAlias, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="serviceName")
     def service_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: serviceName: Service name
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "serviceName"))
 
     @service_name.setter
     def service_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAlias, "service_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "serviceName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="additionalVersion")
     def additional_version(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: additionalVersion: Additional version
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "additionalVersion"))
 
     @additional_version.setter
     def additional_version(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAlias, "additional_version").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "additionalVersion", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="additionalWeight")
     def additional_weight(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: additionalWeight: Traffic weight of additional version. From 0 to 100.
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "additionalWeight"))
 
     @additional_weight.setter
     def additional_weight(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAlias, "additional_weight").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "additionalWeight", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="description")
     def description(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: description: Version description
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "description"))
 
     @description.setter
     def description(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAlias, "description").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "description", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="versionId")
     def version_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: versionId: Version ID
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "versionId"))
 
     @version_id.setter
     def version_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAlias, "version_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "versionId", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-fc.RosAliasProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -1263,14 +1386,22 @@
         :param alias_name: 
         :param service_name: 
         :param additional_version: 
         :param additional_weight: 
         :param description: 
         :param version_id: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosAliasProps.__init__)
+            check_type(argname="argument alias_name", value=alias_name, expected_type=type_hints["alias_name"])
+            check_type(argname="argument service_name", value=service_name, expected_type=type_hints["service_name"])
+            check_type(argname="argument additional_version", value=additional_version, expected_type=type_hints["additional_version"])
+            check_type(argname="argument additional_weight", value=additional_weight, expected_type=type_hints["additional_weight"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument version_id", value=version_id, expected_type=type_hints["version_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "alias_name": alias_name,
             "service_name": service_name,
         }
         if additional_version is not None:
             self._values["additional_version"] = additional_version
         if additional_weight is not None:
@@ -1357,151 +1488,178 @@
 ):
     '''A ROS template type:  ``ALIYUN::FC::CustomDomain``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosCustomDomainProps",
+        props: typing.Union["RosCustomDomainProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::FC::CustomDomain``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosCustomDomain.__init__)
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
+            type_hints = typing.get_type_hints(RosCustomDomain._render_properties)
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
     @jsii.member(jsii_name="attrDomain")
     def attr_domain(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Domain: The domain with protocol.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDomain"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDomainName")
     def attr_domain_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: DomainName: The domain name
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDomainName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="domainName")
     def domain_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: domainName: domain name
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "domainName"))
 
     @domain_name.setter
     def domain_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCustomDomain, "domain_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "domainName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCustomDomain, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="protocol")
     def protocol(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: protocol: HTTP or HTTP,HTTPS
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "protocol"))
 
     @protocol.setter
     def protocol(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCustomDomain, "protocol").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "protocol", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="apiVersion")
     def api_version(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: apiVersion: api version
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "apiVersion"))
 
     @api_version.setter
     def api_version(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCustomDomain, "api_version").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "apiVersion", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="certConfig")
     def cert_config(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosCustomDomain.CertConfigProperty"]]:
         '''
         :Property: certConfig: certificate info
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosCustomDomain.CertConfigProperty"]], jsii.get(self, "certConfig"))
 
     @cert_config.setter
     def cert_config(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosCustomDomain.CertConfigProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCustomDomain, "cert_config").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "certConfig", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="routeConfig")
     def route_config(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosCustomDomain.RouteConfigProperty"]]:
         '''
         :Property: routeConfig: Routing table: path to function mappingwhen a function is called with a custom domain name
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosCustomDomain.RouteConfigProperty"]], jsii.get(self, "routeConfig"))
 
     @route_config.setter
     def route_config(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosCustomDomain.RouteConfigProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCustomDomain, "route_config").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "routeConfig", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-fc.RosCustomDomain.CertConfigProperty",
         jsii_struct_bases=[],
         name_mapping={
             "certificate": "certificate",
@@ -1518,14 +1676,19 @@
             private_key: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         ) -> None:
             '''
             :param certificate: 
             :param cert_name: 
             :param private_key: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosCustomDomain.CertConfigProperty.__init__)
+                check_type(argname="argument certificate", value=certificate, expected_type=type_hints["certificate"])
+                check_type(argname="argument cert_name", value=cert_name, expected_type=type_hints["cert_name"])
+                check_type(argname="argument private_key", value=private_key, expected_type=type_hints["private_key"])
             self._values: typing.Dict[str, typing.Any] = {
                 "certificate": certificate,
                 "cert_name": cert_name,
                 "private_key": private_key,
             }
 
         @builtins.property
@@ -1571,19 +1734,22 @@
         jsii_struct_bases=[],
         name_mapping={"routes": "routes"},
     )
     class RouteConfigProperty:
         def __init__(
             self,
             *,
-            routes: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosCustomDomain.RoutesProperty"]]],
+            routes: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosCustomDomain.RoutesProperty", typing.Dict[str, typing.Any]]]]],
         ) -> None:
             '''
             :param routes: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosCustomDomain.RouteConfigProperty.__init__)
+                check_type(argname="argument routes", value=routes, expected_type=type_hints["routes"])
             self._values: typing.Dict[str, typing.Any] = {
                 "routes": routes,
             }
 
         @builtins.property
         def routes(
             self,
@@ -1627,14 +1793,20 @@
         ) -> None:
             '''
             :param function_name: 
             :param path: 
             :param service_name: 
             :param qualifier: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosCustomDomain.RoutesProperty.__init__)
+                check_type(argname="argument function_name", value=function_name, expected_type=type_hints["function_name"])
+                check_type(argname="argument path", value=path, expected_type=type_hints["path"])
+                check_type(argname="argument service_name", value=service_name, expected_type=type_hints["service_name"])
+                check_type(argname="argument qualifier", value=qualifier, expected_type=type_hints["qualifier"])
             self._values: typing.Dict[str, typing.Any] = {
                 "function_name": function_name,
                 "path": path,
                 "service_name": service_name,
             }
             if qualifier is not None:
                 self._values["qualifier"] = qualifier
@@ -1702,25 +1874,32 @@
 class RosCustomDomainProps:
     def __init__(
         self,
         *,
         domain_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         protocol: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         api_version: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        cert_config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, RosCustomDomain.CertConfigProperty]] = None,
-        route_config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, RosCustomDomain.RouteConfigProperty]] = None,
+        cert_config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosCustomDomain.CertConfigProperty, typing.Dict[str, typing.Any]]]] = None,
+        route_config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosCustomDomain.RouteConfigProperty, typing.Dict[str, typing.Any]]]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::FC::CustomDomain``.
 
         :param domain_name: 
         :param protocol: 
         :param api_version: 
         :param cert_config: 
         :param route_config: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosCustomDomainProps.__init__)
+            check_type(argname="argument domain_name", value=domain_name, expected_type=type_hints["domain_name"])
+            check_type(argname="argument protocol", value=protocol, expected_type=type_hints["protocol"])
+            check_type(argname="argument api_version", value=api_version, expected_type=type_hints["api_version"])
+            check_type(argname="argument cert_config", value=cert_config, expected_type=type_hints["cert_config"])
+            check_type(argname="argument route_config", value=route_config, expected_type=type_hints["route_config"])
         self._values: typing.Dict[str, typing.Any] = {
             "domain_name": domain_name,
             "protocol": protocol,
         }
         if api_version is not None:
             self._values["api_version"] = api_version
         if cert_config is not None:
@@ -1795,358 +1974,418 @@
 ):
     '''A ROS template type:  ``ALIYUN::FC::Function``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosFunctionProps",
+        props: typing.Union["RosFunctionProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::FC::Function``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosFunction.__init__)
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
+            type_hints = typing.get_type_hints(RosFunction._render_properties)
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
     @jsii.member(jsii_name="attrArn")
     def attr_arn(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ARN: The ARN for ALIYUN::ROS::CustomResource
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrArn"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrFunctionId")
     def attr_function_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: FunctionId: The function ID
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrFunctionId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrFunctionName")
     def attr_function_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: FunctionName: The function name
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrFunctionName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrServiceId")
     def attr_service_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ServiceId: The service ID
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrServiceId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrServiceName")
     def attr_service_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ServiceName: The service name
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrServiceName"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosFunction, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="functionName")
     def function_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: functionName: Function name
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "functionName"))
 
     @function_name.setter
     def function_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosFunction, "function_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "functionName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="handler")
     def handler(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: handler: The function execution entry point.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "handler"))
 
     @handler.setter
     def handler(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosFunction, "handler").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "handler", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="runtime")
     def runtime(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: runtime: The function runtime environment. Supporting nodejs6, nodejs8, nodejs10, nodejs12, python2.7, python3, java8, custom, custom-container and so on
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "runtime"))
 
     @runtime.setter
     def runtime(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosFunction, "runtime").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "runtime", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="serviceName")
     def service_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: serviceName: Service name
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "serviceName"))
 
     @service_name.setter
     def service_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosFunction, "service_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "serviceName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="asyncConfiguration")
     def async_configuration(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosFunction.AsyncConfigurationProperty"]]:
         '''
         :Property: asyncConfiguration: Configuration of asynchronous function calls
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosFunction.AsyncConfigurationProperty"]], jsii.get(self, "asyncConfiguration"))
 
     @async_configuration.setter
     def async_configuration(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosFunction.AsyncConfigurationProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosFunction, "async_configuration").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "asyncConfiguration", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="caPort")
     def ca_port(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: caPort: Custom runtime and custom container runtime dedicated fields, which represent the port that the started custom http server listens to. The default value is 9000
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "caPort"))
 
     @ca_port.setter
     def ca_port(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosFunction, "ca_port").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "caPort", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="code")
     def code(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosFunction.CodeProperty"]]:
         '''
         :Property: code: The code that contains the function implementation.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosFunction.CodeProperty"]], jsii.get(self, "code"))
 
     @code.setter
     def code(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosFunction.CodeProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosFunction, "code").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "code", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="customContainerConfig")
     def custom_container_config(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosFunction.CustomContainerConfigProperty"]]:
         '''
         :Property: customContainerConfig: Custom container runtime related configuration. After configuration, the function can be replaced with a custom container to execute the function
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosFunction.CustomContainerConfigProperty"]], jsii.get(self, "customContainerConfig"))
 
     @custom_container_config.setter
     def custom_container_config(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosFunction.CustomContainerConfigProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosFunction, "custom_container_config").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "customContainerConfig", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="description")
     def description(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: description: Function description
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "description"))
 
     @description.setter
     def description(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosFunction, "description").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "description", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="environmentVariables")
     def environment_variables(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]]]:
         '''
         :Property: environmentVariables: The environment variable set for the function, you can get the value of the environment variable in the function.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]]], jsii.get(self, "environmentVariables"))
 
     @environment_variables.setter
     def environment_variables(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosFunction, "environment_variables").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "environmentVariables", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="initializationTimeout")
     def initialization_timeout(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: initializationTimeout: the max execution time of the initializer, in second
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "initializationTimeout"))
 
     @initialization_timeout.setter
     def initialization_timeout(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosFunction, "initialization_timeout").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "initializationTimeout", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="initializer")
     def initializer(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: initializer: the entry point of the initializer
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "initializer"))
 
     @initializer.setter
     def initializer(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosFunction, "initializer").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "initializer", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="instanceConcurrency")
     def instance_concurrency(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: instanceConcurrency: Function instance concurrency. Value can be between 1 to 100.
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "instanceConcurrency"))
 
     @instance_concurrency.setter
     def instance_concurrency(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosFunction, "instance_concurrency").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "instanceConcurrency", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="instanceType")
     def instance_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: instanceType: Instance type. Value:e1: flexible instance. Memory size between 128 and 3072c1: performance instance. Memory size allow values are 4096, 8192, 16384 and 32768
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "instanceType"))
 
     @instance_type.setter
     def instance_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosFunction, "instance_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "instanceType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="memorySize")
     def memory_size(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: memorySize: The amount of memory that’s used to run function, in MB. Function Compute uses this value to allocate CPU resources proportionally. Defaults to 128 MB. It can be multiple of 64 MB and between 128 MB and 3072 MB.
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "memorySize"))
 
     @memory_size.setter
     def memory_size(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosFunction, "memory_size").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "memorySize", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="timeout")
     def timeout(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: timeout: The maximum time duration a function can run, in seconds. After which Function Compute terminates the execution. Defaults to 3 seconds, and can be between 1 to 600 seconds.
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "timeout"))
 
     @timeout.setter
     def timeout(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosFunction, "timeout").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "timeout", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-fc.RosFunction.AsyncConfigurationProperty",
         jsii_struct_bases=[],
         name_mapping={
             "destination": "destination",
@@ -2155,25 +2394,31 @@
             "stateful_invocation": "statefulInvocation",
         },
     )
     class AsyncConfigurationProperty:
         def __init__(
             self,
             *,
-            destination: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosFunction.DestinationProperty"]] = None,
+            destination: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosFunction.DestinationProperty", typing.Dict[str, typing.Any]]]] = None,
             max_async_event_age_in_seconds: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
             max_async_retry_attempts: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
             stateful_invocation: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param destination: 
             :param max_async_event_age_in_seconds: 
             :param max_async_retry_attempts: 
             :param stateful_invocation: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosFunction.AsyncConfigurationProperty.__init__)
+                check_type(argname="argument destination", value=destination, expected_type=type_hints["destination"])
+                check_type(argname="argument max_async_event_age_in_seconds", value=max_async_event_age_in_seconds, expected_type=type_hints["max_async_event_age_in_seconds"])
+                check_type(argname="argument max_async_retry_attempts", value=max_async_retry_attempts, expected_type=type_hints["max_async_retry_attempts"])
+                check_type(argname="argument stateful_invocation", value=stateful_invocation, expected_type=type_hints["stateful_invocation"])
             self._values: typing.Dict[str, typing.Any] = {}
             if destination is not None:
                 self._values["destination"] = destination
             if max_async_event_age_in_seconds is not None:
                 self._values["max_async_event_age_in_seconds"] = max_async_event_age_in_seconds
             if max_async_retry_attempts is not None:
                 self._values["max_async_retry_attempts"] = max_async_retry_attempts
@@ -2252,14 +2497,20 @@
         ) -> None:
             '''
             :param oss_bucket_name: 
             :param oss_object_name: 
             :param source_code: 
             :param zip_file: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosFunction.CodeProperty.__init__)
+                check_type(argname="argument oss_bucket_name", value=oss_bucket_name, expected_type=type_hints["oss_bucket_name"])
+                check_type(argname="argument oss_object_name", value=oss_object_name, expected_type=type_hints["oss_object_name"])
+                check_type(argname="argument source_code", value=source_code, expected_type=type_hints["source_code"])
+                check_type(argname="argument zip_file", value=zip_file, expected_type=type_hints["zip_file"])
             self._values: typing.Dict[str, typing.Any] = {}
             if oss_bucket_name is not None:
                 self._values["oss_bucket_name"] = oss_bucket_name
             if oss_object_name is not None:
                 self._values["oss_object_name"] = oss_object_name
             if source_code is not None:
                 self._values["source_code"] = source_code
@@ -2354,14 +2605,21 @@
             '''
             :param image: 
             :param acceleration_type: 
             :param args: 
             :param command: 
             :param instance_id: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosFunction.CustomContainerConfigProperty.__init__)
+                check_type(argname="argument image", value=image, expected_type=type_hints["image"])
+                check_type(argname="argument acceleration_type", value=acceleration_type, expected_type=type_hints["acceleration_type"])
+                check_type(argname="argument args", value=args, expected_type=type_hints["args"])
+                check_type(argname="argument command", value=command, expected_type=type_hints["command"])
+                check_type(argname="argument instance_id", value=instance_id, expected_type=type_hints["instance_id"])
             self._values: typing.Dict[str, typing.Any] = {
                 "image": image,
             }
             if acceleration_type is not None:
                 self._values["acceleration_type"] = acceleration_type
             if args is not None:
                 self._values["args"] = args
@@ -2446,14 +2704,18 @@
             on_failure: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
             on_success: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param on_failure: 
             :param on_success: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosFunction.DestinationProperty.__init__)
+                check_type(argname="argument on_failure", value=on_failure, expected_type=type_hints["on_failure"])
+                check_type(argname="argument on_success", value=on_success, expected_type=type_hints["on_success"])
             self._values: typing.Dict[str, typing.Any] = {}
             if on_failure is not None:
                 self._values["on_failure"] = on_failure
             if on_success is not None:
                 self._values["on_success"] = on_success
 
         @builtins.property
@@ -2495,130 +2757,151 @@
 ):
     '''A ROS template type:  ``ALIYUN::FC::FunctionInvoker``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosFunctionInvokerProps",
+        props: typing.Union["RosFunctionInvokerProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::FC::FunctionInvoker``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosFunctionInvoker.__init__)
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
+            type_hints = typing.get_type_hints(RosFunctionInvoker._render_properties)
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
     @jsii.member(jsii_name="attrResult")
     def attr_result(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute:
 
         Result: Depends on result type:
         NoResult: Async invoke has no result.
         Success: The response of the function. The response should be utf-8 encoded string, otherwise ROS will report an error. If the response is binary, encode it via base64 before it is returned.
         Failure: Error Message.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrResult"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrResultType")
     def attr_result_type(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute:
 
         ResultType: Result type:
         NoResult: Async invoke has no result.
         Success: Sync invoke succeeds.
         Failure: Sync invoke fails.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrResultType"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosFunctionInvoker, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="functionName")
     def function_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: functionName: Function name
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "functionName"))
 
     @function_name.setter
     def function_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosFunctionInvoker, "function_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "functionName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="serviceName")
     def service_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: serviceName: Service name
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "serviceName"))
 
     @service_name.setter
     def service_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosFunctionInvoker, "service_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "serviceName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="async")
     def async_(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property: async: Invocation type, Sync or Async. Defaults to Sync.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "async"))
 
     @async_.setter
     def async_(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosFunctionInvoker, "async_").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "async", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="checkError")
     def check_error(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -2629,17 +2912,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "checkError"))
 
     @check_error.setter
     def check_error(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosFunctionInvoker, "check_error").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "checkError", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="event")
     def event(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -2649,65 +2935,77 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "event"))
 
     @event.setter
     def event(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosFunctionInvoker, "event").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "event", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="executeVersion")
     def execute_version(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: executeVersion: If the property is not specified for creation and update, the function will not be invoked. The change of the property leads to the invoke of the function.
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "executeVersion"))
 
     @execute_version.setter
     def execute_version(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosFunctionInvoker, "execute_version").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "executeVersion", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="qualifier")
     def qualifier(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: qualifier: service version, can be versionId or aliasName
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "qualifier"))
 
     @qualifier.setter
     def qualifier(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosFunctionInvoker, "qualifier").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "qualifier", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="serviceRegionId")
     def service_region_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: serviceRegionId: Which region service belongs to.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "serviceRegionId"))
 
     @service_region_id.setter
     def service_region_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosFunctionInvoker, "service_region_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "serviceRegionId", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-fc.RosFunctionInvokerProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -2741,14 +3039,24 @@
         :param async_: 
         :param check_error: 
         :param event: 
         :param execute_version: 
         :param qualifier: 
         :param service_region_id: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosFunctionInvokerProps.__init__)
+            check_type(argname="argument function_name", value=function_name, expected_type=type_hints["function_name"])
+            check_type(argname="argument service_name", value=service_name, expected_type=type_hints["service_name"])
+            check_type(argname="argument async_", value=async_, expected_type=type_hints["async_"])
+            check_type(argname="argument check_error", value=check_error, expected_type=type_hints["check_error"])
+            check_type(argname="argument event", value=event, expected_type=type_hints["event"])
+            check_type(argname="argument execute_version", value=execute_version, expected_type=type_hints["execute_version"])
+            check_type(argname="argument qualifier", value=qualifier, expected_type=type_hints["qualifier"])
+            check_type(argname="argument service_region_id", value=service_region_id, expected_type=type_hints["service_region_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "function_name": function_name,
             "service_name": service_name,
         }
         if async_ is not None:
             self._values["async_"] = async_
         if check_error is not None:
@@ -2885,18 +3193,18 @@
     def __init__(
         self,
         *,
         function_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         handler: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         runtime: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         service_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
-        async_configuration: typing.Optional[typing.Union[ros_cdk_core.IResolvable, RosFunction.AsyncConfigurationProperty]] = None,
+        async_configuration: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosFunction.AsyncConfigurationProperty, typing.Dict[str, typing.Any]]]] = None,
         ca_port: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
-        code: typing.Optional[typing.Union[ros_cdk_core.IResolvable, RosFunction.CodeProperty]] = None,
-        custom_container_config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, RosFunction.CustomContainerConfigProperty]] = None,
+        code: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosFunction.CodeProperty, typing.Dict[str, typing.Any]]]] = None,
+        custom_container_config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosFunction.CustomContainerConfigProperty, typing.Dict[str, typing.Any]]]] = None,
         description: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         environment_variables: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]]] = None,
         initialization_timeout: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         initializer: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         instance_concurrency: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         instance_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         memory_size: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
@@ -2917,14 +3225,32 @@
         :param initialization_timeout: 
         :param initializer: 
         :param instance_concurrency: 
         :param instance_type: 
         :param memory_size: 
         :param timeout: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosFunctionProps.__init__)
+            check_type(argname="argument function_name", value=function_name, expected_type=type_hints["function_name"])
+            check_type(argname="argument handler", value=handler, expected_type=type_hints["handler"])
+            check_type(argname="argument runtime", value=runtime, expected_type=type_hints["runtime"])
+            check_type(argname="argument service_name", value=service_name, expected_type=type_hints["service_name"])
+            check_type(argname="argument async_configuration", value=async_configuration, expected_type=type_hints["async_configuration"])
+            check_type(argname="argument ca_port", value=ca_port, expected_type=type_hints["ca_port"])
+            check_type(argname="argument code", value=code, expected_type=type_hints["code"])
+            check_type(argname="argument custom_container_config", value=custom_container_config, expected_type=type_hints["custom_container_config"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument environment_variables", value=environment_variables, expected_type=type_hints["environment_variables"])
+            check_type(argname="argument initialization_timeout", value=initialization_timeout, expected_type=type_hints["initialization_timeout"])
+            check_type(argname="argument initializer", value=initializer, expected_type=type_hints["initializer"])
+            check_type(argname="argument instance_concurrency", value=instance_concurrency, expected_type=type_hints["instance_concurrency"])
+            check_type(argname="argument instance_type", value=instance_type, expected_type=type_hints["instance_type"])
+            check_type(argname="argument memory_size", value=memory_size, expected_type=type_hints["memory_size"])
+            check_type(argname="argument timeout", value=timeout, expected_type=type_hints["timeout"])
         self._values: typing.Dict[str, typing.Any] = {
             "function_name": function_name,
             "handler": handler,
             "runtime": runtime,
             "service_name": service_name,
         }
         if async_configuration is not None:
@@ -3127,142 +3453,166 @@
 ):
     '''A ROS template type:  ``ALIYUN::FC::Layer``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosLayerProps",
+        props: typing.Union["RosLayerProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::FC::Layer``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosLayer.__init__)
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
+            type_hints = typing.get_type_hints(RosLayer._render_properties)
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
     @jsii.member(jsii_name="attrArn")
     def attr_arn(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Arn: The name of the layer resource.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrArn"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrLayerName")
     def attr_layer_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: LayerName: The name of layer
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrLayerName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVersion")
     def attr_version(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Version: The version of the layer resource.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVersion"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="code")
     def code(self) -> typing.Union[ros_cdk_core.IResolvable, "RosLayer.CodeProperty"]:
         '''
         :Property: code: The code of layer.
         '''
         return typing.cast(typing.Union[ros_cdk_core.IResolvable, "RosLayer.CodeProperty"], jsii.get(self, "code"))
 
     @code.setter
     def code(
         self,
         value: typing.Union[ros_cdk_core.IResolvable, "RosLayer.CodeProperty"],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosLayer, "code").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "code", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="compatibleRuntime")
     def compatible_runtime(
         self,
     ) -> typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]:
         '''
         :Property: compatibleRuntime: The runtime environment supported by the layer. For example:nodejs12, nodejs10, nodejs8, nodejs6, python3, and python2.7
         '''
         return typing.cast(typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]], jsii.get(self, "compatibleRuntime"))
 
     @compatible_runtime.setter
     def compatible_runtime(
         self,
         value: typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosLayer, "compatible_runtime").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "compatibleRuntime", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosLayer, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="layerName")
     def layer_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: layerName: The name of layer
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "layerName"))
 
     @layer_name.setter
     def layer_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosLayer, "layer_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "layerName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="description")
     def description(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: description: The description of the layer.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "description"))
 
     @description.setter
     def description(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosLayer, "description").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "description", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-fc.RosLayer.CodeProperty",
         jsii_struct_bases=[],
         name_mapping={
             "oss_bucket_name": "ossBucketName",
@@ -3279,14 +3629,19 @@
             zip_file: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param oss_bucket_name: 
             :param oss_object_name: 
             :param zip_file: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosLayer.CodeProperty.__init__)
+                check_type(argname="argument oss_bucket_name", value=oss_bucket_name, expected_type=type_hints["oss_bucket_name"])
+                check_type(argname="argument oss_object_name", value=oss_object_name, expected_type=type_hints["oss_object_name"])
+                check_type(argname="argument zip_file", value=zip_file, expected_type=type_hints["zip_file"])
             self._values: typing.Dict[str, typing.Any] = {}
             if oss_bucket_name is not None:
                 self._values["oss_bucket_name"] = oss_bucket_name
             if oss_object_name is not None:
                 self._values["oss_object_name"] = oss_object_name
             if zip_file is not None:
                 self._values["zip_file"] = zip_file
@@ -3353,26 +3708,32 @@
         "description": "description",
     },
 )
 class RosLayerProps:
     def __init__(
         self,
         *,
-        code: typing.Union[ros_cdk_core.IResolvable, RosLayer.CodeProperty],
+        code: typing.Union[ros_cdk_core.IResolvable, typing.Union[RosLayer.CodeProperty, typing.Dict[str, typing.Any]]],
         compatible_runtime: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]],
         layer_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         description: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::FC::Layer``.
 
         :param code: 
         :param compatible_runtime: 
         :param layer_name: 
         :param description: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosLayerProps.__init__)
+            check_type(argname="argument code", value=code, expected_type=type_hints["code"])
+            check_type(argname="argument compatible_runtime", value=compatible_runtime, expected_type=type_hints["compatible_runtime"])
+            check_type(argname="argument layer_name", value=layer_name, expected_type=type_hints["layer_name"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
         self._values: typing.Dict[str, typing.Any] = {
             "code": code,
             "compatible_runtime": compatible_runtime,
             "layer_name": layer_name,
         }
         if description is not None:
             self._values["description"] = description
@@ -3435,112 +3796,127 @@
 ):
     '''A ROS template type:  ``ALIYUN::FC::ProvisionConfig``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosProvisionConfigProps",
+        props: typing.Union["RosProvisionConfigProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::FC::ProvisionConfig``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosProvisionConfig.__init__)
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
+            type_hints = typing.get_type_hints(RosProvisionConfig._render_properties)
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
     @jsii.member(jsii_name="attrFunctionName")
     def attr_function_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: FunctionName: The function name
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrFunctionName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrQualifier")
     def attr_qualifier(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Qualifier: The service alias
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrQualifier"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrResource")
     def attr_resource(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Resource: The resource
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrResource"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrServiceName")
     def attr_service_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ServiceName: The service name
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrServiceName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTarget")
     def attr_target(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Target: Number of provision
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTarget"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosProvisionConfig, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="functionName")
     def function_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: functionName: Function name
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "functionName"))
 
     @function_name.setter
     def function_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosProvisionConfig, "function_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "functionName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="qualifier")
     def qualifier(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         qualifier: Service's alias.
         Example : "LATEST"
@@ -3548,44 +3924,53 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "qualifier"))
 
     @qualifier.setter
     def qualifier(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosProvisionConfig, "qualifier").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "qualifier", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="serviceName")
     def service_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: serviceName: Service name
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "serviceName"))
 
     @service_name.setter
     def service_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosProvisionConfig, "service_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "serviceName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="target")
     def target(self) -> typing.Union[jsii.Number, ros_cdk_core.IResolvable]:
         '''
         :Property: target: Number of provision
         '''
         return typing.cast(typing.Union[jsii.Number, ros_cdk_core.IResolvable], jsii.get(self, "target"))
 
     @target.setter
     def target(
         self,
         value: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosProvisionConfig, "target").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "target", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-fc.RosProvisionConfigProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -3607,14 +3992,20 @@
         '''Properties for defining a ``ALIYUN::FC::ProvisionConfig``.
 
         :param function_name: 
         :param qualifier: 
         :param service_name: 
         :param target: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosProvisionConfigProps.__init__)
+            check_type(argname="argument function_name", value=function_name, expected_type=type_hints["function_name"])
+            check_type(argname="argument qualifier", value=qualifier, expected_type=type_hints["qualifier"])
+            check_type(argname="argument service_name", value=service_name, expected_type=type_hints["service_name"])
+            check_type(argname="argument target", value=target, expected_type=type_hints["target"])
         self._values: typing.Dict[str, typing.Any] = {
             "function_name": function_name,
             "qualifier": qualifier,
             "service_name": service_name,
             "target": target,
         }
 
@@ -3676,270 +4067,309 @@
 ):
     '''A ROS template type:  ``ALIYUN::FC::Service``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosServiceProps",
+        props: typing.Union["RosServiceProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::FC::Service``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosService.__init__)
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
+            type_hints = typing.get_type_hints(RosService._render_properties)
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
     @jsii.member(jsii_name="attrInternetAccess")
     def attr_internet_access(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: InternetAccess: Whether enable Internet access
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInternetAccess"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrLogProject")
     def attr_log_project(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: LogProject: Log project of service
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrLogProject"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrLogstore")
     def attr_logstore(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Logstore: Log store of service
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrLogstore"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrRole")
     def attr_role(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Role: Role of service
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrRole"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrServiceId")
     def attr_service_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ServiceId: The service ID
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrServiceId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrServiceName")
     def attr_service_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ServiceName: The service name
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrServiceName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTags")
     def attr_tags(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Tags: Tags of service
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTags"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVpcId")
     def attr_vpc_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: VpcId: VPC ID
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVpcId"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosService, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="serviceName")
     def service_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: serviceName: Service name
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "serviceName"))
 
     @service_name.setter
     def service_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosService, "service_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "serviceName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="deletionForce")
     def deletion_force(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property: deletionForce: Whether force delete the service without waiting for network interfaces to be cleaned up if VpcConfig is specified. Default value is false.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "deletionForce"))
 
     @deletion_force.setter
     def deletion_force(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosService, "deletion_force").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "deletionForce", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="description")
     def description(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: description: Service description
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "description"))
 
     @description.setter
     def description(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosService, "description").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "description", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="internetAccess")
     def internet_access(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property: internetAccess: Set it to true to enable Internet access.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "internetAccess"))
 
     @internet_access.setter
     def internet_access(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosService, "internet_access").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "internetAccess", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="logConfig")
     def log_config(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosService.LogConfigProperty"]]:
         '''
         :Property: logConfig: Log configuration. Function Compute pushes function execution logs to the configured log store.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosService.LogConfigProperty"]], jsii.get(self, "logConfig"))
 
     @log_config.setter
     def log_config(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosService.LogConfigProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosService, "log_config").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "logConfig", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="nasConfig")
     def nas_config(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosService.NasConfigProperty"]]:
         '''
         :Property: nasConfig: NAS configuration. Function Compute uses a specified NAS configured on the service.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosService.NasConfigProperty"]], jsii.get(self, "nasConfig"))
 
     @nas_config.setter
     def nas_config(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosService.NasConfigProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosService, "nas_config").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "nasConfig", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="role")
     def role(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: role: The role grants Function Compute the permission to access user’s cloud resources, such as pushing logs to user’s log store. The temporary STS token generated from this role can be retrieved from function context and used to access cloud resources.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "role"))
 
     @role.setter
     def role(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosService, "role").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "role", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="tags")
     def tags(self) -> typing.Optional[typing.List["RosService.TagsProperty"]]:
         '''
         :Property: tags: Tags to attach to service. Max support 20 tags to add during create service. Each tag with two properties Key and Value, and Key is required.
         '''
         return typing.cast(typing.Optional[typing.List["RosService.TagsProperty"]], jsii.get(self, "tags"))
 
     @tags.setter
     def tags(
         self,
         value: typing.Optional[typing.List["RosService.TagsProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosService, "tags").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "tags", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="tracingConfig")
     def tracing_config(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosService.TracingConfigProperty"]]:
         '''
         :Property: tracingConfig: The Tracing Analysis configuration. After Function Compute integrates with Tracing Analysis, you can record the stay time of a request in Function Compute, view the cold start time for a function, and record the execution time of a function.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosService.TracingConfigProperty"]], jsii.get(self, "tracingConfig"))
 
     @tracing_config.setter
     def tracing_config(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosService.TracingConfigProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosService, "tracing_config").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "tracingConfig", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vpcBindings")
     def vpc_bindings(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]]:
         '''
         :Property:
 
@@ -3949,31 +4379,37 @@
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]], jsii.get(self, "vpcBindings"))
 
     @vpc_bindings.setter
     def vpc_bindings(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosService, "vpc_bindings").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "vpcBindings", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vpcConfig")
     def vpc_config(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosService.VpcConfigProperty"]]:
         '''
         :Property: vpcConfig: VPC configuration. Function Compute uses the config to setup ENI in the specific VPC.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosService.VpcConfigProperty"]], jsii.get(self, "vpcConfig"))
 
     @vpc_config.setter
     def vpc_config(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosService.VpcConfigProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosService, "vpc_config").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "vpcConfig", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-fc.RosService.LogConfigProperty",
         jsii_struct_bases=[],
         name_mapping={
             "enable_request_metrics": "enableRequestMetrics",
@@ -3993,14 +4429,20 @@
         ) -> None:
             '''
             :param enable_request_metrics: 
             :param log_begin_rule: 
             :param logstore: 
             :param project: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosService.LogConfigProperty.__init__)
+                check_type(argname="argument enable_request_metrics", value=enable_request_metrics, expected_type=type_hints["enable_request_metrics"])
+                check_type(argname="argument log_begin_rule", value=log_begin_rule, expected_type=type_hints["log_begin_rule"])
+                check_type(argname="argument logstore", value=logstore, expected_type=type_hints["logstore"])
+                check_type(argname="argument project", value=project, expected_type=type_hints["project"])
             self._values: typing.Dict[str, typing.Any] = {}
             if enable_request_metrics is not None:
                 self._values["enable_request_metrics"] = enable_request_metrics
             if log_begin_rule is not None:
                 self._values["log_begin_rule"] = log_begin_rule
             if logstore is not None:
                 self._values["logstore"] = logstore
@@ -4078,14 +4520,18 @@
             mount_dir: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             server_addr: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         ) -> None:
             '''
             :param mount_dir: 
             :param server_addr: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosService.MountPointsProperty.__init__)
+                check_type(argname="argument mount_dir", value=mount_dir, expected_type=type_hints["mount_dir"])
+                check_type(argname="argument server_addr", value=server_addr, expected_type=type_hints["server_addr"])
             self._values: typing.Dict[str, typing.Any] = {
                 "mount_dir": mount_dir,
                 "server_addr": server_addr,
             }
 
         @builtins.property
         def mount_dir(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
@@ -4126,22 +4572,27 @@
         },
     )
     class NasConfigProperty:
         def __init__(
             self,
             *,
             group_id: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
-            mount_points: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosService.MountPointsProperty"]]],
+            mount_points: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosService.MountPointsProperty", typing.Dict[str, typing.Any]]]]],
             user_id: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
         ) -> None:
             '''
             :param group_id: 
             :param mount_points: 
             :param user_id: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosService.NasConfigProperty.__init__)
+                check_type(argname="argument group_id", value=group_id, expected_type=type_hints["group_id"])
+                check_type(argname="argument mount_points", value=mount_points, expected_type=type_hints["mount_points"])
+                check_type(argname="argument user_id", value=user_id, expected_type=type_hints["user_id"])
             self._values: typing.Dict[str, typing.Any] = {
                 "group_id": group_id,
                 "mount_points": mount_points,
                 "user_id": user_id,
             }
 
         @builtins.property
@@ -4196,14 +4647,18 @@
             key: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param key: 
             :param value: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosService.TagsProperty.__init__)
+                check_type(argname="argument key", value=key, expected_type=type_hints["key"])
+                check_type(argname="argument value", value=value, expected_type=type_hints["value"])
             self._values: typing.Dict[str, typing.Any] = {
                 "key": key,
             }
             if value is not None:
                 self._values["value"] = value
 
         @builtins.property
@@ -4248,14 +4703,18 @@
             params: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]]] = None,
             type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param params: 
             :param type: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosService.TracingConfigProperty.__init__)
+                check_type(argname="argument params", value=params, expected_type=type_hints["params"])
+                check_type(argname="argument type", value=type, expected_type=type_hints["type"])
             self._values: typing.Dict[str, typing.Any] = {}
             if params is not None:
                 self._values["params"] = params
             if type is not None:
                 self._values["type"] = type
 
         @builtins.property
@@ -4307,14 +4766,19 @@
             v_switch_ids: typing.Union[typing.Sequence[typing.Any], ros_cdk_core.IResolvable],
         ) -> None:
             '''
             :param security_group_id: 
             :param vpc_id: 
             :param v_switch_ids: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosService.VpcConfigProperty.__init__)
+                check_type(argname="argument security_group_id", value=security_group_id, expected_type=type_hints["security_group_id"])
+                check_type(argname="argument vpc_id", value=vpc_id, expected_type=type_hints["vpc_id"])
+                check_type(argname="argument v_switch_ids", value=v_switch_ids, expected_type=type_hints["v_switch_ids"])
             self._values: typing.Dict[str, typing.Any] = {
                 "security_group_id": security_group_id,
                 "vpc_id": vpc_id,
                 "v_switch_ids": v_switch_ids,
             }
 
         @builtins.property
@@ -4381,21 +4845,21 @@
     def __init__(
         self,
         *,
         service_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         deletion_force: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         description: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         internet_access: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
-        log_config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, RosService.LogConfigProperty]] = None,
-        nas_config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, RosService.NasConfigProperty]] = None,
+        log_config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosService.LogConfigProperty, typing.Dict[str, typing.Any]]]] = None,
+        nas_config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosService.NasConfigProperty, typing.Dict[str, typing.Any]]]] = None,
         role: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        tags: typing.Optional[typing.Sequence[RosService.TagsProperty]] = None,
-        tracing_config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, RosService.TracingConfigProperty]] = None,
+        tags: typing.Optional[typing.Sequence[typing.Union[RosService.TagsProperty, typing.Dict[str, typing.Any]]]] = None,
+        tracing_config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosService.TracingConfigProperty, typing.Dict[str, typing.Any]]]] = None,
         vpc_bindings: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]] = None,
-        vpc_config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, RosService.VpcConfigProperty]] = None,
+        vpc_config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosService.VpcConfigProperty, typing.Dict[str, typing.Any]]]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::FC::Service``.
 
         :param service_name: 
         :param deletion_force: 
         :param description: 
         :param internet_access: 
@@ -4403,14 +4867,27 @@
         :param nas_config: 
         :param role: 
         :param tags: 
         :param tracing_config: 
         :param vpc_bindings: 
         :param vpc_config: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosServiceProps.__init__)
+            check_type(argname="argument service_name", value=service_name, expected_type=type_hints["service_name"])
+            check_type(argname="argument deletion_force", value=deletion_force, expected_type=type_hints["deletion_force"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument internet_access", value=internet_access, expected_type=type_hints["internet_access"])
+            check_type(argname="argument log_config", value=log_config, expected_type=type_hints["log_config"])
+            check_type(argname="argument nas_config", value=nas_config, expected_type=type_hints["nas_config"])
+            check_type(argname="argument role", value=role, expected_type=type_hints["role"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
+            check_type(argname="argument tracing_config", value=tracing_config, expected_type=type_hints["tracing_config"])
+            check_type(argname="argument vpc_bindings", value=vpc_bindings, expected_type=type_hints["vpc_bindings"])
+            check_type(argname="argument vpc_config", value=vpc_config, expected_type=type_hints["vpc_config"])
         self._values: typing.Dict[str, typing.Any] = {
             "service_name": service_name,
         }
         if deletion_force is not None:
             self._values["deletion_force"] = deletion_force
         if description is not None:
             self._values["description"] = description
@@ -4560,136 +5037,157 @@
 ):
     '''A ROS template type:  ``ALIYUN::FC::Trigger``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosTriggerProps",
+        props: typing.Union["RosTriggerProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::FC::Trigger``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosTrigger.__init__)
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
+            type_hints = typing.get_type_hints(RosTrigger._render_properties)
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
     @jsii.member(jsii_name="attrFunctionName")
     def attr_function_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: FunctionName: Function name.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrFunctionName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrServiceName")
     def attr_service_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ServiceName: Service name.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrServiceName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTriggerId")
     def attr_trigger_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: TriggerId: The trigger ID.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTriggerId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTriggerName")
     def attr_trigger_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: TriggerName: Trigger name.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTriggerName"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosTrigger, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="functionName")
     def function_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: functionName: Function name.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "functionName"))
 
     @function_name.setter
     def function_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTrigger, "function_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "functionName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="serviceName")
     def service_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: serviceName: Service name.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "serviceName"))
 
     @service_name.setter
     def service_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTrigger, "service_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "serviceName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="triggerConfig")
     def trigger_config(
         self,
     ) -> typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]]:
         '''
         :Property: triggerConfig: Event source specific trigger configuration. The value is different according to trigger type.
         '''
         return typing.cast(typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]], jsii.get(self, "triggerConfig"))
 
     @trigger_config.setter
     def trigger_config(
         self,
         value: typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTrigger, "trigger_config").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "triggerConfig", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="triggerName")
     def trigger_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         triggerName: Trigger name.
         Example : "image_resize"
@@ -4697,17 +5195,20 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "triggerName"))
 
     @trigger_name.setter
     def trigger_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTrigger, "trigger_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "triggerName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="triggerType")
     def trigger_type(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         triggerType: Trigger type, e.g. oss, timer, logs. This determines how the trigger config is interpreted.
         Example : "oss"
@@ -4715,17 +5216,20 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "triggerType"))
 
     @trigger_type.setter
     def trigger_type(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTrigger, "trigger_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "triggerType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="invocationRole")
     def invocation_role(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -4735,17 +5239,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "invocationRole"))
 
     @invocation_role.setter
     def invocation_role(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTrigger, "invocation_role").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "invocationRole", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="qualifier")
     def qualifier(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -4755,17 +5262,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "qualifier"))
 
     @qualifier.setter
     def qualifier(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTrigger, "qualifier").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "qualifier", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="sourceArn")
     def source_arn(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -4775,14 +5285,17 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "sourceArn"))
 
     @source_arn.setter
     def source_arn(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTrigger, "source_arn").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "sourceArn", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-fc.RosTriggerProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -4816,14 +5329,24 @@
         :param trigger_config: 
         :param trigger_name: 
         :param trigger_type: 
         :param invocation_role: 
         :param qualifier: 
         :param source_arn: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosTriggerProps.__init__)
+            check_type(argname="argument function_name", value=function_name, expected_type=type_hints["function_name"])
+            check_type(argname="argument service_name", value=service_name, expected_type=type_hints["service_name"])
+            check_type(argname="argument trigger_config", value=trigger_config, expected_type=type_hints["trigger_config"])
+            check_type(argname="argument trigger_name", value=trigger_name, expected_type=type_hints["trigger_name"])
+            check_type(argname="argument trigger_type", value=trigger_type, expected_type=type_hints["trigger_type"])
+            check_type(argname="argument invocation_role", value=invocation_role, expected_type=type_hints["invocation_role"])
+            check_type(argname="argument qualifier", value=qualifier, expected_type=type_hints["qualifier"])
+            check_type(argname="argument source_arn", value=source_arn, expected_type=type_hints["source_arn"])
         self._values: typing.Dict[str, typing.Any] = {
             "function_name": function_name,
             "service_name": service_name,
             "trigger_config": trigger_config,
             "trigger_name": trigger_name,
             "trigger_type": trigger_type,
         }
@@ -4945,102 +5468,120 @@
 ):
     '''A ROS template type:  ``ALIYUN::FC::Version``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosVersionProps",
+        props: typing.Union["RosVersionProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::FC::Version``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosVersion.__init__)
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
+            type_hints = typing.get_type_hints(RosVersion._render_properties)
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
     @jsii.member(jsii_name="attrServiceName")
     def attr_service_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ServiceName: The service name
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrServiceName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVersionId")
     def attr_version_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: VersionId: The version ID
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVersionId"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosVersion, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="serviceName")
     def service_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: serviceName: Service name
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "serviceName"))
 
     @service_name.setter
     def service_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosVersion, "service_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "serviceName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="description")
     def description(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: description: Version description
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "description"))
 
     @description.setter
     def description(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosVersion, "description").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "description", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-fc.RosVersionProps",
     jsii_struct_bases=[],
     name_mapping={"service_name": "serviceName", "description": "description"},
@@ -5053,14 +5594,18 @@
         description: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::FC::Version``.
 
         :param service_name: 
         :param description: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosVersionProps.__init__)
+            check_type(argname="argument service_name", value=service_name, expected_type=type_hints["service_name"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
         self._values: typing.Dict[str, typing.Any] = {
             "service_name": service_name,
         }
         if description is not None:
             self._values["description"] = description
 
     @builtins.property
@@ -5101,73 +5646,79 @@
 ):
     '''A ROS resource type:  ``ALIYUN::FC::Service``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "ServiceProps",
+        props: typing.Union["ServiceProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::FC::Service``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(Service.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInternetAccess")
     def attr_internet_access(self) -> ros_cdk_core.IResolvable:
         '''Attribute InternetAccess: Whether enable Internet access.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInternetAccess"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrLogProject")
     def attr_log_project(self) -> ros_cdk_core.IResolvable:
         '''Attribute LogProject: Log project of service.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrLogProject"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrLogstore")
     def attr_logstore(self) -> ros_cdk_core.IResolvable:
         '''Attribute Logstore: Log store of service.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrLogstore"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrRole")
     def attr_role(self) -> ros_cdk_core.IResolvable:
         '''Attribute Role: Role of service.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrRole"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrServiceId")
     def attr_service_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute ServiceId: The service ID.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrServiceId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrServiceName")
     def attr_service_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute ServiceName: The service name.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrServiceName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTags")
     def attr_tags(self) -> ros_cdk_core.IResolvable:
         '''Attribute Tags: Tags of service.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTags"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVpcId")
     def attr_vpc_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute VpcId: VPC ID.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVpcId"))
 
 
 @jsii.data_type(
@@ -5191,21 +5742,21 @@
     def __init__(
         self,
         *,
         service_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         deletion_force: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         description: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         internet_access: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
-        log_config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, RosService.LogConfigProperty]] = None,
-        nas_config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, RosService.NasConfigProperty]] = None,
+        log_config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosService.LogConfigProperty, typing.Dict[str, typing.Any]]]] = None,
+        nas_config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosService.NasConfigProperty, typing.Dict[str, typing.Any]]]] = None,
         role: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        tags: typing.Optional[typing.Sequence[RosService.TagsProperty]] = None,
-        tracing_config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, RosService.TracingConfigProperty]] = None,
+        tags: typing.Optional[typing.Sequence[typing.Union[RosService.TagsProperty, typing.Dict[str, typing.Any]]]] = None,
+        tracing_config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosService.TracingConfigProperty, typing.Dict[str, typing.Any]]]] = None,
         vpc_bindings: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]] = None,
-        vpc_config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, RosService.VpcConfigProperty]] = None,
+        vpc_config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosService.VpcConfigProperty, typing.Dict[str, typing.Any]]]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::FC::Service``.
 
         :param service_name: Property serviceName: Service name.
         :param deletion_force: Property deletionForce: Whether force delete the service without waiting for network interfaces to be cleaned up if VpcConfig is specified. Default value is false.
         :param description: Property description: Service description.
         :param internet_access: Property internetAccess: Set it to true to enable Internet access.
@@ -5213,14 +5764,27 @@
         :param nas_config: Property nasConfig: NAS configuration. Function Compute uses a specified NAS configured on the service.
         :param role: Property role: The role grants Function Compute the permission to access user’s cloud resources, such as pushing logs to user’s log store. The temporary STS token generated from this role can be retrieved from function context and used to access cloud resources.
         :param tags: Property tags: Tags to attach to service. Max support 20 tags to add during create service. Each tag with two properties Key and Value, and Key is required.
         :param tracing_config: Property tracingConfig: The Tracing Analysis configuration. After Function Compute integrates with Tracing Analysis, you can record the stay time of a request in Function Compute, view the cold start time for a function, and record the execution time of a function.
         :param vpc_bindings: Property vpcBindings: Function Invocation only by Specified VPCs. By default, you can invoke the function by using the Internet endpoint and internal endpoint after a function is created. If you want the function to be invoked only by using specified VPCs, but not the Internet endpoint or internal endpoint, you must bind the specified VPCs to the service.
         :param vpc_config: Property vpcConfig: VPC configuration. Function Compute uses the config to setup ENI in the specific VPC.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(ServiceProps.__init__)
+            check_type(argname="argument service_name", value=service_name, expected_type=type_hints["service_name"])
+            check_type(argname="argument deletion_force", value=deletion_force, expected_type=type_hints["deletion_force"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument internet_access", value=internet_access, expected_type=type_hints["internet_access"])
+            check_type(argname="argument log_config", value=log_config, expected_type=type_hints["log_config"])
+            check_type(argname="argument nas_config", value=nas_config, expected_type=type_hints["nas_config"])
+            check_type(argname="argument role", value=role, expected_type=type_hints["role"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
+            check_type(argname="argument tracing_config", value=tracing_config, expected_type=type_hints["tracing_config"])
+            check_type(argname="argument vpc_bindings", value=vpc_bindings, expected_type=type_hints["vpc_bindings"])
+            check_type(argname="argument vpc_config", value=vpc_config, expected_type=type_hints["vpc_config"])
         self._values: typing.Dict[str, typing.Any] = {
             "service_name": service_name,
         }
         if deletion_force is not None:
             self._values["deletion_force"] = deletion_force
         if description is not None:
             self._values["description"] = description
@@ -5369,49 +5933,55 @@
 ):
     '''A ROS resource type:  ``ALIYUN::FC::Trigger``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "TriggerProps",
+        props: typing.Union["TriggerProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::FC::Trigger``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(Trigger.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrFunctionName")
     def attr_function_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute FunctionName: Function name.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrFunctionName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrServiceName")
     def attr_service_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute ServiceName: Service name.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrServiceName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTriggerId")
     def attr_trigger_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute TriggerId: The trigger ID.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTriggerId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTriggerName")
     def attr_trigger_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute TriggerName: Trigger name.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTriggerName"))
 
 
 @jsii.data_type(
@@ -5448,14 +6018,24 @@
         :param trigger_config: Property triggerConfig: Event source specific trigger configuration. The value is different according to trigger type.
         :param trigger_name: Property triggerName: Trigger name. Example : "image_resize"
         :param trigger_type: Property triggerType: Trigger type, e.g. oss, timer, logs. This determines how the trigger config is interpreted. Example : "oss".
         :param invocation_role: Property invocationRole: The role grants event source the permission to run function on behalf of user. This is optional for some triggers. Example : "acs:ram::1234567890:role/fc-test"
         :param qualifier: Property qualifier: service version or alias. Example : "LATEST"
         :param source_arn: Property sourceArn: The Aliyun Resource Name (ARN) of event source. This is optional for some triggers. Example : "acs:oss:cn-shanghai:12345:mybucket"
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(TriggerProps.__init__)
+            check_type(argname="argument function_name", value=function_name, expected_type=type_hints["function_name"])
+            check_type(argname="argument service_name", value=service_name, expected_type=type_hints["service_name"])
+            check_type(argname="argument trigger_config", value=trigger_config, expected_type=type_hints["trigger_config"])
+            check_type(argname="argument trigger_name", value=trigger_name, expected_type=type_hints["trigger_name"])
+            check_type(argname="argument trigger_type", value=trigger_type, expected_type=type_hints["trigger_type"])
+            check_type(argname="argument invocation_role", value=invocation_role, expected_type=type_hints["invocation_role"])
+            check_type(argname="argument qualifier", value=qualifier, expected_type=type_hints["qualifier"])
+            check_type(argname="argument source_arn", value=source_arn, expected_type=type_hints["source_arn"])
         self._values: typing.Dict[str, typing.Any] = {
             "function_name": function_name,
             "service_name": service_name,
             "trigger_config": trigger_config,
             "trigger_name": trigger_name,
             "trigger_type": trigger_type,
         }
@@ -5563,37 +6143,43 @@
 ):
     '''A ROS resource type:  ``ALIYUN::FC::Version``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "VersionProps",
+        props: typing.Union["VersionProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::FC::Version``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(Version.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrServiceName")
     def attr_service_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute ServiceName: The service name.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrServiceName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVersionId")
     def attr_version_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute VersionId: The version ID.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVersionId"))
 
 
 @jsii.data_type(
@@ -5609,14 +6195,18 @@
         description: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::FC::Version``.
 
         :param service_name: Property serviceName: Service name.
         :param description: Property description: Version description.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(VersionProps.__init__)
+            check_type(argname="argument service_name", value=service_name, expected_type=type_hints["service_name"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
         self._values: typing.Dict[str, typing.Any] = {
             "service_name": service_name,
         }
         if description is not None:
             self._values["description"] = description
 
     @builtins.property
```

### Comparing `ros-cdk-fc-1.0.8/src/ros_cdk_fc.egg-info/PKG-INFO` & `ros-cdk-fc-1.0.9/src/ros_cdk_fc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-fc
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS FC Construct Library
```

