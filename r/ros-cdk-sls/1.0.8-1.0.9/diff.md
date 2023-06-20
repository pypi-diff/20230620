# Comparing `tmp/ros-cdk-sls-1.0.8.tar.gz` & `tmp/ros-cdk-sls-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-sls-1.0.8.tar", last modified: Thu Jul 14 02:11:40 2022, max compression
+gzip compressed data, was "dist/ros-cdk-sls-1.0.9.tar", last modified: Fri Sep 23 11:10:03 2022, max compression
```

## Comparing `ros-cdk-sls-1.0.8.tar` & `ros-cdk-sls-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:11:40.000000 ros-cdk-sls-1.0.8/
--rw-r--r--   0 root         (0) root         (0)    10279 2022-07-14 02:11:40.000000 ros-cdk-sls-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2022-07-14 02:11:40.000000 ros-cdk-sls-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2022-07-14 02:11:40.000000 ros-cdk-sls-1.0.8/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1240 2022-07-14 02:11:40.000000 ros-cdk-sls-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      179 2022-07-14 02:11:40.000000 ros-cdk-sls-1.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)      106 2022-07-14 02:11:40.000000 ros-cdk-sls-1.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-07-14 02:11:40.000000 ros-cdk-sls-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1794 2022-07-14 02:11:40.000000 ros-cdk-sls-1.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:11:40.000000 ros-cdk-sls-1.0.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:11:40.000000 ros-cdk-sls-1.0.8/src/ros_cdk_sls/
--rw-r--r--   0 root         (0) root         (0)   403607 2022-07-14 02:11:40.000000 ros-cdk-sls-1.0.8/src/ros_cdk_sls/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:11:40.000000 ros-cdk-sls-1.0.8/src/ros_cdk_sls/_jsii/
--rw-r--r--   0 root         (0) root         (0)      370 2022-07-14 02:11:40.000000 ros-cdk-sls-1.0.8/src/ros_cdk_sls/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)   136646 2022-07-14 02:11:40.000000 ros-cdk-sls-1.0.8/src/ros_cdk_sls/_jsii/ros-cdk-sls@1.0.8.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:11:40.000000 ros-cdk-sls-1.0.8/src/ros_cdk_sls/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:11:40.000000 ros-cdk-sls-1.0.8/src/ros_cdk_sls.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1240 2022-07-14 02:11:40.000000 ros-cdk-sls-1.0.8/src/ros_cdk_sls.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      400 2022-07-14 02:11:40.000000 ros-cdk-sls-1.0.8/src/ros_cdk_sls.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:11:40.000000 ros-cdk-sls-1.0.8/src/ros_cdk_sls.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2022-07-14 02:11:40.000000 ros-cdk-sls-1.0.8/src/ros_cdk_sls.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2022-07-14 02:11:40.000000 ros-cdk-sls-1.0.8/src/ros_cdk_sls.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:10:03.000000 ros-cdk-sls-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)    10279 2022-09-23 11:10:02.000000 ros-cdk-sls-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-09-23 11:10:02.000000 ros-cdk-sls-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2022-09-23 11:10:02.000000 ros-cdk-sls-1.0.9/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1240 2022-09-23 11:10:03.000000 ros-cdk-sls-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      179 2022-09-23 11:10:02.000000 ros-cdk-sls-1.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      236 2022-09-23 11:10:02.000000 ros-cdk-sls-1.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-09-23 11:10:03.000000 ros-cdk-sls-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1823 2022-09-23 11:10:02.000000 ros-cdk-sls-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:10:03.000000 ros-cdk-sls-1.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:10:03.000000 ros-cdk-sls-1.0.9/src/ros_cdk_sls/
+-rw-r--r--   0 root         (0) root         (0)   485550 2022-09-23 11:10:02.000000 ros-cdk-sls-1.0.9/src/ros_cdk_sls/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:10:03.000000 ros-cdk-sls-1.0.9/src/ros_cdk_sls/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      404 2022-09-23 11:10:02.000000 ros-cdk-sls-1.0.9/src/ros_cdk_sls/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   136702 2022-09-23 11:10:02.000000 ros-cdk-sls-1.0.9/src/ros_cdk_sls/_jsii/ros-cdk-sls@1.0.9.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 11:10:02.000000 ros-cdk-sls-1.0.9/src/ros_cdk_sls/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:10:03.000000 ros-cdk-sls-1.0.9/src/ros_cdk_sls.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1240 2022-09-23 11:10:03.000000 ros-cdk-sls-1.0.9/src/ros_cdk_sls.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      400 2022-09-23 11:10:03.000000 ros-cdk-sls-1.0.9/src/ros_cdk_sls.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 11:10:03.000000 ros-cdk-sls-1.0.9/src/ros_cdk_sls.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2022-09-23 11:10:03.000000 ros-cdk-sls-1.0.9/src/ros_cdk_sls.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2022-09-23 11:10:03.000000 ros-cdk-sls-1.0.9/src/ros_cdk_sls.egg-info/top_level.txt
```

### Comparing `ros-cdk-sls-1.0.8/LICENSE` & `ros-cdk-sls-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-sls-1.0.8/PKG-INFO` & `ros-cdk-sls-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-sls
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS SLS Construct Library
```

### Comparing `ros-cdk-sls-1.0.8/setup.py` & `ros-cdk-sls-1.0.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-sls",
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
         "ros_cdk_sls",
         "ros_cdk_sls._jsii"
     ],
     "package_data": {
         "ros_cdk_sls._jsii": [
-            "ros-cdk-sls@1.0.8.jsii.tgz"
+            "ros-cdk-sls@1.0.9.jsii.tgz"
         ],
         "ros_cdk_sls": [
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

### Comparing `ros-cdk-sls-1.0.8/src/ros_cdk_sls/__init__.py` & `ros-cdk-sls-1.0.9/src/ros_cdk_sls/__init__.py`

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
 
 
 class Alert(
     ros_cdk_core.Resource,
@@ -29,31 +31,37 @@
 ):
     '''A ROS resource type:  ``ALIYUN::SLS::Alert``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "AlertProps",
+        props: typing.Union["AlertProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::SLS::Alert``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(Alert.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrName")
     def attr_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute Name: Alert name.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrName"))
 
 
 @jsii.data_type(
@@ -61,22 +69,26 @@
     jsii_struct_bases=[],
     name_mapping={"detail": "detail", "project": "project"},
 )
 class AlertProps:
     def __init__(
         self,
         *,
-        detail: typing.Union["RosAlert.DetailProperty", ros_cdk_core.IResolvable],
+        detail: typing.Union[typing.Union["RosAlert.DetailProperty", typing.Dict[str, typing.Any]], ros_cdk_core.IResolvable],
         project: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
         '''Properties for defining a ``ALIYUN::SLS::Alert``.
 
         :param detail: Property detail:.
         :param project: Property project: Project name: 1. Only supports lowercase letters, numbers, hyphens (-) and underscores (_). 2. Must start and end with lowercase letters and numbers. 3. The name length is 3-63 characters.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(AlertProps.__init__)
+            check_type(argname="argument detail", value=detail, expected_type=type_hints["detail"])
+            check_type(argname="argument project", value=project, expected_type=type_hints["project"])
         self._values: typing.Dict[str, typing.Any] = {
             "detail": detail,
             "project": project,
         }
 
     @builtins.property
     def detail(
@@ -118,28 +130,34 @@
 ):
     '''A ROS resource type:  ``ALIYUN::SLS::ApplyConfigToMachineGroup``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: typing.Optional["ApplyConfigToMachineGroupProps"] = None,
+        props: typing.Optional[typing.Union["ApplyConfigToMachineGroupProps", typing.Dict[str, typing.Any]]] = None,
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::SLS::ApplyConfigToMachineGroup``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(ApplyConfigToMachineGroup.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-sls.ApplyConfigToMachineGroupProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -158,14 +176,19 @@
     ) -> None:
         '''Properties for defining a ``ALIYUN::SLS::ApplyConfigToMachineGroup``.
 
         :param config_name: Property configName: Apply config to the config name.
         :param group_name: Property groupName: Apply config to the group name.
         :param project_name: Property projectName: Apply config to the project name.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(ApplyConfigToMachineGroupProps.__init__)
+            check_type(argname="argument config_name", value=config_name, expected_type=type_hints["config_name"])
+            check_type(argname="argument group_name", value=group_name, expected_type=type_hints["group_name"])
+            check_type(argname="argument project_name", value=project_name, expected_type=type_hints["project_name"])
         self._values: typing.Dict[str, typing.Any] = {}
         if config_name is not None:
             self._values["config_name"] = config_name
         if group_name is not None:
             self._values["group_name"] = group_name
         if project_name is not None:
             self._values["project_name"] = project_name
@@ -213,31 +236,37 @@
 ):
     '''A ROS resource type:  ``ALIYUN::SLS::Audit``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "AuditProps",
+        props: typing.Union["AuditProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::SLS::Audit``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(Audit.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDisplayName")
     def attr_display_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute DisplayName: Name of SLS log audit.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDisplayName"))
 
 
 @jsii.data_type(
@@ -250,23 +279,28 @@
     },
 )
 class AuditProps:
     def __init__(
         self,
         *,
         display_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
-        variable_map: typing.Union[ros_cdk_core.IResolvable, "RosAudit.VariableMapProperty"],
+        variable_map: typing.Union[ros_cdk_core.IResolvable, typing.Union["RosAudit.VariableMapProperty", typing.Dict[str, typing.Any]]],
         multi_account: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::SLS::Audit``.
 
         :param display_name: Property displayName: Name of SLS log audit.
         :param variable_map: Property variableMap: Log audit detailed configuration.
         :param multi_account: Property multiAccount: Multi-account configuration, please fill in multiple aliuid.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(AuditProps.__init__)
+            check_type(argname="argument display_name", value=display_name, expected_type=type_hints["display_name"])
+            check_type(argname="argument variable_map", value=variable_map, expected_type=type_hints["variable_map"])
+            check_type(argname="argument multi_account", value=multi_account, expected_type=type_hints["multi_account"])
         self._values: typing.Dict[str, typing.Any] = {
             "display_name": display_name,
             "variable_map": variable_map,
         }
         if multi_account is not None:
             self._values["multi_account"] = multi_account
 
@@ -313,37 +347,43 @@
 ):
     '''A ROS resource type:  ``ALIYUN::SLS::Dashboard``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "DashboardProps",
+        props: typing.Union["DashboardProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::SLS::Dashboard``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(Dashboard.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDashboardName")
     def attr_dashboard_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute DashboardName: Dashboard name.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDashboardName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDisplayName")
     def attr_display_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute DisplayName: Display name.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDisplayName"))
 
 
 @jsii.data_type(
@@ -371,14 +411,21 @@
 
         :param charts: Property charts: Chart list.
         :param dashboard_name: Property dashboardName: Dashboard name.
         :param project_name: Property projectName: Project name: 1. Only supports lowercase letters, numbers, hyphens (-) and underscores (_). 2. Must start and end with lowercase letters and numbers. 3. The name length is 3-63 characters.
         :param description: Property description: Dashboard description.
         :param display_name: Property displayName: Dashboard display name.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(DashboardProps.__init__)
+            check_type(argname="argument charts", value=charts, expected_type=type_hints["charts"])
+            check_type(argname="argument dashboard_name", value=dashboard_name, expected_type=type_hints["dashboard_name"])
+            check_type(argname="argument project_name", value=project_name, expected_type=type_hints["project_name"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument display_name", value=display_name, expected_type=type_hints["display_name"])
         self._values: typing.Dict[str, typing.Any] = {
             "charts": charts,
             "dashboard_name": dashboard_name,
             "project_name": project_name,
         }
         if description is not None:
             self._values["description"] = description
@@ -448,31 +495,37 @@
 ):
     '''A ROS resource type:  ``ALIYUN::SLS::Etl``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "EtlProps",
+        props: typing.Union["EtlProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::SLS::Etl``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(Etl.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrName")
     def attr_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute Name: ETL name.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrName"))
 
 
 @jsii.data_type(
@@ -487,30 +540,38 @@
         "description": "description",
     },
 )
 class EtlProps:
     def __init__(
         self,
         *,
-        configuration: typing.Union[ros_cdk_core.IResolvable, "RosEtl.ConfigurationProperty"],
+        configuration: typing.Union[ros_cdk_core.IResolvable, typing.Union["RosEtl.ConfigurationProperty", typing.Dict[str, typing.Any]]],
         display_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         project_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
-        schedule: typing.Union[ros_cdk_core.IResolvable, "RosEtl.ScheduleProperty"],
+        schedule: typing.Union[ros_cdk_core.IResolvable, typing.Union["RosEtl.ScheduleProperty", typing.Dict[str, typing.Any]]],
         description: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::SLS::Etl``.
 
         :param configuration: Property configuration: The configuration of ETL task.
         :param display_name: Property displayName: ETL display name.
         :param name: Property name: ETL name.
         :param project_name: Property projectName: Project name.
         :param schedule: Property schedule: Task scheduling strategy.
         :param description: Property description: ETL description message.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(EtlProps.__init__)
+            check_type(argname="argument configuration", value=configuration, expected_type=type_hints["configuration"])
+            check_type(argname="argument display_name", value=display_name, expected_type=type_hints["display_name"])
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+            check_type(argname="argument project_name", value=project_name, expected_type=type_hints["project_name"])
+            check_type(argname="argument schedule", value=schedule, expected_type=type_hints["schedule"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
         self._values: typing.Dict[str, typing.Any] = {
             "configuration": configuration,
             "display_name": display_name,
             "name": name,
             "project_name": project_name,
             "schedule": schedule,
         }
@@ -583,28 +644,34 @@
 ):
     '''A ROS resource type:  ``ALIYUN::SLS::Index``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "IndexProps",
+        props: typing.Union["IndexProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::SLS::Index``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(Index.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-sls.IndexProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -615,28 +682,35 @@
         "log_reduce": "logReduce",
     },
 )
 class IndexProps:
     def __init__(
         self,
         *,
-        full_text_index: typing.Union[ros_cdk_core.IResolvable, "RosIndex.FullTextIndexProperty"],
+        full_text_index: typing.Union[ros_cdk_core.IResolvable, typing.Union["RosIndex.FullTextIndexProperty", typing.Dict[str, typing.Any]]],
         logstore_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         project_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
-        key_indices: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosIndex.KeyIndicesProperty"]]]] = None,
+        key_indices: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosIndex.KeyIndicesProperty", typing.Dict[str, typing.Any]]]]]] = None,
         log_reduce: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::SLS::Index``.
 
         :param full_text_index: Property fullTextIndex: Full-text indexing configuration. Full-text indexing and key indexing must have at least one enabled.
         :param logstore_name: Property logstoreName: Logstore name: 1. Only supports lowercase letters, numbers, hyphens (-) and underscores (_). 2. Must start and end with lowercase letters and numbers. 3. The name length is 3-63 characters.
         :param project_name: Property projectName: Project name: 1. Only supports lowercase letters, numbers, hyphens (-) and underscores (_). 2. Must start and end with lowercase letters and numbers. 3. The name length is 3-63 characters.
         :param key_indices: Property keyIndices: Key index configurations. Full-text indexing and key indexing must have at least one enabled.
         :param log_reduce: Property logReduce: Whether to enable log reduce. Default to false.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(IndexProps.__init__)
+            check_type(argname="argument full_text_index", value=full_text_index, expected_type=type_hints["full_text_index"])
+            check_type(argname="argument logstore_name", value=logstore_name, expected_type=type_hints["logstore_name"])
+            check_type(argname="argument project_name", value=project_name, expected_type=type_hints["project_name"])
+            check_type(argname="argument key_indices", value=key_indices, expected_type=type_hints["key_indices"])
+            check_type(argname="argument log_reduce", value=log_reduce, expected_type=type_hints["log_reduce"])
         self._values: typing.Dict[str, typing.Any] = {
             "full_text_index": full_text_index,
             "logstore_name": logstore_name,
             "project_name": project_name,
         }
         if key_indices is not None:
             self._values["key_indices"] = key_indices
@@ -720,31 +794,37 @@
 ):
     '''A ROS resource type:  ``ALIYUN::SLS::Logstore``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "LogstoreProps",
+        props: typing.Union["LogstoreProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::SLS::Logstore``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(Logstore.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrLogstoreName")
     def attr_logstore_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute LogstoreName: Logstore name.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrLogstoreName"))
 
 
 @jsii.data_type(
@@ -768,15 +848,15 @@
         self,
         *,
         logstore_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         project_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         append_meta: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         auto_split: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         enable_tracking: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
-        encrypt_conf: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosLogstore.EncryptConfProperty"]] = None,
+        encrypt_conf: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosLogstore.EncryptConfProperty", typing.Dict[str, typing.Any]]]] = None,
         max_split_shard: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         preserve_storage: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         shard_count: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         ttl: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::SLS::Logstore``.
 
@@ -787,14 +867,26 @@
         :param enable_tracking: Property enableTracking: Whether to enable WebTracking, which supports fast capture of various browsers and iOS/Android/APP access information. Default to false.
         :param encrypt_conf: Property encryptConf: Data encryption config.
         :param max_split_shard: Property maxSplitShard: The maximum number of shards when splitting automatically. Must be specified if AutoSplit is set to true. Allowed Values: 1-64.
         :param preserve_storage: Property preserveStorage: Whether to keep the log permanently. If set to true, TTL will be ignored. Default to false.
         :param shard_count: Property shardCount: The number of Shards. Allowed Values: 1-100, default to 2.
         :param ttl: Property ttl: The lifecycle of log in the logstore in days. Allowed Values: 1-3600, default to 30.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(LogstoreProps.__init__)
+            check_type(argname="argument logstore_name", value=logstore_name, expected_type=type_hints["logstore_name"])
+            check_type(argname="argument project_name", value=project_name, expected_type=type_hints["project_name"])
+            check_type(argname="argument append_meta", value=append_meta, expected_type=type_hints["append_meta"])
+            check_type(argname="argument auto_split", value=auto_split, expected_type=type_hints["auto_split"])
+            check_type(argname="argument enable_tracking", value=enable_tracking, expected_type=type_hints["enable_tracking"])
+            check_type(argname="argument encrypt_conf", value=encrypt_conf, expected_type=type_hints["encrypt_conf"])
+            check_type(argname="argument max_split_shard", value=max_split_shard, expected_type=type_hints["max_split_shard"])
+            check_type(argname="argument preserve_storage", value=preserve_storage, expected_type=type_hints["preserve_storage"])
+            check_type(argname="argument shard_count", value=shard_count, expected_type=type_hints["shard_count"])
+            check_type(argname="argument ttl", value=ttl, expected_type=type_hints["ttl"])
         self._values: typing.Dict[str, typing.Any] = {
             "logstore_name": logstore_name,
             "project_name": project_name,
         }
         if append_meta is not None:
             self._values["append_meta"] = append_meta
         if auto_split is not None:
@@ -942,43 +1034,49 @@
 ):
     '''A ROS resource type:  ``ALIYUN::SLS::LogtailConfig``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "LogtailConfigProps",
+        props: typing.Union["LogtailConfigProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::SLS::LogtailConfig``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(LogtailConfig.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrAppliedMachineGroups")
     def attr_applied_machine_groups(self) -> ros_cdk_core.IResolvable:
         '''Attribute AppliedMachineGroups: Applied machine groups.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAppliedMachineGroups"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrEndpoint")
     def attr_endpoint(self) -> ros_cdk_core.IResolvable:
         '''Attribute Endpoint: Endpoint address.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrEndpoint"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrLogtailConfigName")
     def attr_logtail_config_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute LogtailConfigName: Logtail config name.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrLogtailConfigName"))
 
 
 @jsii.data_type(
@@ -995,25 +1093,32 @@
 class LogtailConfigProps:
     def __init__(
         self,
         *,
         logstore_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         logtail_config_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         project_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
-        clone_from: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosLogtailConfig.CloneFromProperty"]] = None,
+        clone_from: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosLogtailConfig.CloneFromProperty", typing.Dict[str, typing.Any]]]] = None,
         raw_config_data: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::SLS::LogtailConfig``.
 
         :param logstore_name: Property logstoreName: Logstore name: 1. Only supports lowercase letters, numbers, hyphens (-) and underscores (_). 2. Must start and end with lowercase letters and numbers. 3. The name length is 3-63 characters.
         :param logtail_config_name: Property logtailConfigName: Logtail config name: 1. Only supports lowercase letters, numbers, hyphens (-) and underscores (_). 2. Must start and end with lowercase letters and numbers. 3. The name length is 3-63 characters.
         :param project_name: Property projectName: Project name: 1. Only supports lowercase letters, numbers, hyphens (-) and underscores (_). 2. Must start and end with lowercase letters and numbers. 3. The name length is 3-63 characters.
         :param clone_from: Property cloneFrom: Clone logtail config data from existing logtail config. Either CloneFrom or RawConfigData must be specified. If CloneFrom and RawConfigData are both specified, logtail config data will be merged from both with RawConfigData first.
         :param raw_config_data: Property rawConfigData: The format is the same as the response of SLS API GetConfig. Either CloneFrom or RawConfigData must be specified. If CloneFrom and RawConfigData are both specified, logtail config data will be merged from both with RawConfigData first. configName, outputType, outputDetail in data will be ignored.For example: { "configName": "test-logtail-config", "createTime": 1574843554, "inputDetail": { "acceptNoEnoughKeys": false, "adjustTimezone": false, "advanced": { "force_multiconfig": false }, "autoExtend": true, "delayAlarmBytes": 0, "delaySkipBytes": 0, "discardNonUtf8": false, "discardUnmatch": false, "dockerExcludeEnv": {}, "dockerExcludeLabel": {}, "dockerFile": false, "dockerIncludeEnv": {}, "dockerIncludeLabel": {}, "enableRawLog": false, "enableTag": false, "fileEncoding": "utf8", "filePattern": "test.log*", "filterKey": [], "filterRegex": [], "key": [ "time", "logger", "level", "request_id", "user_id", "region_id", "content" ], "localStorage": true, "logPath": "/var/log/test", "logTimezone": "", "logType": "delimiter_log", "maxDepth": 100, "maxSendRate": -1, "mergeType": "topic", "preserve": true, "preserveDepth": 1, "priority": 0, "quote": "\\u0001", "sendRateExpire": 0, "sensitive_keys": [], "separator": ",,,", "shardHashKey": [], "tailExisted": false, "timeFormat": "", "timeKey": "", "topicFormat": "none" }, "inputType": "file", "lastModifyTime": 1574843554, "logSample": "2019-11-27 10:48:23,160,,,MAIN,,,INFO,,,98DCC51D-BE5D-49C7-B3FD-37B2BAEFB296,,,123456789,,,cn-hangzhou,,,this is a simple test.", "outputDetail": { "endpoint": "cn-hangzhou-intranet.log.aliyuncs.com", "logstoreName": "test-logstore", "region": "cn-hangzhou" }, "outputType": "LogService" }
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(LogtailConfigProps.__init__)
+            check_type(argname="argument logstore_name", value=logstore_name, expected_type=type_hints["logstore_name"])
+            check_type(argname="argument logtail_config_name", value=logtail_config_name, expected_type=type_hints["logtail_config_name"])
+            check_type(argname="argument project_name", value=project_name, expected_type=type_hints["project_name"])
+            check_type(argname="argument clone_from", value=clone_from, expected_type=type_hints["clone_from"])
+            check_type(argname="argument raw_config_data", value=raw_config_data, expected_type=type_hints["raw_config_data"])
         self._values: typing.Dict[str, typing.Any] = {
             "logstore_name": logstore_name,
             "logtail_config_name": logtail_config_name,
             "project_name": project_name,
         }
         if clone_from is not None:
             self._values["clone_from"] = clone_from
@@ -1164,37 +1269,43 @@
 ):
     '''A ROS resource type:  ``ALIYUN::SLS::MachineGroup``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: typing.Optional["MachineGroupProps"] = None,
+        props: typing.Optional[typing.Union["MachineGroupProps", typing.Dict[str, typing.Any]]] = None,
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::SLS::MachineGroup``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(MachineGroup.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrGroupName")
     def attr_group_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute GroupName: GroupName of SLS.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrGroupName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrProjectName")
     def attr_project_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute ProjectName: ProjectName of SLS.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrProjectName"))
 
 
 @jsii.data_type(
@@ -1225,14 +1336,22 @@
         :param group_attribute: Property groupAttribute: Group attribute, default is null. The object value is groupToic and externalName
         :param group_name: Property groupName: Display name of the group name, the Project only. [2, 128] English or Chinese characters, must start with a letter or Chinese in size, can contain numbers, '_' or '.', '-'
         :param group_type: Property groupType: MachineGroup type, the value is empty or Armory.
         :param machine_identify_type: Property machineIdentifyType: Machine indentify type, the value is 'ip' or 'userdefined'.
         :param machine_list: Property machineList: The machine tag, the value is ip or userdefined-id.
         :param project_name: Property projectName: MachineGroup created in project.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(MachineGroupProps.__init__)
+            check_type(argname="argument group_attribute", value=group_attribute, expected_type=type_hints["group_attribute"])
+            check_type(argname="argument group_name", value=group_name, expected_type=type_hints["group_name"])
+            check_type(argname="argument group_type", value=group_type, expected_type=type_hints["group_type"])
+            check_type(argname="argument machine_identify_type", value=machine_identify_type, expected_type=type_hints["machine_identify_type"])
+            check_type(argname="argument machine_list", value=machine_list, expected_type=type_hints["machine_list"])
+            check_type(argname="argument project_name", value=project_name, expected_type=type_hints["project_name"])
         self._values: typing.Dict[str, typing.Any] = {}
         if group_attribute is not None:
             self._values["group_attribute"] = group_attribute
         if group_name is not None:
             self._values["group_name"] = group_name
         if group_type is not None:
             self._values["group_type"] = group_type
@@ -1316,31 +1435,37 @@
 ):
     '''A ROS resource type:  ``ALIYUN::SLS::MetricStore``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "MetricStoreProps",
+        props: typing.Union["MetricStoreProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::SLS::MetricStore``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(MetricStore.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrLogstoreName")
     def attr_logstore_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute LogstoreName: Metric store name.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrLogstoreName"))
 
 
 @jsii.data_type(
@@ -1368,14 +1493,21 @@
 
         :param logstore_name: Property logstoreName: Metric store name: 1. Only supports lowercase letters, numbers, hyphens (-) and underscores (_). 2. Must start and end with lowercase letters and numbers. 3. The name length is 3-63 characters.
         :param project_name: Property projectName: Project name: 1. Only supports lowercase letters, numbers, hyphens (-) and underscores (_). 2. Must start and end with lowercase letters and numbers. 3. The name length is 3-63 characters.
         :param preserve_storage: Property preserveStorage: Whether to keep the log permanently. If set to true, TTL will be ignored. Default to false.
         :param shard_count: Property shardCount: The number of Shards. Allowed Values: 1-10, default to 2.
         :param ttl: Property ttl: The lifecycle of log in the metrice store in days. Allowed Values: 1-3000, default to 30.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(MetricStoreProps.__init__)
+            check_type(argname="argument logstore_name", value=logstore_name, expected_type=type_hints["logstore_name"])
+            check_type(argname="argument project_name", value=project_name, expected_type=type_hints["project_name"])
+            check_type(argname="argument preserve_storage", value=preserve_storage, expected_type=type_hints["preserve_storage"])
+            check_type(argname="argument shard_count", value=shard_count, expected_type=type_hints["shard_count"])
+            check_type(argname="argument ttl", value=ttl, expected_type=type_hints["ttl"])
         self._values: typing.Dict[str, typing.Any] = {
             "logstore_name": logstore_name,
             "project_name": project_name,
         }
         if preserve_storage is not None:
             self._values["preserve_storage"] = preserve_storage
         if shard_count is not None:
@@ -1460,31 +1592,37 @@
 ):
     '''A ROS resource type:  ``ALIYUN::SLS::Project``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "ProjectProps",
+        props: typing.Union["ProjectProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::SLS::Project``.
 
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
     @jsii.member(jsii_name="attrName")
     def attr_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute Name: Project name.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrName"))
 
 
 @jsii.data_type(
@@ -1494,22 +1632,27 @@
 )
 class ProjectProps:
     def __init__(
         self,
         *,
         name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         description: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        tags: typing.Optional[typing.Sequence["RosProject.TagsProperty"]] = None,
+        tags: typing.Optional[typing.Sequence[typing.Union["RosProject.TagsProperty", typing.Dict[str, typing.Any]]]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::SLS::Project``.
 
         :param name: Property name: Project name: 1. Only supports lowercase letters, numbers, hyphens (-) and underscores (_). 2. Must start and end with lowercase letters and numbers. 3. The name length is 3-63 characters.
         :param description: Property description: Project description: <>'"\\ is not supported, up to 64 characters.
         :param tags: Property tags: Tags to attach to project. Max support 20 tags to add during create project. Each tag with two properties Key and Value, and Key is required.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(ProjectProps.__init__)
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
         self._values: typing.Dict[str, typing.Any] = {
             "name": name,
         }
         if description is not None:
             self._values["description"] = description
         if tags is not None:
             self._values["tags"] = tags
@@ -1562,82 +1705,97 @@
 ):
     '''A ROS template type:  ``ALIYUN::SLS::Alert``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosAlertProps",
+        props: typing.Union["RosAlertProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::SLS::Alert``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosAlert.__init__)
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
+            type_hints = typing.get_type_hints(RosAlert._render_properties)
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
         :Attribute: Name: Alert name.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="detail")
     def detail(
         self,
     ) -> typing.Union["RosAlert.DetailProperty", ros_cdk_core.IResolvable]:
         '''
         :Property: detail:
         '''
         return typing.cast(typing.Union["RosAlert.DetailProperty", ros_cdk_core.IResolvable], jsii.get(self, "detail"))
 
     @detail.setter
     def detail(
         self,
         value: typing.Union["RosAlert.DetailProperty", ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAlert, "detail").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "detail", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAlert, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="project")
     def project(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         project: Project name:
 
@@ -1648,14 +1806,17 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "project"))
 
     @project.setter
     def project(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAlert, "project").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "project", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-sls.RosAlert.AnnotationsProperty",
         jsii_struct_bases=[],
         name_mapping={"key": "key", "value": "value"},
     )
@@ -1666,14 +1827,18 @@
             key: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         ) -> None:
             '''
             :param key: 
             :param value: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosAlert.AnnotationsProperty.__init__)
+                check_type(argname="argument key", value=key, expected_type=type_hints["key"])
+                check_type(argname="argument value", value=value, expected_type=type_hints["value"])
             self._values: typing.Dict[str, typing.Any] = {
                 "key": key,
                 "value": value,
             }
 
         @builtins.property
         def key(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
@@ -1731,29 +1896,29 @@
         },
     )
     class ConfigurationProperty:
         def __init__(
             self,
             *,
             dashboard: typing.Union[builtins.str, ros_cdk_core.IResolvable],
-            query_list: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosAlert.QueryListProperty"]]],
-            annotations: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosAlert.AnnotationsProperty"]]]] = None,
+            query_list: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosAlert.QueryListProperty", typing.Dict[str, typing.Any]]]]],
+            annotations: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosAlert.AnnotationsProperty", typing.Dict[str, typing.Any]]]]]] = None,
             auto_annotation: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
             condition: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-            group_configuration: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosAlert.GroupConfigurationProperty"]] = None,
-            join_configurations: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosAlert.JoinConfigurationsProperty"]]]] = None,
-            labels: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosAlert.LabelsProperty"]]]] = None,
+            group_configuration: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosAlert.GroupConfigurationProperty", typing.Dict[str, typing.Any]]]] = None,
+            join_configurations: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosAlert.JoinConfigurationsProperty", typing.Dict[str, typing.Any]]]]]] = None,
+            labels: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosAlert.LabelsProperty", typing.Dict[str, typing.Any]]]]]] = None,
             mute_until: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
             no_data_fire: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
             no_data_severity: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
-            notification_list: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosAlert.NotificationListProperty"]]]] = None,
+            notification_list: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosAlert.NotificationListProperty", typing.Dict[str, typing.Any]]]]]] = None,
             notify_threshold: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
-            policy_configuration: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosAlert.PolicyConfigurationProperty"]] = None,
+            policy_configuration: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosAlert.PolicyConfigurationProperty", typing.Dict[str, typing.Any]]]] = None,
             send_resolved: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
-            severity_configurations: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosAlert.SeverityConfigurationsProperty"]]]] = None,
+            severity_configurations: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosAlert.SeverityConfigurationsProperty", typing.Dict[str, typing.Any]]]]]] = None,
             threshold: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
             throttling: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
             type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
             version: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param dashboard: 
@@ -1773,14 +1938,36 @@
             :param send_resolved: 
             :param severity_configurations: 
             :param threshold: 
             :param throttling: 
             :param type: 
             :param version: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosAlert.ConfigurationProperty.__init__)
+                check_type(argname="argument dashboard", value=dashboard, expected_type=type_hints["dashboard"])
+                check_type(argname="argument query_list", value=query_list, expected_type=type_hints["query_list"])
+                check_type(argname="argument annotations", value=annotations, expected_type=type_hints["annotations"])
+                check_type(argname="argument auto_annotation", value=auto_annotation, expected_type=type_hints["auto_annotation"])
+                check_type(argname="argument condition", value=condition, expected_type=type_hints["condition"])
+                check_type(argname="argument group_configuration", value=group_configuration, expected_type=type_hints["group_configuration"])
+                check_type(argname="argument join_configurations", value=join_configurations, expected_type=type_hints["join_configurations"])
+                check_type(argname="argument labels", value=labels, expected_type=type_hints["labels"])
+                check_type(argname="argument mute_until", value=mute_until, expected_type=type_hints["mute_until"])
+                check_type(argname="argument no_data_fire", value=no_data_fire, expected_type=type_hints["no_data_fire"])
+                check_type(argname="argument no_data_severity", value=no_data_severity, expected_type=type_hints["no_data_severity"])
+                check_type(argname="argument notification_list", value=notification_list, expected_type=type_hints["notification_list"])
+                check_type(argname="argument notify_threshold", value=notify_threshold, expected_type=type_hints["notify_threshold"])
+                check_type(argname="argument policy_configuration", value=policy_configuration, expected_type=type_hints["policy_configuration"])
+                check_type(argname="argument send_resolved", value=send_resolved, expected_type=type_hints["send_resolved"])
+                check_type(argname="argument severity_configurations", value=severity_configurations, expected_type=type_hints["severity_configurations"])
+                check_type(argname="argument threshold", value=threshold, expected_type=type_hints["threshold"])
+                check_type(argname="argument throttling", value=throttling, expected_type=type_hints["throttling"])
+                check_type(argname="argument type", value=type, expected_type=type_hints["type"])
+                check_type(argname="argument version", value=version, expected_type=type_hints["version"])
             self._values: typing.Dict[str, typing.Any] = {
                 "dashboard": dashboard,
                 "query_list": query_list,
             }
             if annotations is not None:
                 self._values["annotations"] = annotations
             if auto_annotation is not None:
@@ -2056,31 +2243,40 @@
             "type": "type",
         },
     )
     class DetailProperty:
         def __init__(
             self,
             *,
-            configuration: typing.Union[ros_cdk_core.IResolvable, "RosAlert.ConfigurationProperty"],
+            configuration: typing.Union[ros_cdk_core.IResolvable, typing.Union["RosAlert.ConfigurationProperty", typing.Dict[str, typing.Any]]],
             display_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
-            schedule: typing.Union[ros_cdk_core.IResolvable, "RosAlert.ScheduleProperty"],
+            schedule: typing.Union[ros_cdk_core.IResolvable, typing.Union["RosAlert.ScheduleProperty", typing.Dict[str, typing.Any]]],
             description: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
             state: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
             type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param configuration: 
             :param display_name: 
             :param name: 
             :param schedule: 
             :param description: 
             :param state: 
             :param type: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosAlert.DetailProperty.__init__)
+                check_type(argname="argument configuration", value=configuration, expected_type=type_hints["configuration"])
+                check_type(argname="argument display_name", value=display_name, expected_type=type_hints["display_name"])
+                check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+                check_type(argname="argument schedule", value=schedule, expected_type=type_hints["schedule"])
+                check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+                check_type(argname="argument state", value=state, expected_type=type_hints["state"])
+                check_type(argname="argument type", value=type, expected_type=type_hints["type"])
             self._values: typing.Dict[str, typing.Any] = {
                 "configuration": configuration,
                 "display_name": display_name,
                 "name": name,
                 "schedule": schedule,
             }
             if description is not None:
@@ -2187,14 +2383,18 @@
             condition: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
             count_condition: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param condition: 
             :param count_condition: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosAlert.EvalConditionProperty.__init__)
+                check_type(argname="argument condition", value=condition, expected_type=type_hints["condition"])
+                check_type(argname="argument count_condition", value=count_condition, expected_type=type_hints["count_condition"])
             self._values: typing.Dict[str, typing.Any] = {}
             if condition is not None:
                 self._values["condition"] = condition
             if count_condition is not None:
                 self._values["count_condition"] = count_condition
 
         @builtins.property
@@ -2240,14 +2440,18 @@
             type: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             fields: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]] = None,
         ) -> None:
             '''
             :param type: 
             :param fields: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosAlert.GroupConfigurationProperty.__init__)
+                check_type(argname="argument type", value=type, expected_type=type_hints["type"])
+                check_type(argname="argument fields", value=fields, expected_type=type_hints["fields"])
             self._values: typing.Dict[str, typing.Any] = {
                 "type": type,
             }
             if fields is not None:
                 self._values["fields"] = fields
 
         @builtins.property
@@ -2296,14 +2500,18 @@
             type: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             condition: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param type: 
             :param condition: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosAlert.JoinConfigurationsProperty.__init__)
+                check_type(argname="argument type", value=type, expected_type=type_hints["type"])
+                check_type(argname="argument condition", value=condition, expected_type=type_hints["condition"])
             self._values: typing.Dict[str, typing.Any] = {
                 "type": type,
             }
             if condition is not None:
                 self._values["condition"] = condition
 
         @builtins.property
@@ -2348,14 +2556,18 @@
             key: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         ) -> None:
             '''
             :param key: 
             :param value: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosAlert.LabelsProperty.__init__)
+                check_type(argname="argument key", value=key, expected_type=type_hints["key"])
+                check_type(argname="argument value", value=value, expected_type=type_hints["value"])
             self._values: typing.Dict[str, typing.Any] = {
                 "key": key,
                 "value": value,
             }
 
         @builtins.property
         def key(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
@@ -2416,14 +2628,23 @@
             :param content: 
             :param email_list: 
             :param headers: 
             :param method: 
             :param mobile_list: 
             :param service_uri: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosAlert.NotificationListProperty.__init__)
+                check_type(argname="argument type", value=type, expected_type=type_hints["type"])
+                check_type(argname="argument content", value=content, expected_type=type_hints["content"])
+                check_type(argname="argument email_list", value=email_list, expected_type=type_hints["email_list"])
+                check_type(argname="argument headers", value=headers, expected_type=type_hints["headers"])
+                check_type(argname="argument method", value=method, expected_type=type_hints["method"])
+                check_type(argname="argument mobile_list", value=mobile_list, expected_type=type_hints["mobile_list"])
+                check_type(argname="argument service_uri", value=service_uri, expected_type=type_hints["service_uri"])
             self._values: typing.Dict[str, typing.Any] = {
                 "type": type,
             }
             if content is not None:
                 self._values["content"] = content
             if email_list is not None:
                 self._values["email_list"] = email_list
@@ -2542,14 +2763,20 @@
         ) -> None:
             '''
             :param action_policy_id: 
             :param alert_policy_id: 
             :param repeat_interval: 
             :param use_default: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosAlert.PolicyConfigurationProperty.__init__)
+                check_type(argname="argument action_policy_id", value=action_policy_id, expected_type=type_hints["action_policy_id"])
+                check_type(argname="argument alert_policy_id", value=alert_policy_id, expected_type=type_hints["alert_policy_id"])
+                check_type(argname="argument repeat_interval", value=repeat_interval, expected_type=type_hints["repeat_interval"])
+                check_type(argname="argument use_default", value=use_default, expected_type=type_hints["use_default"])
             self._values: typing.Dict[str, typing.Any] = {}
             if action_policy_id is not None:
                 self._values["action_policy_id"] = action_policy_id
             if alert_policy_id is not None:
                 self._values["alert_policy_id"] = alert_policy_id
             if repeat_interval is not None:
                 self._values["repeat_interval"] = repeat_interval
@@ -2655,14 +2882,29 @@
             :param power_sql_mode: 
             :param project: 
             :param region: 
             :param role_arn: 
             :param store: 
             :param store_type: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosAlert.QueryListProperty.__init__)
+                check_type(argname="argument end", value=end, expected_type=type_hints["end"])
+                check_type(argname="argument query", value=query, expected_type=type_hints["query"])
+                check_type(argname="argument start", value=start, expected_type=type_hints["start"])
+                check_type(argname="argument time_span_type", value=time_span_type, expected_type=type_hints["time_span_type"])
+                check_type(argname="argument chart_title", value=chart_title, expected_type=type_hints["chart_title"])
+                check_type(argname="argument dashboard_id", value=dashboard_id, expected_type=type_hints["dashboard_id"])
+                check_type(argname="argument log_store", value=log_store, expected_type=type_hints["log_store"])
+                check_type(argname="argument power_sql_mode", value=power_sql_mode, expected_type=type_hints["power_sql_mode"])
+                check_type(argname="argument project", value=project, expected_type=type_hints["project"])
+                check_type(argname="argument region", value=region, expected_type=type_hints["region"])
+                check_type(argname="argument role_arn", value=role_arn, expected_type=type_hints["role_arn"])
+                check_type(argname="argument store", value=store, expected_type=type_hints["store"])
+                check_type(argname="argument store_type", value=store_type, expected_type=type_hints["store_type"])
             self._values: typing.Dict[str, typing.Any] = {
                 "end": end,
                 "query": query,
                 "start": start,
                 "time_span_type": time_span_type,
             }
             if chart_title is not None:
@@ -2861,14 +3103,23 @@
             :param cron_expression: 
             :param day_of_week: 
             :param delay: 
             :param hour: 
             :param interval: 
             :param run_immediately: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosAlert.ScheduleProperty.__init__)
+                check_type(argname="argument type", value=type, expected_type=type_hints["type"])
+                check_type(argname="argument cron_expression", value=cron_expression, expected_type=type_hints["cron_expression"])
+                check_type(argname="argument day_of_week", value=day_of_week, expected_type=type_hints["day_of_week"])
+                check_type(argname="argument delay", value=delay, expected_type=type_hints["delay"])
+                check_type(argname="argument hour", value=hour, expected_type=type_hints["hour"])
+                check_type(argname="argument interval", value=interval, expected_type=type_hints["interval"])
+                check_type(argname="argument run_immediately", value=run_immediately, expected_type=type_hints["run_immediately"])
             self._values: typing.Dict[str, typing.Any] = {
                 "type": type,
             }
             if cron_expression is not None:
                 self._values["cron_expression"] = cron_expression
             if day_of_week is not None:
                 self._values["day_of_week"] = day_of_week
@@ -2967,20 +3218,24 @@
         name_mapping={"severity": "severity", "eval_condition": "evalCondition"},
     )
     class SeverityConfigurationsProperty:
         def __init__(
             self,
             *,
             severity: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
-            eval_condition: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosAlert.EvalConditionProperty"]] = None,
+            eval_condition: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosAlert.EvalConditionProperty", typing.Dict[str, typing.Any]]]] = None,
         ) -> None:
             '''
             :param severity: 
             :param eval_condition: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosAlert.SeverityConfigurationsProperty.__init__)
+                check_type(argname="argument severity", value=severity, expected_type=type_hints["severity"])
+                check_type(argname="argument eval_condition", value=eval_condition, expected_type=type_hints["eval_condition"])
             self._values: typing.Dict[str, typing.Any] = {
                 "severity": severity,
             }
             if eval_condition is not None:
                 self._values["eval_condition"] = eval_condition
 
         @builtins.property
@@ -3026,22 +3281,26 @@
     jsii_struct_bases=[],
     name_mapping={"detail": "detail", "project": "project"},
 )
 class RosAlertProps:
     def __init__(
         self,
         *,
-        detail: typing.Union[RosAlert.DetailProperty, ros_cdk_core.IResolvable],
+        detail: typing.Union[typing.Union[RosAlert.DetailProperty, typing.Dict[str, typing.Any]], ros_cdk_core.IResolvable],
         project: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
         '''Properties for defining a ``ALIYUN::SLS::Alert``.
 
         :param detail: 
         :param project: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosAlertProps.__init__)
+            check_type(argname="argument detail", value=detail, expected_type=type_hints["detail"])
+            check_type(argname="argument project", value=project, expected_type=type_hints["project"])
         self._values: typing.Dict[str, typing.Any] = {
             "detail": detail,
             "project": project,
         }
 
     @builtins.property
     def detail(self) -> typing.Union[RosAlert.DetailProperty, ros_cdk_core.IResolvable]:
@@ -3086,106 +3345,127 @@
 ):
     '''A ROS template type:  ``ALIYUN::SLS::ApplyConfigToMachineGroup``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosApplyConfigToMachineGroupProps",
+        props: typing.Union["RosApplyConfigToMachineGroupProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::SLS::ApplyConfigToMachineGroup``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosApplyConfigToMachineGroup.__init__)
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
+            type_hints = typing.get_type_hints(RosApplyConfigToMachineGroup._render_properties)
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
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         '''A factory method that creates a new instance of this class from an object containing the properties of this ROS resource.'''
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosApplyConfigToMachineGroup, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="configName")
     def config_name(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: configName: Apply config to the config name
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "configName"))
 
     @config_name.setter
     def config_name(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosApplyConfigToMachineGroup, "config_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "configName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="groupName")
     def group_name(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: groupName: Apply config to the group name
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "groupName"))
 
     @group_name.setter
     def group_name(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosApplyConfigToMachineGroup, "group_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "groupName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="projectName")
     def project_name(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: projectName: Apply config to the project name.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "projectName"))
 
     @project_name.setter
     def project_name(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosApplyConfigToMachineGroup, "project_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "projectName", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-sls.RosApplyConfigToMachineGroupProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -3204,14 +3484,19 @@
     ) -> None:
         '''Properties for defining a ``ALIYUN::SLS::ApplyConfigToMachineGroup``.
 
         :param config_name: 
         :param group_name: 
         :param project_name: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosApplyConfigToMachineGroupProps.__init__)
+            check_type(argname="argument config_name", value=config_name, expected_type=type_hints["config_name"])
+            check_type(argname="argument group_name", value=group_name, expected_type=type_hints["group_name"])
+            check_type(argname="argument project_name", value=project_name, expected_type=type_hints["project_name"])
         self._values: typing.Dict[str, typing.Any] = {}
         if config_name is not None:
             self._values["config_name"] = config_name
         if group_name is not None:
             self._values["group_name"] = group_name
         if project_name is not None:
             self._values["project_name"] = project_name
@@ -3265,111 +3550,132 @@
 ):
     '''A ROS template type:  ``ALIYUN::SLS::Audit``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosAuditProps",
+        props: typing.Union["RosAuditProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::SLS::Audit``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosAudit.__init__)
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
+            type_hints = typing.get_type_hints(RosAudit._render_properties)
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
     @jsii.member(jsii_name="attrDisplayName")
     def attr_display_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: DisplayName: Name of SLS log audit.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDisplayName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="displayName")
     def display_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: displayName: Name of SLS log audit.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "displayName"))
 
     @display_name.setter
     def display_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAudit, "display_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "displayName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAudit, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="variableMap")
     def variable_map(
         self,
     ) -> typing.Union[ros_cdk_core.IResolvable, "RosAudit.VariableMapProperty"]:
         '''
         :Property: variableMap: Log audit detailed configuration.
         '''
         return typing.cast(typing.Union[ros_cdk_core.IResolvable, "RosAudit.VariableMapProperty"], jsii.get(self, "variableMap"))
 
     @variable_map.setter
     def variable_map(
         self,
         value: typing.Union[ros_cdk_core.IResolvable, "RosAudit.VariableMapProperty"],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAudit, "variable_map").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "variableMap", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="multiAccount")
     def multi_account(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]]:
         '''
         :Property: multiAccount: Multi-account configuration, please fill in multiple aliuid.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]], jsii.get(self, "multiAccount"))
 
     @multi_account.setter
     def multi_account(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAudit, "multi_account").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "multiAccount", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-sls.RosAudit.VariableMapProperty",
         jsii_struct_bases=[],
         name_mapping={
             "actiontrail_enabled": "actiontrailEnabled",
@@ -3794,14 +4100,155 @@
             :param slb_sync_ttl: 
             :param waf_access_collection_policy: 
             :param waf_access_policy_setting: 
             :param waf_enabled: 
             :param waf_ti_enabled: 
             :param waf_ttl: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosAudit.VariableMapProperty.__init__)
+                check_type(argname="argument actiontrail_enabled", value=actiontrail_enabled, expected_type=type_hints["actiontrail_enabled"])
+                check_type(argname="argument actiontrail_openapi_collection_policy", value=actiontrail_openapi_collection_policy, expected_type=type_hints["actiontrail_openapi_collection_policy"])
+                check_type(argname="argument actiontrail_openapi_policy_setting", value=actiontrail_openapi_policy_setting, expected_type=type_hints["actiontrail_openapi_policy_setting"])
+                check_type(argname="argument actiontrail_ti_enabled", value=actiontrail_ti_enabled, expected_type=type_hints["actiontrail_ti_enabled"])
+                check_type(argname="argument actiontrail_ttl", value=actiontrail_ttl, expected_type=type_hints["actiontrail_ttl"])
+                check_type(argname="argument apigateway_access_collection_policy", value=apigateway_access_collection_policy, expected_type=type_hints["apigateway_access_collection_policy"])
+                check_type(argname="argument apigateway_access_policy_setting", value=apigateway_access_policy_setting, expected_type=type_hints["apigateway_access_policy_setting"])
+                check_type(argname="argument apigateway_enabled", value=apigateway_enabled, expected_type=type_hints["apigateway_enabled"])
+                check_type(argname="argument apigateway_ti_enabled", value=apigateway_ti_enabled, expected_type=type_hints["apigateway_ti_enabled"])
+                check_type(argname="argument apigateway_ttl", value=apigateway_ttl, expected_type=type_hints["apigateway_ttl"])
+                check_type(argname="argument appconnect_enabled", value=appconnect_enabled, expected_type=type_hints["appconnect_enabled"])
+                check_type(argname="argument appconnect_op_collection_policy", value=appconnect_op_collection_policy, expected_type=type_hints["appconnect_op_collection_policy"])
+                check_type(argname="argument appconnect_op_policy_setting", value=appconnect_op_policy_setting, expected_type=type_hints["appconnect_op_policy_setting"])
+                check_type(argname="argument appconnect_ti_enabled", value=appconnect_ti_enabled, expected_type=type_hints["appconnect_ti_enabled"])
+                check_type(argname="argument appconnect_ttl", value=appconnect_ttl, expected_type=type_hints["appconnect_ttl"])
+                check_type(argname="argument bastion_audit_collection_policy", value=bastion_audit_collection_policy, expected_type=type_hints["bastion_audit_collection_policy"])
+                check_type(argname="argument bastion_audit_policy_setting", value=bastion_audit_policy_setting, expected_type=type_hints["bastion_audit_policy_setting"])
+                check_type(argname="argument bastion_enabled", value=bastion_enabled, expected_type=type_hints["bastion_enabled"])
+                check_type(argname="argument bastion_ti_enabled", value=bastion_ti_enabled, expected_type=type_hints["bastion_ti_enabled"])
+                check_type(argname="argument bastion_ttl", value=bastion_ttl, expected_type=type_hints["bastion_ttl"])
+                check_type(argname="argument cloudfirewall_access_collection_policy", value=cloudfirewall_access_collection_policy, expected_type=type_hints["cloudfirewall_access_collection_policy"])
+                check_type(argname="argument cloudfirewall_access_policy_setting", value=cloudfirewall_access_policy_setting, expected_type=type_hints["cloudfirewall_access_policy_setting"])
+                check_type(argname="argument cloudfirewall_enabled", value=cloudfirewall_enabled, expected_type=type_hints["cloudfirewall_enabled"])
+                check_type(argname="argument cloudfirewall_ti_enabled", value=cloudfirewall_ti_enabled, expected_type=type_hints["cloudfirewall_ti_enabled"])
+                check_type(argname="argument cloudfirewall_ttl", value=cloudfirewall_ttl, expected_type=type_hints["cloudfirewall_ttl"])
+                check_type(argname="argument cps_callback_collection_policy", value=cps_callback_collection_policy, expected_type=type_hints["cps_callback_collection_policy"])
+                check_type(argname="argument cps_callback_policy_setting", value=cps_callback_policy_setting, expected_type=type_hints["cps_callback_policy_setting"])
+                check_type(argname="argument cps_enabled", value=cps_enabled, expected_type=type_hints["cps_enabled"])
+                check_type(argname="argument cps_ti_enabled", value=cps_ti_enabled, expected_type=type_hints["cps_ti_enabled"])
+                check_type(argname="argument cps_ttl", value=cps_ttl, expected_type=type_hints["cps_ttl"])
+                check_type(argname="argument ddos_coo_access_collection_policy", value=ddos_coo_access_collection_policy, expected_type=type_hints["ddos_coo_access_collection_policy"])
+                check_type(argname="argument ddos_coo_access_enabled", value=ddos_coo_access_enabled, expected_type=type_hints["ddos_coo_access_enabled"])
+                check_type(argname="argument ddos_coo_access_policy_setting", value=ddos_coo_access_policy_setting, expected_type=type_hints["ddos_coo_access_policy_setting"])
+                check_type(argname="argument ddos_coo_access_ti_enabled", value=ddos_coo_access_ti_enabled, expected_type=type_hints["ddos_coo_access_ti_enabled"])
+                check_type(argname="argument ddos_coo_access_ttl", value=ddos_coo_access_ttl, expected_type=type_hints["ddos_coo_access_ttl"])
+                check_type(argname="argument drds_audit_collection_policy", value=drds_audit_collection_policy, expected_type=type_hints["drds_audit_collection_policy"])
+                check_type(argname="argument drds_audit_enabled", value=drds_audit_enabled, expected_type=type_hints["drds_audit_enabled"])
+                check_type(argname="argument drds_audit_policy_setting", value=drds_audit_policy_setting, expected_type=type_hints["drds_audit_policy_setting"])
+                check_type(argname="argument drds_audit_ti_enabled", value=drds_audit_ti_enabled, expected_type=type_hints["drds_audit_ti_enabled"])
+                check_type(argname="argument drds_audit_ttl", value=drds_audit_ttl, expected_type=type_hints["drds_audit_ttl"])
+                check_type(argname="argument drds_sync_enabled", value=drds_sync_enabled, expected_type=type_hints["drds_sync_enabled"])
+                check_type(argname="argument drds_sync_ttl", value=drds_sync_ttl, expected_type=type_hints["drds_sync_ttl"])
+                check_type(argname="argument k8_s_audit_collection_policy", value=k8_s_audit_collection_policy, expected_type=type_hints["k8_s_audit_collection_policy"])
+                check_type(argname="argument k8_s_audit_enabled", value=k8_s_audit_enabled, expected_type=type_hints["k8_s_audit_enabled"])
+                check_type(argname="argument k8_s_audit_policy_setting", value=k8_s_audit_policy_setting, expected_type=type_hints["k8_s_audit_policy_setting"])
+                check_type(argname="argument k8_s_audit_ti_enabled", value=k8_s_audit_ti_enabled, expected_type=type_hints["k8_s_audit_ti_enabled"])
+                check_type(argname="argument k8_s_audit_ttl", value=k8_s_audit_ttl, expected_type=type_hints["k8_s_audit_ttl"])
+                check_type(argname="argument k8_s_event_collection_policy", value=k8_s_event_collection_policy, expected_type=type_hints["k8_s_event_collection_policy"])
+                check_type(argname="argument k8_s_event_enabled", value=k8_s_event_enabled, expected_type=type_hints["k8_s_event_enabled"])
+                check_type(argname="argument k8_s_event_policy_setting", value=k8_s_event_policy_setting, expected_type=type_hints["k8_s_event_policy_setting"])
+                check_type(argname="argument k8_s_event_ti_enabled", value=k8_s_event_ti_enabled, expected_type=type_hints["k8_s_event_ti_enabled"])
+                check_type(argname="argument k8_s_event_ttl", value=k8_s_event_ttl, expected_type=type_hints["k8_s_event_ttl"])
+                check_type(argname="argument k8_s_ingress_collection_policy", value=k8_s_ingress_collection_policy, expected_type=type_hints["k8_s_ingress_collection_policy"])
+                check_type(argname="argument k8_s_ingress_enabled", value=k8_s_ingress_enabled, expected_type=type_hints["k8_s_ingress_enabled"])
+                check_type(argname="argument k8_s_ingress_policy_setting", value=k8_s_ingress_policy_setting, expected_type=type_hints["k8_s_ingress_policy_setting"])
+                check_type(argname="argument k8_s_ingress_ti_enabled", value=k8_s_ingress_ti_enabled, expected_type=type_hints["k8_s_ingress_ti_enabled"])
+                check_type(argname="argument k8_s_ingress_ttl", value=k8_s_ingress_ttl, expected_type=type_hints["k8_s_ingress_ttl"])
+                check_type(argname="argument nas_audit_collection_policy", value=nas_audit_collection_policy, expected_type=type_hints["nas_audit_collection_policy"])
+                check_type(argname="argument nas_audit_policy_setting", value=nas_audit_policy_setting, expected_type=type_hints["nas_audit_policy_setting"])
+                check_type(argname="argument nas_enabled", value=nas_enabled, expected_type=type_hints["nas_enabled"])
+                check_type(argname="argument nas_ti_enabled", value=nas_ti_enabled, expected_type=type_hints["nas_ti_enabled"])
+                check_type(argname="argument nas_ttl", value=nas_ttl, expected_type=type_hints["nas_ttl"])
+                check_type(argname="argument oss_access_collection_policy", value=oss_access_collection_policy, expected_type=type_hints["oss_access_collection_policy"])
+                check_type(argname="argument oss_access_enabled", value=oss_access_enabled, expected_type=type_hints["oss_access_enabled"])
+                check_type(argname="argument oss_access_policy_setting", value=oss_access_policy_setting, expected_type=type_hints["oss_access_policy_setting"])
+                check_type(argname="argument oss_access_ti_enabled", value=oss_access_ti_enabled, expected_type=type_hints["oss_access_ti_enabled"])
+                check_type(argname="argument oss_access_ttl", value=oss_access_ttl, expected_type=type_hints["oss_access_ttl"])
+                check_type(argname="argument oss_metering_collection_policy", value=oss_metering_collection_policy, expected_type=type_hints["oss_metering_collection_policy"])
+                check_type(argname="argument oss_metering_enabled", value=oss_metering_enabled, expected_type=type_hints["oss_metering_enabled"])
+                check_type(argname="argument oss_metering_policy_setting", value=oss_metering_policy_setting, expected_type=type_hints["oss_metering_policy_setting"])
+                check_type(argname="argument oss_metering_ti_enabled", value=oss_metering_ti_enabled, expected_type=type_hints["oss_metering_ti_enabled"])
+                check_type(argname="argument oss_metering_ttl", value=oss_metering_ttl, expected_type=type_hints["oss_metering_ttl"])
+                check_type(argname="argument oss_sync_enabled", value=oss_sync_enabled, expected_type=type_hints["oss_sync_enabled"])
+                check_type(argname="argument oss_sync_ttl", value=oss_sync_ttl, expected_type=type_hints["oss_sync_ttl"])
+                check_type(argname="argument polardb_audit_collection_policy", value=polardb_audit_collection_policy, expected_type=type_hints["polardb_audit_collection_policy"])
+                check_type(argname="argument polardb_audit_policy_setting", value=polardb_audit_policy_setting, expected_type=type_hints["polardb_audit_policy_setting"])
+                check_type(argname="argument polardb_enabled", value=polardb_enabled, expected_type=type_hints["polardb_enabled"])
+                check_type(argname="argument polardb_perf_collection_policy", value=polardb_perf_collection_policy, expected_type=type_hints["polardb_perf_collection_policy"])
+                check_type(argname="argument polardb_perf_enabled", value=polardb_perf_enabled, expected_type=type_hints["polardb_perf_enabled"])
+                check_type(argname="argument polardb_perf_policy_setting", value=polardb_perf_policy_setting, expected_type=type_hints["polardb_perf_policy_setting"])
+                check_type(argname="argument polardb_perf_ti_enabled", value=polardb_perf_ti_enabled, expected_type=type_hints["polardb_perf_ti_enabled"])
+                check_type(argname="argument polardb_perf_ttl", value=polardb_perf_ttl, expected_type=type_hints["polardb_perf_ttl"])
+                check_type(argname="argument polardb_slow_collection_policy", value=polardb_slow_collection_policy, expected_type=type_hints["polardb_slow_collection_policy"])
+                check_type(argname="argument polardb_slow_enabled", value=polardb_slow_enabled, expected_type=type_hints["polardb_slow_enabled"])
+                check_type(argname="argument polardb_slow_policy_setting", value=polardb_slow_policy_setting, expected_type=type_hints["polardb_slow_policy_setting"])
+                check_type(argname="argument polardb_slow_ti_enabled", value=polardb_slow_ti_enabled, expected_type=type_hints["polardb_slow_ti_enabled"])
+                check_type(argname="argument polardb_slow_ttl", value=polardb_slow_ttl, expected_type=type_hints["polardb_slow_ttl"])
+                check_type(argname="argument polardb_ti_enabled", value=polardb_ti_enabled, expected_type=type_hints["polardb_ti_enabled"])
+                check_type(argname="argument polardb_ttl", value=polardb_ttl, expected_type=type_hints["polardb_ttl"])
+                check_type(argname="argument rds_audit_collection_policy", value=rds_audit_collection_policy, expected_type=type_hints["rds_audit_collection_policy"])
+                check_type(argname="argument rds_audit_policy_setting", value=rds_audit_policy_setting, expected_type=type_hints["rds_audit_policy_setting"])
+                check_type(argname="argument rds_enabled", value=rds_enabled, expected_type=type_hints["rds_enabled"])
+                check_type(argname="argument rds_perf_collection_policy", value=rds_perf_collection_policy, expected_type=type_hints["rds_perf_collection_policy"])
+                check_type(argname="argument rds_perf_enabled", value=rds_perf_enabled, expected_type=type_hints["rds_perf_enabled"])
+                check_type(argname="argument rds_perf_policy_setting", value=rds_perf_policy_setting, expected_type=type_hints["rds_perf_policy_setting"])
+                check_type(argname="argument rds_perf_ti_enabled", value=rds_perf_ti_enabled, expected_type=type_hints["rds_perf_ti_enabled"])
+                check_type(argname="argument rds_perf_ttl", value=rds_perf_ttl, expected_type=type_hints["rds_perf_ttl"])
+                check_type(argname="argument rds_slow_collection_policy", value=rds_slow_collection_policy, expected_type=type_hints["rds_slow_collection_policy"])
+                check_type(argname="argument rds_slow_enabled", value=rds_slow_enabled, expected_type=type_hints["rds_slow_enabled"])
+                check_type(argname="argument rds_slow_policy_setting", value=rds_slow_policy_setting, expected_type=type_hints["rds_slow_policy_setting"])
+                check_type(argname="argument rds_slow_ti_enabled", value=rds_slow_ti_enabled, expected_type=type_hints["rds_slow_ti_enabled"])
+                check_type(argname="argument rds_slow_ttl", value=rds_slow_ttl, expected_type=type_hints["rds_slow_ttl"])
+                check_type(argname="argument rds_ti_enabled", value=rds_ti_enabled, expected_type=type_hints["rds_ti_enabled"])
+                check_type(argname="argument rds_ttl", value=rds_ttl, expected_type=type_hints["rds_ttl"])
+                check_type(argname="argument redis_audit_collection_policy", value=redis_audit_collection_policy, expected_type=type_hints["redis_audit_collection_policy"])
+                check_type(argname="argument redis_audit_enabled", value=redis_audit_enabled, expected_type=type_hints["redis_audit_enabled"])
+                check_type(argname="argument redis_audit_policy_setting", value=redis_audit_policy_setting, expected_type=type_hints["redis_audit_policy_setting"])
+                check_type(argname="argument redis_audit_ti_enabled", value=redis_audit_ti_enabled, expected_type=type_hints["redis_audit_ti_enabled"])
+                check_type(argname="argument redis_audit_ttl", value=redis_audit_ttl, expected_type=type_hints["redis_audit_ttl"])
+                check_type(argname="argument redis_sync_enabled", value=redis_sync_enabled, expected_type=type_hints["redis_sync_enabled"])
+                check_type(argname="argument redis_sync_ttl", value=redis_sync_ttl, expected_type=type_hints["redis_sync_ttl"])
+                check_type(argname="argument sas_crack_enabled", value=sas_crack_enabled, expected_type=type_hints["sas_crack_enabled"])
+                check_type(argname="argument sas_dns_enabled", value=sas_dns_enabled, expected_type=type_hints["sas_dns_enabled"])
+                check_type(argname="argument sas_http_enabled", value=sas_http_enabled, expected_type=type_hints["sas_http_enabled"])
+                check_type(argname="argument sas_local_dns_enabled", value=sas_local_dns_enabled, expected_type=type_hints["sas_local_dns_enabled"])
+                check_type(argname="argument sas_login_enabled", value=sas_login_enabled, expected_type=type_hints["sas_login_enabled"])
+                check_type(argname="argument sas_network_enabled", value=sas_network_enabled, expected_type=type_hints["sas_network_enabled"])
+                check_type(argname="argument sas_process_enabled", value=sas_process_enabled, expected_type=type_hints["sas_process_enabled"])
+                check_type(argname="argument sas_security_alert_enabled", value=sas_security_alert_enabled, expected_type=type_hints["sas_security_alert_enabled"])
+                check_type(argname="argument sas_security_hc_enabled", value=sas_security_hc_enabled, expected_type=type_hints["sas_security_hc_enabled"])
+                check_type(argname="argument sas_security_vul_enabled", value=sas_security_vul_enabled, expected_type=type_hints["sas_security_vul_enabled"])
+                check_type(argname="argument sas_session_enabled", value=sas_session_enabled, expected_type=type_hints["sas_session_enabled"])
+                check_type(argname="argument sas_snapshot_account_enabled", value=sas_snapshot_account_enabled, expected_type=type_hints["sas_snapshot_account_enabled"])
+                check_type(argname="argument sas_snapshot_port_enabled", value=sas_snapshot_port_enabled, expected_type=type_hints["sas_snapshot_port_enabled"])
+                check_type(argname="argument sas_snapshot_process_enabled", value=sas_snapshot_process_enabled, expected_type=type_hints["sas_snapshot_process_enabled"])
+                check_type(argname="argument sas_ti_enabled", value=sas_ti_enabled, expected_type=type_hints["sas_ti_enabled"])
+                check_type(argname="argument sas_ttl", value=sas_ttl, expected_type=type_hints["sas_ttl"])
+                check_type(argname="argument slb_access_collection_policy", value=slb_access_collection_policy, expected_type=type_hints["slb_access_collection_policy"])
+                check_type(argname="argument slb_access_enabled", value=slb_access_enabled, expected_type=type_hints["slb_access_enabled"])
+                check_type(argname="argument slb_access_policy_setting", value=slb_access_policy_setting, expected_type=type_hints["slb_access_policy_setting"])
+                check_type(argname="argument slb_access_ti_enabled", value=slb_access_ti_enabled, expected_type=type_hints["slb_access_ti_enabled"])
+                check_type(argname="argument slb_access_ttl", value=slb_access_ttl, expected_type=type_hints["slb_access_ttl"])
+                check_type(argname="argument slb_sync_enabled", value=slb_sync_enabled, expected_type=type_hints["slb_sync_enabled"])
+                check_type(argname="argument slb_sync_ttl", value=slb_sync_ttl, expected_type=type_hints["slb_sync_ttl"])
+                check_type(argname="argument waf_access_collection_policy", value=waf_access_collection_policy, expected_type=type_hints["waf_access_collection_policy"])
+                check_type(argname="argument waf_access_policy_setting", value=waf_access_policy_setting, expected_type=type_hints["waf_access_policy_setting"])
+                check_type(argname="argument waf_enabled", value=waf_enabled, expected_type=type_hints["waf_enabled"])
+                check_type(argname="argument waf_ti_enabled", value=waf_ti_enabled, expected_type=type_hints["waf_ti_enabled"])
+                check_type(argname="argument waf_ttl", value=waf_ttl, expected_type=type_hints["waf_ttl"])
             self._values: typing.Dict[str, typing.Any] = {}
             if actiontrail_enabled is not None:
                 self._values["actiontrail_enabled"] = actiontrail_enabled
             if actiontrail_openapi_collection_policy is not None:
                 self._values["actiontrail_openapi_collection_policy"] = actiontrail_openapi_collection_policy
             if actiontrail_openapi_policy_setting is not None:
                 self._values["actiontrail_openapi_policy_setting"] = actiontrail_openapi_policy_setting
@@ -5490,23 +5937,28 @@
     },
 )
 class RosAuditProps:
     def __init__(
         self,
         *,
         display_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
-        variable_map: typing.Union[ros_cdk_core.IResolvable, RosAudit.VariableMapProperty],
+        variable_map: typing.Union[ros_cdk_core.IResolvable, typing.Union[RosAudit.VariableMapProperty, typing.Dict[str, typing.Any]]],
         multi_account: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::SLS::Audit``.
 
         :param display_name: 
         :param variable_map: 
         :param multi_account: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosAuditProps.__init__)
+            check_type(argname="argument display_name", value=display_name, expected_type=type_hints["display_name"])
+            check_type(argname="argument variable_map", value=variable_map, expected_type=type_hints["variable_map"])
+            check_type(argname="argument multi_account", value=multi_account, expected_type=type_hints["multi_account"])
         self._values: typing.Dict[str, typing.Any] = {
             "display_name": display_name,
             "variable_map": variable_map,
         }
         if multi_account is not None:
             self._values["multi_account"] = multi_account
 
@@ -5559,105 +6011,123 @@
 ):
     '''A ROS template type:  ``ALIYUN::SLS::Dashboard``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosDashboardProps",
+        props: typing.Union["RosDashboardProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::SLS::Dashboard``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosDashboard.__init__)
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
+            type_hints = typing.get_type_hints(RosDashboard._render_properties)
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
     @jsii.member(jsii_name="attrDashboardName")
     def attr_dashboard_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: DashboardName: Dashboard name.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDashboardName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDisplayName")
     def attr_display_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: DisplayName: Display name.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDisplayName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="charts")
     def charts(
         self,
     ) -> typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Mapping[builtins.str, typing.Any]]]:
         '''
         :Property: charts: Chart list.
         '''
         return typing.cast(typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Mapping[builtins.str, typing.Any]]], jsii.get(self, "charts"))
 
     @charts.setter
     def charts(
         self,
         value: typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Mapping[builtins.str, typing.Any]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDashboard, "charts").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "charts", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dashboardName")
     def dashboard_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: dashboardName: Dashboard name.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "dashboardName"))
 
     @dashboard_name.setter
     def dashboard_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDashboard, "dashboard_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dashboardName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDashboard, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="projectName")
     def project_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         projectName: Project name:
 
@@ -5668,48 +6138,57 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "projectName"))
 
     @project_name.setter
     def project_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDashboard, "project_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "projectName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="description")
     def description(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: description: Dashboard description.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "description"))
 
     @description.setter
     def description(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDashboard, "description").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "description", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="displayName")
     def display_name(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: displayName: Dashboard display name.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "displayName"))
 
     @display_name.setter
     def display_name(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDashboard, "display_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "displayName", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-sls.RosDashboardProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -5734,14 +6213,21 @@
 
         :param charts: 
         :param dashboard_name: 
         :param project_name: 
         :param description: 
         :param display_name: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosDashboardProps.__init__)
+            check_type(argname="argument charts", value=charts, expected_type=type_hints["charts"])
+            check_type(argname="argument dashboard_name", value=dashboard_name, expected_type=type_hints["dashboard_name"])
+            check_type(argname="argument project_name", value=project_name, expected_type=type_hints["project_name"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument display_name", value=display_name, expected_type=type_hints["display_name"])
         self._values: typing.Dict[str, typing.Any] = {
             "charts": charts,
             "dashboard_name": dashboard_name,
             "project_name": project_name,
         }
         if description is not None:
             self._values["description"] = description
@@ -5822,155 +6308,185 @@
 ):
     '''A ROS template type:  ``ALIYUN::SLS::Etl``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosEtlProps",
+        props: typing.Union["RosEtlProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::SLS::Etl``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosEtl.__init__)
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
+            type_hints = typing.get_type_hints(RosEtl._render_properties)
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
         :Attribute: Name: ETL name.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="configuration")
     def configuration(
         self,
     ) -> typing.Union[ros_cdk_core.IResolvable, "RosEtl.ConfigurationProperty"]:
         '''
         :Property: configuration: The configuration of ETL task
         '''
         return typing.cast(typing.Union[ros_cdk_core.IResolvable, "RosEtl.ConfigurationProperty"], jsii.get(self, "configuration"))
 
     @configuration.setter
     def configuration(
         self,
         value: typing.Union[ros_cdk_core.IResolvable, "RosEtl.ConfigurationProperty"],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosEtl, "configuration").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "configuration", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="displayName")
     def display_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: displayName: ETL display name
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "displayName"))
 
     @display_name.setter
     def display_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosEtl, "display_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "displayName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosEtl, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="name")
     def name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: name: ETL name
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "name"))
 
     @name.setter
     def name(self, value: typing.Union[builtins.str, ros_cdk_core.IResolvable]) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosEtl, "name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "name", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="projectName")
     def project_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: projectName: Project name
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "projectName"))
 
     @project_name.setter
     def project_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosEtl, "project_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "projectName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="schedule")
     def schedule(
         self,
     ) -> typing.Union[ros_cdk_core.IResolvable, "RosEtl.ScheduleProperty"]:
         '''
         :Property: schedule: Task scheduling strategy
         '''
         return typing.cast(typing.Union[ros_cdk_core.IResolvable, "RosEtl.ScheduleProperty"], jsii.get(self, "schedule"))
 
     @schedule.setter
     def schedule(
         self,
         value: typing.Union[ros_cdk_core.IResolvable, "RosEtl.ScheduleProperty"],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosEtl, "schedule").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "schedule", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="description")
     def description(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: description: ETL description message.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "description"))
 
     @description.setter
     def description(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosEtl, "description").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "description", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-sls.RosEtl.ConfigurationProperty",
         jsii_struct_bases=[],
         name_mapping={
             "logstore": "logstore",
@@ -5985,15 +6501,15 @@
     )
     class ConfigurationProperty:
         def __init__(
             self,
             *,
             logstore: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             script: typing.Union[builtins.str, ros_cdk_core.IResolvable],
-            sinks: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosEtl.SinksProperty"]]],
+            sinks: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosEtl.SinksProperty", typing.Dict[str, typing.Any]]]]],
             from_time: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
             parameters: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]]] = None,
             role_arn: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
             to_time: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
             version: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
@@ -6002,14 +6518,24 @@
             :param sinks: 
             :param from_time: 
             :param parameters: 
             :param role_arn: 
             :param to_time: 
             :param version: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosEtl.ConfigurationProperty.__init__)
+                check_type(argname="argument logstore", value=logstore, expected_type=type_hints["logstore"])
+                check_type(argname="argument script", value=script, expected_type=type_hints["script"])
+                check_type(argname="argument sinks", value=sinks, expected_type=type_hints["sinks"])
+                check_type(argname="argument from_time", value=from_time, expected_type=type_hints["from_time"])
+                check_type(argname="argument parameters", value=parameters, expected_type=type_hints["parameters"])
+                check_type(argname="argument role_arn", value=role_arn, expected_type=type_hints["role_arn"])
+                check_type(argname="argument to_time", value=to_time, expected_type=type_hints["to_time"])
+                check_type(argname="argument version", value=version, expected_type=type_hints["version"])
             self._values: typing.Dict[str, typing.Any] = {
                 "logstore": logstore,
                 "script": script,
                 "sinks": sinks,
             }
             if from_time is not None:
                 self._values["from_time"] = from_time
@@ -6122,14 +6648,17 @@
             self,
             *,
             type: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         ) -> None:
             '''
             :param type: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosEtl.ScheduleProperty.__init__)
+                check_type(argname="argument type", value=type, expected_type=type_hints["type"])
             self._values: typing.Dict[str, typing.Any] = {
                 "type": type,
             }
 
         @builtins.property
         def type(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
             '''
@@ -6177,14 +6706,22 @@
             :param logstore: 
             :param name: 
             :param project: 
             :param endpoint: 
             :param role_arn: 
             :param type: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosEtl.SinksProperty.__init__)
+                check_type(argname="argument logstore", value=logstore, expected_type=type_hints["logstore"])
+                check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+                check_type(argname="argument project", value=project, expected_type=type_hints["project"])
+                check_type(argname="argument endpoint", value=endpoint, expected_type=type_hints["endpoint"])
+                check_type(argname="argument role_arn", value=role_arn, expected_type=type_hints["role_arn"])
+                check_type(argname="argument type", value=type, expected_type=type_hints["type"])
             self._values: typing.Dict[str, typing.Any] = {
                 "logstore": logstore,
                 "name": name,
                 "project": project,
             }
             if endpoint is not None:
                 self._values["endpoint"] = endpoint
@@ -6274,30 +6811,38 @@
         "description": "description",
     },
 )
 class RosEtlProps:
     def __init__(
         self,
         *,
-        configuration: typing.Union[ros_cdk_core.IResolvable, RosEtl.ConfigurationProperty],
+        configuration: typing.Union[ros_cdk_core.IResolvable, typing.Union[RosEtl.ConfigurationProperty, typing.Dict[str, typing.Any]]],
         display_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         project_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
-        schedule: typing.Union[ros_cdk_core.IResolvable, RosEtl.ScheduleProperty],
+        schedule: typing.Union[ros_cdk_core.IResolvable, typing.Union[RosEtl.ScheduleProperty, typing.Dict[str, typing.Any]]],
         description: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::SLS::Etl``.
 
         :param configuration: 
         :param display_name: 
         :param name: 
         :param project_name: 
         :param schedule: 
         :param description: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosEtlProps.__init__)
+            check_type(argname="argument configuration", value=configuration, expected_type=type_hints["configuration"])
+            check_type(argname="argument display_name", value=display_name, expected_type=type_hints["display_name"])
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+            check_type(argname="argument project_name", value=project_name, expected_type=type_hints["project_name"])
+            check_type(argname="argument schedule", value=schedule, expected_type=type_hints["schedule"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
         self._values: typing.Dict[str, typing.Any] = {
             "configuration": configuration,
             "display_name": display_name,
             "name": name,
             "project_name": project_name,
             "schedule": schedule,
         }
@@ -6382,58 +6927,70 @@
 ):
     '''A ROS template type:  ``ALIYUN::SLS::Index``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosIndexProps",
+        props: typing.Union["RosIndexProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::SLS::Index``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosIndex.__init__)
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
+            type_hints = typing.get_type_hints(RosIndex._render_properties)
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
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         '''A factory method that creates a new instance of this class from an object containing the properties of this ROS resource.'''
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosIndex, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="fullTextIndex")
     def full_text_index(
         self,
     ) -> typing.Union[ros_cdk_core.IResolvable, "RosIndex.FullTextIndexProperty"]:
         '''
         :Property:
 
@@ -6443,17 +7000,20 @@
         return typing.cast(typing.Union[ros_cdk_core.IResolvable, "RosIndex.FullTextIndexProperty"], jsii.get(self, "fullTextIndex"))
 
     @full_text_index.setter
     def full_text_index(
         self,
         value: typing.Union[ros_cdk_core.IResolvable, "RosIndex.FullTextIndexProperty"],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosIndex, "full_text_index").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "fullTextIndex", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="logstoreName")
     def logstore_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         logstoreName: Logstore name:
 
@@ -6464,17 +7024,20 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "logstoreName"))
 
     @logstore_name.setter
     def logstore_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosIndex, "logstore_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "logstoreName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="projectName")
     def project_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         projectName: Project name:
 
@@ -6485,17 +7048,20 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "projectName"))
 
     @project_name.setter
     def project_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosIndex, "project_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "projectName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="keyIndices")
     def key_indices(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosIndex.KeyIndicesProperty"]]]]:
         '''
         :Property:
 
@@ -6505,31 +7071,37 @@
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosIndex.KeyIndicesProperty"]]]], jsii.get(self, "keyIndices"))
 
     @key_indices.setter
     def key_indices(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosIndex.KeyIndicesProperty"]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosIndex, "key_indices").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "keyIndices", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="logReduce")
     def log_reduce(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property: logReduce: Whether to enable log reduce. Default to false.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "logReduce"))
 
     @log_reduce.setter
     def log_reduce(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosIndex, "log_reduce").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "logReduce", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-sls.RosIndex.FullTextIndexProperty",
         jsii_struct_bases=[],
         name_mapping={
             "enable": "enable",
@@ -6549,14 +7121,20 @@
         ) -> None:
             '''
             :param enable: 
             :param case_sensitive: 
             :param delimiter: 
             :param include_chinese: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosIndex.FullTextIndexProperty.__init__)
+                check_type(argname="argument enable", value=enable, expected_type=type_hints["enable"])
+                check_type(argname="argument case_sensitive", value=case_sensitive, expected_type=type_hints["case_sensitive"])
+                check_type(argname="argument delimiter", value=delimiter, expected_type=type_hints["delimiter"])
+                check_type(argname="argument include_chinese", value=include_chinese, expected_type=type_hints["include_chinese"])
             self._values: typing.Dict[str, typing.Any] = {
                 "enable": enable,
             }
             if case_sensitive is not None:
                 self._values["case_sensitive"] = case_sensitive
             if delimiter is not None:
                 self._values["delimiter"] = delimiter
@@ -6635,14 +7213,20 @@
         ) -> None:
             '''
             :param name: 
             :param type: 
             :param alias: 
             :param enable_analytics: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosIndex.JsonKeyIndicesProperty.__init__)
+                check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+                check_type(argname="argument type", value=type, expected_type=type_hints["type"])
+                check_type(argname="argument alias", value=alias, expected_type=type_hints["alias"])
+                check_type(argname="argument enable_analytics", value=enable_analytics, expected_type=type_hints["enable_analytics"])
             self._values: typing.Dict[str, typing.Any] = {
                 "name": name,
                 "type": type,
             }
             if alias is not None:
                 self._values["alias"] = alias
             if enable_analytics is not None:
@@ -6718,26 +7302,36 @@
             name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             type: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             alias: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
             case_sensitive: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
             delimiter: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
             enable_analytics: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
             include_chinese: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
-            json_key_indices: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosIndex.JsonKeyIndicesProperty"]]]] = None,
+            json_key_indices: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosIndex.JsonKeyIndicesProperty", typing.Dict[str, typing.Any]]]]]] = None,
         ) -> None:
             '''
             :param name: 
             :param type: 
             :param alias: 
             :param case_sensitive: 
             :param delimiter: 
             :param enable_analytics: 
             :param include_chinese: 
             :param json_key_indices: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosIndex.KeyIndicesProperty.__init__)
+                check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+                check_type(argname="argument type", value=type, expected_type=type_hints["type"])
+                check_type(argname="argument alias", value=alias, expected_type=type_hints["alias"])
+                check_type(argname="argument case_sensitive", value=case_sensitive, expected_type=type_hints["case_sensitive"])
+                check_type(argname="argument delimiter", value=delimiter, expected_type=type_hints["delimiter"])
+                check_type(argname="argument enable_analytics", value=enable_analytics, expected_type=type_hints["enable_analytics"])
+                check_type(argname="argument include_chinese", value=include_chinese, expected_type=type_hints["include_chinese"])
+                check_type(argname="argument json_key_indices", value=json_key_indices, expected_type=type_hints["json_key_indices"])
             self._values: typing.Dict[str, typing.Any] = {
                 "name": name,
                 "type": type,
             }
             if alias is not None:
                 self._values["alias"] = alias
             if case_sensitive is not None:
@@ -6853,28 +7447,35 @@
         "log_reduce": "logReduce",
     },
 )
 class RosIndexProps:
     def __init__(
         self,
         *,
-        full_text_index: typing.Union[ros_cdk_core.IResolvable, RosIndex.FullTextIndexProperty],
+        full_text_index: typing.Union[ros_cdk_core.IResolvable, typing.Union[RosIndex.FullTextIndexProperty, typing.Dict[str, typing.Any]]],
         logstore_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         project_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
-        key_indices: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosIndex.KeyIndicesProperty]]]] = None,
+        key_indices: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosIndex.KeyIndicesProperty, typing.Dict[str, typing.Any]]]]]] = None,
         log_reduce: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::SLS::Index``.
 
         :param full_text_index: 
         :param logstore_name: 
         :param project_name: 
         :param key_indices: 
         :param log_reduce: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosIndexProps.__init__)
+            check_type(argname="argument full_text_index", value=full_text_index, expected_type=type_hints["full_text_index"])
+            check_type(argname="argument logstore_name", value=logstore_name, expected_type=type_hints["logstore_name"])
+            check_type(argname="argument project_name", value=project_name, expected_type=type_hints["project_name"])
+            check_type(argname="argument key_indices", value=key_indices, expected_type=type_hints["key_indices"])
+            check_type(argname="argument log_reduce", value=log_reduce, expected_type=type_hints["log_reduce"])
         self._values: typing.Dict[str, typing.Any] = {
             "full_text_index": full_text_index,
             "logstore_name": logstore_name,
             "project_name": project_name,
         }
         if key_indices is not None:
             self._values["key_indices"] = key_indices
@@ -6967,65 +7568,77 @@
 ):
     '''A ROS template type:  ``ALIYUN::SLS::Logstore``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosLogstoreProps",
+        props: typing.Union["RosLogstoreProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::SLS::Logstore``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosLogstore.__init__)
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
+            type_hints = typing.get_type_hints(RosLogstore._render_properties)
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
     @jsii.member(jsii_name="attrLogstoreName")
     def attr_logstore_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: LogstoreName: Logstore name.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrLogstoreName"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosLogstore, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="logstoreName")
     def logstore_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         logstoreName: Logstore name:
 
@@ -7036,17 +7649,20 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "logstoreName"))
 
     @logstore_name.setter
     def logstore_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosLogstore, "logstore_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "logstoreName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="projectName")
     def project_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         projectName: Project name:
 
@@ -7057,17 +7673,20 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "projectName"))
 
     @project_name.setter
     def project_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosLogstore, "project_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "projectName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="appendMeta")
     def append_meta(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -7077,17 +7696,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "appendMeta"))
 
     @append_meta.setter
     def append_meta(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosLogstore, "append_meta").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "appendMeta", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="autoSplit")
     def auto_split(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -7097,17 +7719,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "autoSplit"))
 
     @auto_split.setter
     def auto_split(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosLogstore, "auto_split").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "autoSplit", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableTracking")
     def enable_tracking(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -7117,34 +7742,40 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "enableTracking"))
 
     @enable_tracking.setter
     def enable_tracking(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosLogstore, "enable_tracking").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableTracking", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="encryptConf")
     def encrypt_conf(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosLogstore.EncryptConfProperty"]]:
         '''
         :Property: encryptConf: Data encryption config
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosLogstore.EncryptConfProperty"]], jsii.get(self, "encryptConf"))
 
     @encrypt_conf.setter
     def encrypt_conf(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosLogstore.EncryptConfProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosLogstore, "encrypt_conf").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "encryptConf", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="maxSplitShard")
     def max_split_shard(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -7154,17 +7785,20 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "maxSplitShard"))
 
     @max_split_shard.setter
     def max_split_shard(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosLogstore, "max_split_shard").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "maxSplitShard", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="preserveStorage")
     def preserve_storage(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -7175,17 +7809,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "preserveStorage"))
 
     @preserve_storage.setter
     def preserve_storage(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosLogstore, "preserve_storage").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "preserveStorage", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="shardCount")
     def shard_count(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -7195,17 +7832,20 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "shardCount"))
 
     @shard_count.setter
     def shard_count(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosLogstore, "shard_count").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "shardCount", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="ttl")
     def ttl(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -7215,14 +7855,17 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "ttl"))
 
     @ttl.setter
     def ttl(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosLogstore, "ttl").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "ttl", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-sls.RosLogstore.EncryptConfProperty",
         jsii_struct_bases=[],
         name_mapping={
             "enable": "enable",
@@ -7232,21 +7875,26 @@
     )
     class EncryptConfProperty:
         def __init__(
             self,
             *,
             enable: typing.Union[builtins.bool, ros_cdk_core.IResolvable],
             encrypt_type: typing.Union[builtins.str, ros_cdk_core.IResolvable],
-            user_cmk_info: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosLogstore.UserCmkInfoProperty"]] = None,
+            user_cmk_info: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosLogstore.UserCmkInfoProperty", typing.Dict[str, typing.Any]]]] = None,
         ) -> None:
             '''
             :param enable: 
             :param encrypt_type: 
             :param user_cmk_info: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosLogstore.EncryptConfProperty.__init__)
+                check_type(argname="argument enable", value=enable, expected_type=type_hints["enable"])
+                check_type(argname="argument encrypt_type", value=encrypt_type, expected_type=type_hints["encrypt_type"])
+                check_type(argname="argument user_cmk_info", value=user_cmk_info, expected_type=type_hints["user_cmk_info"])
             self._values: typing.Dict[str, typing.Any] = {
                 "enable": enable,
                 "encrypt_type": encrypt_type,
             }
             if user_cmk_info is not None:
                 self._values["user_cmk_info"] = user_cmk_info
 
@@ -7309,14 +7957,19 @@
             region_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         ) -> None:
             '''
             :param arn: 
             :param cmk_key_id: 
             :param region_id: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosLogstore.UserCmkInfoProperty.__init__)
+                check_type(argname="argument arn", value=arn, expected_type=type_hints["arn"])
+                check_type(argname="argument cmk_key_id", value=cmk_key_id, expected_type=type_hints["cmk_key_id"])
+                check_type(argname="argument region_id", value=region_id, expected_type=type_hints["region_id"])
             self._values: typing.Dict[str, typing.Any] = {
                 "arn": arn,
                 "cmk_key_id": cmk_key_id,
                 "region_id": region_id,
             }
 
         @builtins.property
@@ -7386,15 +8039,15 @@
         self,
         *,
         logstore_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         project_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         append_meta: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         auto_split: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         enable_tracking: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
-        encrypt_conf: typing.Optional[typing.Union[ros_cdk_core.IResolvable, RosLogstore.EncryptConfProperty]] = None,
+        encrypt_conf: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosLogstore.EncryptConfProperty, typing.Dict[str, typing.Any]]]] = None,
         max_split_shard: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         preserve_storage: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         shard_count: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         ttl: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::SLS::Logstore``.
 
@@ -7405,14 +8058,26 @@
         :param enable_tracking: 
         :param encrypt_conf: 
         :param max_split_shard: 
         :param preserve_storage: 
         :param shard_count: 
         :param ttl: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosLogstoreProps.__init__)
+            check_type(argname="argument logstore_name", value=logstore_name, expected_type=type_hints["logstore_name"])
+            check_type(argname="argument project_name", value=project_name, expected_type=type_hints["project_name"])
+            check_type(argname="argument append_meta", value=append_meta, expected_type=type_hints["append_meta"])
+            check_type(argname="argument auto_split", value=auto_split, expected_type=type_hints["auto_split"])
+            check_type(argname="argument enable_tracking", value=enable_tracking, expected_type=type_hints["enable_tracking"])
+            check_type(argname="argument encrypt_conf", value=encrypt_conf, expected_type=type_hints["encrypt_conf"])
+            check_type(argname="argument max_split_shard", value=max_split_shard, expected_type=type_hints["max_split_shard"])
+            check_type(argname="argument preserve_storage", value=preserve_storage, expected_type=type_hints["preserve_storage"])
+            check_type(argname="argument shard_count", value=shard_count, expected_type=type_hints["shard_count"])
+            check_type(argname="argument ttl", value=ttl, expected_type=type_hints["ttl"])
         self._values: typing.Dict[str, typing.Any] = {
             "logstore_name": logstore_name,
             "project_name": project_name,
         }
         if append_meta is not None:
             self._values["append_meta"] = append_meta
         if auto_split is not None:
@@ -7581,81 +8246,93 @@
 ):
     '''A ROS template type:  ``ALIYUN::SLS::LogtailConfig``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosLogtailConfigProps",
+        props: typing.Union["RosLogtailConfigProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::SLS::LogtailConfig``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosLogtailConfig.__init__)
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
+            type_hints = typing.get_type_hints(RosLogtailConfig._render_properties)
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
     @jsii.member(jsii_name="attrAppliedMachineGroups")
     def attr_applied_machine_groups(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: AppliedMachineGroups: Applied machine groups.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAppliedMachineGroups"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrEndpoint")
     def attr_endpoint(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Endpoint: Endpoint address.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrEndpoint"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrLogtailConfigName")
     def attr_logtail_config_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: LogtailConfigName: Logtail config name.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrLogtailConfigName"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosLogtailConfig, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="logstoreName")
     def logstore_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         logstoreName: Logstore name:
 
@@ -7666,17 +8343,20 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "logstoreName"))
 
     @logstore_name.setter
     def logstore_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosLogtailConfig, "logstore_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "logstoreName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="logtailConfigName")
     def logtail_config_name(
         self,
     ) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
@@ -7689,17 +8369,20 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "logtailConfigName"))
 
     @logtail_config_name.setter
     def logtail_config_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosLogtailConfig, "logtail_config_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "logtailConfigName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="projectName")
     def project_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         projectName: Project name:
 
@@ -7710,17 +8393,20 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "projectName"))
 
     @project_name.setter
     def project_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosLogtailConfig, "project_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "projectName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="cloneFrom")
     def clone_from(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosLogtailConfig.CloneFromProperty"]]:
         '''
         :Property:
 
@@ -7730,17 +8416,20 @@
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosLogtailConfig.CloneFromProperty"]], jsii.get(self, "cloneFrom"))
 
     @clone_from.setter
     def clone_from(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosLogtailConfig.CloneFromProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosLogtailConfig, "clone_from").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "cloneFrom", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rawConfigData")
     def raw_config_data(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]]]:
         '''
         :Property:
 
@@ -7815,14 +8504,17 @@
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]]], jsii.get(self, "rawConfigData"))
 
     @raw_config_data.setter
     def raw_config_data(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosLogtailConfig, "raw_config_data").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "rawConfigData", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-sls.RosLogtailConfig.CloneFromProperty",
         jsii_struct_bases=[],
         name_mapping={
             "logtail_config_name": "logtailConfigName",
@@ -7836,14 +8528,18 @@
             logtail_config_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             project_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         ) -> None:
             '''
             :param logtail_config_name: 
             :param project_name: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosLogtailConfig.CloneFromProperty.__init__)
+                check_type(argname="argument logtail_config_name", value=logtail_config_name, expected_type=type_hints["logtail_config_name"])
+                check_type(argname="argument project_name", value=project_name, expected_type=type_hints["project_name"])
             self._values: typing.Dict[str, typing.Any] = {
                 "logtail_config_name": logtail_config_name,
                 "project_name": project_name,
             }
 
         @builtins.property
         def logtail_config_name(
@@ -7903,25 +8599,32 @@
 class RosLogtailConfigProps:
     def __init__(
         self,
         *,
         logstore_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         logtail_config_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         project_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
-        clone_from: typing.Optional[typing.Union[ros_cdk_core.IResolvable, RosLogtailConfig.CloneFromProperty]] = None,
+        clone_from: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosLogtailConfig.CloneFromProperty, typing.Dict[str, typing.Any]]]] = None,
         raw_config_data: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Mapping[builtins.str, typing.Any]]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::SLS::LogtailConfig``.
 
         :param logstore_name: 
         :param logtail_config_name: 
         :param project_name: 
         :param clone_from: 
         :param raw_config_data: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosLogtailConfigProps.__init__)
+            check_type(argname="argument logstore_name", value=logstore_name, expected_type=type_hints["logstore_name"])
+            check_type(argname="argument logtail_config_name", value=logtail_config_name, expected_type=type_hints["logtail_config_name"])
+            check_type(argname="argument project_name", value=project_name, expected_type=type_hints["project_name"])
+            check_type(argname="argument clone_from", value=clone_from, expected_type=type_hints["clone_from"])
+            check_type(argname="argument raw_config_data", value=raw_config_data, expected_type=type_hints["raw_config_data"])
         self._values: typing.Dict[str, typing.Any] = {
             "logstore_name": logstore_name,
             "logtail_config_name": logtail_config_name,
             "project_name": project_name,
         }
         if clone_from is not None:
             self._values["clone_from"] = clone_from
@@ -8085,172 +8788,202 @@
 ):
     '''A ROS template type:  ``ALIYUN::SLS::MachineGroup``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosMachineGroupProps",
+        props: typing.Union["RosMachineGroupProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::SLS::MachineGroup``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosMachineGroup.__init__)
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
+            type_hints = typing.get_type_hints(RosMachineGroup._render_properties)
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
     @jsii.member(jsii_name="attrGroupName")
     def attr_group_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: GroupName: GroupName of SLS.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrGroupName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrProjectName")
     def attr_project_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ProjectName: ProjectName of SLS.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrProjectName"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosMachineGroup, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="groupAttribute")
     def group_attribute(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: groupAttribute: Group attribute, default is null. The object value is groupToic and externalName
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "groupAttribute"))
 
     @group_attribute.setter
     def group_attribute(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosMachineGroup, "group_attribute").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "groupAttribute", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="groupName")
     def group_name(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: groupName: Display name of the group name, the Project only. [2, 128] English or Chinese characters, must start with a letter or Chinese in size, can contain numbers, '_' or '.', '-'
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "groupName"))
 
     @group_name.setter
     def group_name(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosMachineGroup, "group_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "groupName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="groupType")
     def group_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: groupType: MachineGroup type, the value is empty or Armory
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "groupType"))
 
     @group_type.setter
     def group_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosMachineGroup, "group_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "groupType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="machineIdentifyType")
     def machine_identify_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: machineIdentifyType: Machine indentify type, the value is 'ip' or 'userdefined'
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "machineIdentifyType"))
 
     @machine_identify_type.setter
     def machine_identify_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosMachineGroup, "machine_identify_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "machineIdentifyType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="machineList")
     def machine_list(
         self,
     ) -> typing.Optional[typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]]:
         '''
         :Property: machineList: The machine tag, the value is ip or userdefined-id.
         '''
         return typing.cast(typing.Optional[typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]], jsii.get(self, "machineList"))
 
     @machine_list.setter
     def machine_list(
         self,
         value: typing.Optional[typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosMachineGroup, "machine_list").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "machineList", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="projectName")
     def project_name(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: projectName: MachineGroup created in project.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "projectName"))
 
     @project_name.setter
     def project_name(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosMachineGroup, "project_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "projectName", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-sls.RosMachineGroupProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -8278,14 +9011,22 @@
         :param group_attribute: 
         :param group_name: 
         :param group_type: 
         :param machine_identify_type: 
         :param machine_list: 
         :param project_name: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosMachineGroupProps.__init__)
+            check_type(argname="argument group_attribute", value=group_attribute, expected_type=type_hints["group_attribute"])
+            check_type(argname="argument group_name", value=group_name, expected_type=type_hints["group_name"])
+            check_type(argname="argument group_type", value=group_type, expected_type=type_hints["group_type"])
+            check_type(argname="argument machine_identify_type", value=machine_identify_type, expected_type=type_hints["machine_identify_type"])
+            check_type(argname="argument machine_list", value=machine_list, expected_type=type_hints["machine_list"])
+            check_type(argname="argument project_name", value=project_name, expected_type=type_hints["project_name"])
         self._values: typing.Dict[str, typing.Any] = {}
         if group_attribute is not None:
             self._values["group_attribute"] = group_attribute
         if group_name is not None:
             self._values["group_name"] = group_name
         if group_type is not None:
             self._values["group_type"] = group_type
@@ -8375,65 +9116,77 @@
 ):
     '''A ROS template type:  ``ALIYUN::SLS::MetricStore``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosMetricStoreProps",
+        props: typing.Union["RosMetricStoreProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::SLS::MetricStore``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosMetricStore.__init__)
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
+            type_hints = typing.get_type_hints(RosMetricStore._render_properties)
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
     @jsii.member(jsii_name="attrLogstoreName")
     def attr_logstore_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: LogstoreName: Metric store name.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrLogstoreName"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosMetricStore, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="logstoreName")
     def logstore_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         logstoreName: Metric store name:
 
@@ -8444,17 +9197,20 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "logstoreName"))
 
     @logstore_name.setter
     def logstore_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosMetricStore, "logstore_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "logstoreName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="projectName")
     def project_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         projectName: Project name:
 
@@ -8465,17 +9221,20 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "projectName"))
 
     @project_name.setter
     def project_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosMetricStore, "project_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "projectName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="preserveStorage")
     def preserve_storage(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -8486,17 +9245,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "preserveStorage"))
 
     @preserve_storage.setter
     def preserve_storage(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosMetricStore, "preserve_storage").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "preserveStorage", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="shardCount")
     def shard_count(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -8506,17 +9268,20 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "shardCount"))
 
     @shard_count.setter
     def shard_count(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosMetricStore, "shard_count").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "shardCount", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="ttl")
     def ttl(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -8526,14 +9291,17 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "ttl"))
 
     @ttl.setter
     def ttl(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosMetricStore, "ttl").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "ttl", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-sls.RosMetricStoreProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -8558,14 +9326,21 @@
 
         :param logstore_name: 
         :param project_name: 
         :param preserve_storage: 
         :param shard_count: 
         :param ttl: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosMetricStoreProps.__init__)
+            check_type(argname="argument logstore_name", value=logstore_name, expected_type=type_hints["logstore_name"])
+            check_type(argname="argument project_name", value=project_name, expected_type=type_hints["project_name"])
+            check_type(argname="argument preserve_storage", value=preserve_storage, expected_type=type_hints["preserve_storage"])
+            check_type(argname="argument shard_count", value=shard_count, expected_type=type_hints["shard_count"])
+            check_type(argname="argument ttl", value=ttl, expected_type=type_hints["ttl"])
         self._values: typing.Dict[str, typing.Any] = {
             "logstore_name": logstore_name,
             "project_name": project_name,
         }
         if preserve_storage is not None:
             self._values["preserve_storage"] = preserve_storage
         if shard_count is not None:
@@ -8662,65 +9437,77 @@
 ):
     '''A ROS template type:  ``ALIYUN::SLS::Project``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosProjectProps",
+        props: typing.Union["RosProjectProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::SLS::Project``.
 
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
     @jsii.member(jsii_name="attrName")
     def attr_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Name: Project name.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrName"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosProject, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="name")
     def name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         name: Project name:
 
@@ -8728,46 +9515,55 @@
         2. Must start and end with lowercase letters and numbers.
         3. The name length is 3-63 characters.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "name"))
 
     @name.setter
     def name(self, value: typing.Union[builtins.str, ros_cdk_core.IResolvable]) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosProject, "name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "name", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="description")
     def description(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: description: Project description: <>'"\\ is not supported, up to 64 characters.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "description"))
 
     @description.setter
     def description(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosProject, "description").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "description", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="tags")
     def tags(self) -> typing.Optional[typing.List["RosProject.TagsProperty"]]:
         '''
         :Property: tags: Tags to attach to project. Max support 20 tags to add during create project. Each tag with two properties Key and Value, and Key is required.
         '''
         return typing.cast(typing.Optional[typing.List["RosProject.TagsProperty"]], jsii.get(self, "tags"))
 
     @tags.setter
     def tags(
         self,
         value: typing.Optional[typing.List["RosProject.TagsProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosProject, "tags").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "tags", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-sls.RosProject.TagsProperty",
         jsii_struct_bases=[],
         name_mapping={"key": "key", "value": "value"},
     )
@@ -8778,14 +9574,18 @@
             key: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param key: 
             :param value: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosProject.TagsProperty.__init__)
+                check_type(argname="argument key", value=key, expected_type=type_hints["key"])
+                check_type(argname="argument value", value=value, expected_type=type_hints["value"])
             self._values: typing.Dict[str, typing.Any] = {
                 "key": key,
             }
             if value is not None:
                 self._values["value"] = value
 
         @builtins.property
@@ -8826,22 +9626,27 @@
 )
 class RosProjectProps:
     def __init__(
         self,
         *,
         name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         description: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        tags: typing.Optional[typing.Sequence[RosProject.TagsProperty]] = None,
+        tags: typing.Optional[typing.Sequence[typing.Union[RosProject.TagsProperty, typing.Dict[str, typing.Any]]]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::SLS::Project``.
 
         :param name: 
         :param description: 
         :param tags: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosProjectProps.__init__)
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
         self._values: typing.Dict[str, typing.Any] = {
             "name": name,
         }
         if description is not None:
             self._values["description"] = description
         if tags is not None:
             self._values["tags"] = tags
@@ -8898,94 +9703,112 @@
 ):
     '''A ROS template type:  ``ALIYUN::SLS::Savedsearch``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosSavedsearchProps",
+        props: typing.Union["RosSavedsearchProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::SLS::Savedsearch``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosSavedsearch.__init__)
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
+            type_hints = typing.get_type_hints(RosSavedsearch._render_properties)
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
     @jsii.member(jsii_name="attrSavedsearchName")
     def attr_savedsearch_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: SavedsearchName: Savedsearch name.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrSavedsearchName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="detail")
     def detail(
         self,
     ) -> typing.Union[ros_cdk_core.IResolvable, "RosSavedsearch.DetailProperty"]:
         '''
         :Property: detail:
         '''
         return typing.cast(typing.Union[ros_cdk_core.IResolvable, "RosSavedsearch.DetailProperty"], jsii.get(self, "detail"))
 
     @detail.setter
     def detail(
         self,
         value: typing.Union[ros_cdk_core.IResolvable, "RosSavedsearch.DetailProperty"],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSavedsearch, "detail").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "detail", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSavedsearch, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="project")
     def project(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: project: Project name
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "project"))
 
     @project.setter
     def project(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSavedsearch, "project").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "project", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-sls.RosSavedsearch.DetailProperty",
         jsii_struct_bases=[],
         name_mapping={
             "logstore": "logstore",
@@ -9008,14 +9831,21 @@
             '''
             :param logstore: 
             :param savedsearch_name: 
             :param search_query: 
             :param topic: 
             :param display_name: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosSavedsearch.DetailProperty.__init__)
+                check_type(argname="argument logstore", value=logstore, expected_type=type_hints["logstore"])
+                check_type(argname="argument savedsearch_name", value=savedsearch_name, expected_type=type_hints["savedsearch_name"])
+                check_type(argname="argument search_query", value=search_query, expected_type=type_hints["search_query"])
+                check_type(argname="argument topic", value=topic, expected_type=type_hints["topic"])
+                check_type(argname="argument display_name", value=display_name, expected_type=type_hints["display_name"])
             self._values: typing.Dict[str, typing.Any] = {
                 "logstore": logstore,
                 "savedsearch_name": savedsearch_name,
                 "search_query": search_query,
                 "topic": topic,
             }
             if display_name is not None:
@@ -9086,22 +9916,26 @@
     jsii_struct_bases=[],
     name_mapping={"detail": "detail", "project": "project"},
 )
 class RosSavedsearchProps:
     def __init__(
         self,
         *,
-        detail: typing.Union[ros_cdk_core.IResolvable, RosSavedsearch.DetailProperty],
+        detail: typing.Union[ros_cdk_core.IResolvable, typing.Union[RosSavedsearch.DetailProperty, typing.Dict[str, typing.Any]]],
         project: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
         '''Properties for defining a ``ALIYUN::SLS::Savedsearch``.
 
         :param detail: 
         :param project: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosSavedsearchProps.__init__)
+            check_type(argname="argument detail", value=detail, expected_type=type_hints["detail"])
+            check_type(argname="argument project", value=project, expected_type=type_hints["project"])
         self._values: typing.Dict[str, typing.Any] = {
             "detail": detail,
             "project": project,
         }
 
     @builtins.property
     def detail(
@@ -9142,31 +9976,37 @@
 ):
     '''A ROS resource type:  ``ALIYUN::SLS::Savedsearch``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "SavedsearchProps",
+        props: typing.Union["SavedsearchProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::SLS::Savedsearch``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(Savedsearch.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrSavedsearchName")
     def attr_savedsearch_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute SavedsearchName: Savedsearch name.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrSavedsearchName"))
 
 
 @jsii.data_type(
@@ -9174,22 +10014,26 @@
     jsii_struct_bases=[],
     name_mapping={"detail": "detail", "project": "project"},
 )
 class SavedsearchProps:
     def __init__(
         self,
         *,
-        detail: typing.Union[ros_cdk_core.IResolvable, RosSavedsearch.DetailProperty],
+        detail: typing.Union[ros_cdk_core.IResolvable, typing.Union[RosSavedsearch.DetailProperty, typing.Dict[str, typing.Any]]],
         project: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
         '''Properties for defining a ``ALIYUN::SLS::Savedsearch``.
 
         :param detail: Property detail:.
         :param project: Property project: Project name.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(SavedsearchProps.__init__)
+            check_type(argname="argument detail", value=detail, expected_type=type_hints["detail"])
+            check_type(argname="argument project", value=project, expected_type=type_hints["project"])
         self._values: typing.Dict[str, typing.Any] = {
             "detail": detail,
             "project": project,
         }
 
     @builtins.property
     def detail(
```

### Comparing `ros-cdk-sls-1.0.8/src/ros_cdk_sls.egg-info/PKG-INFO` & `ros-cdk-sls-1.0.9/src/ros_cdk_sls.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-sls
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS SLS Construct Library
```

