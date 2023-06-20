# Comparing `tmp/ros-cdk-oos-1.0.8.tar.gz` & `tmp/ros-cdk-oos-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-oos-1.0.8.tar", last modified: Thu Jul 14 02:42:50 2022, max compression
+gzip compressed data, was "dist/ros-cdk-oos-1.0.9.tar", last modified: Fri Sep 23 11:38:37 2022, max compression
```

## Comparing `ros-cdk-oos-1.0.8.tar` & `ros-cdk-oos-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:42:50.000000 ros-cdk-oos-1.0.8/
--rw-r--r--   0 root         (0) root         (0)    10279 2022-07-14 02:42:50.000000 ros-cdk-oos-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2022-07-14 02:42:50.000000 ros-cdk-oos-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2022-07-14 02:42:50.000000 ros-cdk-oos-1.0.8/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1240 2022-07-14 02:42:50.000000 ros-cdk-oos-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      179 2022-07-14 02:42:50.000000 ros-cdk-oos-1.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)      106 2022-07-14 02:42:50.000000 ros-cdk-oos-1.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-07-14 02:42:50.000000 ros-cdk-oos-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1794 2022-07-14 02:42:50.000000 ros-cdk-oos-1.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:42:50.000000 ros-cdk-oos-1.0.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:42:50.000000 ros-cdk-oos-1.0.8/src/ros_cdk_oos/
--rw-r--r--   0 root         (0) root         (0)    71270 2022-07-14 02:42:50.000000 ros-cdk-oos-1.0.8/src/ros_cdk_oos/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:42:50.000000 ros-cdk-oos-1.0.8/src/ros_cdk_oos/_jsii/
--rw-r--r--   0 root         (0) root         (0)      370 2022-07-14 02:42:50.000000 ros-cdk-oos-1.0.8/src/ros_cdk_oos/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    51066 2022-07-14 02:42:50.000000 ros-cdk-oos-1.0.8/src/ros_cdk_oos/_jsii/ros-cdk-oos@1.0.8.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:42:50.000000 ros-cdk-oos-1.0.8/src/ros_cdk_oos/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:42:50.000000 ros-cdk-oos-1.0.8/src/ros_cdk_oos.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1240 2022-07-14 02:42:50.000000 ros-cdk-oos-1.0.8/src/ros_cdk_oos.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      400 2022-07-14 02:42:50.000000 ros-cdk-oos-1.0.8/src/ros_cdk_oos.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:42:50.000000 ros-cdk-oos-1.0.8/src/ros_cdk_oos.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2022-07-14 02:42:50.000000 ros-cdk-oos-1.0.8/src/ros_cdk_oos.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2022-07-14 02:42:50.000000 ros-cdk-oos-1.0.8/src/ros_cdk_oos.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:38:37.000000 ros-cdk-oos-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)    10279 2022-09-23 11:38:37.000000 ros-cdk-oos-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-09-23 11:38:37.000000 ros-cdk-oos-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2022-09-23 11:38:37.000000 ros-cdk-oos-1.0.9/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1240 2022-09-23 11:38:37.000000 ros-cdk-oos-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      179 2022-09-23 11:38:37.000000 ros-cdk-oos-1.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      236 2022-09-23 11:38:37.000000 ros-cdk-oos-1.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-09-23 11:38:37.000000 ros-cdk-oos-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1823 2022-09-23 11:38:37.000000 ros-cdk-oos-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:38:37.000000 ros-cdk-oos-1.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:38:37.000000 ros-cdk-oos-1.0.9/src/ros_cdk_oos/
+-rw-r--r--   0 root         (0) root         (0)    84677 2022-09-23 11:38:37.000000 ros-cdk-oos-1.0.9/src/ros_cdk_oos/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:38:37.000000 ros-cdk-oos-1.0.9/src/ros_cdk_oos/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      404 2022-09-23 11:38:37.000000 ros-cdk-oos-1.0.9/src/ros_cdk_oos/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    51121 2022-09-23 11:38:37.000000 ros-cdk-oos-1.0.9/src/ros_cdk_oos/_jsii/ros-cdk-oos@1.0.9.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 11:38:37.000000 ros-cdk-oos-1.0.9/src/ros_cdk_oos/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:38:37.000000 ros-cdk-oos-1.0.9/src/ros_cdk_oos.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1240 2022-09-23 11:38:37.000000 ros-cdk-oos-1.0.9/src/ros_cdk_oos.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      400 2022-09-23 11:38:37.000000 ros-cdk-oos-1.0.9/src/ros_cdk_oos.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 11:38:37.000000 ros-cdk-oos-1.0.9/src/ros_cdk_oos.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2022-09-23 11:38:37.000000 ros-cdk-oos-1.0.9/src/ros_cdk_oos.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2022-09-23 11:38:37.000000 ros-cdk-oos-1.0.9/src/ros_cdk_oos.egg-info/top_level.txt
```

### Comparing `ros-cdk-oos-1.0.8/LICENSE` & `ros-cdk-oos-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-oos-1.0.8/PKG-INFO` & `ros-cdk-oos-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-oos
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS OOS Construct Library
```

### Comparing `ros-cdk-oos-1.0.8/setup.py` & `ros-cdk-oos-1.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-oos",
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
         "ros_cdk_oos",
         "ros_cdk_oos._jsii"
     ],
     "package_data": {
         "ros_cdk_oos._jsii": [
-            "ros-cdk-oos@1.0.8.jsii.tgz"
+            "ros-cdk-oos@1.0.9.jsii.tgz"
         ],
         "ros_cdk_oos": [
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

### Comparing `ros-cdk-oos-1.0.8/src/ros_cdk_oos/__init__.py` & `ros-cdk-oos-1.0.9/src/ros_cdk_oos/__init__.py`

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
 
 
 class Execution(
     ros_cdk_core.Resource,
@@ -29,82 +31,88 @@
 ):
     '''A ROS resource type:  ``ALIYUN::OOS::Execution``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "ExecutionProps",
+        props: typing.Union["ExecutionProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::OOS::Execution``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(Execution.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrCounters")
     def attr_counters(self) -> ros_cdk_core.IResolvable:
         '''Attribute Counters: Task statistics: FailedTasks, SuccessTasks, TotalTasks.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrCounters"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrCurlCli")
     def attr_curl_cli(self) -> ros_cdk_core.IResolvable:
         '''Attribute CurlCli: Convenience attribute, provides curl CLI command prefix, which can be used to notify oos execution instead of OOS API NotifyExecution.
 
         You can notify approve to oos execution by adding --data-binary '{"data": {"NotifyType": "Approve"}}'
         For more parameters in data, refer to https://help.aliyun.com/document_detail/120777.html.
         You can also notify execution via ROS API SignalResource. API parameters Status and UniqueId are ignored. Use API parameter Data to pass data.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrCurlCli"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrExecutionId")
     def attr_execution_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute ExecutionId: Execution ID.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrExecutionId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrOutputs")
     def attr_outputs(self) -> ros_cdk_core.IResolvable:
         '''Attribute Outputs: Execution output.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrOutputs"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPowerShellCurlCli")
     def attr_power_shell_curl_cli(self) -> ros_cdk_core.IResolvable:
         '''Attribute PowerShellCurlCli: Convenience attribute, provides curl CLI command prefix for PowerShell, which can be used to notify oos execution instead of OOS API NotifyExecution.
 
         You can notify approve to oos execution by adding -Body '{"data": {"NotifyType": "Approve"}}'
         For more parameters in data, refer to https://help.aliyun.com/document_detail/120777.html.You can also notify execution via ROS API SignalResource. API parameters Status and UniqueId are ignored. Use API parameter Data to pass data.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPowerShellCurlCli"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrStatus")
     def attr_status(self) -> ros_cdk_core.IResolvable:
         '''Attribute Status: Execution status.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrStatus"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrStatusMessage")
     def attr_status_message(self) -> ros_cdk_core.IResolvable:
         '''Attribute StatusMessage: Execution status information.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrStatusMessage"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrWindowsCurlCli")
     def attr_windows_curl_cli(self) -> ros_cdk_core.IResolvable:
         '''Attribute WindowsCurlCli: Convenience attribute, provides curl CLI command prefix for Windows, which can be used to notify oos execution instead of OOS API NotifyExecution.
 
         You can notify approve to oos execution by adding --data-binary "{"data": {"NotifyType": "Approve"}}"
         For more parameters in data, refer to https://help.aliyun.com/document_detail/120777.html.You can also notify execution via ROS API SignalResource. API parameters Status and UniqueId are ignored. Use API parameter Data to pass data.
         '''
@@ -131,15 +139,15 @@
         self,
         *,
         template_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         mode: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         parameters: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]]] = None,
         parent_execution_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         resource_group_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        resource_options: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosExecution.ResourceOptionsProperty"]] = None,
+        resource_options: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosExecution.ResourceOptionsProperty", typing.Dict[str, typing.Any]]]] = None,
         safety_check: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         tags: typing.Optional[typing.Mapping[builtins.str, typing.Any]] = None,
         template_version: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::OOS::Execution``.
 
         :param template_name: Property templateName: Template name. Content is limited to letters, numbers, underlined, underline, the length of 200 characters.
@@ -148,14 +156,25 @@
         :param parent_execution_id: Property parentExecutionId: Parent execution ID.
         :param resource_group_id: Property resourceGroupId: Resource group id.
         :param resource_options: Property resourceOptions: Resource options user by ROS.
         :param safety_check: Property safetyCheck: Security check mode. Allowed values: - Skip: This option means that customers understand the risks, you can do anything without confirmation Action, no matter what the level of risk. It takes effect only if Mode is Automatic. - ConfirmEveryHighRiskAction (default): This option would require customers to confirm each Action a high risk. NotifyExecution by calling customer interface to confirm or cancel.
         :param tags: Property tags: Tag value and the key mapping, the label of the key number can be up to 20.
         :param template_version: Property templateVersion: Version number of template. Default to the latest version.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(ExecutionProps.__init__)
+            check_type(argname="argument template_name", value=template_name, expected_type=type_hints["template_name"])
+            check_type(argname="argument mode", value=mode, expected_type=type_hints["mode"])
+            check_type(argname="argument parameters", value=parameters, expected_type=type_hints["parameters"])
+            check_type(argname="argument parent_execution_id", value=parent_execution_id, expected_type=type_hints["parent_execution_id"])
+            check_type(argname="argument resource_group_id", value=resource_group_id, expected_type=type_hints["resource_group_id"])
+            check_type(argname="argument resource_options", value=resource_options, expected_type=type_hints["resource_options"])
+            check_type(argname="argument safety_check", value=safety_check, expected_type=type_hints["safety_check"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
+            check_type(argname="argument template_version", value=template_version, expected_type=type_hints["template_version"])
         self._values: typing.Dict[str, typing.Any] = {
             "template_name": template_name,
         }
         if mode is not None:
             self._values["mode"] = mode
         if parameters is not None:
             self._values["parameters"] = parameters
@@ -272,37 +291,43 @@
 ):
     '''A ROS resource type:  ``ALIYUN::OOS::Parameter``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "ParameterProps",
+        props: typing.Union["ParameterProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::OOS::Parameter``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(Parameter.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrName")
     def attr_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute Name: The Name of the parameter.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrValue")
     def attr_value(self) -> ros_cdk_core.IResolvable:
         '''Attribute Value: The Value of the parameter.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrValue"))
 
 
 @jsii.data_type(
@@ -333,14 +358,22 @@
         :param name: Property name: The name of the parameter. The name must be 1 to 200 characters in length,and can contain letters, digits, hyphens (-), and underscores (_). It cannot start with ALIYUN, ACS, ALIBABA, ALICLOUD, or OOS.
         :param type: Property type: The data type of the common parameter. Valid values: String and StringList.
         :param value: Property value: The value of the parameter. The value must be 1 to 4096 characters in length.
         :param constraints: Property constraints: The constraints of the parameter. By default, this parameter is null. Valid values: AllowedValues: The value that is allowed for the parameter. It must be an array string. AllowedPattern: The pattern that is allowed for the parameter. It must be a regular expression. MinLength: The minimum length of the parameter. MaxLength: The maximum length of the parameter.
         :param description: Property description: The description of the parameter. The description must be 1 to 200 characters in length.
         :param resource_group_id: Property resourceGroupId: Resource group id.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(ParameterProps.__init__)
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+            check_type(argname="argument type", value=type, expected_type=type_hints["type"])
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+            check_type(argname="argument constraints", value=constraints, expected_type=type_hints["constraints"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument resource_group_id", value=resource_group_id, expected_type=type_hints["resource_group_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "name": name,
             "type": type,
             "value": value,
         }
         if constraints is not None:
             self._values["constraints"] = constraints
@@ -433,234 +466,264 @@
 ):
     '''A ROS template type:  ``ALIYUN::OOS::Execution``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosExecutionProps",
+        props: typing.Union["RosExecutionProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::OOS::Execution``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosExecution.__init__)
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
+            type_hints = typing.get_type_hints(RosExecution._render_properties)
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
     @jsii.member(jsii_name="attrCounters")
     def attr_counters(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Counters: Task statistics: FailedTasks, SuccessTasks, TotalTasks.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrCounters"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrCurlCli")
     def attr_curl_cli(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute:
 
         CurlCli: Convenience attribute, provides curl CLI command prefix, which can be used to notify oos execution instead of OOS API NotifyExecution.
         You can notify approve to oos execution by adding --data-binary '{"data": {"NotifyType": "Approve"}}'
         For more parameters in data, refer to https://help.aliyun.com/document_detail/120777.html.
         You can also notify execution via ROS API SignalResource. API parameters Status and UniqueId are ignored. Use API parameter Data to pass data.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrCurlCli"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrExecutionId")
     def attr_execution_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ExecutionId: Execution ID.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrExecutionId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrOutputs")
     def attr_outputs(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Outputs: Execution output.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrOutputs"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPowerShellCurlCli")
     def attr_power_shell_curl_cli(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute:
 
         PowerShellCurlCli: Convenience attribute, provides curl CLI command prefix for PowerShell, which can be used to notify oos execution instead of OOS API NotifyExecution.
         You can notify approve to oos execution by adding -Body '{"data": {"NotifyType": "Approve"}}'
         For more parameters in data, refer to https://help.aliyun.com/document_detail/120777.html.You can also notify execution via ROS API SignalResource. API parameters Status and UniqueId are ignored. Use API parameter Data to pass data.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPowerShellCurlCli"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrStatus")
     def attr_status(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Status: Execution status.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrStatus"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrStatusMessage")
     def attr_status_message(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: StatusMessage: Execution status information.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrStatusMessage"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrWindowsCurlCli")
     def attr_windows_curl_cli(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute:
 
         WindowsCurlCli: Convenience attribute, provides curl CLI command prefix for Windows, which can be used to notify oos execution instead of OOS API NotifyExecution.
         You can notify approve to oos execution by adding --data-binary "{"data": {"NotifyType": "Approve"}}"
         For more parameters in data, refer to https://help.aliyun.com/document_detail/120777.html.You can also notify execution via ROS API SignalResource. API parameters Status and UniqueId are ignored. Use API parameter Data to pass data.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrWindowsCurlCli"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosExecution, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="templateName")
     def template_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: templateName: Template name. Content is limited to letters, numbers, underlined, underline, the length of 200 characters.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "templateName"))
 
     @template_name.setter
     def template_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosExecution, "template_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "templateName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="mode")
     def mode(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: mode: Execution mode.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "mode"))
 
     @mode.setter
     def mode(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosExecution, "mode").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "mode", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="parameters")
     def parameters(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]]]:
         '''
         :Property: parameters: Parameters for the execution of template.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]]], jsii.get(self, "parameters"))
 
     @parameters.setter
     def parameters(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosExecution, "parameters").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "parameters", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="parentExecutionId")
     def parent_execution_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: parentExecutionId: Parent execution ID.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "parentExecutionId"))
 
     @parent_execution_id.setter
     def parent_execution_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosExecution, "parent_execution_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "parentExecutionId", value)
 
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
+            type_hints = typing.get_type_hints(getattr(RosExecution, "resource_group_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "resourceGroupId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="resourceOptions")
     def resource_options(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosExecution.ResourceOptionsProperty"]]:
         '''
         :Property: resourceOptions: Resource options user by ROS.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosExecution.ResourceOptionsProperty"]], jsii.get(self, "resourceOptions"))
 
     @resource_options.setter
     def resource_options(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosExecution.ResourceOptionsProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosExecution, "resource_options").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "resourceOptions", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="safetyCheck")
     def safety_check(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -672,46 +735,55 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "safetyCheck"))
 
     @safety_check.setter
     def safety_check(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosExecution, "safety_check").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "safetyCheck", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="tags")
     def tags(self) -> typing.Optional[typing.Mapping[builtins.str, typing.Any]]:
         '''
         :Property: tags: Tag value and the key mapping, the label of the key number can be up to 20.
         '''
         return typing.cast(typing.Optional[typing.Mapping[builtins.str, typing.Any]], jsii.get(self, "tags"))
 
     @tags.setter
     def tags(
         self,
         value: typing.Optional[typing.Mapping[builtins.str, typing.Any]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosExecution, "tags").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "tags", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="templateVersion")
     def template_version(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: templateVersion: Version number of template. Default to the latest version.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "templateVersion"))
 
     @template_version.setter
     def template_version(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosExecution, "template_version").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "templateVersion", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-oos.RosExecution.ResourceOptionsProperty",
         jsii_struct_bases=[],
         name_mapping={
             "cancel_on_delete": "cancelOnDelete",
@@ -731,14 +803,20 @@
         ) -> None:
             '''
             :param cancel_on_delete: 
             :param failure_statuses: 
             :param success_statuses: 
             :param timeout: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosExecution.ResourceOptionsProperty.__init__)
+                check_type(argname="argument cancel_on_delete", value=cancel_on_delete, expected_type=type_hints["cancel_on_delete"])
+                check_type(argname="argument failure_statuses", value=failure_statuses, expected_type=type_hints["failure_statuses"])
+                check_type(argname="argument success_statuses", value=success_statuses, expected_type=type_hints["success_statuses"])
+                check_type(argname="argument timeout", value=timeout, expected_type=type_hints["timeout"])
             self._values: typing.Dict[str, typing.Any] = {}
             if cancel_on_delete is not None:
                 self._values["cancel_on_delete"] = cancel_on_delete
             if failure_statuses is not None:
                 self._values["failure_statuses"] = failure_statuses
             if success_statuses is not None:
                 self._values["success_statuses"] = success_statuses
@@ -828,15 +906,15 @@
         self,
         *,
         template_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         mode: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         parameters: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]]] = None,
         parent_execution_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         resource_group_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        resource_options: typing.Optional[typing.Union[ros_cdk_core.IResolvable, RosExecution.ResourceOptionsProperty]] = None,
+        resource_options: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosExecution.ResourceOptionsProperty, typing.Dict[str, typing.Any]]]] = None,
         safety_check: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         tags: typing.Optional[typing.Mapping[builtins.str, typing.Any]] = None,
         template_version: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::OOS::Execution``.
 
         :param template_name: 
@@ -845,14 +923,25 @@
         :param parent_execution_id: 
         :param resource_group_id: 
         :param resource_options: 
         :param safety_check: 
         :param tags: 
         :param template_version: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosExecutionProps.__init__)
+            check_type(argname="argument template_name", value=template_name, expected_type=type_hints["template_name"])
+            check_type(argname="argument mode", value=mode, expected_type=type_hints["mode"])
+            check_type(argname="argument parameters", value=parameters, expected_type=type_hints["parameters"])
+            check_type(argname="argument parent_execution_id", value=parent_execution_id, expected_type=type_hints["parent_execution_id"])
+            check_type(argname="argument resource_group_id", value=resource_group_id, expected_type=type_hints["resource_group_id"])
+            check_type(argname="argument resource_options", value=resource_options, expected_type=type_hints["resource_options"])
+            check_type(argname="argument safety_check", value=safety_check, expected_type=type_hints["safety_check"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
+            check_type(argname="argument template_version", value=template_version, expected_type=type_hints["template_version"])
         self._values: typing.Dict[str, typing.Any] = {
             "template_name": template_name,
         }
         if mode is not None:
             self._values["mode"] = mode
         if parameters is not None:
             self._values["parameters"] = parameters
@@ -980,104 +1069,122 @@
 ):
     '''A ROS template type:  ``ALIYUN::OOS::Parameter``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosParameterProps",
+        props: typing.Union["RosParameterProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::OOS::Parameter``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosParameter.__init__)
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
+            type_hints = typing.get_type_hints(RosParameter._render_properties)
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
         :Attribute: Name: The Name of the parameter.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrValue")
     def attr_value(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Value: The Value of the parameter.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrValue"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosParameter, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="name")
     def name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         name: The name of the parameter.
         The name must be 1 to 200 characters in length,and can contain letters, digits, hyphens (-), and underscores (_).
         It cannot start with ALIYUN, ACS, ALIBABA, ALICLOUD, or OOS.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "name"))
 
     @name.setter
     def name(self, value: typing.Union[builtins.str, ros_cdk_core.IResolvable]) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosParameter, "name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "name", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="type")
     def type(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         type: The data type of the common parameter.
         Valid values: String and StringList.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "type"))
 
     @type.setter
     def type(self, value: typing.Union[builtins.str, ros_cdk_core.IResolvable]) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosParameter, "type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "type", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="value")
     def value(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         value: The value of the parameter.
         The value must be 1 to 4096 characters in length.
@@ -1085,17 +1192,20 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "value"))
 
     @value.setter
     def value(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosParameter, "value").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "value", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="constraints")
     def constraints(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -1109,17 +1219,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "constraints"))
 
     @constraints.setter
     def constraints(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosParameter, "constraints").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "constraints", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="description")
     def description(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -1129,31 +1242,37 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "description"))
 
     @description.setter
     def description(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosParameter, "description").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "description", value)
 
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
+            type_hints = typing.get_type_hints(getattr(RosParameter, "resource_group_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "resourceGroupId", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-oos.RosParameterProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -1181,14 +1300,22 @@
         :param name: 
         :param type: 
         :param value: 
         :param constraints: 
         :param description: 
         :param resource_group_id: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosParameterProps.__init__)
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+            check_type(argname="argument type", value=type, expected_type=type_hints["type"])
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+            check_type(argname="argument constraints", value=constraints, expected_type=type_hints["constraints"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument resource_group_id", value=resource_group_id, expected_type=type_hints["resource_group_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "name": name,
             "type": type,
             "value": value,
         }
         if constraints is not None:
             self._values["constraints"] = constraints
@@ -1293,140 +1420,164 @@
 ):
     '''A ROS template type:  ``ALIYUN::OOS::Template``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosTemplateProps",
+        props: typing.Union["RosTemplateProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::OOS::Template``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosTemplate.__init__)
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
+            type_hints = typing.get_type_hints(RosTemplate._render_properties)
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
     @jsii.member(jsii_name="attrExecutionPolicy")
     def attr_execution_policy(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ExecutionPolicy: Execution Policy
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrExecutionPolicy"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTemplateId")
     def attr_template_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: TemplateId: Template ID
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTemplateId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTemplateName")
     def attr_template_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: TemplateName: Template Name
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTemplateName"))
 
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
         :Property: content: The content of the template. The template must be in the JSON or YAML format. Maximum size: 64 KB.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "content"))
 
     @content.setter
     def content(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTemplate, "content").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "content", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTemplate, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="templateName")
     def template_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: templateName: The name of the template. The template name can be up to 200 characters in length. The name can contain letters, digits, hyphens (-), and underscores (_). It cannot start with ALIYUN, ACS, ALIBABA, or ALICLOUD.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "templateName"))
 
     @template_name.setter
     def template_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTemplate, "template_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "templateName", value)
 
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
+            type_hints = typing.get_type_hints(getattr(RosTemplate, "resource_group_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "resourceGroupId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="tags")
     def tags(self) -> typing.Optional[typing.Mapping[builtins.str, typing.Any]]:
         '''
         :Property: tags: Tag value and the key mapping, the label of the key number can be up to 20.
         '''
         return typing.cast(typing.Optional[typing.Mapping[builtins.str, typing.Any]], jsii.get(self, "tags"))
 
     @tags.setter
     def tags(
         self,
         value: typing.Optional[typing.Mapping[builtins.str, typing.Any]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTemplate, "tags").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "tags", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-oos.RosTemplateProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -1448,14 +1599,20 @@
         '''Properties for defining a ``ALIYUN::OOS::Template``.
 
         :param content: 
         :param template_name: 
         :param resource_group_id: 
         :param tags: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosTemplateProps.__init__)
+            check_type(argname="argument content", value=content, expected_type=type_hints["content"])
+            check_type(argname="argument template_name", value=template_name, expected_type=type_hints["template_name"])
+            check_type(argname="argument resource_group_id", value=resource_group_id, expected_type=type_hints["resource_group_id"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
         self._values: typing.Dict[str, typing.Any] = {
             "content": content,
             "template_name": template_name,
         }
         if resource_group_id is not None:
             self._values["resource_group_id"] = resource_group_id
         if tags is not None:
@@ -1516,43 +1673,49 @@
 ):
     '''A ROS resource type:  ``ALIYUN::OOS::Template``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "TemplateProps",
+        props: typing.Union["TemplateProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::OOS::Template``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(Template.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrExecutionPolicy")
     def attr_execution_policy(self) -> ros_cdk_core.IResolvable:
         '''Attribute ExecutionPolicy: Execution Policy.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrExecutionPolicy"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTemplateId")
     def attr_template_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute TemplateId: Template ID.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTemplateId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTemplateName")
     def attr_template_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute TemplateName: Template Name.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTemplateName"))
 
 
 @jsii.data_type(
@@ -1577,14 +1740,20 @@
         '''Properties for defining a ``ALIYUN::OOS::Template``.
 
         :param content: Property content: The content of the template. The template must be in the JSON or YAML format. Maximum size: 64 KB.
         :param template_name: Property templateName: The name of the template. The template name can be up to 200 characters in length. The name can contain letters, digits, hyphens (-), and underscores (_). It cannot start with ALIYUN, ACS, ALIBABA, or ALICLOUD.
         :param resource_group_id: Property resourceGroupId: Resource group id.
         :param tags: Property tags: Tag value and the key mapping, the label of the key number can be up to 20.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(TemplateProps.__init__)
+            check_type(argname="argument content", value=content, expected_type=type_hints["content"])
+            check_type(argname="argument template_name", value=template_name, expected_type=type_hints["template_name"])
+            check_type(argname="argument resource_group_id", value=resource_group_id, expected_type=type_hints["resource_group_id"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
         self._values: typing.Dict[str, typing.Any] = {
             "content": content,
             "template_name": template_name,
         }
         if resource_group_id is not None:
             self._values["resource_group_id"] = resource_group_id
         if tags is not None:
```

### Comparing `ros-cdk-oos-1.0.8/src/ros_cdk_oos.egg-info/PKG-INFO` & `ros-cdk-oos-1.0.9/src/ros_cdk_oos.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-oos
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS OOS Construct Library
```

