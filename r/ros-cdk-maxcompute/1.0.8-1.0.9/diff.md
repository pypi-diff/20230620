# Comparing `tmp/ros-cdk-maxcompute-1.0.8.tar.gz` & `tmp/ros-cdk-maxcompute-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-maxcompute-1.0.8.tar", last modified: Thu Jul 14 02:16:41 2022, max compression
+gzip compressed data, was "dist/ros-cdk-maxcompute-1.0.9.tar", last modified: Fri Sep 23 11:16:17 2022, max compression
```

## Comparing `ros-cdk-maxcompute-1.0.8.tar` & `ros-cdk-maxcompute-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:16:41.000000 ros-cdk-maxcompute-1.0.8/
--rw-r--r--   0 root         (0) root         (0)    10279 2022-07-14 02:16:41.000000 ros-cdk-maxcompute-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2022-07-14 02:16:41.000000 ros-cdk-maxcompute-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2022-07-14 02:16:41.000000 ros-cdk-maxcompute-1.0.8/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1268 2022-07-14 02:16:41.000000 ros-cdk-maxcompute-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      200 2022-07-14 02:16:41.000000 ros-cdk-maxcompute-1.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)      106 2022-07-14 02:16:41.000000 ros-cdk-maxcompute-1.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-07-14 02:16:41.000000 ros-cdk-maxcompute-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1836 2022-07-14 02:16:41.000000 ros-cdk-maxcompute-1.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:16:41.000000 ros-cdk-maxcompute-1.0.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:16:41.000000 ros-cdk-maxcompute-1.0.8/src/ros_cdk_maxcompute/
--rw-r--r--   0 root         (0) root         (0)    28609 2022-07-14 02:16:41.000000 ros-cdk-maxcompute-1.0.8/src/ros_cdk_maxcompute/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:16:41.000000 ros-cdk-maxcompute-1.0.8/src/ros_cdk_maxcompute/_jsii/
--rw-r--r--   0 root         (0) root         (0)      397 2022-07-14 02:16:41.000000 ros-cdk-maxcompute-1.0.8/src/ros_cdk_maxcompute/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    34683 2022-07-14 02:16:41.000000 ros-cdk-maxcompute-1.0.8/src/ros_cdk_maxcompute/_jsii/ros-cdk-maxcompute@1.0.8.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:16:41.000000 ros-cdk-maxcompute-1.0.8/src/ros_cdk_maxcompute/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:16:41.000000 ros-cdk-maxcompute-1.0.8/src/ros_cdk_maxcompute.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1268 2022-07-14 02:16:41.000000 ros-cdk-maxcompute-1.0.8/src/ros_cdk_maxcompute.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      470 2022-07-14 02:16:41.000000 ros-cdk-maxcompute-1.0.8/src/ros_cdk_maxcompute.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:16:41.000000 ros-cdk-maxcompute-1.0.8/src/ros_cdk_maxcompute.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2022-07-14 02:16:41.000000 ros-cdk-maxcompute-1.0.8/src/ros_cdk_maxcompute.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2022-07-14 02:16:41.000000 ros-cdk-maxcompute-1.0.8/src/ros_cdk_maxcompute.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:16:17.000000 ros-cdk-maxcompute-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)    10279 2022-09-23 11:16:17.000000 ros-cdk-maxcompute-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-09-23 11:16:17.000000 ros-cdk-maxcompute-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2022-09-23 11:16:17.000000 ros-cdk-maxcompute-1.0.9/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1268 2022-09-23 11:16:17.000000 ros-cdk-maxcompute-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      200 2022-09-23 11:16:17.000000 ros-cdk-maxcompute-1.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      236 2022-09-23 11:16:17.000000 ros-cdk-maxcompute-1.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-09-23 11:16:17.000000 ros-cdk-maxcompute-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1865 2022-09-23 11:16:17.000000 ros-cdk-maxcompute-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:16:17.000000 ros-cdk-maxcompute-1.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:16:17.000000 ros-cdk-maxcompute-1.0.9/src/ros_cdk_maxcompute/
+-rw-r--r--   0 root         (0) root         (0)    34417 2022-09-23 11:16:17.000000 ros-cdk-maxcompute-1.0.9/src/ros_cdk_maxcompute/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:16:17.000000 ros-cdk-maxcompute-1.0.9/src/ros_cdk_maxcompute/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      431 2022-09-23 11:16:17.000000 ros-cdk-maxcompute-1.0.9/src/ros_cdk_maxcompute/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    34750 2022-09-23 11:16:17.000000 ros-cdk-maxcompute-1.0.9/src/ros_cdk_maxcompute/_jsii/ros-cdk-maxcompute@1.0.9.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 11:16:17.000000 ros-cdk-maxcompute-1.0.9/src/ros_cdk_maxcompute/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:16:17.000000 ros-cdk-maxcompute-1.0.9/src/ros_cdk_maxcompute.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1268 2022-09-23 11:16:17.000000 ros-cdk-maxcompute-1.0.9/src/ros_cdk_maxcompute.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      470 2022-09-23 11:16:17.000000 ros-cdk-maxcompute-1.0.9/src/ros_cdk_maxcompute.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 11:16:17.000000 ros-cdk-maxcompute-1.0.9/src/ros_cdk_maxcompute.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2022-09-23 11:16:17.000000 ros-cdk-maxcompute-1.0.9/src/ros_cdk_maxcompute.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2022-09-23 11:16:17.000000 ros-cdk-maxcompute-1.0.9/src/ros_cdk_maxcompute.egg-info/top_level.txt
```

### Comparing `ros-cdk-maxcompute-1.0.8/LICENSE` & `ros-cdk-maxcompute-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-maxcompute-1.0.8/PKG-INFO` & `ros-cdk-maxcompute-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-maxcompute
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS MAXCOMPUTE Construct Library
```

### Comparing `ros-cdk-maxcompute-1.0.8/setup.py` & `ros-cdk-maxcompute-1.0.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-maxcompute",
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
         "ros_cdk_maxcompute",
         "ros_cdk_maxcompute._jsii"
     ],
     "package_data": {
         "ros_cdk_maxcompute._jsii": [
-            "ros-cdk-maxcompute@1.0.8.jsii.tgz"
+            "ros-cdk-maxcompute@1.0.9.jsii.tgz"
         ],
         "ros_cdk_maxcompute": [
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

### Comparing `ros-cdk-maxcompute-1.0.8/src/ros_cdk_maxcompute/__init__.py` & `ros-cdk-maxcompute-1.0.9/src/ros_cdk_maxcompute/__init__.py`

 * *Files 21% similar despite different names*

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
 
 
 class RosTable(
     ros_cdk_core.RosResource,
@@ -29,117 +31,138 @@
 ):
     '''A ROS template type:  ``ALIYUN::MaxCompute::Table``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosTableProps",
+        props: typing.Union["RosTableProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::MaxCompute::Table``.
 
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
     @jsii.member(jsii_name="attrName")
     def attr_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Name: Table name
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrProject")
     def attr_project(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Project: Project name
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrProject"))
 
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
     @jsii.member(jsii_name="name")
     def name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: name: Table name
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "name"))
 
     @name.setter
     def name(self, value: typing.Union[builtins.str, ros_cdk_core.IResolvable]) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTable, "name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "name", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="project")
     def project(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: project: Project name, if not provided, will be the default project
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "project"))
 
     @project.setter
     def project(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTable, "project").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "project", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="comment")
     def comment(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: comment: Table comment
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "comment"))
 
     @comment.setter
     def comment(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTable, "comment").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "comment", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="ifNotExists")
     def if_not_exists(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -155,51 +178,60 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "ifNotExists"))
 
     @if_not_exists.setter
     def if_not_exists(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTable, "if_not_exists").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "ifNotExists", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="lifecycle")
     def lifecycle(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: lifecycle: Table's lifecycle.
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "lifecycle"))
 
     @lifecycle.setter
     def lifecycle(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTable, "lifecycle").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "lifecycle", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="schema")
     def schema(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosTable.SchemaProperty"]]:
         '''
         :Property: schema: Table schema
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosTable.SchemaProperty"]], jsii.get(self, "schema"))
 
     @schema.setter
     def schema(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosTable.SchemaProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTable, "schema").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "schema", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="stringSchema")
     def string_schema(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -209,14 +241,17 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "stringSchema"))
 
     @string_schema.setter
     def string_schema(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTable, "string_schema").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "stringSchema", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-maxcompute.RosTable.ColumnsProperty",
         jsii_struct_bases=[],
         name_mapping={"name": "name", "type": "type", "comment": "comment"},
     )
@@ -229,14 +264,19 @@
             comment: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param name: 
             :param type: 
             :param comment: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosTable.ColumnsProperty.__init__)
+                check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+                check_type(argname="argument type", value=type, expected_type=type_hints["type"])
+                check_type(argname="argument comment", value=comment, expected_type=type_hints["comment"])
             self._values: typing.Dict[str, typing.Any] = {
                 "name": name,
                 "type": type,
             }
             if comment is not None:
                 self._values["comment"] = comment
 
@@ -293,14 +333,19 @@
             comment: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param name: 
             :param type: 
             :param comment: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosTable.PartitionsProperty.__init__)
+                check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+                check_type(argname="argument type", value=type, expected_type=type_hints["type"])
+                check_type(argname="argument comment", value=comment, expected_type=type_hints["comment"])
             self._values: typing.Dict[str, typing.Any] = {
                 "name": name,
                 "type": type,
             }
             if comment is not None:
                 self._values["comment"] = comment
 
@@ -348,21 +393,25 @@
         jsii_struct_bases=[],
         name_mapping={"columns": "columns", "partitions": "partitions"},
     )
     class SchemaProperty:
         def __init__(
             self,
             *,
-            columns: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosTable.ColumnsProperty"]]],
-            partitions: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosTable.PartitionsProperty"]]]] = None,
+            columns: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosTable.ColumnsProperty", typing.Dict[str, typing.Any]]]]],
+            partitions: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosTable.PartitionsProperty", typing.Dict[str, typing.Any]]]]]] = None,
         ) -> None:
             '''
             :param columns: 
             :param partitions: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosTable.SchemaProperty.__init__)
+                check_type(argname="argument columns", value=columns, expected_type=type_hints["columns"])
+                check_type(argname="argument partitions", value=partitions, expected_type=type_hints["partitions"])
             self._values: typing.Dict[str, typing.Any] = {
                 "columns": columns,
             }
             if partitions is not None:
                 self._values["partitions"] = partitions
 
         @builtins.property
@@ -416,27 +465,36 @@
         self,
         *,
         name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         project: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         comment: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         if_not_exists: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         lifecycle: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
-        schema: typing.Optional[typing.Union[ros_cdk_core.IResolvable, RosTable.SchemaProperty]] = None,
+        schema: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosTable.SchemaProperty, typing.Dict[str, typing.Any]]]] = None,
         string_schema: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::MaxCompute::Table``.
 
         :param name: 
         :param project: 
         :param comment: 
         :param if_not_exists: 
         :param lifecycle: 
         :param schema: 
         :param string_schema: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosTableProps.__init__)
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+            check_type(argname="argument project", value=project, expected_type=type_hints["project"])
+            check_type(argname="argument comment", value=comment, expected_type=type_hints["comment"])
+            check_type(argname="argument if_not_exists", value=if_not_exists, expected_type=type_hints["if_not_exists"])
+            check_type(argname="argument lifecycle", value=lifecycle, expected_type=type_hints["lifecycle"])
+            check_type(argname="argument schema", value=schema, expected_type=type_hints["schema"])
+            check_type(argname="argument string_schema", value=string_schema, expected_type=type_hints["string_schema"])
         self._values: typing.Dict[str, typing.Any] = {
             "name": name,
             "project": project,
         }
         if comment is not None:
             self._values["comment"] = comment
         if if_not_exists is not None:
@@ -547,37 +605,43 @@
 ):
     '''A ROS resource type:  ``ALIYUN::MaxCompute::Table``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "TableProps",
+        props: typing.Union["TableProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::MaxCompute::Table``.
 
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
     @jsii.member(jsii_name="attrName")
     def attr_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute Name: Table name.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrProject")
     def attr_project(self) -> ros_cdk_core.IResolvable:
         '''Attribute Project: Project name.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrProject"))
 
 
 @jsii.data_type(
@@ -598,27 +662,36 @@
         self,
         *,
         name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         project: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         comment: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         if_not_exists: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         lifecycle: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
-        schema: typing.Optional[typing.Union[ros_cdk_core.IResolvable, RosTable.SchemaProperty]] = None,
+        schema: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosTable.SchemaProperty, typing.Dict[str, typing.Any]]]] = None,
         string_schema: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::MaxCompute::Table``.
 
         :param name: Property name: Table name.
         :param project: Property project: Project name, if not provided, will be the default project.
         :param comment: Property comment: Table comment.
         :param if_not_exists: Property ifNotExists: If you create a table by using the name of an existing table and the parameter set to false, an error is returned. If you specify the if not exists parameter, a success message is returned when you create a table by using the name of an existing table. The success message is returned even if the schema of the existing table is different from that of the table you want to create. If you create a table by using the name of an existing table, the table is not created and the metadata of the existing table is not changed.
         :param lifecycle: Property lifecycle: Table's lifecycle.
         :param schema: Property schema: Table schema.
         :param string_schema: Property stringSchema: Create a table with field names and field type strings. Example: 'num bigint, num2 double', 'pt string'
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(TableProps.__init__)
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+            check_type(argname="argument project", value=project, expected_type=type_hints["project"])
+            check_type(argname="argument comment", value=comment, expected_type=type_hints["comment"])
+            check_type(argname="argument if_not_exists", value=if_not_exists, expected_type=type_hints["if_not_exists"])
+            check_type(argname="argument lifecycle", value=lifecycle, expected_type=type_hints["lifecycle"])
+            check_type(argname="argument schema", value=schema, expected_type=type_hints["schema"])
+            check_type(argname="argument string_schema", value=string_schema, expected_type=type_hints["string_schema"])
         self._values: typing.Dict[str, typing.Any] = {
             "name": name,
             "project": project,
         }
         if comment is not None:
             self._values["comment"] = comment
         if if_not_exists is not None:
```

### Comparing `ros-cdk-maxcompute-1.0.8/src/ros_cdk_maxcompute.egg-info/PKG-INFO` & `ros-cdk-maxcompute-1.0.9/src/ros_cdk_maxcompute.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-maxcompute
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS MAXCOMPUTE Construct Library
```

