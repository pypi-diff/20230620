# Comparing `tmp/ros-cdk-acm-1.0.8.tar.gz` & `tmp/ros-cdk-acm-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-acm-1.0.8.tar", last modified: Thu Jul 14 02:21:26 2022, max compression
+gzip compressed data, was "dist/ros-cdk-acm-1.0.9.tar", last modified: Fri Sep 23 10:56:47 2022, max compression
```

## Comparing `ros-cdk-acm-1.0.8.tar` & `ros-cdk-acm-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:21:26.000000 ros-cdk-acm-1.0.8/
--rw-r--r--   0 root         (0) root         (0)    10279 2022-07-14 02:21:26.000000 ros-cdk-acm-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2022-07-14 02:21:26.000000 ros-cdk-acm-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2022-07-14 02:21:26.000000 ros-cdk-acm-1.0.8/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1240 2022-07-14 02:21:26.000000 ros-cdk-acm-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      179 2022-07-14 02:21:26.000000 ros-cdk-acm-1.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)      106 2022-07-14 02:21:26.000000 ros-cdk-acm-1.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-07-14 02:21:26.000000 ros-cdk-acm-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1794 2022-07-14 02:21:26.000000 ros-cdk-acm-1.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:21:26.000000 ros-cdk-acm-1.0.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:21:26.000000 ros-cdk-acm-1.0.8/src/ros_cdk_acm/
--rw-r--r--   0 root         (0) root         (0)    31213 2022-07-14 02:21:26.000000 ros-cdk-acm-1.0.8/src/ros_cdk_acm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:21:26.000000 ros-cdk-acm-1.0.8/src/ros_cdk_acm/_jsii/
--rw-r--r--   0 root         (0) root         (0)      370 2022-07-14 02:21:26.000000 ros-cdk-acm-1.0.8/src/ros_cdk_acm/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    35890 2022-07-14 02:21:26.000000 ros-cdk-acm-1.0.8/src/ros_cdk_acm/_jsii/ros-cdk-acm@1.0.8.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:21:26.000000 ros-cdk-acm-1.0.8/src/ros_cdk_acm/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:21:26.000000 ros-cdk-acm-1.0.8/src/ros_cdk_acm.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1240 2022-07-14 02:21:26.000000 ros-cdk-acm-1.0.8/src/ros_cdk_acm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      400 2022-07-14 02:21:26.000000 ros-cdk-acm-1.0.8/src/ros_cdk_acm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:21:26.000000 ros-cdk-acm-1.0.8/src/ros_cdk_acm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2022-07-14 02:21:26.000000 ros-cdk-acm-1.0.8/src/ros_cdk_acm.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2022-07-14 02:21:26.000000 ros-cdk-acm-1.0.8/src/ros_cdk_acm.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 10:56:47.000000 ros-cdk-acm-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)    10279 2022-09-23 10:56:47.000000 ros-cdk-acm-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-09-23 10:56:47.000000 ros-cdk-acm-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2022-09-23 10:56:47.000000 ros-cdk-acm-1.0.9/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1240 2022-09-23 10:56:47.000000 ros-cdk-acm-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      179 2022-09-23 10:56:47.000000 ros-cdk-acm-1.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      236 2022-09-23 10:56:47.000000 ros-cdk-acm-1.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-09-23 10:56:47.000000 ros-cdk-acm-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1823 2022-09-23 10:56:47.000000 ros-cdk-acm-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 10:56:47.000000 ros-cdk-acm-1.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 10:56:47.000000 ros-cdk-acm-1.0.9/src/ros_cdk_acm/
+-rw-r--r--   0 root         (0) root         (0)    38081 2022-09-23 10:56:47.000000 ros-cdk-acm-1.0.9/src/ros_cdk_acm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 10:56:47.000000 ros-cdk-acm-1.0.9/src/ros_cdk_acm/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      404 2022-09-23 10:56:47.000000 ros-cdk-acm-1.0.9/src/ros_cdk_acm/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    35959 2022-09-23 10:56:47.000000 ros-cdk-acm-1.0.9/src/ros_cdk_acm/_jsii/ros-cdk-acm@1.0.9.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 10:56:47.000000 ros-cdk-acm-1.0.9/src/ros_cdk_acm/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 10:56:47.000000 ros-cdk-acm-1.0.9/src/ros_cdk_acm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1240 2022-09-23 10:56:47.000000 ros-cdk-acm-1.0.9/src/ros_cdk_acm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      400 2022-09-23 10:56:47.000000 ros-cdk-acm-1.0.9/src/ros_cdk_acm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 10:56:47.000000 ros-cdk-acm-1.0.9/src/ros_cdk_acm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2022-09-23 10:56:47.000000 ros-cdk-acm-1.0.9/src/ros_cdk_acm.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2022-09-23 10:56:47.000000 ros-cdk-acm-1.0.9/src/ros_cdk_acm.egg-info/top_level.txt
```

### Comparing `ros-cdk-acm-1.0.8/LICENSE` & `ros-cdk-acm-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-acm-1.0.8/PKG-INFO` & `ros-cdk-acm-1.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-acm
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS ACM Construct Library
```

### Comparing `ros-cdk-acm-1.0.8/setup.py` & `ros-cdk-acm-1.0.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-acm",
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
         "ros_cdk_acm",
         "ros_cdk_acm._jsii"
     ],
     "package_data": {
         "ros_cdk_acm._jsii": [
-            "ros-cdk-acm@1.0.8.jsii.tgz"
+            "ros-cdk-acm@1.0.9.jsii.tgz"
         ],
         "ros_cdk_acm": [
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

### Comparing `ros-cdk-acm-1.0.8/src/ros_cdk_acm/__init__.py` & `ros-cdk-acm-1.0.9/src/ros_cdk_acm/__init__.py`

 * *Files 22% similar despite different names*

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
 
 
 class Configuration(
     ros_cdk_core.Resource,
@@ -29,43 +31,49 @@
 ):
     '''A ROS resource type:  ``ALIYUN::ACM::Configuration``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "ConfigurationProps",
+        props: typing.Union["ConfigurationProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::ACM::Configuration``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(Configuration.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDataId")
     def attr_data_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute DataId: The ID of the configuration.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDataId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrGroup")
     def attr_group(self) -> ros_cdk_core.IResolvable:
         '''Attribute Group: Group.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrGroup"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrNamespaceId")
     def attr_namespace_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute NamespaceId: ID of namespace.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrNamespaceId"))
 
 
 @jsii.data_type(
@@ -102,14 +110,24 @@
         :param namespace_id: Property namespaceId: ID of namespace.
         :param app_name: Property appName: Configuration application name.
         :param desc: Property desc: Configuration description explains.
         :param group: Property group: Group.
         :param tags: Property tags: Label configurations, such as the presence of a plurality of tags, separated by commas.
         :param type: Property type: Provisioning content format, optional values as follows: text, json, xml, yaml, text/html, properties.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(ConfigurationProps.__init__)
+            check_type(argname="argument content", value=content, expected_type=type_hints["content"])
+            check_type(argname="argument data_id", value=data_id, expected_type=type_hints["data_id"])
+            check_type(argname="argument namespace_id", value=namespace_id, expected_type=type_hints["namespace_id"])
+            check_type(argname="argument app_name", value=app_name, expected_type=type_hints["app_name"])
+            check_type(argname="argument desc", value=desc, expected_type=type_hints["desc"])
+            check_type(argname="argument group", value=group, expected_type=type_hints["group"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
+            check_type(argname="argument type", value=type, expected_type=type_hints["type"])
         self._values: typing.Dict[str, typing.Any] = {
             "content": content,
             "data_id": data_id,
             "namespace_id": namespace_id,
         }
         if app_name is not None:
             self._values["app_name"] = app_name
@@ -205,37 +223,43 @@
 ):
     '''A ROS resource type:  ``ALIYUN::ACM::Namespace``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "NamespaceProps",
+        props: typing.Union["NamespaceProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::ACM::Namespace``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(Namespace.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrEndpoint")
     def attr_endpoint(self) -> ros_cdk_core.IResolvable:
         '''Attribute Endpoint: Endpoint.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrEndpoint"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrNamespaceId")
     def attr_namespace_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute NamespaceId: ID namespace.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrNamespaceId"))
 
 
 @jsii.data_type(
@@ -249,14 +273,17 @@
         *,
         name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
         '''Properties for defining a ``ALIYUN::ACM::Namespace``.
 
         :param name: Property name: Namespace name.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(NamespaceProps.__init__)
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
         self._values: typing.Dict[str, typing.Any] = {
             "name": name,
         }
 
     @builtins.property
     def name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''Property name: Namespace name.'''
@@ -283,87 +310,99 @@
 ):
     '''A ROS template type:  ``ALIYUN::ACM::Configuration``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosConfigurationProps",
+        props: typing.Union["RosConfigurationProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::ACM::Configuration``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosConfiguration.__init__)
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
+            type_hints = typing.get_type_hints(RosConfiguration._render_properties)
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
     @jsii.member(jsii_name="attrDataId")
     def attr_data_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: DataId: The ID of the configuration
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDataId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrGroup")
     def attr_group(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Group: Group
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrGroup"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrNamespaceId")
     def attr_namespace_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: NamespaceId: ID of namespace
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrNamespaceId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="content")
     def content(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: content: The contents of the configuration
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "content"))
 
     @content.setter
     def content(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosConfiguration, "content").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "content", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dataId")
     def data_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         dataId: The ID of the configuration. Allowed characters are upper and lower case letters, numbers, decimal points (.), Colons (:), asterisks (*), underscores (_), and underscores (-). When the ID prefix is the following value, ACM will automatically use KMS service to encrypt this configuration:
         The prefix is cipher-: the KMS service is called to encrypt and decrypt the configuration. The size of the encrypted data does not exceed 4 KB, and the maximum does not exceed 6 KB. Special symbols such as and (&) will decrypt errors and are not recommended.
@@ -372,104 +411,125 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "dataId"))
 
     @data_id.setter
     def data_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosConfiguration, "data_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dataId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosConfiguration, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="namespaceId")
     def namespace_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: namespaceId: ID of namespace
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "namespaceId"))
 
     @namespace_id.setter
     def namespace_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosConfiguration, "namespace_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "namespaceId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="appName")
     def app_name(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: appName: Configuration application name
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "appName"))
 
     @app_name.setter
     def app_name(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosConfiguration, "app_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "appName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="desc")
     def desc(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: desc: Configuration description explains
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "desc"))
 
     @desc.setter
     def desc(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosConfiguration, "desc").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "desc", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="group")
     def group(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: group: Group
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "group"))
 
     @group.setter
     def group(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosConfiguration, "group").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "group", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="tags")
     def tags(self) -> typing.Optional[builtins.str]:
         '''
         :Property: tags: Label configurations, such as the presence of a plurality of tags, separated by commas
         '''
         return typing.cast(typing.Optional[builtins.str], jsii.get(self, "tags"))
 
     @tags.setter
     def tags(self, value: typing.Optional[builtins.str]) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosConfiguration, "tags").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "tags", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="type")
     def type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -479,14 +539,17 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "type"))
 
     @type.setter
     def type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosConfiguration, "type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "type", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-acm.RosConfigurationProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -520,14 +583,24 @@
         :param namespace_id: 
         :param app_name: 
         :param desc: 
         :param group: 
         :param tags: 
         :param type: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosConfigurationProps.__init__)
+            check_type(argname="argument content", value=content, expected_type=type_hints["content"])
+            check_type(argname="argument data_id", value=data_id, expected_type=type_hints["data_id"])
+            check_type(argname="argument namespace_id", value=namespace_id, expected_type=type_hints["namespace_id"])
+            check_type(argname="argument app_name", value=app_name, expected_type=type_hints["app_name"])
+            check_type(argname="argument desc", value=desc, expected_type=type_hints["desc"])
+            check_type(argname="argument group", value=group, expected_type=type_hints["group"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
+            check_type(argname="argument type", value=type, expected_type=type_hints["type"])
         self._values: typing.Dict[str, typing.Any] = {
             "content": content,
             "data_id": data_id,
             "namespace_id": namespace_id,
         }
         if app_name is not None:
             self._values["app_name"] = app_name
@@ -641,82 +714,97 @@
 ):
     '''A ROS template type:  ``ALIYUN::ACM::Namespace``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosNamespaceProps",
+        props: typing.Union["RosNamespaceProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::ACM::Namespace``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosNamespace.__init__)
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
+            type_hints = typing.get_type_hints(RosNamespace._render_properties)
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
     @jsii.member(jsii_name="attrEndpoint")
     def attr_endpoint(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Endpoint: Endpoint
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrEndpoint"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrNamespaceId")
     def attr_namespace_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: NamespaceId: ID namespace
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrNamespaceId"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosNamespace, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="name")
     def name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: name: Namespace name
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "name"))
 
     @name.setter
     def name(self, value: typing.Union[builtins.str, ros_cdk_core.IResolvable]) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosNamespace, "name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "name", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-acm.RosNamespaceProps",
     jsii_struct_bases=[],
     name_mapping={"name": "name"},
@@ -727,14 +815,17 @@
         *,
         name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
         '''Properties for defining a ``ALIYUN::ACM::Namespace``.
 
         :param name: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosNamespaceProps.__init__)
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
         self._values: typing.Dict[str, typing.Any] = {
             "name": name,
         }
 
     @builtins.property
     def name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
```

### Comparing `ros-cdk-acm-1.0.8/src/ros_cdk_acm.egg-info/PKG-INFO` & `ros-cdk-acm-1.0.9/src/ros_cdk_acm.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-acm
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS ACM Construct Library
```

