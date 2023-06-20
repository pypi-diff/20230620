# Comparing `tmp/ros-cdk-ots-1.0.8.tar.gz` & `tmp/ros-cdk-ots-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-ots-1.0.8.tar", last modified: Thu Jul 14 02:23:07 2022, max compression
+gzip compressed data, was "dist/ros-cdk-ots-1.0.9.tar", last modified: Fri Sep 23 11:45:41 2022, max compression
```

## Comparing `ros-cdk-ots-1.0.8.tar` & `ros-cdk-ots-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:23:07.000000 ros-cdk-ots-1.0.8/
--rw-r--r--   0 root         (0) root         (0)    10279 2022-07-14 02:23:07.000000 ros-cdk-ots-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2022-07-14 02:23:07.000000 ros-cdk-ots-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2022-07-14 02:23:07.000000 ros-cdk-ots-1.0.8/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1240 2022-07-14 02:23:07.000000 ros-cdk-ots-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      179 2022-07-14 02:23:07.000000 ros-cdk-ots-1.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)      106 2022-07-14 02:23:07.000000 ros-cdk-ots-1.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-07-14 02:23:07.000000 ros-cdk-ots-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1794 2022-07-14 02:23:07.000000 ros-cdk-ots-1.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:23:07.000000 ros-cdk-ots-1.0.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:23:07.000000 ros-cdk-ots-1.0.8/src/ros_cdk_ots/
--rw-r--r--   0 root         (0) root         (0)   120147 2022-07-14 02:23:07.000000 ros-cdk-ots-1.0.8/src/ros_cdk_ots/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:23:07.000000 ros-cdk-ots-1.0.8/src/ros_cdk_ots/_jsii/
--rw-r--r--   0 root         (0) root         (0)      370 2022-07-14 02:23:07.000000 ros-cdk-ots-1.0.8/src/ros_cdk_ots/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    67137 2022-07-14 02:23:07.000000 ros-cdk-ots-1.0.8/src/ros_cdk_ots/_jsii/ros-cdk-ots@1.0.8.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:23:07.000000 ros-cdk-ots-1.0.8/src/ros_cdk_ots/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:23:07.000000 ros-cdk-ots-1.0.8/src/ros_cdk_ots.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1240 2022-07-14 02:23:07.000000 ros-cdk-ots-1.0.8/src/ros_cdk_ots.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      400 2022-07-14 02:23:07.000000 ros-cdk-ots-1.0.8/src/ros_cdk_ots.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:23:07.000000 ros-cdk-ots-1.0.8/src/ros_cdk_ots.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2022-07-14 02:23:07.000000 ros-cdk-ots-1.0.8/src/ros_cdk_ots.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2022-07-14 02:23:07.000000 ros-cdk-ots-1.0.8/src/ros_cdk_ots.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:45:41.000000 ros-cdk-ots-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)    10279 2022-09-23 11:45:41.000000 ros-cdk-ots-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-09-23 11:45:41.000000 ros-cdk-ots-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2022-09-23 11:45:41.000000 ros-cdk-ots-1.0.9/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1240 2022-09-23 11:45:41.000000 ros-cdk-ots-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      179 2022-09-23 11:45:41.000000 ros-cdk-ots-1.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      236 2022-09-23 11:45:41.000000 ros-cdk-ots-1.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-09-23 11:45:41.000000 ros-cdk-ots-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1823 2022-09-23 11:45:41.000000 ros-cdk-ots-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:45:41.000000 ros-cdk-ots-1.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:45:41.000000 ros-cdk-ots-1.0.9/src/ros_cdk_ots/
+-rw-r--r--   0 root         (0) root         (0)   144290 2022-09-23 11:45:41.000000 ros-cdk-ots-1.0.9/src/ros_cdk_ots/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:45:41.000000 ros-cdk-ots-1.0.9/src/ros_cdk_ots/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      404 2022-09-23 11:45:41.000000 ros-cdk-ots-1.0.9/src/ros_cdk_ots/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    67205 2022-09-23 11:45:41.000000 ros-cdk-ots-1.0.9/src/ros_cdk_ots/_jsii/ros-cdk-ots@1.0.9.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 11:45:41.000000 ros-cdk-ots-1.0.9/src/ros_cdk_ots/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:45:41.000000 ros-cdk-ots-1.0.9/src/ros_cdk_ots.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1240 2022-09-23 11:45:41.000000 ros-cdk-ots-1.0.9/src/ros_cdk_ots.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      400 2022-09-23 11:45:41.000000 ros-cdk-ots-1.0.9/src/ros_cdk_ots.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 11:45:41.000000 ros-cdk-ots-1.0.9/src/ros_cdk_ots.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2022-09-23 11:45:41.000000 ros-cdk-ots-1.0.9/src/ros_cdk_ots.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2022-09-23 11:45:41.000000 ros-cdk-ots-1.0.9/src/ros_cdk_ots.egg-info/top_level.txt
```

### Comparing `ros-cdk-ots-1.0.8/LICENSE` & `ros-cdk-ots-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-ots-1.0.8/PKG-INFO` & `ros-cdk-ots-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-ots
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS OTS Construct Library
```

### Comparing `ros-cdk-ots-1.0.8/setup.py` & `ros-cdk-ots-1.0.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-ots",
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
         "ros_cdk_ots",
         "ros_cdk_ots._jsii"
     ],
     "package_data": {
         "ros_cdk_ots._jsii": [
-            "ros-cdk-ots@1.0.8.jsii.tgz"
+            "ros-cdk-ots@1.0.9.jsii.tgz"
         ],
         "ros_cdk_ots": [
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

### Comparing `ros-cdk-ots-1.0.8/src/ros_cdk_ots/__init__.py` & `ros-cdk-ots-1.0.9/src/ros_cdk_ots/__init__.py`

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
 
 
 class Instance(
     ros_cdk_core.Resource,
@@ -29,49 +31,55 @@
 ):
     '''A ROS resource type:  ``ALIYUN::OTS::Instance``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "InstanceProps",
+        props: typing.Union["InstanceProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::OTS::Instance``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(Instance.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInstanceName")
     def attr_instance_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute InstanceName: Instance name.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInstanceName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPrivateEndpoint")
     def attr_private_endpoint(self) -> ros_cdk_core.IResolvable:
         '''Attribute PrivateEndpoint: Private endpoint.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPrivateEndpoint"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPublicEndpoint")
     def attr_public_endpoint(self) -> ros_cdk_core.IResolvable:
         '''Attribute PublicEndpoint: Public endpoint.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPublicEndpoint"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVpcEndpoint")
     def attr_vpc_endpoint(self) -> ros_cdk_core.IResolvable:
         '''Attribute VpcEndpoint: Vpc endpoint.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVpcEndpoint"))
 
 
 @jsii.data_type(
@@ -89,24 +97,31 @@
     def __init__(
         self,
         *,
         instance_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         cluster_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         description: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         network: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        tags: typing.Optional[typing.Sequence["RosInstance.TagsProperty"]] = None,
+        tags: typing.Optional[typing.Sequence[typing.Union["RosInstance.TagsProperty", typing.Dict[str, typing.Any]]]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::OTS::Instance``.
 
         :param instance_name: Property instanceName: The name of the instance.
         :param cluster_type: Property clusterType: Cluster type, the default is SSD.
         :param description: Property description: Instance description.
         :param network: Property network: Instance network type, default is NORMAL.
         :param tags: Property tags: Tags to attach to instance. Max support 5 tags to add during create instance. Each tag with two properties Key and Value, and Key is required.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(InstanceProps.__init__)
+            check_type(argname="argument instance_name", value=instance_name, expected_type=type_hints["instance_name"])
+            check_type(argname="argument cluster_type", value=cluster_type, expected_type=type_hints["cluster_type"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument network", value=network, expected_type=type_hints["network"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
         self._values: typing.Dict[str, typing.Any] = {
             "instance_name": instance_name,
         }
         if cluster_type is not None:
             self._values["cluster_type"] = cluster_type
         if description is not None:
             self._values["description"] = description
@@ -174,167 +189,194 @@
 ):
     '''A ROS template type:  ``ALIYUN::OTS::Instance``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosInstanceProps",
+        props: typing.Union["RosInstanceProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::OTS::Instance``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosInstance.__init__)
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
+            type_hints = typing.get_type_hints(RosInstance._render_properties)
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
     @jsii.member(jsii_name="attrInstanceName")
     def attr_instance_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: InstanceName: Instance name
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInstanceName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPrivateEndpoint")
     def attr_private_endpoint(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: PrivateEndpoint: Private endpoint
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPrivateEndpoint"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPublicEndpoint")
     def attr_public_endpoint(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: PublicEndpoint: Public endpoint
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPublicEndpoint"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVpcEndpoint")
     def attr_vpc_endpoint(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: VpcEndpoint: Vpc endpoint
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVpcEndpoint"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosInstance, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="instanceName")
     def instance_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: instanceName: The name of the instance.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "instanceName"))
 
     @instance_name.setter
     def instance_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "instance_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "instanceName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="clusterType")
     def cluster_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: clusterType: Cluster type, the default is SSD.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "clusterType"))
 
     @cluster_type.setter
     def cluster_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "cluster_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "clusterType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="description")
     def description(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: description: Instance description.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "description"))
 
     @description.setter
     def description(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "description").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "description", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="network")
     def network(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: network: Instance network type, default is NORMAL.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "network"))
 
     @network.setter
     def network(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "network").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "network", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="tags")
     def tags(self) -> typing.Optional[typing.List["RosInstance.TagsProperty"]]:
         '''
         :Property: tags: Tags to attach to instance. Max support 5 tags to add during create instance. Each tag with two properties Key and Value, and Key is required.
         '''
         return typing.cast(typing.Optional[typing.List["RosInstance.TagsProperty"]], jsii.get(self, "tags"))
 
     @tags.setter
     def tags(
         self,
         value: typing.Optional[typing.List["RosInstance.TagsProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "tags").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "tags", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-ots.RosInstance.TagsProperty",
         jsii_struct_bases=[],
         name_mapping={"key": "key", "value": "value"},
     )
@@ -345,14 +387,18 @@
             key: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param key: 
             :param value: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosInstance.TagsProperty.__init__)
+                check_type(argname="argument key", value=key, expected_type=type_hints["key"])
+                check_type(argname="argument value", value=value, expected_type=type_hints["value"])
             self._values: typing.Dict[str, typing.Any] = {
                 "key": key,
             }
             if value is not None:
                 self._values["value"] = value
 
         @builtins.property
@@ -401,24 +447,31 @@
     def __init__(
         self,
         *,
         instance_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         cluster_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         description: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         network: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        tags: typing.Optional[typing.Sequence[RosInstance.TagsProperty]] = None,
+        tags: typing.Optional[typing.Sequence[typing.Union[RosInstance.TagsProperty, typing.Dict[str, typing.Any]]]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::OTS::Instance``.
 
         :param instance_name: 
         :param cluster_type: 
         :param description: 
         :param network: 
         :param tags: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosInstanceProps.__init__)
+            check_type(argname="argument instance_name", value=instance_name, expected_type=type_hints["instance_name"])
+            check_type(argname="argument cluster_type", value=cluster_type, expected_type=type_hints["cluster_type"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument network", value=network, expected_type=type_hints["network"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
         self._values: typing.Dict[str, typing.Any] = {
             "instance_name": instance_name,
         }
         if cluster_type is not None:
             self._values["cluster_type"] = cluster_type
         if description is not None:
             self._values["description"] = description
@@ -493,144 +546,171 @@
 ):
     '''A ROS template type:  ``ALIYUN::OTS::SearchIndex``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosSearchIndexProps",
+        props: typing.Union["RosSearchIndexProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::OTS::SearchIndex``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosSearchIndex.__init__)
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
+            type_hints = typing.get_type_hints(RosSearchIndex._render_properties)
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
     @jsii.member(jsii_name="attrIndexName")
     def attr_index_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: IndexName: Index name.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrIndexName"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosSearchIndex, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="fieldSchemas")
     def field_schemas(
         self,
     ) -> typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosSearchIndex.FieldSchemasProperty"]]]:
         '''
         :Property: fieldSchemas: list of field_schema.
         '''
         return typing.cast(typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosSearchIndex.FieldSchemasProperty"]]], jsii.get(self, "fieldSchemas"))
 
     @field_schemas.setter
     def field_schemas(
         self,
         value: typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosSearchIndex.FieldSchemasProperty"]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSearchIndex, "field_schemas").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "fieldSchemas", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="indexName")
     def index_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: indexName: The index name.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "indexName"))
 
     @index_name.setter
     def index_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSearchIndex, "index_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "indexName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="instanceName")
     def instance_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: instanceName: The name of the OTS instance in which table will locate.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "instanceName"))
 
     @instance_name.setter
     def instance_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSearchIndex, "instance_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "instanceName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="tableName")
     def table_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: tableName: The table name of the OTS instance.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "tableName"))
 
     @table_name.setter
     def table_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSearchIndex, "table_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "tableName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="indexSetting")
     def index_setting(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosSearchIndex.IndexSettingProperty"]]:
         '''
         :Property: indexSetting: Index settings
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosSearchIndex.IndexSettingProperty"]], jsii.get(self, "indexSetting"))
 
     @index_setting.setter
     def index_setting(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosSearchIndex.IndexSettingProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSearchIndex, "index_setting").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "indexSetting", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="indexSort")
     def index_sort(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosSearchIndex.IndexSortProperty"]]:
         '''
         :Property:
 
@@ -641,14 +721,17 @@
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosSearchIndex.IndexSortProperty"]], jsii.get(self, "indexSort"))
 
     @index_sort.setter
     def index_sort(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosSearchIndex.IndexSortProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSearchIndex, "index_sort").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "indexSort", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-ots.RosSearchIndex.FieldSchemasProperty",
         jsii_struct_bases=[],
         name_mapping={
             "field_name": "fieldName",
@@ -668,26 +751,36 @@
             field_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             field_type: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             analyzer: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
             enable_sort_and_agg: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
             index: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
             is_array: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
             store: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
-            sub_field_schemas: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosSearchIndex.SubFieldSchemasProperty"]]]] = None,
+            sub_field_schemas: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosSearchIndex.SubFieldSchemasProperty", typing.Dict[str, typing.Any]]]]]] = None,
         ) -> None:
             '''
             :param field_name: 
             :param field_type: 
             :param analyzer: 
             :param enable_sort_and_agg: 
             :param index: 
             :param is_array: 
             :param store: 
             :param sub_field_schemas: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosSearchIndex.FieldSchemasProperty.__init__)
+                check_type(argname="argument field_name", value=field_name, expected_type=type_hints["field_name"])
+                check_type(argname="argument field_type", value=field_type, expected_type=type_hints["field_type"])
+                check_type(argname="argument analyzer", value=analyzer, expected_type=type_hints["analyzer"])
+                check_type(argname="argument enable_sort_and_agg", value=enable_sort_and_agg, expected_type=type_hints["enable_sort_and_agg"])
+                check_type(argname="argument index", value=index, expected_type=type_hints["index"])
+                check_type(argname="argument is_array", value=is_array, expected_type=type_hints["is_array"])
+                check_type(argname="argument store", value=store, expected_type=type_hints["store"])
+                check_type(argname="argument sub_field_schemas", value=sub_field_schemas, expected_type=type_hints["sub_field_schemas"])
             self._values: typing.Dict[str, typing.Any] = {
                 "field_name": field_name,
                 "field_type": field_type,
             }
             if analyzer is not None:
                 self._values["analyzer"] = analyzer
             if enable_sort_and_agg is not None:
@@ -831,14 +924,19 @@
             sort_order: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param field_name: 
             :param sort_mode: 
             :param sort_order: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosSearchIndex.FieldSortProperty.__init__)
+                check_type(argname="argument field_name", value=field_name, expected_type=type_hints["field_name"])
+                check_type(argname="argument sort_mode", value=sort_mode, expected_type=type_hints["sort_mode"])
+                check_type(argname="argument sort_order", value=sort_order, expected_type=type_hints["sort_order"])
             self._values: typing.Dict[str, typing.Any] = {
                 "field_name": field_name,
             }
             if sort_mode is not None:
                 self._values["sort_mode"] = sort_mode
             if sort_order is not None:
                 self._values["sort_order"] = sort_order
@@ -904,14 +1002,20 @@
         ) -> None:
             '''
             :param field_name: 
             :param points: 
             :param sort_mode: 
             :param sort_order: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosSearchIndex.GeoDistanceSortProperty.__init__)
+                check_type(argname="argument field_name", value=field_name, expected_type=type_hints["field_name"])
+                check_type(argname="argument points", value=points, expected_type=type_hints["points"])
+                check_type(argname="argument sort_mode", value=sort_mode, expected_type=type_hints["sort_mode"])
+                check_type(argname="argument sort_order", value=sort_order, expected_type=type_hints["sort_order"])
             self._values: typing.Dict[str, typing.Any] = {
                 "field_name": field_name,
                 "points": points,
             }
             if sort_mode is not None:
                 self._values["sort_mode"] = sort_mode
             if sort_order is not None:
@@ -978,14 +1082,17 @@
             self,
             *,
             routing_fields: typing.Optional[typing.Union[typing.Sequence[typing.Any], ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param routing_fields: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosSearchIndex.IndexSettingProperty.__init__)
+                check_type(argname="argument routing_fields", value=routing_fields, expected_type=type_hints["routing_fields"])
             self._values: typing.Dict[str, typing.Any] = {}
             if routing_fields is not None:
                 self._values["routing_fields"] = routing_fields
 
         @builtins.property
         def routing_fields(
             self,
@@ -1017,19 +1124,22 @@
         jsii_struct_bases=[],
         name_mapping={"sorters": "sorters"},
     )
     class IndexSortProperty:
         def __init__(
             self,
             *,
-            sorters: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosSearchIndex.SortersProperty"]]],
+            sorters: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosSearchIndex.SortersProperty", typing.Dict[str, typing.Any]]]]],
         ) -> None:
             '''
             :param sorters: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosSearchIndex.IndexSortProperty.__init__)
+                check_type(argname="argument sorters", value=sorters, expected_type=type_hints["sorters"])
             self._values: typing.Dict[str, typing.Any] = {
                 "sorters": sorters,
             }
 
         @builtins.property
         def sorters(
             self,
@@ -1067,14 +1177,17 @@
             self,
             *,
             sort_order: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param sort_order: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosSearchIndex.PrimaryKeySortProperty.__init__)
+                check_type(argname="argument sort_order", value=sort_order, expected_type=type_hints["sort_order"])
             self._values: typing.Dict[str, typing.Any] = {}
             if sort_order is not None:
                 self._values["sort_order"] = sort_order
 
         @builtins.property
         def sort_order(
             self,
@@ -1106,14 +1219,17 @@
             self,
             *,
             sort_order: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param sort_order: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosSearchIndex.ScoreSortProperty.__init__)
+                check_type(argname="argument sort_order", value=sort_order, expected_type=type_hints["sort_order"])
             self._values: typing.Dict[str, typing.Any] = {}
             if sort_order is not None:
                 self._values["sort_order"] = sort_order
 
         @builtins.property
         def sort_order(
             self,
@@ -1145,25 +1261,31 @@
             "score_sort": "scoreSort",
         },
     )
     class SortersProperty:
         def __init__(
             self,
             *,
-            field_sort: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosSearchIndex.FieldSortProperty"]] = None,
-            geo_distance_sort: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosSearchIndex.GeoDistanceSortProperty"]] = None,
-            primary_key_sort: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosSearchIndex.PrimaryKeySortProperty"]] = None,
-            score_sort: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosSearchIndex.ScoreSortProperty"]] = None,
+            field_sort: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosSearchIndex.FieldSortProperty", typing.Dict[str, typing.Any]]]] = None,
+            geo_distance_sort: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosSearchIndex.GeoDistanceSortProperty", typing.Dict[str, typing.Any]]]] = None,
+            primary_key_sort: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosSearchIndex.PrimaryKeySortProperty", typing.Dict[str, typing.Any]]]] = None,
+            score_sort: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosSearchIndex.ScoreSortProperty", typing.Dict[str, typing.Any]]]] = None,
         ) -> None:
             '''
             :param field_sort: 
             :param geo_distance_sort: 
             :param primary_key_sort: 
             :param score_sort: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosSearchIndex.SortersProperty.__init__)
+                check_type(argname="argument field_sort", value=field_sort, expected_type=type_hints["field_sort"])
+                check_type(argname="argument geo_distance_sort", value=geo_distance_sort, expected_type=type_hints["geo_distance_sort"])
+                check_type(argname="argument primary_key_sort", value=primary_key_sort, expected_type=type_hints["primary_key_sort"])
+                check_type(argname="argument score_sort", value=score_sort, expected_type=type_hints["score_sort"])
             self._values: typing.Dict[str, typing.Any] = {}
             if field_sort is not None:
                 self._values["field_sort"] = field_sort
             if geo_distance_sort is not None:
                 self._values["geo_distance_sort"] = geo_distance_sort
             if primary_key_sort is not None:
                 self._values["primary_key_sort"] = primary_key_sort
@@ -1258,14 +1380,23 @@
             :param field_type: 
             :param analyzer: 
             :param enable_sort_and_agg: 
             :param index: 
             :param is_array: 
             :param store: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosSearchIndex.SubFieldSchemasProperty.__init__)
+                check_type(argname="argument field_name", value=field_name, expected_type=type_hints["field_name"])
+                check_type(argname="argument field_type", value=field_type, expected_type=type_hints["field_type"])
+                check_type(argname="argument analyzer", value=analyzer, expected_type=type_hints["analyzer"])
+                check_type(argname="argument enable_sort_and_agg", value=enable_sort_and_agg, expected_type=type_hints["enable_sort_and_agg"])
+                check_type(argname="argument index", value=index, expected_type=type_hints["index"])
+                check_type(argname="argument is_array", value=is_array, expected_type=type_hints["is_array"])
+                check_type(argname="argument store", value=store, expected_type=type_hints["store"])
             self._values: typing.Dict[str, typing.Any] = {
                 "field_name": field_name,
                 "field_type": field_type,
             }
             if analyzer is not None:
                 self._values["analyzer"] = analyzer
             if enable_sort_and_agg is not None:
@@ -1389,30 +1520,38 @@
         "index_sort": "indexSort",
     },
 )
 class RosSearchIndexProps:
     def __init__(
         self,
         *,
-        field_schemas: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosSearchIndex.FieldSchemasProperty]]],
+        field_schemas: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosSearchIndex.FieldSchemasProperty, typing.Dict[str, typing.Any]]]]],
         index_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         instance_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         table_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
-        index_setting: typing.Optional[typing.Union[ros_cdk_core.IResolvable, RosSearchIndex.IndexSettingProperty]] = None,
-        index_sort: typing.Optional[typing.Union[ros_cdk_core.IResolvable, RosSearchIndex.IndexSortProperty]] = None,
+        index_setting: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosSearchIndex.IndexSettingProperty, typing.Dict[str, typing.Any]]]] = None,
+        index_sort: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosSearchIndex.IndexSortProperty, typing.Dict[str, typing.Any]]]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::OTS::SearchIndex``.
 
         :param field_schemas: 
         :param index_name: 
         :param instance_name: 
         :param table_name: 
         :param index_setting: 
         :param index_sort: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosSearchIndexProps.__init__)
+            check_type(argname="argument field_schemas", value=field_schemas, expected_type=type_hints["field_schemas"])
+            check_type(argname="argument index_name", value=index_name, expected_type=type_hints["index_name"])
+            check_type(argname="argument instance_name", value=instance_name, expected_type=type_hints["instance_name"])
+            check_type(argname="argument table_name", value=table_name, expected_type=type_hints["table_name"])
+            check_type(argname="argument index_setting", value=index_setting, expected_type=type_hints["index_setting"])
+            check_type(argname="argument index_sort", value=index_sort, expected_type=type_hints["index_sort"])
         self._values: typing.Dict[str, typing.Any] = {
             "field_schemas": field_schemas,
             "index_name": index_name,
             "instance_name": instance_name,
             "table_name": table_name,
         }
         if index_setting is not None:
@@ -1501,211 +1640,250 @@
 ):
     '''A ROS template type:  ``ALIYUN::OTS::Table``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosTableProps",
+        props: typing.Union["RosTableProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::OTS::Table``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosTable.__init__)
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
+            type_hints = typing.get_type_hints(RosTable._render_properties)
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
     @jsii.member(jsii_name="attrTableName")
     def attr_table_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: TableName: Table name
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTableName"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosTable, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="instanceName")
     def instance_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: instanceName: The name of the OTS instance in which table will locate.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "instanceName"))
 
     @instance_name.setter
     def instance_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTable, "instance_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "instanceName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="primaryKey")
     def primary_key(
         self,
     ) -> typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosTable.PrimaryKeyProperty"]]]:
         '''
         :Property: primaryKey: It describes the attribute value of primary key. The number of primary_key should not be less than one and not be more than four.
         '''
         return typing.cast(typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosTable.PrimaryKeyProperty"]]], jsii.get(self, "primaryKey"))
 
     @primary_key.setter
     def primary_key(
         self,
         value: typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosTable.PrimaryKeyProperty"]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTable, "primary_key").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "primaryKey", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="tableName")
     def table_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: tableName: The table name of the OTS instance.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "tableName"))
 
     @table_name.setter
     def table_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTable, "table_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "tableName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="columns")
     def columns(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosTable.ColumnsProperty"]]]]:
         '''
         :Property: columns: Attribute column for table store.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosTable.ColumnsProperty"]]]], jsii.get(self, "columns"))
 
     @columns.setter
     def columns(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosTable.ColumnsProperty"]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTable, "columns").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "columns", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="deviationCellVersionInSec")
     def deviation_cell_version_in_sec(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: deviationCellVersionInSec: Maximum version deviation. The purpose is mainly to prohibit writing and expected large data, such as setting the deviation_cell_version_in_sec to 1000, and if the current timestamp is 10000, the timestamp range allowed to be written is [10000 - 1000, 10000 + 1000]. The valid value is 1-9223372036854775807. Defaults to 86400.
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "deviationCellVersionInSec"))
 
     @deviation_cell_version_in_sec.setter
     def deviation_cell_version_in_sec(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTable, "deviation_cell_version_in_sec").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "deviationCellVersionInSec", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="maxVersions")
     def max_versions(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: maxVersions: The maximum number of versions stored in this table. The valid value is 1-2147483647. Default to 1.
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "maxVersions"))
 
     @max_versions.setter
     def max_versions(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTable, "max_versions").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "maxVersions", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="reservedThroughput")
     def reserved_throughput(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosTable.ReservedThroughputProperty"]]:
         '''
         :Property: reservedThroughput: The initial reserved read/write throughput setting of the table to be created, the reserved read throughput and reserved write throughput of any table cannot exceed 5000.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosTable.ReservedThroughputProperty"]], jsii.get(self, "reservedThroughput"))
 
     @reserved_throughput.setter
     def reserved_throughput(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosTable.ReservedThroughputProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTable, "reserved_throughput").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "reservedThroughput", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="secondaryIndices")
     def secondary_indices(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosTable.SecondaryIndicesProperty"]]]]:
         '''
         :Property: secondaryIndices: The secondary indices of the table.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosTable.SecondaryIndicesProperty"]]]], jsii.get(self, "secondaryIndices"))
 
     @secondary_indices.setter
     def secondary_indices(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosTable.SecondaryIndicesProperty"]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTable, "secondary_indices").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "secondaryIndices", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="timeToLive")
     def time_to_live(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: timeToLive: The retention time of data stored in this table (unit: second). The value maximum is 2147483647 and -1 means never expired. Default to -1.
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "timeToLive"))
 
     @time_to_live.setter
     def time_to_live(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTable, "time_to_live").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "timeToLive", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-ots.RosTable.ColumnsProperty",
         jsii_struct_bases=[],
         name_mapping={"name": "name", "type": "type"},
     )
@@ -1716,14 +1894,18 @@
             name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             type: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         ) -> None:
             '''
             :param name: 
             :param type: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosTable.ColumnsProperty.__init__)
+                check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+                check_type(argname="argument type", value=type, expected_type=type_hints["type"])
             self._values: typing.Dict[str, typing.Any] = {
                 "name": name,
                 "type": type,
             }
 
         @builtins.property
         def name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
@@ -1766,14 +1948,18 @@
             name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             type: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         ) -> None:
             '''
             :param name: 
             :param type: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosTable.PrimaryKeyProperty.__init__)
+                check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+                check_type(argname="argument type", value=type, expected_type=type_hints["type"])
             self._values: typing.Dict[str, typing.Any] = {
                 "name": name,
                 "type": type,
             }
 
         @builtins.property
         def name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
@@ -1816,14 +2002,18 @@
             read: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
             write: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
         ) -> None:
             '''
             :param read: 
             :param write: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosTable.ReservedThroughputProperty.__init__)
+                check_type(argname="argument read", value=read, expected_type=type_hints["read"])
+                check_type(argname="argument write", value=write, expected_type=type_hints["write"])
             self._values: typing.Dict[str, typing.Any] = {
                 "read": read,
                 "write": write,
             }
 
         @builtins.property
         def read(self) -> typing.Union[jsii.Number, ros_cdk_core.IResolvable]:
@@ -1875,14 +2065,20 @@
         ) -> None:
             '''
             :param columns: 
             :param index_name: 
             :param primary_keys: 
             :param index_type: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosTable.SecondaryIndicesProperty.__init__)
+                check_type(argname="argument columns", value=columns, expected_type=type_hints["columns"])
+                check_type(argname="argument index_name", value=index_name, expected_type=type_hints["index_name"])
+                check_type(argname="argument primary_keys", value=primary_keys, expected_type=type_hints["primary_keys"])
+                check_type(argname="argument index_type", value=index_type, expected_type=type_hints["index_type"])
             self._values: typing.Dict[str, typing.Any] = {
                 "columns": columns,
                 "index_name": index_name,
                 "primary_keys": primary_keys,
             }
             if index_type is not None:
                 self._values["index_type"] = index_type
@@ -1956,35 +2152,46 @@
     },
 )
 class RosTableProps:
     def __init__(
         self,
         *,
         instance_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
-        primary_key: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosTable.PrimaryKeyProperty]]],
+        primary_key: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosTable.PrimaryKeyProperty, typing.Dict[str, typing.Any]]]]],
         table_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
-        columns: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosTable.ColumnsProperty]]]] = None,
+        columns: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosTable.ColumnsProperty, typing.Dict[str, typing.Any]]]]]] = None,
         deviation_cell_version_in_sec: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         max_versions: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
-        reserved_throughput: typing.Optional[typing.Union[ros_cdk_core.IResolvable, RosTable.ReservedThroughputProperty]] = None,
-        secondary_indices: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosTable.SecondaryIndicesProperty]]]] = None,
+        reserved_throughput: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosTable.ReservedThroughputProperty, typing.Dict[str, typing.Any]]]] = None,
+        secondary_indices: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosTable.SecondaryIndicesProperty, typing.Dict[str, typing.Any]]]]]] = None,
         time_to_live: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::OTS::Table``.
 
         :param instance_name: 
         :param primary_key: 
         :param table_name: 
         :param columns: 
         :param deviation_cell_version_in_sec: 
         :param max_versions: 
         :param reserved_throughput: 
         :param secondary_indices: 
         :param time_to_live: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosTableProps.__init__)
+            check_type(argname="argument instance_name", value=instance_name, expected_type=type_hints["instance_name"])
+            check_type(argname="argument primary_key", value=primary_key, expected_type=type_hints["primary_key"])
+            check_type(argname="argument table_name", value=table_name, expected_type=type_hints["table_name"])
+            check_type(argname="argument columns", value=columns, expected_type=type_hints["columns"])
+            check_type(argname="argument deviation_cell_version_in_sec", value=deviation_cell_version_in_sec, expected_type=type_hints["deviation_cell_version_in_sec"])
+            check_type(argname="argument max_versions", value=max_versions, expected_type=type_hints["max_versions"])
+            check_type(argname="argument reserved_throughput", value=reserved_throughput, expected_type=type_hints["reserved_throughput"])
+            check_type(argname="argument secondary_indices", value=secondary_indices, expected_type=type_hints["secondary_indices"])
+            check_type(argname="argument time_to_live", value=time_to_live, expected_type=type_hints["time_to_live"])
         self._values: typing.Dict[str, typing.Any] = {
             "instance_name": instance_name,
             "primary_key": primary_key,
             "table_name": table_name,
         }
         if columns is not None:
             self._values["columns"] = columns
@@ -2107,102 +2314,120 @@
 ):
     '''A ROS template type:  ``ALIYUN::OTS::VpcBinder``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosVpcBinderProps",
+        props: typing.Union["RosVpcBinderProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::OTS::VpcBinder``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosVpcBinder.__init__)
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
+            type_hints = typing.get_type_hints(RosVpcBinder._render_properties)
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
     @jsii.member(jsii_name="attrDomains")
     def attr_domains(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Domains: The domain names used to access the OTS instance in the VPC.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDomains"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrEndpoints")
     def attr_endpoints(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Endpoints: Private network addresses used to access the OTS instance in the VPC.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrEndpoints"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosVpcBinder, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="instanceName")
     def instance_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: instanceName: Instance name
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "instanceName"))
 
     @instance_name.setter
     def instance_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosVpcBinder, "instance_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "instanceName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vpcs")
     def vpcs(
         self,
     ) -> typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosVpcBinder.VpcsProperty"]]]:
         '''
         :Property: vpcs: Vpc binding configuration.
         '''
         return typing.cast(typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosVpcBinder.VpcsProperty"]]], jsii.get(self, "vpcs"))
 
     @vpcs.setter
     def vpcs(
         self,
         value: typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosVpcBinder.VpcsProperty"]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosVpcBinder, "vpcs").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "vpcs", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-ots.RosVpcBinder.VpcsProperty",
         jsii_struct_bases=[],
         name_mapping={
             "instance_vpc_name": "instanceVpcName",
@@ -2222,14 +2447,20 @@
         ) -> None:
             '''
             :param instance_vpc_name: 
             :param network: 
             :param virtual_switch_id: 
             :param vpc_id: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosVpcBinder.VpcsProperty.__init__)
+                check_type(argname="argument instance_vpc_name", value=instance_vpc_name, expected_type=type_hints["instance_vpc_name"])
+                check_type(argname="argument network", value=network, expected_type=type_hints["network"])
+                check_type(argname="argument virtual_switch_id", value=virtual_switch_id, expected_type=type_hints["virtual_switch_id"])
+                check_type(argname="argument vpc_id", value=vpc_id, expected_type=type_hints["vpc_id"])
             self._values: typing.Dict[str, typing.Any] = {
                 "instance_vpc_name": instance_vpc_name,
                 "network": network,
                 "virtual_switch_id": virtual_switch_id,
                 "vpc_id": vpc_id,
             }
 
@@ -2296,21 +2527,25 @@
     name_mapping={"instance_name": "instanceName", "vpcs": "vpcs"},
 )
 class RosVpcBinderProps:
     def __init__(
         self,
         *,
         instance_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
-        vpcs: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosVpcBinder.VpcsProperty]]],
+        vpcs: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosVpcBinder.VpcsProperty, typing.Dict[str, typing.Any]]]]],
     ) -> None:
         '''Properties for defining a ``ALIYUN::OTS::VpcBinder``.
 
         :param instance_name: 
         :param vpcs: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosVpcBinderProps.__init__)
+            check_type(argname="argument instance_name", value=instance_name, expected_type=type_hints["instance_name"])
+            check_type(argname="argument vpcs", value=vpcs, expected_type=type_hints["vpcs"])
         self._values: typing.Dict[str, typing.Any] = {
             "instance_name": instance_name,
             "vpcs": vpcs,
         }
 
     @builtins.property
     def instance_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
@@ -2351,31 +2586,37 @@
 ):
     '''A ROS resource type:  ``ALIYUN::OTS::SearchIndex``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "SearchIndexProps",
+        props: typing.Union["SearchIndexProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::OTS::SearchIndex``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(SearchIndex.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrIndexName")
     def attr_index_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute IndexName: Index name.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrIndexName"))
 
 
 @jsii.data_type(
@@ -2390,30 +2631,38 @@
         "index_sort": "indexSort",
     },
 )
 class SearchIndexProps:
     def __init__(
         self,
         *,
-        field_schemas: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosSearchIndex.FieldSchemasProperty]]],
+        field_schemas: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosSearchIndex.FieldSchemasProperty, typing.Dict[str, typing.Any]]]]],
         index_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         instance_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         table_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
-        index_setting: typing.Optional[typing.Union[ros_cdk_core.IResolvable, RosSearchIndex.IndexSettingProperty]] = None,
-        index_sort: typing.Optional[typing.Union[ros_cdk_core.IResolvable, RosSearchIndex.IndexSortProperty]] = None,
+        index_setting: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosSearchIndex.IndexSettingProperty, typing.Dict[str, typing.Any]]]] = None,
+        index_sort: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosSearchIndex.IndexSortProperty, typing.Dict[str, typing.Any]]]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::OTS::SearchIndex``.
 
         :param field_schemas: Property fieldSchemas: list of field_schema.
         :param index_name: Property indexName: The index name.
         :param instance_name: Property instanceName: The name of the OTS instance in which table will locate.
         :param table_name: Property tableName: The table name of the OTS instance.
         :param index_setting: Property indexSetting: Index settings.
         :param index_sort: Property indexSort: This parameter specifies how data is sorted. By default, the data is sorted in the same way as the primary key of the table. If the search index contains NESTED fields, data is not sorted by default.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(SearchIndexProps.__init__)
+            check_type(argname="argument field_schemas", value=field_schemas, expected_type=type_hints["field_schemas"])
+            check_type(argname="argument index_name", value=index_name, expected_type=type_hints["index_name"])
+            check_type(argname="argument instance_name", value=instance_name, expected_type=type_hints["instance_name"])
+            check_type(argname="argument table_name", value=table_name, expected_type=type_hints["table_name"])
+            check_type(argname="argument index_setting", value=index_setting, expected_type=type_hints["index_setting"])
+            check_type(argname="argument index_sort", value=index_sort, expected_type=type_hints["index_sort"])
         self._values: typing.Dict[str, typing.Any] = {
             "field_schemas": field_schemas,
             "index_name": index_name,
             "instance_name": instance_name,
             "table_name": table_name,
         }
         if index_setting is not None:
@@ -2490,31 +2739,37 @@
 ):
     '''A ROS resource type:  ``ALIYUN::OTS::Table``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "TableProps",
+        props: typing.Union["TableProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::OTS::Table``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(Table.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTableName")
     def attr_table_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute TableName: Table name.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTableName"))
 
 
 @jsii.data_type(
@@ -2533,35 +2788,46 @@
     },
 )
 class TableProps:
     def __init__(
         self,
         *,
         instance_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
-        primary_key: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosTable.PrimaryKeyProperty]]],
+        primary_key: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosTable.PrimaryKeyProperty, typing.Dict[str, typing.Any]]]]],
         table_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
-        columns: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosTable.ColumnsProperty]]]] = None,
+        columns: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosTable.ColumnsProperty, typing.Dict[str, typing.Any]]]]]] = None,
         deviation_cell_version_in_sec: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         max_versions: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
-        reserved_throughput: typing.Optional[typing.Union[ros_cdk_core.IResolvable, RosTable.ReservedThroughputProperty]] = None,
-        secondary_indices: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosTable.SecondaryIndicesProperty]]]] = None,
+        reserved_throughput: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosTable.ReservedThroughputProperty, typing.Dict[str, typing.Any]]]] = None,
+        secondary_indices: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosTable.SecondaryIndicesProperty, typing.Dict[str, typing.Any]]]]]] = None,
         time_to_live: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::OTS::Table``.
 
         :param instance_name: Property instanceName: The name of the OTS instance in which table will locate.
         :param primary_key: Property primaryKey: It describes the attribute value of primary key. The number of primary_key should not be less than one and not be more than four.
         :param table_name: Property tableName: The table name of the OTS instance.
         :param columns: Property columns: Attribute column for table store.
         :param deviation_cell_version_in_sec: Property deviationCellVersionInSec: Maximum version deviation. The purpose is mainly to prohibit writing and expected large data, such as setting the deviation_cell_version_in_sec to 1000, and if the current timestamp is 10000, the timestamp range allowed to be written is [10000 - 1000, 10000 + 1000]. The valid value is 1-9223372036854775807. Defaults to 86400.
         :param max_versions: Property maxVersions: The maximum number of versions stored in this table. The valid value is 1-2147483647. Default to 1.
         :param reserved_throughput: Property reservedThroughput: The initial reserved read/write throughput setting of the table to be created, the reserved read throughput and reserved write throughput of any table cannot exceed 5000.
         :param secondary_indices: Property secondaryIndices: The secondary indices of the table.
         :param time_to_live: Property timeToLive: The retention time of data stored in this table (unit: second). The value maximum is 2147483647 and -1 means never expired. Default to -1.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(TableProps.__init__)
+            check_type(argname="argument instance_name", value=instance_name, expected_type=type_hints["instance_name"])
+            check_type(argname="argument primary_key", value=primary_key, expected_type=type_hints["primary_key"])
+            check_type(argname="argument table_name", value=table_name, expected_type=type_hints["table_name"])
+            check_type(argname="argument columns", value=columns, expected_type=type_hints["columns"])
+            check_type(argname="argument deviation_cell_version_in_sec", value=deviation_cell_version_in_sec, expected_type=type_hints["deviation_cell_version_in_sec"])
+            check_type(argname="argument max_versions", value=max_versions, expected_type=type_hints["max_versions"])
+            check_type(argname="argument reserved_throughput", value=reserved_throughput, expected_type=type_hints["reserved_throughput"])
+            check_type(argname="argument secondary_indices", value=secondary_indices, expected_type=type_hints["secondary_indices"])
+            check_type(argname="argument time_to_live", value=time_to_live, expected_type=type_hints["time_to_live"])
         self._values: typing.Dict[str, typing.Any] = {
             "instance_name": instance_name,
             "primary_key": primary_key,
             "table_name": table_name,
         }
         if columns is not None:
             self._values["columns"] = columns
@@ -2678,37 +2944,43 @@
 ):
     '''A ROS resource type:  ``ALIYUN::OTS::VpcBinder``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "VpcBinderProps",
+        props: typing.Union["VpcBinderProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::OTS::VpcBinder``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(VpcBinder.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDomains")
     def attr_domains(self) -> ros_cdk_core.IResolvable:
         '''Attribute Domains: The domain names used to access the OTS instance in the VPC.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDomains"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrEndpoints")
     def attr_endpoints(self) -> ros_cdk_core.IResolvable:
         '''Attribute Endpoints: Private network addresses used to access the OTS instance in the VPC.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrEndpoints"))
 
 
 @jsii.data_type(
@@ -2717,21 +2989,25 @@
     name_mapping={"instance_name": "instanceName", "vpcs": "vpcs"},
 )
 class VpcBinderProps:
     def __init__(
         self,
         *,
         instance_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
-        vpcs: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosVpcBinder.VpcsProperty]]],
+        vpcs: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosVpcBinder.VpcsProperty, typing.Dict[str, typing.Any]]]]],
     ) -> None:
         '''Properties for defining a ``ALIYUN::OTS::VpcBinder``.
 
         :param instance_name: Property instanceName: Instance name.
         :param vpcs: Property vpcs: Vpc binding configuration.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(VpcBinderProps.__init__)
+            check_type(argname="argument instance_name", value=instance_name, expected_type=type_hints["instance_name"])
+            check_type(argname="argument vpcs", value=vpcs, expected_type=type_hints["vpcs"])
         self._values: typing.Dict[str, typing.Any] = {
             "instance_name": instance_name,
             "vpcs": vpcs,
         }
 
     @builtins.property
     def instance_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
```

### Comparing `ros-cdk-ots-1.0.8/src/ros_cdk_ots.egg-info/PKG-INFO` & `ros-cdk-ots-1.0.9/src/ros_cdk_ots.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-ots
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS OTS Construct Library
```

