# Comparing `tmp/ros-cdk-eventbridge-1.0.8.tar.gz` & `tmp/ros-cdk-eventbridge-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-eventbridge-1.0.8.tar", last modified: Thu Jul 14 02:27:52 2022, max compression
+gzip compressed data, was "dist/ros-cdk-eventbridge-1.0.9.tar", last modified: Fri Sep 23 10:52:06 2022, max compression
```

## Comparing `ros-cdk-eventbridge-1.0.8.tar` & `ros-cdk-eventbridge-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:27:52.000000 ros-cdk-eventbridge-1.0.8/
--rw-r--r--   0 root         (0) root         (0)    10279 2022-07-14 02:27:52.000000 ros-cdk-eventbridge-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2022-07-14 02:27:52.000000 ros-cdk-eventbridge-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2022-07-14 02:27:52.000000 ros-cdk-eventbridge-1.0.8/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1272 2022-07-14 02:27:52.000000 ros-cdk-eventbridge-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      203 2022-07-14 02:27:52.000000 ros-cdk-eventbridge-1.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)      106 2022-07-14 02:27:52.000000 ros-cdk-eventbridge-1.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-07-14 02:27:52.000000 ros-cdk-eventbridge-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1842 2022-07-14 02:27:52.000000 ros-cdk-eventbridge-1.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:27:52.000000 ros-cdk-eventbridge-1.0.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:27:52.000000 ros-cdk-eventbridge-1.0.8/src/ros_cdk_eventbridge/
--rw-r--r--   0 root         (0) root         (0)    27498 2022-07-14 02:27:52.000000 ros-cdk-eventbridge-1.0.8/src/ros_cdk_eventbridge/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:27:52.000000 ros-cdk-eventbridge-1.0.8/src/ros_cdk_eventbridge/_jsii/
--rw-r--r--   0 root         (0) root         (0)      399 2022-07-14 02:27:52.000000 ros-cdk-eventbridge-1.0.8/src/ros_cdk_eventbridge/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    35563 2022-07-14 02:27:52.000000 ros-cdk-eventbridge-1.0.8/src/ros_cdk_eventbridge/_jsii/ros-cdk-eventbridge@1.0.8.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:27:52.000000 ros-cdk-eventbridge-1.0.8/src/ros_cdk_eventbridge/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:27:52.000000 ros-cdk-eventbridge-1.0.8/src/ros_cdk_eventbridge.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1272 2022-07-14 02:27:52.000000 ros-cdk-eventbridge-1.0.8/src/ros_cdk_eventbridge.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      480 2022-07-14 02:27:52.000000 ros-cdk-eventbridge-1.0.8/src/ros_cdk_eventbridge.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:27:52.000000 ros-cdk-eventbridge-1.0.8/src/ros_cdk_eventbridge.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2022-07-14 02:27:52.000000 ros-cdk-eventbridge-1.0.8/src/ros_cdk_eventbridge.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2022-07-14 02:27:52.000000 ros-cdk-eventbridge-1.0.8/src/ros_cdk_eventbridge.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 10:52:06.000000 ros-cdk-eventbridge-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)    10279 2022-09-23 10:52:05.000000 ros-cdk-eventbridge-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-09-23 10:52:05.000000 ros-cdk-eventbridge-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2022-09-23 10:52:05.000000 ros-cdk-eventbridge-1.0.9/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1272 2022-09-23 10:52:06.000000 ros-cdk-eventbridge-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      203 2022-09-23 10:52:05.000000 ros-cdk-eventbridge-1.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      236 2022-09-23 10:52:05.000000 ros-cdk-eventbridge-1.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-09-23 10:52:06.000000 ros-cdk-eventbridge-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1871 2022-09-23 10:52:05.000000 ros-cdk-eventbridge-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 10:52:06.000000 ros-cdk-eventbridge-1.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 10:52:06.000000 ros-cdk-eventbridge-1.0.9/src/ros_cdk_eventbridge/
+-rw-r--r--   0 root         (0) root         (0)    32932 2022-09-23 10:52:05.000000 ros-cdk-eventbridge-1.0.9/src/ros_cdk_eventbridge/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 10:52:06.000000 ros-cdk-eventbridge-1.0.9/src/ros_cdk_eventbridge/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      433 2022-09-23 10:52:05.000000 ros-cdk-eventbridge-1.0.9/src/ros_cdk_eventbridge/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    35633 2022-09-23 10:52:05.000000 ros-cdk-eventbridge-1.0.9/src/ros_cdk_eventbridge/_jsii/ros-cdk-eventbridge@1.0.9.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 10:52:05.000000 ros-cdk-eventbridge-1.0.9/src/ros_cdk_eventbridge/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 10:52:06.000000 ros-cdk-eventbridge-1.0.9/src/ros_cdk_eventbridge.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1272 2022-09-23 10:52:06.000000 ros-cdk-eventbridge-1.0.9/src/ros_cdk_eventbridge.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      480 2022-09-23 10:52:06.000000 ros-cdk-eventbridge-1.0.9/src/ros_cdk_eventbridge.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 10:52:06.000000 ros-cdk-eventbridge-1.0.9/src/ros_cdk_eventbridge.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2022-09-23 10:52:06.000000 ros-cdk-eventbridge-1.0.9/src/ros_cdk_eventbridge.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2022-09-23 10:52:06.000000 ros-cdk-eventbridge-1.0.9/src/ros_cdk_eventbridge.egg-info/top_level.txt
```

### Comparing `ros-cdk-eventbridge-1.0.8/LICENSE` & `ros-cdk-eventbridge-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-eventbridge-1.0.8/PKG-INFO` & `ros-cdk-eventbridge-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-eventbridge
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS EVENTBRIDGE Construct Library
```

### Comparing `ros-cdk-eventbridge-1.0.8/setup.py` & `ros-cdk-eventbridge-1.0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-eventbridge",
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
         "ros_cdk_eventbridge",
         "ros_cdk_eventbridge._jsii"
     ],
     "package_data": {
         "ros_cdk_eventbridge._jsii": [
-            "ros-cdk-eventbridge@1.0.8.jsii.tgz"
+            "ros-cdk-eventbridge@1.0.9.jsii.tgz"
         ],
         "ros_cdk_eventbridge": [
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

### Comparing `ros-cdk-eventbridge-1.0.8/src/ros_cdk_eventbridge/__init__.py` & `ros-cdk-eventbridge-1.0.9/src/ros_cdk_eventbridge/__init__.py`

 * *Files 14% similar despite different names*

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
 
 
 class RosRule(
     ros_cdk_core.RosResource,
@@ -29,162 +31,189 @@
 ):
     '''A ROS template type:  ``ALIYUN::EventBridge::Rule``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosRuleProps",
+        props: typing.Union["RosRuleProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::EventBridge::Rule``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosRule.__init__)
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
+            type_hints = typing.get_type_hints(RosRule._render_properties)
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
     @jsii.member(jsii_name="attrEventBusName")
     def attr_event_bus_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: EventBusName: The name of the event bus.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrEventBusName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrRuleArn")
     def attr_rule_arn(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: RuleARN: The Alibaba Cloud Resource Name (ARN) of the event rule. The ARN is used for authorization.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrRuleArn"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrRuleName")
     def attr_rule_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: RuleName: The name of the event rule.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrRuleName"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosRule, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="eventBusName")
     def event_bus_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: eventBusName: The name of the event bus.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "eventBusName"))
 
     @event_bus_name.setter
     def event_bus_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosRule, "event_bus_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "eventBusName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="filterPattern")
     def filter_pattern(
         self,
     ) -> typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]]:
         '''
         :Property: filterPattern: The event pattern, in the JSON format.
         '''
         return typing.cast(typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]], jsii.get(self, "filterPattern"))
 
     @filter_pattern.setter
     def filter_pattern(
         self,
         value: typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosRule, "filter_pattern").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "filterPattern", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="ruleName")
     def rule_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: ruleName: The name of the event rule.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "ruleName"))
 
     @rule_name.setter
     def rule_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosRule, "rule_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "ruleName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="targets")
     def targets(
         self,
     ) -> typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosRule.TargetsProperty"]]]:
         '''
         :Property: targets: The event target to which events are delivered.
         '''
         return typing.cast(typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosRule.TargetsProperty"]]], jsii.get(self, "targets"))
 
     @targets.setter
     def targets(
         self,
         value: typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosRule.TargetsProperty"]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosRule, "targets").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "targets", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="description")
     def description(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: description: The description of the event rule.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "description"))
 
     @description.setter
     def description(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosRule, "description").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "description", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="status")
     def status(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -195,14 +224,17 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "status"))
 
     @status.setter
     def status(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosRule, "status").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "status", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-eventbridge.RosRule.ParamListProperty",
         jsii_struct_bases=[],
         name_mapping={
             "form": "form",
@@ -222,14 +254,20 @@
         ) -> None:
             '''
             :param form: 
             :param resource_key: 
             :param value: 
             :param template: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosRule.ParamListProperty.__init__)
+                check_type(argname="argument form", value=form, expected_type=type_hints["form"])
+                check_type(argname="argument resource_key", value=resource_key, expected_type=type_hints["resource_key"])
+                check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+                check_type(argname="argument template", value=template, expected_type=type_hints["template"])
             self._values: typing.Dict[str, typing.Any] = {
                 "form": form,
                 "resource_key": resource_key,
                 "value": value,
             }
             if template is not None:
                 self._values["template"] = template
@@ -295,25 +333,32 @@
     )
     class TargetsProperty:
         def __init__(
             self,
             *,
             endpoint: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
-            param_list: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosRule.ParamListProperty"]]],
+            param_list: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosRule.ParamListProperty", typing.Dict[str, typing.Any]]]]],
             type: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             push_retry_strategy: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param endpoint: 
             :param id: 
             :param param_list: 
             :param type: 
             :param push_retry_strategy: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosRule.TargetsProperty.__init__)
+                check_type(argname="argument endpoint", value=endpoint, expected_type=type_hints["endpoint"])
+                check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+                check_type(argname="argument param_list", value=param_list, expected_type=type_hints["param_list"])
+                check_type(argname="argument type", value=type, expected_type=type_hints["type"])
+                check_type(argname="argument push_retry_strategy", value=push_retry_strategy, expected_type=type_hints["push_retry_strategy"])
             self._values: typing.Dict[str, typing.Any] = {
                 "endpoint": endpoint,
                 "id": id,
                 "param_list": param_list,
                 "type": type,
             }
             if push_retry_strategy is not None:
@@ -394,27 +439,35 @@
 class RosRuleProps:
     def __init__(
         self,
         *,
         event_bus_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         filter_pattern: typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]],
         rule_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
-        targets: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosRule.TargetsProperty]]],
+        targets: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosRule.TargetsProperty, typing.Dict[str, typing.Any]]]]],
         description: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         status: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::EventBridge::Rule``.
 
         :param event_bus_name: 
         :param filter_pattern: 
         :param rule_name: 
         :param targets: 
         :param description: 
         :param status: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosRuleProps.__init__)
+            check_type(argname="argument event_bus_name", value=event_bus_name, expected_type=type_hints["event_bus_name"])
+            check_type(argname="argument filter_pattern", value=filter_pattern, expected_type=type_hints["filter_pattern"])
+            check_type(argname="argument rule_name", value=rule_name, expected_type=type_hints["rule_name"])
+            check_type(argname="argument targets", value=targets, expected_type=type_hints["targets"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument status", value=status, expected_type=type_hints["status"])
         self._values: typing.Dict[str, typing.Any] = {
             "event_bus_name": event_bus_name,
             "filter_pattern": filter_pattern,
             "rule_name": rule_name,
             "targets": targets,
         }
         if description is not None:
@@ -505,46 +558,52 @@
 ):
     '''A ROS resource type:  ``ALIYUN::EventBridge::Rule``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RuleProps",
+        props: typing.Union["RuleProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::EventBridge::Rule``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(Rule.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrEventBusName")
     def attr_event_bus_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute EventBusName: The name of the event bus.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrEventBusName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrRuleArn")
     def attr_rule_arn(self) -> ros_cdk_core.IResolvable:
         '''Attribute RuleARN: The Alibaba Cloud Resource Name (ARN) of the event rule.
 
         The ARN is used for authorization.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrRuleArn"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrRuleName")
     def attr_rule_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute RuleName: The name of the event rule.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrRuleName"))
 
 
 @jsii.data_type(
@@ -562,27 +621,35 @@
 class RuleProps:
     def __init__(
         self,
         *,
         event_bus_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         filter_pattern: typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]],
         rule_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
-        targets: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosRule.TargetsProperty]]],
+        targets: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosRule.TargetsProperty, typing.Dict[str, typing.Any]]]]],
         description: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         status: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::EventBridge::Rule``.
 
         :param event_bus_name: Property eventBusName: The name of the event bus.
         :param filter_pattern: Property filterPattern: The event pattern, in the JSON format.
         :param rule_name: Property ruleName: The name of the event rule.
         :param targets: Property targets: The event target to which events are delivered.
         :param description: Property description: The description of the event rule.
         :param status: Property status: The status of the event rule. Valid values: ENABLE: The event rule is enabled. It is the default state of the event rule. DISABLE: The event rule is disabled.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RuleProps.__init__)
+            check_type(argname="argument event_bus_name", value=event_bus_name, expected_type=type_hints["event_bus_name"])
+            check_type(argname="argument filter_pattern", value=filter_pattern, expected_type=type_hints["filter_pattern"])
+            check_type(argname="argument rule_name", value=rule_name, expected_type=type_hints["rule_name"])
+            check_type(argname="argument targets", value=targets, expected_type=type_hints["targets"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument status", value=status, expected_type=type_hints["status"])
         self._values: typing.Dict[str, typing.Any] = {
             "event_bus_name": event_bus_name,
             "filter_pattern": filter_pattern,
             "rule_name": rule_name,
             "targets": targets,
         }
         if description is not None:
```

### Comparing `ros-cdk-eventbridge-1.0.8/src/ros_cdk_eventbridge.egg-info/PKG-INFO` & `ros-cdk-eventbridge-1.0.9/src/ros_cdk_eventbridge.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-eventbridge
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS EVENTBRIDGE Construct Library
```

