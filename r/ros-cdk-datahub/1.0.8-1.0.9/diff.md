# Comparing `tmp/ros-cdk-datahub-1.0.8.tar.gz` & `tmp/ros-cdk-datahub-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-datahub-1.0.8.tar", last modified: Thu Jul 14 02:15:51 2022, max compression
+gzip compressed data, was "dist/ros-cdk-datahub-1.0.9.tar", last modified: Fri Sep 23 12:20:06 2022, max compression
```

## Comparing `ros-cdk-datahub-1.0.8.tar` & `ros-cdk-datahub-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:15:51.000000 ros-cdk-datahub-1.0.8/
--rw-r--r--   0 root         (0) root         (0)    10279 2022-07-14 02:15:51.000000 ros-cdk-datahub-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2022-07-14 02:15:51.000000 ros-cdk-datahub-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2022-07-14 02:15:51.000000 ros-cdk-datahub-1.0.8/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1256 2022-07-14 02:15:51.000000 ros-cdk-datahub-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      191 2022-07-14 02:15:51.000000 ros-cdk-datahub-1.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)      106 2022-07-14 02:15:51.000000 ros-cdk-datahub-1.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-07-14 02:15:51.000000 ros-cdk-datahub-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1818 2022-07-14 02:15:51.000000 ros-cdk-datahub-1.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:15:51.000000 ros-cdk-datahub-1.0.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:15:51.000000 ros-cdk-datahub-1.0.8/src/ros_cdk_datahub/
--rw-r--r--   0 root         (0) root         (0)    28830 2022-07-14 02:15:51.000000 ros-cdk-datahub-1.0.8/src/ros_cdk_datahub/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:15:51.000000 ros-cdk-datahub-1.0.8/src/ros_cdk_datahub/_jsii/
--rw-r--r--   0 root         (0) root         (0)      391 2022-07-14 02:15:51.000000 ros-cdk-datahub-1.0.8/src/ros_cdk_datahub/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    35117 2022-07-14 02:15:51.000000 ros-cdk-datahub-1.0.8/src/ros_cdk_datahub/_jsii/ros-cdk-datahub@1.0.8.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:15:51.000000 ros-cdk-datahub-1.0.8/src/ros_cdk_datahub/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:15:51.000000 ros-cdk-datahub-1.0.8/src/ros_cdk_datahub.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1256 2022-07-14 02:15:51.000000 ros-cdk-datahub-1.0.8/src/ros_cdk_datahub.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      440 2022-07-14 02:15:51.000000 ros-cdk-datahub-1.0.8/src/ros_cdk_datahub.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:15:51.000000 ros-cdk-datahub-1.0.8/src/ros_cdk_datahub.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2022-07-14 02:15:51.000000 ros-cdk-datahub-1.0.8/src/ros_cdk_datahub.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2022-07-14 02:15:51.000000 ros-cdk-datahub-1.0.8/src/ros_cdk_datahub.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:20:06.000000 ros-cdk-datahub-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)    10279 2022-09-23 12:20:06.000000 ros-cdk-datahub-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-09-23 12:20:06.000000 ros-cdk-datahub-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2022-09-23 12:20:06.000000 ros-cdk-datahub-1.0.9/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1256 2022-09-23 12:20:06.000000 ros-cdk-datahub-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      191 2022-09-23 12:20:06.000000 ros-cdk-datahub-1.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      236 2022-09-23 12:20:06.000000 ros-cdk-datahub-1.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-09-23 12:20:06.000000 ros-cdk-datahub-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1847 2022-09-23 12:20:06.000000 ros-cdk-datahub-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:20:06.000000 ros-cdk-datahub-1.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:20:06.000000 ros-cdk-datahub-1.0.9/src/ros_cdk_datahub/
+-rw-r--r--   0 root         (0) root         (0)    35917 2022-09-23 12:20:06.000000 ros-cdk-datahub-1.0.9/src/ros_cdk_datahub/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:20:06.000000 ros-cdk-datahub-1.0.9/src/ros_cdk_datahub/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      425 2022-09-23 12:20:06.000000 ros-cdk-datahub-1.0.9/src/ros_cdk_datahub/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    35189 2022-09-23 12:20:06.000000 ros-cdk-datahub-1.0.9/src/ros_cdk_datahub/_jsii/ros-cdk-datahub@1.0.9.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 12:20:06.000000 ros-cdk-datahub-1.0.9/src/ros_cdk_datahub/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:20:06.000000 ros-cdk-datahub-1.0.9/src/ros_cdk_datahub.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1256 2022-09-23 12:20:06.000000 ros-cdk-datahub-1.0.9/src/ros_cdk_datahub.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      440 2022-09-23 12:20:06.000000 ros-cdk-datahub-1.0.9/src/ros_cdk_datahub.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 12:20:06.000000 ros-cdk-datahub-1.0.9/src/ros_cdk_datahub.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2022-09-23 12:20:06.000000 ros-cdk-datahub-1.0.9/src/ros_cdk_datahub.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2022-09-23 12:20:06.000000 ros-cdk-datahub-1.0.9/src/ros_cdk_datahub.egg-info/top_level.txt
```

### Comparing `ros-cdk-datahub-1.0.8/LICENSE` & `ros-cdk-datahub-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-datahub-1.0.8/PKG-INFO` & `ros-cdk-datahub-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-datahub
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS DATAHUB Construct Library
```

### Comparing `ros-cdk-datahub-1.0.8/setup.py` & `ros-cdk-datahub-1.0.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-datahub",
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
         "ros_cdk_datahub",
         "ros_cdk_datahub._jsii"
     ],
     "package_data": {
         "ros_cdk_datahub._jsii": [
-            "ros-cdk-datahub@1.0.8.jsii.tgz"
+            "ros-cdk-datahub@1.0.9.jsii.tgz"
         ],
         "ros_cdk_datahub": [
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

### Comparing `ros-cdk-datahub-1.0.8/src/ros_cdk_datahub/__init__.py` & `ros-cdk-datahub-1.0.9/src/ros_cdk_datahub/__init__.py`

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
 
 
 class Project(
     ros_cdk_core.Resource,
@@ -29,31 +31,37 @@
 ):
     '''A ROS resource type:  ``ALIYUN::DATAHUB::Project``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "ProjectProps",
+        props: typing.Union["ProjectProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::DATAHUB::Project``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(Project.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrProjectName")
     def attr_project_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute ProjectName: Project name.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrProjectName"))
 
 
 @jsii.data_type(
@@ -69,14 +77,18 @@
         project_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
         '''Properties for defining a ``ALIYUN::DATAHUB::Project``.
 
         :param comment: Property comment: The comment of project.
         :param project_name: Property projectName: The name of the project. Length [3, 32]. Beginning with characters, only characters, numbers and _ are allowed.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(ProjectProps.__init__)
+            check_type(argname="argument comment", value=comment, expected_type=type_hints["comment"])
+            check_type(argname="argument project_name", value=project_name, expected_type=type_hints["project_name"])
         self._values: typing.Dict[str, typing.Any] = {
             "comment": comment,
             "project_name": project_name,
         }
 
     @builtins.property
     def comment(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
@@ -114,92 +126,110 @@
 ):
     '''A ROS template type:  ``ALIYUN::DATAHUB::Project``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosProjectProps",
+        props: typing.Union["RosProjectProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::DATAHUB::Project``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosProject.__init__)
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
+            type_hints = typing.get_type_hints(RosProject._render_properties)
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
     @jsii.member(jsii_name="attrProjectName")
     def attr_project_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ProjectName: Project name
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrProjectName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="comment")
     def comment(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: comment: The comment of project.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "comment"))
 
     @comment.setter
     def comment(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosProject, "comment").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "comment", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosProject, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="projectName")
     def project_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: projectName: The name of the project. Length [3, 32]. Beginning with characters, only characters, numbers and _ are allowed.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "projectName"))
 
     @project_name.setter
     def project_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosProject, "project_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "projectName", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-datahub.RosProjectProps",
     jsii_struct_bases=[],
     name_mapping={"comment": "comment", "project_name": "projectName"},
@@ -212,14 +242,18 @@
         project_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
         '''Properties for defining a ``ALIYUN::DATAHUB::Project``.
 
         :param comment: 
         :param project_name: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosProjectProps.__init__)
+            check_type(argname="argument comment", value=comment, expected_type=type_hints["comment"])
+            check_type(argname="argument project_name", value=project_name, expected_type=type_hints["project_name"])
         self._values: typing.Dict[str, typing.Any] = {
             "comment": comment,
             "project_name": project_name,
         }
 
     @builtins.property
     def comment(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
@@ -258,181 +292,214 @@
 ):
     '''A ROS template type:  ``ALIYUN::DATAHUB::Topic``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosTopicProps",
+        props: typing.Union["RosTopicProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::DATAHUB::Topic``.
 
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
     @jsii.member(jsii_name="attrProjectName")
     def attr_project_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ProjectName: Project name
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrProjectName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTopicName")
     def attr_topic_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: TopicName: Topic name
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTopicName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="comment")
     def comment(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: comment: The comment of topic.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "comment"))
 
     @comment.setter
     def comment(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTopic, "comment").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "comment", value)
 
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
     @jsii.member(jsii_name="projectName")
     def project_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: projectName: The name of the project. Length [3, 32]. Beginning with characters, only characters, numbers and _ are allowed.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "projectName"))
 
     @project_name.setter
     def project_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTopic, "project_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "projectName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="recordType")
     def record_type(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: recordType: Record type. TUPLE: structured data, BLOB: unstructured data.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "recordType"))
 
     @record_type.setter
     def record_type(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTopic, "record_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "recordType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="topicName")
     def topic_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: topicName: The name of the topic. Length [3, 64]. Beginning with characters, only characters, numbers and _ are allowed.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "topicName"))
 
     @topic_name.setter
     def topic_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTopic, "topic_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "topicName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="lifecycle")
     def lifecycle(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: lifecycle: Data storage life cycle.
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "lifecycle"))
 
     @lifecycle.setter
     def lifecycle(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTopic, "lifecycle").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "lifecycle", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="recordSchema")
     def record_schema(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: recordSchema: When creating a TUPLE type topic, you need to specify the schema, but the BLOB type does not pass this parameter.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "recordSchema"))
 
     @record_schema.setter
     def record_schema(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTopic, "record_schema").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "recordSchema", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="shardCount")
     def shard_count(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: shardCount: Initial shard number.
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "shardCount"))
 
     @shard_count.setter
     def shard_count(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTopic, "shard_count").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "shardCount", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-datahub.RosTopicProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -463,14 +530,23 @@
         :param project_name: 
         :param record_type: 
         :param topic_name: 
         :param lifecycle: 
         :param record_schema: 
         :param shard_count: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosTopicProps.__init__)
+            check_type(argname="argument comment", value=comment, expected_type=type_hints["comment"])
+            check_type(argname="argument project_name", value=project_name, expected_type=type_hints["project_name"])
+            check_type(argname="argument record_type", value=record_type, expected_type=type_hints["record_type"])
+            check_type(argname="argument topic_name", value=topic_name, expected_type=type_hints["topic_name"])
+            check_type(argname="argument lifecycle", value=lifecycle, expected_type=type_hints["lifecycle"])
+            check_type(argname="argument record_schema", value=record_schema, expected_type=type_hints["record_schema"])
+            check_type(argname="argument shard_count", value=shard_count, expected_type=type_hints["shard_count"])
         self._values: typing.Dict[str, typing.Any] = {
             "comment": comment,
             "project_name": project_name,
             "record_type": record_type,
             "topic_name": topic_name,
         }
         if lifecycle is not None:
@@ -565,37 +641,43 @@
 ):
     '''A ROS resource type:  ``ALIYUN::DATAHUB::Topic``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "TopicProps",
+        props: typing.Union["TopicProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::DATAHUB::Topic``.
 
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
     @jsii.member(jsii_name="attrProjectName")
     def attr_project_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute ProjectName: Project name.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrProjectName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTopicName")
     def attr_topic_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute TopicName: Topic name.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTopicName"))
 
 
 @jsii.data_type(
@@ -629,14 +711,23 @@
         :param project_name: Property projectName: The name of the project. Length [3, 32]. Beginning with characters, only characters, numbers and _ are allowed.
         :param record_type: Property recordType: Record type. TUPLE: structured data, BLOB: unstructured data.
         :param topic_name: Property topicName: The name of the topic. Length [3, 64]. Beginning with characters, only characters, numbers and _ are allowed.
         :param lifecycle: Property lifecycle: Data storage life cycle.
         :param record_schema: Property recordSchema: When creating a TUPLE type topic, you need to specify the schema, but the BLOB type does not pass this parameter.
         :param shard_count: Property shardCount: Initial shard number.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(TopicProps.__init__)
+            check_type(argname="argument comment", value=comment, expected_type=type_hints["comment"])
+            check_type(argname="argument project_name", value=project_name, expected_type=type_hints["project_name"])
+            check_type(argname="argument record_type", value=record_type, expected_type=type_hints["record_type"])
+            check_type(argname="argument topic_name", value=topic_name, expected_type=type_hints["topic_name"])
+            check_type(argname="argument lifecycle", value=lifecycle, expected_type=type_hints["lifecycle"])
+            check_type(argname="argument record_schema", value=record_schema, expected_type=type_hints["record_schema"])
+            check_type(argname="argument shard_count", value=shard_count, expected_type=type_hints["shard_count"])
         self._values: typing.Dict[str, typing.Any] = {
             "comment": comment,
             "project_name": project_name,
             "record_type": record_type,
             "topic_name": topic_name,
         }
         if lifecycle is not None:
```

### Comparing `ros-cdk-datahub-1.0.8/src/ros_cdk_datahub.egg-info/PKG-INFO` & `ros-cdk-datahub-1.0.9/src/ros_cdk_datahub.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-datahub
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS DATAHUB Construct Library
```

