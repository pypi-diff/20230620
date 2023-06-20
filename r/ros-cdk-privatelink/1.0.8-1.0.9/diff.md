# Comparing `tmp/ros-cdk-privatelink-1.0.8.tar.gz` & `tmp/ros-cdk-privatelink-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-privatelink-1.0.8.tar", last modified: Thu Jul 14 02:19:03 2022, max compression
+gzip compressed data, was "dist/ros-cdk-privatelink-1.0.9.tar", last modified: Fri Sep 23 11:25:12 2022, max compression
```

## Comparing `ros-cdk-privatelink-1.0.8.tar` & `ros-cdk-privatelink-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:19:03.000000 ros-cdk-privatelink-1.0.8/
--rw-r--r--   0 root         (0) root         (0)    10279 2022-07-14 02:19:03.000000 ros-cdk-privatelink-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2022-07-14 02:19:03.000000 ros-cdk-privatelink-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2022-07-14 02:19:03.000000 ros-cdk-privatelink-1.0.8/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1272 2022-07-14 02:19:03.000000 ros-cdk-privatelink-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      203 2022-07-14 02:19:03.000000 ros-cdk-privatelink-1.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)      106 2022-07-14 02:19:03.000000 ros-cdk-privatelink-1.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-07-14 02:19:03.000000 ros-cdk-privatelink-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1842 2022-07-14 02:19:03.000000 ros-cdk-privatelink-1.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:19:03.000000 ros-cdk-privatelink-1.0.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:19:03.000000 ros-cdk-privatelink-1.0.8/src/ros_cdk_privatelink/
--rw-r--r--   0 root         (0) root         (0)    70197 2022-07-14 02:19:03.000000 ros-cdk-privatelink-1.0.8/src/ros_cdk_privatelink/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:19:03.000000 ros-cdk-privatelink-1.0.8/src/ros_cdk_privatelink/_jsii/
--rw-r--r--   0 root         (0) root         (0)      399 2022-07-14 02:19:03.000000 ros-cdk-privatelink-1.0.8/src/ros_cdk_privatelink/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    46693 2022-07-14 02:19:03.000000 ros-cdk-privatelink-1.0.8/src/ros_cdk_privatelink/_jsii/ros-cdk-privatelink@1.0.8.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:19:03.000000 ros-cdk-privatelink-1.0.8/src/ros_cdk_privatelink/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:19:03.000000 ros-cdk-privatelink-1.0.8/src/ros_cdk_privatelink.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1272 2022-07-14 02:19:03.000000 ros-cdk-privatelink-1.0.8/src/ros_cdk_privatelink.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      480 2022-07-14 02:19:03.000000 ros-cdk-privatelink-1.0.8/src/ros_cdk_privatelink.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:19:03.000000 ros-cdk-privatelink-1.0.8/src/ros_cdk_privatelink.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2022-07-14 02:19:03.000000 ros-cdk-privatelink-1.0.8/src/ros_cdk_privatelink.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2022-07-14 02:19:03.000000 ros-cdk-privatelink-1.0.8/src/ros_cdk_privatelink.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:25:12.000000 ros-cdk-privatelink-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)    10279 2022-09-23 11:25:11.000000 ros-cdk-privatelink-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-09-23 11:25:11.000000 ros-cdk-privatelink-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2022-09-23 11:25:11.000000 ros-cdk-privatelink-1.0.9/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1272 2022-09-23 11:25:12.000000 ros-cdk-privatelink-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      203 2022-09-23 11:25:11.000000 ros-cdk-privatelink-1.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      236 2022-09-23 11:25:11.000000 ros-cdk-privatelink-1.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-09-23 11:25:12.000000 ros-cdk-privatelink-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1871 2022-09-23 11:25:11.000000 ros-cdk-privatelink-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:25:12.000000 ros-cdk-privatelink-1.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:25:12.000000 ros-cdk-privatelink-1.0.9/src/ros_cdk_privatelink/
+-rw-r--r--   0 root         (0) root         (0)    95945 2022-09-23 11:25:11.000000 ros-cdk-privatelink-1.0.9/src/ros_cdk_privatelink/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:25:12.000000 ros-cdk-privatelink-1.0.9/src/ros_cdk_privatelink/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      433 2022-09-23 11:25:11.000000 ros-cdk-privatelink-1.0.9/src/ros_cdk_privatelink/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    49302 2022-09-23 11:25:11.000000 ros-cdk-privatelink-1.0.9/src/ros_cdk_privatelink/_jsii/ros-cdk-privatelink@1.0.9.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 11:25:11.000000 ros-cdk-privatelink-1.0.9/src/ros_cdk_privatelink/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:25:12.000000 ros-cdk-privatelink-1.0.9/src/ros_cdk_privatelink.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1272 2022-09-23 11:25:12.000000 ros-cdk-privatelink-1.0.9/src/ros_cdk_privatelink.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      480 2022-09-23 11:25:12.000000 ros-cdk-privatelink-1.0.9/src/ros_cdk_privatelink.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 11:25:12.000000 ros-cdk-privatelink-1.0.9/src/ros_cdk_privatelink.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2022-09-23 11:25:12.000000 ros-cdk-privatelink-1.0.9/src/ros_cdk_privatelink.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2022-09-23 11:25:12.000000 ros-cdk-privatelink-1.0.9/src/ros_cdk_privatelink.egg-info/top_level.txt
```

### Comparing `ros-cdk-privatelink-1.0.8/LICENSE` & `ros-cdk-privatelink-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-privatelink-1.0.8/PKG-INFO` & `ros-cdk-privatelink-1.0.9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-privatelink
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS PRIVATELINK Construct Library
```

### Comparing `ros-cdk-privatelink-1.0.8/setup.py` & `ros-cdk-privatelink-1.0.9/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-privatelink",
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
         "ros_cdk_privatelink",
         "ros_cdk_privatelink._jsii"
     ],
     "package_data": {
         "ros_cdk_privatelink._jsii": [
-            "ros-cdk-privatelink@1.0.8.jsii.tgz"
+            "ros-cdk-privatelink@1.0.9.jsii.tgz"
         ],
         "ros_cdk_privatelink": [
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

### Comparing `ros-cdk-privatelink-1.0.8/src/ros_cdk_privatelink/__init__.py` & `ros-cdk-privatelink-1.0.9/src/ros_cdk_privatelink/__init__.py`

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
 
 
 class RosVpcEndpoint(
     ros_cdk_core.RosResource,
@@ -29,153 +31,171 @@
 ):
     '''A ROS template type:  ``ALIYUN::PrivateLink::VpcEndpoint``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosVpcEndpointProps",
+        props: typing.Union["RosVpcEndpointProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::PrivateLink::VpcEndpoint``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosVpcEndpoint.__init__)
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
+            type_hints = typing.get_type_hints(RosVpcEndpoint._render_properties)
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
     @jsii.member(jsii_name="attrBandwidth")
     def attr_bandwidth(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Bandwidth: The bandwidth of the endpoint.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrBandwidth"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrEndpointDomain")
     def attr_endpoint_domain(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: EndpointDomain: The domain name of the endpoint.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrEndpointDomain"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrEndpointId")
     def attr_endpoint_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: EndpointId: The ID of the endpoint.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrEndpointId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrEndpointName")
     def attr_endpoint_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: EndpointName: The name of the endpoint.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrEndpointName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrServiceId")
     def attr_service_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ServiceId: The ID of endpoint service that is associated with the endpoint.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrServiceId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrServiceName")
     def attr_service_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ServiceName: The name of endpoint service that is associated with the endpoint.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrServiceName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVpcId")
     def attr_vpc_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: VpcId: The vpc ID of endpoint.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVpcId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrZoneDomains")
     def attr_zone_domains(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ZoneDomains: The zone domains.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrZoneDomains"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosVpcEndpoint, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="securityGroupId")
     def security_group_id(
         self,
     ) -> typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]:
         '''
         :Property: securityGroupId: The security group associated with the endpoint network interface. The security group can control the data communication from the VPC to the endpoint network interface.
         '''
         return typing.cast(typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]], jsii.get(self, "securityGroupId"))
 
     @security_group_id.setter
     def security_group_id(
         self,
         value: typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosVpcEndpoint, "security_group_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "securityGroupId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vpcId")
     def vpc_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: vpcId: The VPC to which the endpoint belongs.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "vpcId"))
 
     @vpc_id.setter
     def vpc_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosVpcEndpoint, "vpc_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "vpcId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="endpointDescription")
     def endpoint_description(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -185,17 +205,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "endpointDescription"))
 
     @endpoint_description.setter
     def endpoint_description(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosVpcEndpoint, "endpoint_description").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "endpointDescription", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="endpointName")
     def endpoint_name(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -206,105 +229,203 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "endpointName"))
 
     @endpoint_name.setter
     def endpoint_name(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosVpcEndpoint, "endpoint_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "endpointName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
+    @jsii.member(jsii_name="endpointType")
+    def endpoint_type(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
+        '''
+        :Property: endpointType: Endpoint type.
+        '''
+        return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "endpointType"))
+
+    @endpoint_type.setter
+    def endpoint_type(
+        self,
+        value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosVpcEndpoint, "endpoint_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "endpointType", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="protectedEnabled")
+    def protected_enabled(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
+        '''
+        :Property:
+
+        protectedEnabled: Specifies whether to enable user authentication. This parameter is available in Security Token Service (STS) mode. Valid values:
+        true: yes After user authentication is enabled, only the user who creates the endpoint can modify or delete the endpoint in STS mode.
+        false (default): no
+        '''
+        return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "protectedEnabled"))
+
+    @protected_enabled.setter
+    def protected_enabled(
+        self,
+        value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosVpcEndpoint, "protected_enabled").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "protectedEnabled", value)
+
+    @builtins.property
     @jsii.member(jsii_name="serviceId")
     def service_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: serviceId: The endpoint service that is associated with the endpoint. One of ServiceId and ServiceName is required.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "serviceId"))
 
     @service_id.setter
     def service_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosVpcEndpoint, "service_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "serviceId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="serviceName")
     def service_name(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: serviceName: The name of the endpoint service that is associated with the endpoint. One of ServiceId and ServiceName is required.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "serviceName"))
 
     @service_name.setter
     def service_name(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosVpcEndpoint, "service_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "serviceName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="zone")
     def zone(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosVpcEndpoint.ZoneProperty"]]]]:
         '''
         :Property: zone:
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosVpcEndpoint.ZoneProperty"]]]], jsii.get(self, "zone"))
 
     @zone.setter
     def zone(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosVpcEndpoint.ZoneProperty"]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosVpcEndpoint, "zone").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "zone", value)
 
+    @builtins.property
+    @jsii.member(jsii_name="zonePrivateIpAddressCount")
+    def zone_private_ip_address_count(
+        self,
+    ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
+        '''
+        :Property: zonePrivateIpAddressCount: The number of private IP addresses that can be used by an elastic network interface (ENI) in each zone. Set the value to 1.
+        '''
+        return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "zonePrivateIpAddressCount"))
+
+    @zone_private_ip_address_count.setter
+    def zone_private_ip_address_count(
+        self,
+        value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosVpcEndpoint, "zone_private_ip_address_count").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "zonePrivateIpAddressCount", value)
+
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-privatelink.RosVpcEndpoint.ZoneProperty",
         jsii_struct_bases=[],
-        name_mapping={"v_switch_id": "vSwitchId", "zone_id": "zoneId"},
+        name_mapping={"ip": "ip", "v_switch_id": "vSwitchId", "zone_id": "zoneId"},
     )
     class ZoneProperty:
         def __init__(
             self,
             *,
-            v_switch_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
-            zone_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
+            ip: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
+            v_switch_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
+            zone_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
+            :param ip: 
             :param v_switch_id: 
             :param zone_id: 
             '''
-            self._values: typing.Dict[str, typing.Any] = {
-                "v_switch_id": v_switch_id,
-                "zone_id": zone_id,
-            }
+            if __debug__:
+                type_hints = typing.get_type_hints(RosVpcEndpoint.ZoneProperty.__init__)
+                check_type(argname="argument ip", value=ip, expected_type=type_hints["ip"])
+                check_type(argname="argument v_switch_id", value=v_switch_id, expected_type=type_hints["v_switch_id"])
+                check_type(argname="argument zone_id", value=zone_id, expected_type=type_hints["zone_id"])
+            self._values: typing.Dict[str, typing.Any] = {}
+            if ip is not None:
+                self._values["ip"] = ip
+            if v_switch_id is not None:
+                self._values["v_switch_id"] = v_switch_id
+            if zone_id is not None:
+                self._values["zone_id"] = zone_id
 
         @builtins.property
-        def v_switch_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
+        def ip(
+            self,
+        ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
+            '''
+            :Property: ip: The IP address of the zone in which the endpoint is deployed.
+            '''
+            result = self._values.get("ip")
+            return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], result)
+
+        @builtins.property
+        def v_switch_id(
+            self,
+        ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
             '''
             :Property: vSwitchId: The switch of the endpoint network interface in the given zone.
             '''
             result = self._values.get("v_switch_id")
-            assert result is not None, "Required property 'v_switch_id' is missing"
-            return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], result)
+            return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], result)
 
         @builtins.property
-        def zone_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
+        def zone_id(
+            self,
+        ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
             '''
             :Property: zoneId: The zone of the associated endpoint service.
             '''
             result = self._values.get("zone_id")
-            assert result is not None, "Required property 'zone_id' is missing"
-            return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], result)
+            return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], result)
 
         def __eq__(self, rhs: typing.Any) -> builtins.bool:
             return isinstance(rhs, self.__class__) and rhs._values == self._values
 
         def __ne__(self, rhs: typing.Any) -> builtins.bool:
             return not (rhs == self)
 
@@ -318,55 +439,82 @@
     jsii_type="@alicloud/ros-cdk-privatelink.RosVpcEndpointProps",
     jsii_struct_bases=[],
     name_mapping={
         "security_group_id": "securityGroupId",
         "vpc_id": "vpcId",
         "endpoint_description": "endpointDescription",
         "endpoint_name": "endpointName",
+        "endpoint_type": "endpointType",
+        "protected_enabled": "protectedEnabled",
         "service_id": "serviceId",
         "service_name": "serviceName",
         "zone": "zone",
+        "zone_private_ip_address_count": "zonePrivateIpAddressCount",
     },
 )
 class RosVpcEndpointProps:
     def __init__(
         self,
         *,
         security_group_id: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]],
         vpc_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         endpoint_description: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         endpoint_name: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
+        endpoint_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
+        protected_enabled: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         service_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         service_name: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        zone: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosVpcEndpoint.ZoneProperty]]]] = None,
+        zone: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosVpcEndpoint.ZoneProperty, typing.Dict[str, typing.Any]]]]]] = None,
+        zone_private_ip_address_count: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::PrivateLink::VpcEndpoint``.
 
         :param security_group_id: 
         :param vpc_id: 
         :param endpoint_description: 
         :param endpoint_name: 
+        :param endpoint_type: 
+        :param protected_enabled: 
         :param service_id: 
         :param service_name: 
         :param zone: 
+        :param zone_private_ip_address_count: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosVpcEndpointProps.__init__)
+            check_type(argname="argument security_group_id", value=security_group_id, expected_type=type_hints["security_group_id"])
+            check_type(argname="argument vpc_id", value=vpc_id, expected_type=type_hints["vpc_id"])
+            check_type(argname="argument endpoint_description", value=endpoint_description, expected_type=type_hints["endpoint_description"])
+            check_type(argname="argument endpoint_name", value=endpoint_name, expected_type=type_hints["endpoint_name"])
+            check_type(argname="argument endpoint_type", value=endpoint_type, expected_type=type_hints["endpoint_type"])
+            check_type(argname="argument protected_enabled", value=protected_enabled, expected_type=type_hints["protected_enabled"])
+            check_type(argname="argument service_id", value=service_id, expected_type=type_hints["service_id"])
+            check_type(argname="argument service_name", value=service_name, expected_type=type_hints["service_name"])
+            check_type(argname="argument zone", value=zone, expected_type=type_hints["zone"])
+            check_type(argname="argument zone_private_ip_address_count", value=zone_private_ip_address_count, expected_type=type_hints["zone_private_ip_address_count"])
         self._values: typing.Dict[str, typing.Any] = {
             "security_group_id": security_group_id,
             "vpc_id": vpc_id,
         }
         if endpoint_description is not None:
             self._values["endpoint_description"] = endpoint_description
         if endpoint_name is not None:
             self._values["endpoint_name"] = endpoint_name
+        if endpoint_type is not None:
+            self._values["endpoint_type"] = endpoint_type
+        if protected_enabled is not None:
+            self._values["protected_enabled"] = protected_enabled
         if service_id is not None:
             self._values["service_id"] = service_id
         if service_name is not None:
             self._values["service_name"] = service_name
         if zone is not None:
             self._values["zone"] = zone
+        if zone_private_ip_address_count is not None:
+            self._values["zone_private_ip_address_count"] = zone_private_ip_address_count
 
     @builtins.property
     def security_group_id(
         self,
     ) -> typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]:
         '''
         :Property: securityGroupId: The security group associated with the endpoint network interface. The security group can control the data communication from the VPC to the endpoint network interface.
@@ -408,14 +556,38 @@
         The name must be 2 to 128 characters in length and can contain digits, underscores
         (_), and hyphens (-). The name must start with a letter.
         '''
         result = self._values.get("endpoint_name")
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], result)
 
     @builtins.property
+    def endpoint_type(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
+        '''
+        :Property: endpointType: Endpoint type.
+        '''
+        result = self._values.get("endpoint_type")
+        return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], result)
+
+    @builtins.property
+    def protected_enabled(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
+        '''
+        :Property:
+
+        protectedEnabled: Specifies whether to enable user authentication. This parameter is available in Security Token Service (STS) mode. Valid values:
+        true: yes After user authentication is enabled, only the user who creates the endpoint can modify or delete the endpoint in STS mode.
+        false (default): no
+        '''
+        result = self._values.get("protected_enabled")
+        return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], result)
+
+    @builtins.property
     def service_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: serviceId: The endpoint service that is associated with the endpoint. One of ServiceId and ServiceName is required.
         '''
         result = self._values.get("service_id")
@@ -437,14 +609,24 @@
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, RosVpcEndpoint.ZoneProperty]]]]:
         '''
         :Property: zone:
         '''
         result = self._values.get("zone")
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, RosVpcEndpoint.ZoneProperty]]]], result)
 
+    @builtins.property
+    def zone_private_ip_address_count(
+        self,
+    ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
+        '''
+        :Property: zonePrivateIpAddressCount: The number of private IP addresses that can be used by an elastic network interface (ENI) in each zone. Set the value to 1.
+        '''
+        result = self._values.get("zone_private_ip_address_count")
+        return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], result)
+
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
@@ -460,105 +642,117 @@
 ):
     '''A ROS template type:  ``ALIYUN::PrivateLink::VpcEndpointService``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosVpcEndpointServiceProps",
+        props: typing.Union["RosVpcEndpointServiceProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::PrivateLink::VpcEndpointService``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosVpcEndpointService.__init__)
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
+            type_hints = typing.get_type_hints(RosVpcEndpointService._render_properties)
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
     @jsii.member(jsii_name="attrMaxBandwidth")
     def attr_max_bandwidth(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: MaxBandwidth: The maximum bandwidth of the endpoint connection.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrMaxBandwidth"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrMinBandwidth")
     def attr_min_bandwidth(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: MinBandwidth: The minimum bandwidth of the endpoint connection.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrMinBandwidth"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrServiceDescription")
     def attr_service_description(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ServiceDescription: The description of the endpoint service.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrServiceDescription"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrServiceDomain")
     def attr_service_domain(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ServiceDomain: The domain name of the endpoint service.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrServiceDomain"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrServiceId")
     def attr_service_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ServiceId: The ID of the endpoint service.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrServiceId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrServiceName")
     def attr_service_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ServiceName: The name of the endpoint service.
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
+            type_hints = typing.get_type_hints(getattr(RosVpcEndpointService, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="autoAcceptEnabled")
     def auto_accept_enabled(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -569,34 +763,40 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "autoAcceptEnabled"))
 
     @auto_accept_enabled.setter
     def auto_accept_enabled(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosVpcEndpointService, "auto_accept_enabled").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "autoAcceptEnabled", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="connectBandwidth")
     def connect_bandwidth(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: connectBandwidth: The default maximum bandwidth of the endpoint connection. Valid values: 100 to 1024. Unit: Mbit/s.
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "connectBandwidth"))
 
     @connect_bandwidth.setter
     def connect_bandwidth(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosVpcEndpointService, "connect_bandwidth").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "connectBandwidth", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="payer")
     def payer(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -607,68 +807,100 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "payer"))
 
     @payer.setter
     def payer(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosVpcEndpointService, "payer").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "payer", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="resource")
     def resource(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosVpcEndpointService.ResourceProperty"]]]]:
         '''
         :Property: resource:
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosVpcEndpointService.ResourceProperty"]]]], jsii.get(self, "resource"))
 
     @resource.setter
     def resource(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosVpcEndpointService.ResourceProperty"]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosVpcEndpointService, "resource").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "resource", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="serviceDescription")
     def service_description(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: serviceDescription: The description for the endpoint service.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "serviceDescription"))
 
     @service_description.setter
     def service_description(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosVpcEndpointService, "service_description").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "serviceDescription", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
+    @jsii.member(jsii_name="serviceResourceType")
+    def service_resource_type(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
+        '''
+        :Property: serviceResourceType: Service resource type.
+        '''
+        return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "serviceResourceType"))
+
+    @service_resource_type.setter
+    def service_resource_type(
+        self,
+        value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosVpcEndpointService, "service_resource_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "serviceResourceType", value)
+
+    @builtins.property
     @jsii.member(jsii_name="user")
     def user(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]]:
         '''
         :Property: user: Account IDs to the whitelist of an endpoint service.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]], jsii.get(self, "user"))
 
     @user.setter
     def user(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosVpcEndpointService, "user").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "user", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="zoneAffinityEnabled")
     def zone_affinity_enabled(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -679,14 +911,17 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "zoneAffinityEnabled"))
 
     @zone_affinity_enabled.setter
     def zone_affinity_enabled(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosVpcEndpointService, "zone_affinity_enabled").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "zoneAffinityEnabled", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-privatelink.RosVpcEndpointService.ResourceProperty",
         jsii_struct_bases=[],
         name_mapping={
             "resource_id": "resourceId",
@@ -703,14 +938,19 @@
             zone_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         ) -> None:
             '''
             :param resource_id: 
             :param resource_type: 
             :param zone_id: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosVpcEndpointService.ResourceProperty.__init__)
+                check_type(argname="argument resource_id", value=resource_id, expected_type=type_hints["resource_id"])
+                check_type(argname="argument resource_type", value=resource_type, expected_type=type_hints["resource_type"])
+                check_type(argname="argument zone_id", value=zone_id, expected_type=type_hints["zone_id"])
             self._values: typing.Dict[str, typing.Any] = {
                 "resource_id": resource_id,
                 "resource_type": resource_type,
                 "zone_id": zone_id,
             }
 
         @builtins.property
@@ -721,19 +961,15 @@
             result = self._values.get("resource_id")
             assert result is not None, "Required property 'resource_id' is missing"
             return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], result)
 
         @builtins.property
         def resource_type(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
             '''
-            :Property:
-
-            resourceType: The type of service resource. Set the value to slb (SLB instances that support PrivateLink and are deployed in a VPC).
-            Note Only Server Load Balancer (SLB) instances that support PrivateLink can serve as service
-            resources for endpoint services.
+            :Property: resourceType: The type of service resource. Supports slb, nlb, vpcNat.
             '''
             result = self._values.get("resource_type")
             assert result is not None, "Required property 'resource_type' is missing"
             return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], result)
 
         @builtins.property
         def zone_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
@@ -763,123 +999,144 @@
 ):
     '''A ROS template type:  ``ALIYUN::PrivateLink::VpcEndpointServiceAttachment``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosVpcEndpointServiceAttachmentProps",
+        props: typing.Union["RosVpcEndpointServiceAttachmentProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::PrivateLink::VpcEndpointServiceAttachment``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosVpcEndpointServiceAttachment.__init__)
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
+            type_hints = typing.get_type_hints(RosVpcEndpointServiceAttachment._render_properties)
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
     @jsii.member(jsii_name="attrResourceId")
     def attr_resource_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ResourceId: The resource id.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrResourceId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrResourceType")
     def attr_resource_type(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ResourceType: The resource type.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrResourceType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrServiceId")
     def attr_service_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ServiceId: The endpoint service that is associated with the endpoint.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrServiceId"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosVpcEndpointServiceAttachment, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="resourceId")
     def resource_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: resourceId: The resource id.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "resourceId"))
 
     @resource_id.setter
     def resource_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosVpcEndpointServiceAttachment, "resource_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "resourceId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="resourceType")
     def resource_type(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: resourceType: The resource type.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "resourceType"))
 
     @resource_type.setter
     def resource_type(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosVpcEndpointServiceAttachment, "resource_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "resourceType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="serviceId")
     def service_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: serviceId: The endpoint service that is associated with the endpoint.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "serviceId"))
 
     @service_id.setter
     def service_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosVpcEndpointServiceAttachment, "service_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "serviceId", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-privatelink.RosVpcEndpointServiceAttachmentProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -898,14 +1155,19 @@
     ) -> None:
         '''Properties for defining a ``ALIYUN::PrivateLink::VpcEndpointServiceAttachment``.
 
         :param resource_id: 
         :param resource_type: 
         :param service_id: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosVpcEndpointServiceAttachmentProps.__init__)
+            check_type(argname="argument resource_id", value=resource_id, expected_type=type_hints["resource_id"])
+            check_type(argname="argument resource_type", value=resource_type, expected_type=type_hints["resource_type"])
+            check_type(argname="argument service_id", value=service_id, expected_type=type_hints["service_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "resource_id": resource_id,
             "resource_type": resource_type,
             "service_id": service_id,
         }
 
     @builtins.property
@@ -952,51 +1214,66 @@
     jsii_struct_bases=[],
     name_mapping={
         "auto_accept_enabled": "autoAcceptEnabled",
         "connect_bandwidth": "connectBandwidth",
         "payer": "payer",
         "resource": "resource",
         "service_description": "serviceDescription",
+        "service_resource_type": "serviceResourceType",
         "user": "user",
         "zone_affinity_enabled": "zoneAffinityEnabled",
     },
 )
 class RosVpcEndpointServiceProps:
     def __init__(
         self,
         *,
         auto_accept_enabled: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         connect_bandwidth: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         payer: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        resource: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosVpcEndpointService.ResourceProperty]]]] = None,
+        resource: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosVpcEndpointService.ResourceProperty, typing.Dict[str, typing.Any]]]]]] = None,
         service_description: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
+        service_resource_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         user: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]] = None,
         zone_affinity_enabled: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::PrivateLink::VpcEndpointService``.
 
         :param auto_accept_enabled: 
         :param connect_bandwidth: 
         :param payer: 
         :param resource: 
         :param service_description: 
+        :param service_resource_type: 
         :param user: 
         :param zone_affinity_enabled: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosVpcEndpointServiceProps.__init__)
+            check_type(argname="argument auto_accept_enabled", value=auto_accept_enabled, expected_type=type_hints["auto_accept_enabled"])
+            check_type(argname="argument connect_bandwidth", value=connect_bandwidth, expected_type=type_hints["connect_bandwidth"])
+            check_type(argname="argument payer", value=payer, expected_type=type_hints["payer"])
+            check_type(argname="argument resource", value=resource, expected_type=type_hints["resource"])
+            check_type(argname="argument service_description", value=service_description, expected_type=type_hints["service_description"])
+            check_type(argname="argument service_resource_type", value=service_resource_type, expected_type=type_hints["service_resource_type"])
+            check_type(argname="argument user", value=user, expected_type=type_hints["user"])
+            check_type(argname="argument zone_affinity_enabled", value=zone_affinity_enabled, expected_type=type_hints["zone_affinity_enabled"])
         self._values: typing.Dict[str, typing.Any] = {}
         if auto_accept_enabled is not None:
             self._values["auto_accept_enabled"] = auto_accept_enabled
         if connect_bandwidth is not None:
             self._values["connect_bandwidth"] = connect_bandwidth
         if payer is not None:
             self._values["payer"] = payer
         if resource is not None:
             self._values["resource"] = resource
         if service_description is not None:
             self._values["service_description"] = service_description
+        if service_resource_type is not None:
+            self._values["service_resource_type"] = service_resource_type
         if user is not None:
             self._values["user"] = user
         if zone_affinity_enabled is not None:
             self._values["zone_affinity_enabled"] = zone_affinity_enabled
 
     @builtins.property
     def auto_accept_enabled(
@@ -1053,14 +1330,24 @@
         '''
         :Property: serviceDescription: The description for the endpoint service.
         '''
         result = self._values.get("service_description")
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], result)
 
     @builtins.property
+    def service_resource_type(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
+        '''
+        :Property: serviceResourceType: Service resource type.
+        '''
+        result = self._values.get("service_resource_type")
+        return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], result)
+
+    @builtins.property
     def user(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]]:
         '''
         :Property: user: Account IDs to the whitelist of an endpoint service.
         '''
         result = self._values.get("user")
@@ -1099,128 +1386,161 @@
 ):
     '''A ROS resource type:  ``ALIYUN::PrivateLink::VpcEndpoint``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "VpcEndpointProps",
+        props: typing.Union["VpcEndpointProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::PrivateLink::VpcEndpoint``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(VpcEndpoint.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrBandwidth")
     def attr_bandwidth(self) -> ros_cdk_core.IResolvable:
         '''Attribute Bandwidth: The bandwidth of the endpoint.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrBandwidth"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrEndpointDomain")
     def attr_endpoint_domain(self) -> ros_cdk_core.IResolvable:
         '''Attribute EndpointDomain: The domain name of the endpoint.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrEndpointDomain"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrEndpointId")
     def attr_endpoint_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute EndpointId: The ID of the endpoint.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrEndpointId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrEndpointName")
     def attr_endpoint_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute EndpointName: The name of the endpoint.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrEndpointName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrServiceId")
     def attr_service_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute ServiceId: The ID of endpoint service that is associated with the endpoint.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrServiceId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrServiceName")
     def attr_service_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute ServiceName: The name of endpoint service that is associated with the endpoint.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrServiceName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVpcId")
     def attr_vpc_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute VpcId: The vpc ID of endpoint.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVpcId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrZoneDomains")
     def attr_zone_domains(self) -> ros_cdk_core.IResolvable:
         '''Attribute ZoneDomains: The zone domains.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrZoneDomains"))
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-privatelink.VpcEndpointProps",
     jsii_struct_bases=[],
     name_mapping={
         "security_group_id": "securityGroupId",
         "vpc_id": "vpcId",
         "endpoint_description": "endpointDescription",
         "endpoint_name": "endpointName",
+        "endpoint_type": "endpointType",
+        "protected_enabled": "protectedEnabled",
         "service_id": "serviceId",
         "service_name": "serviceName",
         "zone": "zone",
+        "zone_private_ip_address_count": "zonePrivateIpAddressCount",
     },
 )
 class VpcEndpointProps:
     def __init__(
         self,
         *,
         security_group_id: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]],
         vpc_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         endpoint_description: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         endpoint_name: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
+        endpoint_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
+        protected_enabled: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         service_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         service_name: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        zone: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosVpcEndpoint.ZoneProperty]]]] = None,
+        zone: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosVpcEndpoint.ZoneProperty, typing.Dict[str, typing.Any]]]]]] = None,
+        zone_private_ip_address_count: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::PrivateLink::VpcEndpoint``.
 
         :param security_group_id: Property securityGroupId: The security group associated with the endpoint network interface. The security group can control the data communication from the VPC to the endpoint network interface.
         :param vpc_id: Property vpcId: The VPC to which the endpoint belongs.
         :param endpoint_description: Property endpointDescription: The description of the endpoint. The description must be 2 to 256 characters in length and cannot start with http:// or https://.
         :param endpoint_name: Property endpointName: The name of the endpoint. The name must be 2 to 128 characters in length and can contain digits, underscores (_), and hyphens (-). The name must start with a letter.
+        :param endpoint_type: Property endpointType: Endpoint type.
+        :param protected_enabled: Property protectedEnabled: Specifies whether to enable user authentication. This parameter is available in Security Token Service (STS) mode. Valid values: true: yes After user authentication is enabled, only the user who creates the endpoint can modify or delete the endpoint in STS mode. false (default): no
         :param service_id: Property serviceId: The endpoint service that is associated with the endpoint. One of ServiceId and ServiceName is required.
         :param service_name: Property serviceName: The name of the endpoint service that is associated with the endpoint. One of ServiceId and ServiceName is required.
         :param zone: Property zone:.
+        :param zone_private_ip_address_count: Property zonePrivateIpAddressCount: The number of private IP addresses that can be used by an elastic network interface (ENI) in each zone. Set the value to 1.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(VpcEndpointProps.__init__)
+            check_type(argname="argument security_group_id", value=security_group_id, expected_type=type_hints["security_group_id"])
+            check_type(argname="argument vpc_id", value=vpc_id, expected_type=type_hints["vpc_id"])
+            check_type(argname="argument endpoint_description", value=endpoint_description, expected_type=type_hints["endpoint_description"])
+            check_type(argname="argument endpoint_name", value=endpoint_name, expected_type=type_hints["endpoint_name"])
+            check_type(argname="argument endpoint_type", value=endpoint_type, expected_type=type_hints["endpoint_type"])
+            check_type(argname="argument protected_enabled", value=protected_enabled, expected_type=type_hints["protected_enabled"])
+            check_type(argname="argument service_id", value=service_id, expected_type=type_hints["service_id"])
+            check_type(argname="argument service_name", value=service_name, expected_type=type_hints["service_name"])
+            check_type(argname="argument zone", value=zone, expected_type=type_hints["zone"])
+            check_type(argname="argument zone_private_ip_address_count", value=zone_private_ip_address_count, expected_type=type_hints["zone_private_ip_address_count"])
         self._values: typing.Dict[str, typing.Any] = {
             "security_group_id": security_group_id,
             "vpc_id": vpc_id,
         }
         if endpoint_description is not None:
             self._values["endpoint_description"] = endpoint_description
         if endpoint_name is not None:
             self._values["endpoint_name"] = endpoint_name
+        if endpoint_type is not None:
+            self._values["endpoint_type"] = endpoint_type
+        if protected_enabled is not None:
+            self._values["protected_enabled"] = protected_enabled
         if service_id is not None:
             self._values["service_id"] = service_id
         if service_name is not None:
             self._values["service_name"] = service_name
         if zone is not None:
             self._values["zone"] = zone
+        if zone_private_ip_address_count is not None:
+            self._values["zone_private_ip_address_count"] = zone_private_ip_address_count
 
     @builtins.property
     def security_group_id(
         self,
     ) -> typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]:
         '''Property securityGroupId: The security group associated with the endpoint network interface.
 
@@ -1257,14 +1577,35 @@
         The name must be 2 to 128 characters in length and can contain digits, underscores
         (_), and hyphens (-). The name must start with a letter.
         '''
         result = self._values.get("endpoint_name")
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], result)
 
     @builtins.property
+    def endpoint_type(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
+        '''Property endpointType: Endpoint type.'''
+        result = self._values.get("endpoint_type")
+        return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], result)
+
+    @builtins.property
+    def protected_enabled(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
+        '''Property protectedEnabled: Specifies whether to enable user authentication.
+
+        This parameter is available in Security Token Service (STS) mode. Valid values:
+        true: yes After user authentication is enabled, only the user who creates the endpoint can modify or delete the endpoint in STS mode.
+        false (default): no
+        '''
+        result = self._values.get("protected_enabled")
+        return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], result)
+
+    @builtins.property
     def service_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''Property serviceId: The endpoint service that is associated with the endpoint.
 
         One of ServiceId and ServiceName is required.
         '''
@@ -1286,14 +1627,25 @@
     def zone(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, RosVpcEndpoint.ZoneProperty]]]]:
         '''Property zone:.'''
         result = self._values.get("zone")
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, RosVpcEndpoint.ZoneProperty]]]], result)
 
+    @builtins.property
+    def zone_private_ip_address_count(
+        self,
+    ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
+        '''Property zonePrivateIpAddressCount: The number of private IP addresses that can be used by an elastic network interface (ENI) in each zone.
+
+        Set the value to 1.
+        '''
+        result = self._values.get("zone_private_ip_address_count")
+        return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], result)
+
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
@@ -1309,61 +1661,67 @@
 ):
     '''A ROS resource type:  ``ALIYUN::PrivateLink::VpcEndpointService``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: typing.Optional["VpcEndpointServiceProps"] = None,
+        props: typing.Optional[typing.Union["VpcEndpointServiceProps", typing.Dict[str, typing.Any]]] = None,
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::PrivateLink::VpcEndpointService``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(VpcEndpointService.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrMaxBandwidth")
     def attr_max_bandwidth(self) -> ros_cdk_core.IResolvable:
         '''Attribute MaxBandwidth: The maximum bandwidth of the endpoint connection.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrMaxBandwidth"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrMinBandwidth")
     def attr_min_bandwidth(self) -> ros_cdk_core.IResolvable:
         '''Attribute MinBandwidth: The minimum bandwidth of the endpoint connection.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrMinBandwidth"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrServiceDescription")
     def attr_service_description(self) -> ros_cdk_core.IResolvable:
         '''Attribute ServiceDescription: The description of the endpoint service.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrServiceDescription"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrServiceDomain")
     def attr_service_domain(self) -> ros_cdk_core.IResolvable:
         '''Attribute ServiceDomain: The domain name of the endpoint service.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrServiceDomain"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrServiceId")
     def attr_service_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute ServiceId: The ID of the endpoint service.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrServiceId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrServiceName")
     def attr_service_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute ServiceName: The name of the endpoint service.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrServiceName"))
 
 
 class VpcEndpointServiceAttachment(
@@ -1373,43 +1731,49 @@
 ):
     '''A ROS resource type:  ``ALIYUN::PrivateLink::VpcEndpointServiceAttachment``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "VpcEndpointServiceAttachmentProps",
+        props: typing.Union["VpcEndpointServiceAttachmentProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::PrivateLink::VpcEndpointServiceAttachment``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(VpcEndpointServiceAttachment.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrResourceId")
     def attr_resource_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute ResourceId: The resource id.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrResourceId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrResourceType")
     def attr_resource_type(self) -> ros_cdk_core.IResolvable:
         '''Attribute ResourceType: The resource type.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrResourceType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrServiceId")
     def attr_service_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute ServiceId: The endpoint service that is associated with the endpoint.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrServiceId"))
 
 
 @jsii.data_type(
@@ -1431,14 +1795,19 @@
     ) -> None:
         '''Properties for defining a ``ALIYUN::PrivateLink::VpcEndpointServiceAttachment``.
 
         :param resource_id: Property resourceId: The resource id.
         :param resource_type: Property resourceType: The resource type.
         :param service_id: Property serviceId: The endpoint service that is associated with the endpoint.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(VpcEndpointServiceAttachmentProps.__init__)
+            check_type(argname="argument resource_id", value=resource_id, expected_type=type_hints["resource_id"])
+            check_type(argname="argument resource_type", value=resource_type, expected_type=type_hints["resource_type"])
+            check_type(argname="argument service_id", value=service_id, expected_type=type_hints["service_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "resource_id": resource_id,
             "resource_type": resource_type,
             "service_id": service_id,
         }
 
     @builtins.property
@@ -1479,51 +1848,66 @@
     jsii_struct_bases=[],
     name_mapping={
         "auto_accept_enabled": "autoAcceptEnabled",
         "connect_bandwidth": "connectBandwidth",
         "payer": "payer",
         "resource": "resource",
         "service_description": "serviceDescription",
+        "service_resource_type": "serviceResourceType",
         "user": "user",
         "zone_affinity_enabled": "zoneAffinityEnabled",
     },
 )
 class VpcEndpointServiceProps:
     def __init__(
         self,
         *,
         auto_accept_enabled: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         connect_bandwidth: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         payer: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        resource: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosVpcEndpointService.ResourceProperty]]]] = None,
+        resource: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosVpcEndpointService.ResourceProperty, typing.Dict[str, typing.Any]]]]]] = None,
         service_description: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
+        service_resource_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         user: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]] = None,
         zone_affinity_enabled: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::PrivateLink::VpcEndpointService``.
 
         :param auto_accept_enabled: Property autoAcceptEnabled: Specifies whether to automatically accept endpoint connection requests. Valid values: true: automatically accepts endpoint connection requests. false: does not automatically accept endpoint connection requests.
         :param connect_bandwidth: Property connectBandwidth: The default maximum bandwidth of the endpoint connection. Valid values: 100 to 1024. Unit: Mbit/s.
         :param payer: Property payer: The payer of the endpoint service. Valid values: Endpoint: the service consumer. EndpointService: the service provider.
         :param resource: Property resource:.
         :param service_description: Property serviceDescription: The description for the endpoint service.
+        :param service_resource_type: Property serviceResourceType: Service resource type.
         :param user: Property user: Account IDs to the whitelist of an endpoint service.
         :param zone_affinity_enabled: Property zoneAffinityEnabled: Specifies whether to resolve domain names to IP addresses in the nearest zone. true: yes. false (default): no
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(VpcEndpointServiceProps.__init__)
+            check_type(argname="argument auto_accept_enabled", value=auto_accept_enabled, expected_type=type_hints["auto_accept_enabled"])
+            check_type(argname="argument connect_bandwidth", value=connect_bandwidth, expected_type=type_hints["connect_bandwidth"])
+            check_type(argname="argument payer", value=payer, expected_type=type_hints["payer"])
+            check_type(argname="argument resource", value=resource, expected_type=type_hints["resource"])
+            check_type(argname="argument service_description", value=service_description, expected_type=type_hints["service_description"])
+            check_type(argname="argument service_resource_type", value=service_resource_type, expected_type=type_hints["service_resource_type"])
+            check_type(argname="argument user", value=user, expected_type=type_hints["user"])
+            check_type(argname="argument zone_affinity_enabled", value=zone_affinity_enabled, expected_type=type_hints["zone_affinity_enabled"])
         self._values: typing.Dict[str, typing.Any] = {}
         if auto_accept_enabled is not None:
             self._values["auto_accept_enabled"] = auto_accept_enabled
         if connect_bandwidth is not None:
             self._values["connect_bandwidth"] = connect_bandwidth
         if payer is not None:
             self._values["payer"] = payer
         if resource is not None:
             self._values["resource"] = resource
         if service_description is not None:
             self._values["service_description"] = service_description
+        if service_resource_type is not None:
+            self._values["service_resource_type"] = service_resource_type
         if user is not None:
             self._values["user"] = user
         if zone_affinity_enabled is not None:
             self._values["zone_affinity_enabled"] = zone_affinity_enabled
 
     @builtins.property
     def auto_accept_enabled(
@@ -1575,14 +1959,22 @@
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''Property serviceDescription: The description for the endpoint service.'''
         result = self._values.get("service_description")
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], result)
 
     @builtins.property
+    def service_resource_type(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
+        '''Property serviceResourceType: Service resource type.'''
+        result = self._values.get("service_resource_type")
+        return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], result)
+
+    @builtins.property
     def user(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]]:
         '''Property user: Account IDs to the whitelist of an endpoint service.'''
         result = self._values.get("user")
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]], result)
```

### Comparing `ros-cdk-privatelink-1.0.8/src/ros_cdk_privatelink.egg-info/PKG-INFO` & `ros-cdk-privatelink-1.0.9/src/ros_cdk_privatelink.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-privatelink
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS PRIVATELINK Construct Library
```

