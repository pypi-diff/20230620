# Comparing `tmp/ros-cdk-fnf-1.0.8.tar.gz` & `tmp/ros-cdk-fnf-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-fnf-1.0.8.tar", last modified: Thu Jul 14 02:21:13 2022, max compression
+gzip compressed data, was "dist/ros-cdk-fnf-1.0.9.tar", last modified: Fri Sep 23 11:07:08 2022, max compression
```

## Comparing `ros-cdk-fnf-1.0.8.tar` & `ros-cdk-fnf-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:21:13.000000 ros-cdk-fnf-1.0.8/
--rw-r--r--   0 root         (0) root         (0)    10279 2022-07-14 02:21:13.000000 ros-cdk-fnf-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2022-07-14 02:21:13.000000 ros-cdk-fnf-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2022-07-14 02:21:13.000000 ros-cdk-fnf-1.0.8/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1240 2022-07-14 02:21:13.000000 ros-cdk-fnf-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      179 2022-07-14 02:21:13.000000 ros-cdk-fnf-1.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)      106 2022-07-14 02:21:13.000000 ros-cdk-fnf-1.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-07-14 02:21:13.000000 ros-cdk-fnf-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1794 2022-07-14 02:21:13.000000 ros-cdk-fnf-1.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:21:13.000000 ros-cdk-fnf-1.0.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:21:13.000000 ros-cdk-fnf-1.0.8/src/ros_cdk_fnf/
--rw-r--r--   0 root         (0) root         (0)    34427 2022-07-14 02:21:13.000000 ros-cdk-fnf-1.0.8/src/ros_cdk_fnf/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:21:13.000000 ros-cdk-fnf-1.0.8/src/ros_cdk_fnf/_jsii/
--rw-r--r--   0 root         (0) root         (0)      370 2022-07-14 02:21:13.000000 ros-cdk-fnf-1.0.8/src/ros_cdk_fnf/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    35660 2022-07-14 02:21:13.000000 ros-cdk-fnf-1.0.8/src/ros_cdk_fnf/_jsii/ros-cdk-fnf@1.0.8.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:21:13.000000 ros-cdk-fnf-1.0.8/src/ros_cdk_fnf/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:21:13.000000 ros-cdk-fnf-1.0.8/src/ros_cdk_fnf.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1240 2022-07-14 02:21:13.000000 ros-cdk-fnf-1.0.8/src/ros_cdk_fnf.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      400 2022-07-14 02:21:13.000000 ros-cdk-fnf-1.0.8/src/ros_cdk_fnf.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:21:13.000000 ros-cdk-fnf-1.0.8/src/ros_cdk_fnf.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2022-07-14 02:21:13.000000 ros-cdk-fnf-1.0.8/src/ros_cdk_fnf.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2022-07-14 02:21:13.000000 ros-cdk-fnf-1.0.8/src/ros_cdk_fnf.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:07:08.000000 ros-cdk-fnf-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)    10279 2022-09-23 11:07:07.000000 ros-cdk-fnf-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-09-23 11:07:07.000000 ros-cdk-fnf-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2022-09-23 11:07:07.000000 ros-cdk-fnf-1.0.9/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1240 2022-09-23 11:07:08.000000 ros-cdk-fnf-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      179 2022-09-23 11:07:07.000000 ros-cdk-fnf-1.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      236 2022-09-23 11:07:07.000000 ros-cdk-fnf-1.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-09-23 11:07:08.000000 ros-cdk-fnf-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1823 2022-09-23 11:07:07.000000 ros-cdk-fnf-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:07:08.000000 ros-cdk-fnf-1.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:07:08.000000 ros-cdk-fnf-1.0.9/src/ros_cdk_fnf/
+-rw-r--r--   0 root         (0) root         (0)    42113 2022-09-23 11:07:07.000000 ros-cdk-fnf-1.0.9/src/ros_cdk_fnf/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:07:08.000000 ros-cdk-fnf-1.0.9/src/ros_cdk_fnf/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      404 2022-09-23 11:07:07.000000 ros-cdk-fnf-1.0.9/src/ros_cdk_fnf/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    35727 2022-09-23 11:07:07.000000 ros-cdk-fnf-1.0.9/src/ros_cdk_fnf/_jsii/ros-cdk-fnf@1.0.9.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 11:07:07.000000 ros-cdk-fnf-1.0.9/src/ros_cdk_fnf/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:07:08.000000 ros-cdk-fnf-1.0.9/src/ros_cdk_fnf.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1240 2022-09-23 11:07:07.000000 ros-cdk-fnf-1.0.9/src/ros_cdk_fnf.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      400 2022-09-23 11:07:07.000000 ros-cdk-fnf-1.0.9/src/ros_cdk_fnf.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 11:07:07.000000 ros-cdk-fnf-1.0.9/src/ros_cdk_fnf.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2022-09-23 11:07:07.000000 ros-cdk-fnf-1.0.9/src/ros_cdk_fnf.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2022-09-23 11:07:07.000000 ros-cdk-fnf-1.0.9/src/ros_cdk_fnf.egg-info/top_level.txt
```

### Comparing `ros-cdk-fnf-1.0.8/LICENSE` & `ros-cdk-fnf-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-fnf-1.0.8/PKG-INFO` & `ros-cdk-fnf-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-fnf
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS FNF Construct Library
```

### Comparing `ros-cdk-fnf-1.0.8/setup.py` & `ros-cdk-fnf-1.0.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-fnf",
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
         "ros_cdk_fnf",
         "ros_cdk_fnf._jsii"
     ],
     "package_data": {
         "ros_cdk_fnf._jsii": [
-            "ros-cdk-fnf@1.0.8.jsii.tgz"
+            "ros-cdk-fnf@1.0.9.jsii.tgz"
         ],
         "ros_cdk_fnf": [
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

### Comparing `ros-cdk-fnf-1.0.8/src/ros_cdk_fnf/__init__.py` & `ros-cdk-fnf-1.0.9/src/ros_cdk_fnf/__init__.py`

 * *Files 16% similar despite different names*

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
 
 
 class Flow(
     ros_cdk_core.Resource,
@@ -29,49 +31,55 @@
 ):
     '''A ROS resource type:  ``ALIYUN::FNF::Flow``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "FlowProps",
+        props: typing.Union["FlowProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::FNF::Flow``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(Flow.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrCreatedTime")
     def attr_created_time(self) -> ros_cdk_core.IResolvable:
         '''Attribute CreatedTime: Flow creation time.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrCreatedTime"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrId")
     def attr_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute Id: The unique ID of the flow.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrLastModifiedTime")
     def attr_last_modified_time(self) -> ros_cdk_core.IResolvable:
         '''Attribute LastModifiedTime: The most recently modified time of the flow.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrLastModifiedTime"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrName")
     def attr_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute Name: The name of the flow created.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrName"))
 
 
 @jsii.data_type(
@@ -99,14 +107,21 @@
 
         :param definition: Property definition: The definition of the created flow following the FDL syntax standard.
         :param name: Property name: The name of the flow created. This name is unique under the account.
         :param description: Property description: Create a description of the flow.
         :param request_id: Property requestId: The specified Request ID for this request. If not specified, our system will help you generate a random one.
         :param role_arn: Property roleArn: Optional parameter, the resource descriptor information required for the execution of the flow, used to perform the assume role during FnF execution.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(FlowProps.__init__)
+            check_type(argname="argument definition", value=definition, expected_type=type_hints["definition"])
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument request_id", value=request_id, expected_type=type_hints["request_id"])
+            check_type(argname="argument role_arn", value=role_arn, expected_type=type_hints["role_arn"])
         self._values: typing.Dict[str, typing.Any] = {
             "definition": definition,
             "name": name,
         }
         if description is not None:
             self._values["description"] = description
         if request_id is not None:
@@ -177,164 +192,191 @@
 ):
     '''A ROS template type:  ``ALIYUN::FNF::Flow``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosFlowProps",
+        props: typing.Union["RosFlowProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::FNF::Flow``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosFlow.__init__)
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
+            type_hints = typing.get_type_hints(RosFlow._render_properties)
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
     @jsii.member(jsii_name="attrCreatedTime")
     def attr_created_time(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: CreatedTime: Flow creation time.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrCreatedTime"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrId")
     def attr_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Id: The unique ID of the flow.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrLastModifiedTime")
     def attr_last_modified_time(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: LastModifiedTime: The most recently modified time of the flow.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrLastModifiedTime"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrName")
     def attr_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Name: The name of the flow created.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="definition")
     def definition(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: definition: The definition of the created flow following the FDL syntax standard.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "definition"))
 
     @definition.setter
     def definition(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosFlow, "definition").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "definition", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosFlow, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="name")
     def name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: name: The name of the flow created. This name is unique under the account.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "name"))
 
     @name.setter
     def name(self, value: typing.Union[builtins.str, ros_cdk_core.IResolvable]) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosFlow, "name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "name", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="description")
     def description(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: description: Create a description of the flow.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "description"))
 
     @description.setter
     def description(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosFlow, "description").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "description", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="requestId")
     def request_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: requestId: The specified Request ID for this request. If not specified, our system will help you generate a random one.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "requestId"))
 
     @request_id.setter
     def request_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosFlow, "request_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "requestId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="roleArn")
     def role_arn(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: roleArn: Optional parameter, the resource descriptor information required for the execution of the flow, used to perform the assume role during FnF execution.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "roleArn"))
 
     @role_arn.setter
     def role_arn(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosFlow, "role_arn").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "roleArn", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-fnf.RosFlowProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -359,14 +401,21 @@
 
         :param definition: 
         :param name: 
         :param description: 
         :param request_id: 
         :param role_arn: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosFlowProps.__init__)
+            check_type(argname="argument definition", value=definition, expected_type=type_hints["definition"])
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument request_id", value=request_id, expected_type=type_hints["request_id"])
+            check_type(argname="argument role_arn", value=role_arn, expected_type=type_hints["role_arn"])
         self._values: typing.Dict[str, typing.Any] = {
             "definition": definition,
             "name": name,
         }
         if description is not None:
             self._values["description"] = description
         if request_id is not None:
@@ -441,174 +490,204 @@
 ):
     '''A ROS template type:  ``ALIYUN::FNF::Schedule``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosScheduleProps",
+        props: typing.Union["RosScheduleProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::FNF::Schedule``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosSchedule.__init__)
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
+            type_hints = typing.get_type_hints(RosSchedule._render_properties)
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
     @jsii.member(jsii_name="attrFlowName")
     def attr_flow_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: FlowName: Flow name.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrFlowName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrScheduleId")
     def attr_schedule_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ScheduleId: Schedule Id
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrScheduleId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrScheduleName")
     def attr_schedule_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ScheduleName: Schedule name.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrScheduleName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="cronExpression")
     def cron_expression(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: cronExpression: Cron expression.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "cronExpression"))
 
     @cron_expression.setter
     def cron_expression(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSchedule, "cron_expression").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "cronExpression", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSchedule, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="flowName")
     def flow_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: flowName: Flow name.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "flowName"))
 
     @flow_name.setter
     def flow_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSchedule, "flow_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "flowName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="scheduleName")
     def schedule_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: scheduleName: Schedule name.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "scheduleName"))
 
     @schedule_name.setter
     def schedule_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSchedule, "schedule_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "scheduleName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="description")
     def description(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: description: Description of the schedule.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "description"))
 
     @description.setter
     def description(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSchedule, "description").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "description", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enable")
     def enable(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property: enable: Whether enable schedule.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "enable"))
 
     @enable.setter
     def enable(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSchedule, "enable").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enable", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="payload")
     def payload(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: payload: Payload.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "payload"))
 
     @payload.setter
     def payload(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSchedule, "payload").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "payload", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-fnf.RosScheduleProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -636,14 +715,22 @@
         :param cron_expression: 
         :param flow_name: 
         :param schedule_name: 
         :param description: 
         :param enable: 
         :param payload: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosScheduleProps.__init__)
+            check_type(argname="argument cron_expression", value=cron_expression, expected_type=type_hints["cron_expression"])
+            check_type(argname="argument flow_name", value=flow_name, expected_type=type_hints["flow_name"])
+            check_type(argname="argument schedule_name", value=schedule_name, expected_type=type_hints["schedule_name"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument enable", value=enable, expected_type=type_hints["enable"])
+            check_type(argname="argument payload", value=payload, expected_type=type_hints["payload"])
         self._values: typing.Dict[str, typing.Any] = {
             "cron_expression": cron_expression,
             "flow_name": flow_name,
             "schedule_name": schedule_name,
         }
         if description is not None:
             self._values["description"] = description
@@ -728,43 +815,49 @@
 ):
     '''A ROS resource type:  ``ALIYUN::FNF::Schedule``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "ScheduleProps",
+        props: typing.Union["ScheduleProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::FNF::Schedule``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(Schedule.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrFlowName")
     def attr_flow_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute FlowName: Flow name.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrFlowName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrScheduleId")
     def attr_schedule_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute ScheduleId: Schedule Id.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrScheduleId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrScheduleName")
     def attr_schedule_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute ScheduleName: Schedule name.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrScheduleName"))
 
 
 @jsii.data_type(
@@ -795,14 +888,22 @@
         :param cron_expression: Property cronExpression: Cron expression.
         :param flow_name: Property flowName: Flow name.
         :param schedule_name: Property scheduleName: Schedule name.
         :param description: Property description: Description of the schedule.
         :param enable: Property enable: Whether enable schedule.
         :param payload: Property payload: Payload.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(ScheduleProps.__init__)
+            check_type(argname="argument cron_expression", value=cron_expression, expected_type=type_hints["cron_expression"])
+            check_type(argname="argument flow_name", value=flow_name, expected_type=type_hints["flow_name"])
+            check_type(argname="argument schedule_name", value=schedule_name, expected_type=type_hints["schedule_name"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument enable", value=enable, expected_type=type_hints["enable"])
+            check_type(argname="argument payload", value=payload, expected_type=type_hints["payload"])
         self._values: typing.Dict[str, typing.Any] = {
             "cron_expression": cron_expression,
             "flow_name": flow_name,
             "schedule_name": schedule_name,
         }
         if description is not None:
             self._values["description"] = description
```

### Comparing `ros-cdk-fnf-1.0.8/src/ros_cdk_fnf.egg-info/PKG-INFO` & `ros-cdk-fnf-1.0.9/src/ros_cdk_fnf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-fnf
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS FNF Construct Library
```

