# Comparing `tmp/ros-cdk-rocketmq-1.0.8.tar.gz` & `tmp/ros-cdk-rocketmq-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-rocketmq-1.0.8.tar", last modified: Thu Jul 14 02:25:57 2022, max compression
+gzip compressed data, was "dist/ros-cdk-rocketmq-1.0.9.tar", last modified: Fri Sep 23 11:54:52 2022, max compression
```

## Comparing `ros-cdk-rocketmq-1.0.8.tar` & `ros-cdk-rocketmq-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:25:57.000000 ros-cdk-rocketmq-1.0.8/
--rw-r--r--   0 root         (0) root         (0)    10279 2022-07-14 02:25:57.000000 ros-cdk-rocketmq-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2022-07-14 02:25:57.000000 ros-cdk-rocketmq-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2022-07-14 02:25:57.000000 ros-cdk-rocketmq-1.0.8/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1260 2022-07-14 02:25:57.000000 ros-cdk-rocketmq-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      194 2022-07-14 02:25:57.000000 ros-cdk-rocketmq-1.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)      106 2022-07-14 02:25:57.000000 ros-cdk-rocketmq-1.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-07-14 02:25:57.000000 ros-cdk-rocketmq-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1824 2022-07-14 02:25:57.000000 ros-cdk-rocketmq-1.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:25:57.000000 ros-cdk-rocketmq-1.0.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:25:57.000000 ros-cdk-rocketmq-1.0.8/src/ros_cdk_rocketmq/
--rw-r--r--   0 root         (0) root         (0)    49461 2022-07-14 02:25:57.000000 ros-cdk-rocketmq-1.0.8/src/ros_cdk_rocketmq/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:25:57.000000 ros-cdk-rocketmq-1.0.8/src/ros_cdk_rocketmq/_jsii/
--rw-r--r--   0 root         (0) root         (0)      393 2022-07-14 02:25:57.000000 ros-cdk-rocketmq-1.0.8/src/ros_cdk_rocketmq/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    44072 2022-07-14 02:25:57.000000 ros-cdk-rocketmq-1.0.8/src/ros_cdk_rocketmq/_jsii/ros-cdk-rocketmq@1.0.8.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:25:57.000000 ros-cdk-rocketmq-1.0.8/src/ros_cdk_rocketmq/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:25:57.000000 ros-cdk-rocketmq-1.0.8/src/ros_cdk_rocketmq.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1260 2022-07-14 02:25:57.000000 ros-cdk-rocketmq-1.0.8/src/ros_cdk_rocketmq.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      450 2022-07-14 02:25:57.000000 ros-cdk-rocketmq-1.0.8/src/ros_cdk_rocketmq.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:25:57.000000 ros-cdk-rocketmq-1.0.8/src/ros_cdk_rocketmq.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2022-07-14 02:25:57.000000 ros-cdk-rocketmq-1.0.8/src/ros_cdk_rocketmq.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2022-07-14 02:25:57.000000 ros-cdk-rocketmq-1.0.8/src/ros_cdk_rocketmq.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:54:52.000000 ros-cdk-rocketmq-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)    10279 2022-09-23 11:54:52.000000 ros-cdk-rocketmq-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-09-23 11:54:52.000000 ros-cdk-rocketmq-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2022-09-23 11:54:52.000000 ros-cdk-rocketmq-1.0.9/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1260 2022-09-23 11:54:52.000000 ros-cdk-rocketmq-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      194 2022-09-23 11:54:52.000000 ros-cdk-rocketmq-1.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      236 2022-09-23 11:54:52.000000 ros-cdk-rocketmq-1.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-09-23 11:54:52.000000 ros-cdk-rocketmq-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1853 2022-09-23 11:54:52.000000 ros-cdk-rocketmq-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:54:52.000000 ros-cdk-rocketmq-1.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:54:52.000000 ros-cdk-rocketmq-1.0.9/src/ros_cdk_rocketmq/
+-rw-r--r--   0 root         (0) root         (0)    58952 2022-09-23 11:54:52.000000 ros-cdk-rocketmq-1.0.9/src/ros_cdk_rocketmq/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:54:52.000000 ros-cdk-rocketmq-1.0.9/src/ros_cdk_rocketmq/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      427 2022-09-23 11:54:52.000000 ros-cdk-rocketmq-1.0.9/src/ros_cdk_rocketmq/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    44135 2022-09-23 11:54:52.000000 ros-cdk-rocketmq-1.0.9/src/ros_cdk_rocketmq/_jsii/ros-cdk-rocketmq@1.0.9.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 11:54:52.000000 ros-cdk-rocketmq-1.0.9/src/ros_cdk_rocketmq/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:54:52.000000 ros-cdk-rocketmq-1.0.9/src/ros_cdk_rocketmq.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1260 2022-09-23 11:54:52.000000 ros-cdk-rocketmq-1.0.9/src/ros_cdk_rocketmq.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      450 2022-09-23 11:54:52.000000 ros-cdk-rocketmq-1.0.9/src/ros_cdk_rocketmq.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 11:54:52.000000 ros-cdk-rocketmq-1.0.9/src/ros_cdk_rocketmq.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2022-09-23 11:54:52.000000 ros-cdk-rocketmq-1.0.9/src/ros_cdk_rocketmq.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2022-09-23 11:54:52.000000 ros-cdk-rocketmq-1.0.9/src/ros_cdk_rocketmq.egg-info/top_level.txt
```

### Comparing `ros-cdk-rocketmq-1.0.8/LICENSE` & `ros-cdk-rocketmq-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-rocketmq-1.0.8/PKG-INFO` & `ros-cdk-rocketmq-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-rocketmq
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS ROCKETMQ Construct Library
```

### Comparing `ros-cdk-rocketmq-1.0.8/setup.py` & `ros-cdk-rocketmq-1.0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-rocketmq",
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
         "ros_cdk_rocketmq",
         "ros_cdk_rocketmq._jsii"
     ],
     "package_data": {
         "ros_cdk_rocketmq._jsii": [
-            "ros-cdk-rocketmq@1.0.8.jsii.tgz"
+            "ros-cdk-rocketmq@1.0.9.jsii.tgz"
         ],
         "ros_cdk_rocketmq": [
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

### Comparing `ros-cdk-rocketmq-1.0.8/src/ros_cdk_rocketmq/__init__.py` & `ros-cdk-rocketmq-1.0.9/src/ros_cdk_rocketmq/__init__.py`

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
 
 
 class Group(
     ros_cdk_core.Resource,
@@ -29,43 +31,49 @@
 ):
     '''A ROS resource type:  ``ALIYUN::ROCKETMQ::Group``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "GroupProps",
+        props: typing.Union["GroupProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::ROCKETMQ::Group``.
 
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
     @jsii.member(jsii_name="attrGroupId")
     def attr_group_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute GroupId: Group ID.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrGroupId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrGroupType")
     def attr_group_type(self) -> ros_cdk_core.IResolvable:
         '''Attribute GroupType: Group Type.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrGroupType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInstanceId")
     def attr_instance_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute InstanceId: Instance ID.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInstanceId"))
 
 
 @jsii.data_type(
@@ -90,14 +98,20 @@
         '''Properties for defining a ``ALIYUN::ROCKETMQ::Group``.
 
         :param group_id: Property groupId: The group ID of the consumption cluster. When creating a group ID, pay attention to the following aspects: A group ID starts with"GID_" or "GID-", and contains letters, numbers, hyphens (-), and underscores (_). A group ID ranges from 7 to 64 bytes. Once a group ID is created, it cannot be edited anymore.
         :param instance_id: Property instanceId: The ID of the instance.
         :param group_type: Property groupType: Group ID specify the creation of applicable agreements. Group ID TCP protocol and the HTTP protocol can not be shared, the need to create separately. Value as follows: tcp: Default, indicates Group ID is created only for the TCP protocol messaging. http: represents the Group ID was created only for the HTTP protocol messaging.
         :param remark: Property remark: The remarks on the request.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(GroupProps.__init__)
+            check_type(argname="argument group_id", value=group_id, expected_type=type_hints["group_id"])
+            check_type(argname="argument instance_id", value=instance_id, expected_type=type_hints["instance_id"])
+            check_type(argname="argument group_type", value=group_type, expected_type=type_hints["group_type"])
+            check_type(argname="argument remark", value=remark, expected_type=type_hints["remark"])
         self._values: typing.Dict[str, typing.Any] = {
             "group_id": group_id,
             "instance_id": instance_id,
         }
         if group_type is not None:
             self._values["group_type"] = group_type
         if remark is not None:
@@ -163,67 +177,73 @@
 ):
     '''A ROS resource type:  ``ALIYUN::ROCKETMQ::Instance``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "InstanceProps",
+        props: typing.Union["InstanceProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::ROCKETMQ::Instance``.
 
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
     @jsii.member(jsii_name="attrHttpInternalEndpoint")
     def attr_http_internal_endpoint(self) -> ros_cdk_core.IResolvable:
         '''Attribute HttpInternalEndpoint: The internal HTTP endpoint for the Message Queue for Apache RocketMQ instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrHttpInternalEndpoint"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrHttpInternetEndpoint")
     def attr_http_internet_endpoint(self) -> ros_cdk_core.IResolvable:
         '''Attribute HttpInternetEndpoint: The Internet HTTP endpoint for the Message Queue for Apache RocketMQ instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrHttpInternetEndpoint"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrHttpInternetSecureEndpoint")
     def attr_http_internet_secure_endpoint(self) -> ros_cdk_core.IResolvable:
         '''Attribute HttpInternetSecureEndpoint: The Internet HTTPS endpoint for the Message Queue for Apache RocketMQ instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrHttpInternetSecureEndpoint"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInstanceId")
     def attr_instance_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute InstanceId: Instance ID created.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInstanceId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInstanceName")
     def attr_instance_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute InstanceName: Instance name.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInstanceName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInstanceType")
     def attr_instance_type(self) -> ros_cdk_core.IResolvable:
         '''Attribute InstanceType: Instance Type.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInstanceType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTcpEndpoint")
     def attr_tcp_endpoint(self) -> ros_cdk_core.IResolvable:
         '''Attribute TcpEndpoint: The TCP endpoint for the Message Queue for Apache RocketMQ instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTcpEndpoint"))
 
 
 @jsii.data_type(
@@ -233,22 +253,27 @@
 )
 class InstanceProps:
     def __init__(
         self,
         *,
         instance_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         remark: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        tags: typing.Optional[typing.Sequence["RosInstance.TagsProperty"]] = None,
+        tags: typing.Optional[typing.Sequence[typing.Union["RosInstance.TagsProperty", typing.Dict[str, typing.Any]]]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::ROCKETMQ::Instance``.
 
         :param instance_name: Property instanceName: The name of the instance, which contains 3 to 64 characters in Chinese or English.
         :param remark: Property remark: The remark of instance.
         :param tags: Property tags: Tags to attach to instance. Max support 20 tags to add during create instance. Each tag with two properties Key and Value, and Key is required.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(InstanceProps.__init__)
+            check_type(argname="argument instance_name", value=instance_name, expected_type=type_hints["instance_name"])
+            check_type(argname="argument remark", value=remark, expected_type=type_hints["remark"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
         self._values: typing.Dict[str, typing.Any] = {
             "instance_name": instance_name,
         }
         if remark is not None:
             self._values["remark"] = remark
         if tags is not None:
             self._values["tags"] = tags
@@ -296,81 +321,93 @@
 ):
     '''A ROS template type:  ``ALIYUN::ROCKETMQ::Group``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosGroupProps",
+        props: typing.Union["RosGroupProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::ROCKETMQ::Group``.
 
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
     @jsii.member(jsii_name="attrGroupId")
     def attr_group_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: GroupId: Group ID
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrGroupId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrGroupType")
     def attr_group_type(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: GroupType: Group Type
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrGroupType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInstanceId")
     def attr_instance_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: InstanceId: Instance ID
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInstanceId"))
 
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
     @jsii.member(jsii_name="groupId")
     def group_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         groupId: The group ID of the consumption cluster. When creating a group ID, pay attention to the following aspects:
         A group ID starts with"GID_" or "GID-", and contains letters, numbers, hyphens (-), and underscores (_).
@@ -380,32 +417,38 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "groupId"))
 
     @group_id.setter
     def group_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosGroup, "group_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "groupId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="instanceId")
     def instance_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: instanceId: The ID of the instance.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "instanceId"))
 
     @instance_id.setter
     def instance_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosGroup, "instance_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "instanceId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="groupType")
     def group_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -416,31 +459,37 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "groupType"))
 
     @group_type.setter
     def group_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosGroup, "group_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "groupType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="remark")
     def remark(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: remark: The remarks on the request.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "remark"))
 
     @remark.setter
     def remark(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosGroup, "remark").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "remark", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-rocketmq.RosGroupProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -462,14 +511,20 @@
         '''Properties for defining a ``ALIYUN::ROCKETMQ::Group``.
 
         :param group_id: 
         :param instance_id: 
         :param group_type: 
         :param remark: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosGroupProps.__init__)
+            check_type(argname="argument group_id", value=group_id, expected_type=type_hints["group_id"])
+            check_type(argname="argument instance_id", value=instance_id, expected_type=type_hints["instance_id"])
+            check_type(argname="argument group_type", value=group_type, expected_type=type_hints["group_type"])
+            check_type(argname="argument remark", value=remark, expected_type=type_hints["remark"])
         self._values: typing.Dict[str, typing.Any] = {
             "group_id": group_id,
             "instance_id": instance_id,
         }
         if group_type is not None:
             self._values["group_type"] = group_type
         if remark is not None:
@@ -541,157 +596,178 @@
 ):
     '''A ROS template type:  ``ALIYUN::ROCKETMQ::Instance``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosInstanceProps",
+        props: typing.Union["RosInstanceProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::ROCKETMQ::Instance``.
 
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
     @jsii.member(jsii_name="attrHttpInternalEndpoint")
     def attr_http_internal_endpoint(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: HttpInternalEndpoint: The internal HTTP endpoint for the Message Queue for Apache RocketMQ instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrHttpInternalEndpoint"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrHttpInternetEndpoint")
     def attr_http_internet_endpoint(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: HttpInternetEndpoint: The Internet HTTP endpoint for the Message Queue for Apache RocketMQ instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrHttpInternetEndpoint"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrHttpInternetSecureEndpoint")
     def attr_http_internet_secure_endpoint(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: HttpInternetSecureEndpoint: The Internet HTTPS endpoint for the Message Queue for Apache RocketMQ instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrHttpInternetSecureEndpoint"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInstanceId")
     def attr_instance_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: InstanceId: Instance ID created
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInstanceId"))
 
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
     @jsii.member(jsii_name="attrInstanceType")
     def attr_instance_type(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: InstanceType: Instance Type
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInstanceType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTcpEndpoint")
     def attr_tcp_endpoint(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: TcpEndpoint: The TCP endpoint for the Message Queue for Apache RocketMQ instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTcpEndpoint"))
 
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
         :Property: instanceName: The name of the instance, which contains 3 to 64 characters in Chinese or English.
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
     @jsii.member(jsii_name="remark")
     def remark(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: remark: The remark of instance.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "remark"))
 
     @remark.setter
     def remark(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "remark").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "remark", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="tags")
     def tags(self) -> typing.Optional[typing.List["RosInstance.TagsProperty"]]:
         '''
         :Property: tags: Tags to attach to instance. Max support 20 tags to add during create instance. Each tag with two properties Key and Value, and Key is required.
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
         jsii_type="@alicloud/ros-cdk-rocketmq.RosInstance.TagsProperty",
         jsii_struct_bases=[],
         name_mapping={"key": "key", "value": "value"},
     )
@@ -702,14 +778,18 @@
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
@@ -750,22 +830,27 @@
 )
 class RosInstanceProps:
     def __init__(
         self,
         *,
         instance_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         remark: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        tags: typing.Optional[typing.Sequence[RosInstance.TagsProperty]] = None,
+        tags: typing.Optional[typing.Sequence[typing.Union[RosInstance.TagsProperty, typing.Dict[str, typing.Any]]]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::ROCKETMQ::Instance``.
 
         :param instance_name: 
         :param remark: 
         :param tags: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosInstanceProps.__init__)
+            check_type(argname="argument instance_name", value=instance_name, expected_type=type_hints["instance_name"])
+            check_type(argname="argument remark", value=remark, expected_type=type_hints["remark"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
         self._values: typing.Dict[str, typing.Any] = {
             "instance_name": instance_name,
         }
         if remark is not None:
             self._values["remark"] = remark
         if tags is not None:
             self._values["tags"] = tags
@@ -816,96 +901,111 @@
 ):
     '''A ROS template type:  ``ALIYUN::ROCKETMQ::Topic``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosTopicProps",
+        props: typing.Union["RosTopicProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::ROCKETMQ::Topic``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosTopic.__init__)
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
+            type_hints = typing.get_type_hints(RosTopic._render_properties)
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
     @jsii.member(jsii_name="attrInstanceId")
     def attr_instance_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: InstanceId: The ID of the instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInstanceId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrMessageType")
     def attr_message_type(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: MessageType: The type of the message.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrMessageType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTopic")
     def attr_topic(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Topic: The name of the topic.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTopic"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosTopic, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="instanceId")
     def instance_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: instanceId: The ID of the instance.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "instanceId"))
 
     @instance_id.setter
     def instance_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTopic, "instance_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "instanceId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="messageType")
     def message_type(self) -> typing.Union[jsii.Number, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         messageType: The type of the message. Valid values:
         0: normal message
@@ -917,17 +1017,20 @@
         return typing.cast(typing.Union[jsii.Number, ros_cdk_core.IResolvable], jsii.get(self, "messageType"))
 
     @message_type.setter
     def message_type(
         self,
         value: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTopic, "message_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "messageType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="topic")
     def topic(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         topic: The name of the topic you want to create.
         Note:
@@ -938,31 +1041,37 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "topic"))
 
     @topic.setter
     def topic(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTopic, "topic").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "topic", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="remark")
     def remark(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: remark: The remarks on the request. This parameter can be left blank.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "remark"))
 
     @remark.setter
     def remark(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTopic, "remark").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "remark", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-rocketmq.RosTopicProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -984,14 +1093,20 @@
         '''Properties for defining a ``ALIYUN::ROCKETMQ::Topic``.
 
         :param instance_id: 
         :param message_type: 
         :param topic: 
         :param remark: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosTopicProps.__init__)
+            check_type(argname="argument instance_id", value=instance_id, expected_type=type_hints["instance_id"])
+            check_type(argname="argument message_type", value=message_type, expected_type=type_hints["message_type"])
+            check_type(argname="argument topic", value=topic, expected_type=type_hints["topic"])
+            check_type(argname="argument remark", value=remark, expected_type=type_hints["remark"])
         self._values: typing.Dict[str, typing.Any] = {
             "instance_id": instance_id,
             "message_type": message_type,
             "topic": topic,
         }
         if remark is not None:
             self._values["remark"] = remark
@@ -1065,43 +1180,49 @@
 ):
     '''A ROS resource type:  ``ALIYUN::ROCKETMQ::Topic``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "TopicProps",
+        props: typing.Union["TopicProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::ROCKETMQ::Topic``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(Topic.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInstanceId")
     def attr_instance_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute InstanceId: The ID of the instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInstanceId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrMessageType")
     def attr_message_type(self) -> ros_cdk_core.IResolvable:
         '''Attribute MessageType: The type of the message.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrMessageType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTopic")
     def attr_topic(self) -> ros_cdk_core.IResolvable:
         '''Attribute Topic: The name of the topic.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTopic"))
 
 
 @jsii.data_type(
@@ -1126,14 +1247,20 @@
         '''Properties for defining a ``ALIYUN::ROCKETMQ::Topic``.
 
         :param instance_id: Property instanceId: The ID of the instance.
         :param message_type: Property messageType: The type of the message. Valid values: 0: normal message 1: partitionally ordered message 2: globally ordered message 4: transactional message 5: scheduled/delayed message
         :param topic: Property topic: The name of the topic you want to create. Note: "CID" and "GID" are the reserved fields of a group ID, and they cannot be the start of a topic name. If namespaces are available in the instance for which the topic is created, the topic name must be unique in the instance and can be duplicated across instances. If no namespaces are available in the instance, the topic name must be unique both in the instance and across instances.
         :param remark: Property remark: The remarks on the request. This parameter can be left blank.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(TopicProps.__init__)
+            check_type(argname="argument instance_id", value=instance_id, expected_type=type_hints["instance_id"])
+            check_type(argname="argument message_type", value=message_type, expected_type=type_hints["message_type"])
+            check_type(argname="argument topic", value=topic, expected_type=type_hints["topic"])
+            check_type(argname="argument remark", value=remark, expected_type=type_hints["remark"])
         self._values: typing.Dict[str, typing.Any] = {
             "instance_id": instance_id,
             "message_type": message_type,
             "topic": topic,
         }
         if remark is not None:
             self._values["remark"] = remark
```

### Comparing `ros-cdk-rocketmq-1.0.8/src/ros_cdk_rocketmq.egg-info/PKG-INFO` & `ros-cdk-rocketmq-1.0.9/src/ros_cdk_rocketmq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-rocketmq
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS ROCKETMQ Construct Library
```

