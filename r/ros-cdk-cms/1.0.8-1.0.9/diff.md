# Comparing `tmp/ros-cdk-cms-1.0.8.tar.gz` & `tmp/ros-cdk-cms-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-cms-1.0.8.tar", last modified: Thu Jul 14 02:23:55 2022, max compression
+gzip compressed data, was "dist/ros-cdk-cms-1.0.9.tar", last modified: Fri Sep 23 12:03:30 2022, max compression
```

## Comparing `ros-cdk-cms-1.0.8.tar` & `ros-cdk-cms-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:23:55.000000 ros-cdk-cms-1.0.8/
--rw-r--r--   0 root         (0) root         (0)    10279 2022-07-14 02:23:55.000000 ros-cdk-cms-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2022-07-14 02:23:55.000000 ros-cdk-cms-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2022-07-14 02:23:55.000000 ros-cdk-cms-1.0.8/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1240 2022-07-14 02:23:55.000000 ros-cdk-cms-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      179 2022-07-14 02:23:55.000000 ros-cdk-cms-1.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)      106 2022-07-14 02:23:55.000000 ros-cdk-cms-1.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-07-14 02:23:55.000000 ros-cdk-cms-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1794 2022-07-14 02:23:55.000000 ros-cdk-cms-1.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:23:55.000000 ros-cdk-cms-1.0.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:23:55.000000 ros-cdk-cms-1.0.8/src/ros_cdk_cms/
--rw-r--r--   0 root         (0) root         (0)   374606 2022-07-14 02:23:55.000000 ros-cdk-cms-1.0.8/src/ros_cdk_cms/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:23:55.000000 ros-cdk-cms-1.0.8/src/ros_cdk_cms/_jsii/
--rw-r--r--   0 root         (0) root         (0)      370 2022-07-14 02:23:55.000000 ros-cdk-cms-1.0.8/src/ros_cdk_cms/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)   142055 2022-07-14 02:23:55.000000 ros-cdk-cms-1.0.8/src/ros_cdk_cms/_jsii/ros-cdk-cms@1.0.8.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:23:55.000000 ros-cdk-cms-1.0.8/src/ros_cdk_cms/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:23:55.000000 ros-cdk-cms-1.0.8/src/ros_cdk_cms.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1240 2022-07-14 02:23:55.000000 ros-cdk-cms-1.0.8/src/ros_cdk_cms.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      400 2022-07-14 02:23:55.000000 ros-cdk-cms-1.0.8/src/ros_cdk_cms.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:23:55.000000 ros-cdk-cms-1.0.8/src/ros_cdk_cms.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2022-07-14 02:23:55.000000 ros-cdk-cms-1.0.8/src/ros_cdk_cms.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2022-07-14 02:23:55.000000 ros-cdk-cms-1.0.8/src/ros_cdk_cms.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:03:30.000000 ros-cdk-cms-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)    10279 2022-09-23 12:03:30.000000 ros-cdk-cms-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-09-23 12:03:30.000000 ros-cdk-cms-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2022-09-23 12:03:30.000000 ros-cdk-cms-1.0.9/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1240 2022-09-23 12:03:30.000000 ros-cdk-cms-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      179 2022-09-23 12:03:30.000000 ros-cdk-cms-1.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      236 2022-09-23 12:03:30.000000 ros-cdk-cms-1.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-09-23 12:03:30.000000 ros-cdk-cms-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1823 2022-09-23 12:03:30.000000 ros-cdk-cms-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:03:30.000000 ros-cdk-cms-1.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:03:30.000000 ros-cdk-cms-1.0.9/src/ros_cdk_cms/
+-rw-r--r--   0 root         (0) root         (0)   449524 2022-09-23 12:03:30.000000 ros-cdk-cms-1.0.9/src/ros_cdk_cms/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:03:30.000000 ros-cdk-cms-1.0.9/src/ros_cdk_cms/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      404 2022-09-23 12:03:30.000000 ros-cdk-cms-1.0.9/src/ros_cdk_cms/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   142122 2022-09-23 12:03:30.000000 ros-cdk-cms-1.0.9/src/ros_cdk_cms/_jsii/ros-cdk-cms@1.0.9.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 12:03:30.000000 ros-cdk-cms-1.0.9/src/ros_cdk_cms/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:03:30.000000 ros-cdk-cms-1.0.9/src/ros_cdk_cms.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1240 2022-09-23 12:03:30.000000 ros-cdk-cms-1.0.9/src/ros_cdk_cms.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      400 2022-09-23 12:03:30.000000 ros-cdk-cms-1.0.9/src/ros_cdk_cms.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 12:03:30.000000 ros-cdk-cms-1.0.9/src/ros_cdk_cms.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2022-09-23 12:03:30.000000 ros-cdk-cms-1.0.9/src/ros_cdk_cms.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2022-09-23 12:03:30.000000 ros-cdk-cms-1.0.9/src/ros_cdk_cms.egg-info/top_level.txt
```

### Comparing `ros-cdk-cms-1.0.8/LICENSE` & `ros-cdk-cms-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-cms-1.0.8/PKG-INFO` & `ros-cdk-cms-1.0.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-cms
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS CMS Construct Library
```

### Comparing `ros-cdk-cms-1.0.8/setup.py` & `ros-cdk-cms-1.0.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-cms",
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
         "ros_cdk_cms",
         "ros_cdk_cms._jsii"
     ],
     "package_data": {
         "ros_cdk_cms._jsii": [
-            "ros-cdk-cms@1.0.8.jsii.tgz"
+            "ros-cdk-cms@1.0.9.jsii.tgz"
         ],
         "ros_cdk_cms": [
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

### Comparing `ros-cdk-cms-1.0.8/src/ros_cdk_cms/__init__.py` & `ros-cdk-cms-1.0.9/src/ros_cdk_cms/__init__.py`

 * *Files 26% similar despite different names*

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
 
 
 class Contact(
     ros_cdk_core.Resource,
@@ -29,31 +31,37 @@
 ):
     '''A ROS resource type:  ``ALIYUN::CMS::Contact``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "ContactProps",
+        props: typing.Union["ContactProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::CMS::Contact``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(Contact.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrContactName")
     def attr_contact_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute ContactName: The name of the alarm contact.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrContactName"))
 
 
 class ContactGroup(
@@ -63,31 +71,37 @@
 ):
     '''A ROS resource type:  ``ALIYUN::CMS::ContactGroup``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "ContactGroupProps",
+        props: typing.Union["ContactGroupProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::CMS::ContactGroup``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(ContactGroup.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrContactGroupName")
     def attr_contact_group_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute ContactGroupName: The name of the alert contact group.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrContactGroupName"))
 
 
 @jsii.data_type(
@@ -109,14 +123,19 @@
     ) -> None:
         '''Properties for defining a ``ALIYUN::CMS::ContactGroup``.
 
         :param contact_group_name: Property contactGroupName: The name of the alert contact group.
         :param contact_names: Property contactNames: The name of the alert contact.
         :param describe: Property describe: The description of the alert contact group.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(ContactGroupProps.__init__)
+            check_type(argname="argument contact_group_name", value=contact_group_name, expected_type=type_hints["contact_group_name"])
+            check_type(argname="argument contact_names", value=contact_names, expected_type=type_hints["contact_names"])
+            check_type(argname="argument describe", value=describe, expected_type=type_hints["describe"])
         self._values: typing.Dict[str, typing.Any] = {
             "contact_group_name": contact_group_name,
             "contact_names": contact_names,
             "describe": describe,
         }
 
     @builtins.property
@@ -165,24 +184,29 @@
         "describe": "describe",
     },
 )
 class ContactProps:
     def __init__(
         self,
         *,
-        channels: typing.Union["RosContact.ChannelsProperty", ros_cdk_core.IResolvable],
+        channels: typing.Union[typing.Union["RosContact.ChannelsProperty", typing.Dict[str, typing.Any]], ros_cdk_core.IResolvable],
         contact_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         describe: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
         '''Properties for defining a ``ALIYUN::CMS::Contact``.
 
         :param channels: Property channels: undefined.
         :param contact_name: Property contactName: The name of the alarm contact.
         :param describe: Property describe: The description of the alert contact.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(ContactProps.__init__)
+            check_type(argname="argument channels", value=channels, expected_type=type_hints["channels"])
+            check_type(argname="argument contact_name", value=contact_name, expected_type=type_hints["contact_name"])
+            check_type(argname="argument describe", value=describe, expected_type=type_hints["describe"])
         self._values: typing.Dict[str, typing.Any] = {
             "channels": channels,
             "contact_name": contact_name,
             "describe": describe,
         }
 
     @builtins.property
@@ -227,37 +251,43 @@
 ):
     '''A ROS resource type:  ``ALIYUN::CMS::DynamicTagGroup``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "DynamicTagGroupProps",
+        props: typing.Union["DynamicTagGroupProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::CMS::DynamicTagGroup``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(DynamicTagGroup.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDynamicTagRuleId")
     def attr_dynamic_tag_rule_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute DynamicTagRuleId: Dynamic tag rule ID.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDynamicTagRuleId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTagKey")
     def attr_tag_key(self) -> ros_cdk_core.IResolvable:
         '''Attribute TagKey: Tag key.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTagKey"))
 
 
 @jsii.data_type(
@@ -277,28 +307,37 @@
     def __init__(
         self,
         *,
         contact_group_list: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]],
         tag_key: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         enable_install_agent: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         enable_subscribe_event: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
-        match_express: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosDynamicTagGroup.MatchExpressProperty"]]]] = None,
+        match_express: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosDynamicTagGroup.MatchExpressProperty", typing.Dict[str, typing.Any]]]]]] = None,
         match_express_filter_relation: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         template_id_list: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::CMS::DynamicTagGroup``.
 
         :param contact_group_list: Property contactGroupList: Alarm contacts.
         :param tag_key: Property tagKey: Tag key.
         :param enable_install_agent: Property enableInstallAgent: Whether to enable initial installation monitoring plug, not installed by default. Values are: true: enable installation Note If ECS generated instances group does not monitor plug-in installed will attempt to automatically install. false: disable installation
         :param enable_subscribe_event: Property enableSubscribeEvent: Whether the event subscription is enabled. Values are :true: enable event subscription false: disable event subscription
         :param match_express: Property matchExpress: Matching list. Only supports one currently.
         :param match_express_filter_relation: Property matchExpressFilterRelation: The relationship between the conditional expressions. Values are: and: the relationship between or: the relationship or the Description currently supports only one combination of conditions, the follow-up Ali cloud will support a variety of combinations of conditions.
         :param template_id_list: Property templateIdList: Alarm template ID list. When the automatically generated application group synchronizes tags, it will generate alarm rules according to the specified alarm template.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(DynamicTagGroupProps.__init__)
+            check_type(argname="argument contact_group_list", value=contact_group_list, expected_type=type_hints["contact_group_list"])
+            check_type(argname="argument tag_key", value=tag_key, expected_type=type_hints["tag_key"])
+            check_type(argname="argument enable_install_agent", value=enable_install_agent, expected_type=type_hints["enable_install_agent"])
+            check_type(argname="argument enable_subscribe_event", value=enable_subscribe_event, expected_type=type_hints["enable_subscribe_event"])
+            check_type(argname="argument match_express", value=match_express, expected_type=type_hints["match_express"])
+            check_type(argname="argument match_express_filter_relation", value=match_express_filter_relation, expected_type=type_hints["match_express_filter_relation"])
+            check_type(argname="argument template_id_list", value=template_id_list, expected_type=type_hints["template_id_list"])
         self._values: typing.Dict[str, typing.Any] = {
             "contact_group_list": contact_group_list,
             "tag_key": tag_key,
         }
         if enable_install_agent is not None:
             self._values["enable_install_agent"] = enable_install_agent
         if enable_subscribe_event is not None:
@@ -408,31 +447,37 @@
 ):
     '''A ROS resource type:  ``ALIYUN::CMS::EventRule``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "EventRuleProps",
+        props: typing.Union["EventRuleProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::CMS::EventRule``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(EventRule.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrData")
     def attr_data(self) -> ros_cdk_core.IResolvable:
         '''Attribute Data: Number of rows affected.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrData"))
 
 
 @jsii.data_type(
@@ -447,15 +492,15 @@
         "state": "state",
     },
 )
 class EventRuleProps:
     def __init__(
         self,
         *,
-        event_pattern: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosEventRule.EventPatternProperty"]]],
+        event_pattern: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosEventRule.EventPatternProperty", typing.Dict[str, typing.Any]]]]],
         rule_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         description: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         event_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         group_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         state: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::CMS::EventRule``.
@@ -463,14 +508,22 @@
         :param event_pattern: Property eventPattern: Event pattern configuration.A maximum of 20 event patterns.
         :param rule_name: Property ruleName: The name of the alarm rule.
         :param description: Property description: The description of the alert rule.
         :param event_type: Property eventType: The type of the event alert. Valid values: SYSTEM CUSTOM
         :param group_id: Property groupId: The ID of the application group.
         :param state: Property state: The status of the alert rule. Valid values: ENABLED DISABLED
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(EventRuleProps.__init__)
+            check_type(argname="argument event_pattern", value=event_pattern, expected_type=type_hints["event_pattern"])
+            check_type(argname="argument rule_name", value=rule_name, expected_type=type_hints["rule_name"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument event_type", value=event_type, expected_type=type_hints["event_type"])
+            check_type(argname="argument group_id", value=group_id, expected_type=type_hints["group_id"])
+            check_type(argname="argument state", value=state, expected_type=type_hints["state"])
         self._values: typing.Dict[str, typing.Any] = {
             "event_pattern": event_pattern,
             "rule_name": rule_name,
         }
         if description is not None:
             self._values["description"] = description
         if event_type is not None:
@@ -557,28 +610,34 @@
 ):
     '''A ROS resource type:  ``ALIYUN::CMS::EventRuleTargets``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "EventRuleTargetsProps",
+        props: typing.Union["EventRuleTargetsProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::CMS::EventRuleTargets``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(EventRuleTargets.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-cms.EventRuleTargetsProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -591,29 +650,37 @@
     },
 )
 class EventRuleTargetsProps:
     def __init__(
         self,
         *,
         rule_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
-        contact_parameters: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosEventRuleTargets.ContactParametersProperty"]]]] = None,
-        fc_parameters: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosEventRuleTargets.FcParametersProperty"]]]] = None,
-        mns_parameters: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosEventRuleTargets.MnsParametersProperty"]]]] = None,
-        sls_parameters: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosEventRuleTargets.SlsParametersProperty"]]]] = None,
-        webhook_parameters: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosEventRuleTargets.WebhookParametersProperty"]]]] = None,
+        contact_parameters: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosEventRuleTargets.ContactParametersProperty", typing.Dict[str, typing.Any]]]]]] = None,
+        fc_parameters: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosEventRuleTargets.FcParametersProperty", typing.Dict[str, typing.Any]]]]]] = None,
+        mns_parameters: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosEventRuleTargets.MnsParametersProperty", typing.Dict[str, typing.Any]]]]]] = None,
+        sls_parameters: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosEventRuleTargets.SlsParametersProperty", typing.Dict[str, typing.Any]]]]]] = None,
+        webhook_parameters: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosEventRuleTargets.WebhookParametersProperty", typing.Dict[str, typing.Any]]]]]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::CMS::EventRuleTargets``.
 
         :param rule_name: Property ruleName: The name of the alert rule.
         :param contact_parameters: Property contactParameters: CONTACT configuration.A maximum of 5 parameters.
         :param fc_parameters: Property fcParameters: FC configuration.A maximum of 5 parameters.
         :param mns_parameters: Property mnsParameters: MNS configuration.A maximum of 5 parameters.
         :param sls_parameters: Property slsParameters: SLS configuration.A maximum of 5 parameters.
         :param webhook_parameters: Property webhookParameters: WEBHOOK configuration.A maximum of 5 parameters.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(EventRuleTargetsProps.__init__)
+            check_type(argname="argument rule_name", value=rule_name, expected_type=type_hints["rule_name"])
+            check_type(argname="argument contact_parameters", value=contact_parameters, expected_type=type_hints["contact_parameters"])
+            check_type(argname="argument fc_parameters", value=fc_parameters, expected_type=type_hints["fc_parameters"])
+            check_type(argname="argument mns_parameters", value=mns_parameters, expected_type=type_hints["mns_parameters"])
+            check_type(argname="argument sls_parameters", value=sls_parameters, expected_type=type_hints["sls_parameters"])
+            check_type(argname="argument webhook_parameters", value=webhook_parameters, expected_type=type_hints["webhook_parameters"])
         self._values: typing.Dict[str, typing.Any] = {
             "rule_name": rule_name,
         }
         if contact_parameters is not None:
             self._values["contact_parameters"] = contact_parameters
         if fc_parameters is not None:
             self._values["fc_parameters"] = fc_parameters
@@ -690,31 +757,37 @@
 ):
     '''A ROS resource type:  ``ALIYUN::CMS::GroupMetricRule``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "GroupMetricRuleProps",
+        props: typing.Union["GroupMetricRuleProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::CMS::GroupMetricRule``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(GroupMetricRule.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrRuleId")
     def attr_rule_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute RuleId: Rule ID.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrRuleId"))
 
 
 @jsii.data_type(
@@ -739,15 +812,15 @@
     },
 )
 class GroupMetricRuleProps:
     def __init__(
         self,
         *,
         category: typing.Union[builtins.str, ros_cdk_core.IResolvable],
-        escalations: typing.Union[ros_cdk_core.IResolvable, "RosGroupMetricRule.EscalationsProperty"],
+        escalations: typing.Union[ros_cdk_core.IResolvable, typing.Union["RosGroupMetricRule.EscalationsProperty", typing.Dict[str, typing.Any]]],
         group_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         metric_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         namespace: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         rule_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         rule_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         dimensions: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         effective_interval: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
@@ -772,14 +845,31 @@
         :param email_subject: Property emailSubject: The subject of the alert notification email.
         :param interval: Property interval: The detection period of alerts.
         :param no_effective_interval: Property noEffectiveInterval: The period when the alert rule is ineffective.
         :param period: Property period: The aggregation period. Unite: second.
         :param silence_time: Property silenceTime: The duration of the mute period during which new alerts are not sent even if the trigger conditions are met. Unit: second. Default value: 86400. Minimum value: 60.
         :param webhook: Property webhook: The URL of the callback triggered when an alert occurs.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(GroupMetricRuleProps.__init__)
+            check_type(argname="argument category", value=category, expected_type=type_hints["category"])
+            check_type(argname="argument escalations", value=escalations, expected_type=type_hints["escalations"])
+            check_type(argname="argument group_id", value=group_id, expected_type=type_hints["group_id"])
+            check_type(argname="argument metric_name", value=metric_name, expected_type=type_hints["metric_name"])
+            check_type(argname="argument namespace", value=namespace, expected_type=type_hints["namespace"])
+            check_type(argname="argument rule_id", value=rule_id, expected_type=type_hints["rule_id"])
+            check_type(argname="argument rule_name", value=rule_name, expected_type=type_hints["rule_name"])
+            check_type(argname="argument dimensions", value=dimensions, expected_type=type_hints["dimensions"])
+            check_type(argname="argument effective_interval", value=effective_interval, expected_type=type_hints["effective_interval"])
+            check_type(argname="argument email_subject", value=email_subject, expected_type=type_hints["email_subject"])
+            check_type(argname="argument interval", value=interval, expected_type=type_hints["interval"])
+            check_type(argname="argument no_effective_interval", value=no_effective_interval, expected_type=type_hints["no_effective_interval"])
+            check_type(argname="argument period", value=period, expected_type=type_hints["period"])
+            check_type(argname="argument silence_time", value=silence_time, expected_type=type_hints["silence_time"])
+            check_type(argname="argument webhook", value=webhook, expected_type=type_hints["webhook"])
         self._values: typing.Dict[str, typing.Any] = {
             "category": category,
             "escalations": escalations,
             "group_id": group_id,
             "metric_name": metric_name,
             "namespace": namespace,
             "rule_id": rule_id,
@@ -991,37 +1081,43 @@
 ):
     '''A ROS resource type:  ``ALIYUN::CMS::MetricRuleTargets``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "MetricRuleTargetsProps",
+        props: typing.Union["MetricRuleTargetsProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::CMS::MetricRuleTargets``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(MetricRuleTargets.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrArns")
     def attr_arns(self) -> ros_cdk_core.IResolvable:
         '''Attribute Arns: The ARN list of targets.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrArns"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrIds")
     def attr_ids(self) -> ros_cdk_core.IResolvable:
         '''Attribute Ids: The ID list of targets.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrIds"))
 
 
 @jsii.data_type(
@@ -1030,21 +1126,25 @@
     name_mapping={"rule_id": "ruleId", "targets": "targets"},
 )
 class MetricRuleTargetsProps:
     def __init__(
         self,
         *,
         rule_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
-        targets: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosMetricRuleTargets.TargetsProperty"]]],
+        targets: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosMetricRuleTargets.TargetsProperty", typing.Dict[str, typing.Any]]]]],
     ) -> None:
         '''Properties for defining a ``ALIYUN::CMS::MetricRuleTargets``.
 
         :param rule_id: Property ruleId: The ID of the alert rule.
         :param targets: Property targets: undefined.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(MetricRuleTargetsProps.__init__)
+            check_type(argname="argument rule_id", value=rule_id, expected_type=type_hints["rule_id"])
+            check_type(argname="argument targets", value=targets, expected_type=type_hints["targets"])
         self._values: typing.Dict[str, typing.Any] = {
             "rule_id": rule_id,
             "targets": targets,
         }
 
     @builtins.property
     def rule_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
@@ -1081,31 +1181,37 @@
 ):
     '''A ROS resource type:  ``ALIYUN::CMS::MetricRuleTemplate``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "MetricRuleTemplateProps",
+        props: typing.Union["MetricRuleTemplateProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::CMS::MetricRuleTemplate``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(MetricRuleTemplate.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrId")
     def attr_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute Id: Alarm template ID.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrId"))
 
 
 @jsii.data_type(
@@ -1120,27 +1226,34 @@
     },
 )
 class MetricRuleTemplateProps:
     def __init__(
         self,
         *,
         name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
-        alert_templates: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosMetricRuleTemplate.AlertTemplatesProperty"]]]] = None,
+        alert_templates: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosMetricRuleTemplate.AlertTemplatesProperty", typing.Dict[str, typing.Any]]]]]] = None,
         description: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         rest_version: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         template_id: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::CMS::MetricRuleTemplate``.
 
         :param name: Property name: The name of the alert template.
         :param alert_templates: Property alertTemplates: Valid values of N: 0 to 200.
         :param description: Property description: The description of the alert template.
         :param rest_version: Property restVersion: The version of the alert template. Call DescribeMetricRuleTemplateList or DescribeMetricRuleTemplateAttribute to obtain information about the alert templates. The combination of version and ID uniquely identifies an alert template.
         :param template_id: Property templateId: The ID of the alert template.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(MetricRuleTemplateProps.__init__)
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+            check_type(argname="argument alert_templates", value=alert_templates, expected_type=type_hints["alert_templates"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument rest_version", value=rest_version, expected_type=type_hints["rest_version"])
+            check_type(argname="argument template_id", value=template_id, expected_type=type_hints["template_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "name": name,
         }
         if alert_templates is not None:
             self._values["alert_templates"] = alert_templates
         if description is not None:
             self._values["description"] = description
@@ -1212,31 +1325,37 @@
 ):
     '''A ROS resource type:  ``ALIYUN::CMS::MonitorGroup``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "MonitorGroupProps",
+        props: typing.Union["MonitorGroupProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::CMS::MonitorGroup``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(MonitorGroup.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrGroupId")
     def attr_group_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute GroupId: Application group ID generated after the group is created.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrGroupId"))
 
 
 class MonitorGroupInstances(
@@ -1246,31 +1365,37 @@
 ):
     '''A ROS resource type:  ``ALIYUN::CMS::MonitorGroupInstances``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "MonitorGroupInstancesProps",
+        props: typing.Union["MonitorGroupInstancesProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::CMS::MonitorGroupInstances``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(MonitorGroupInstances.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrGroupId")
     def attr_group_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute GroupId: The ID of the application group.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrGroupId"))
 
 
 @jsii.data_type(
@@ -1279,21 +1404,25 @@
     name_mapping={"group_id": "groupId", "instances": "instances"},
 )
 class MonitorGroupInstancesProps:
     def __init__(
         self,
         *,
         group_id: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
-        instances: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosMonitorGroupInstances.InstancesProperty"]]],
+        instances: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosMonitorGroupInstances.InstancesProperty", typing.Dict[str, typing.Any]]]]],
     ) -> None:
         '''Properties for defining a ``ALIYUN::CMS::MonitorGroupInstances``.
 
         :param group_id: Property groupId: The ID of the application group.
         :param instances: Property instances:.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(MonitorGroupInstancesProps.__init__)
+            check_type(argname="argument group_id", value=group_id, expected_type=type_hints["group_id"])
+            check_type(argname="argument instances", value=instances, expected_type=type_hints["instances"])
         self._values: typing.Dict[str, typing.Any] = {
             "group_id": group_id,
             "instances": instances,
         }
 
     @builtins.property
     def group_id(self) -> typing.Union[jsii.Number, ros_cdk_core.IResolvable]:
@@ -1336,14 +1465,18 @@
         contact_groups: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::CMS::MonitorGroup``.
 
         :param group_name: Property groupName: The name of the application group.
         :param contact_groups: Property contactGroups: The alert contact group. Alert notifications for the application group are sent to the specified alert contact group.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(MonitorGroupProps.__init__)
+            check_type(argname="argument group_name", value=group_name, expected_type=type_hints["group_name"])
+            check_type(argname="argument contact_groups", value=contact_groups, expected_type=type_hints["contact_groups"])
         self._values: typing.Dict[str, typing.Any] = {
             "group_name": group_name,
         }
         if contact_groups is not None:
             self._values["contact_groups"] = contact_groups
 
     @builtins.property
@@ -1384,31 +1517,37 @@
 ):
     '''A ROS resource type:  ``ALIYUN::CMS::MonitoringAgentProcess``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "MonitoringAgentProcessProps",
+        props: typing.Union["MonitoringAgentProcessProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::CMS::MonitoringAgentProcess``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(MonitoringAgentProcess.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrId")
     def attr_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute Id: The process ID.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrId"))
 
 
 @jsii.data_type(
@@ -1430,14 +1569,19 @@
     ) -> None:
         '''Properties for defining a ``ALIYUN::CMS::MonitoringAgentProcess``.
 
         :param instance_id: Property instanceId: The ID of the instance.
         :param process_name: Property processName: The name of the process.
         :param process_user: Property processUser: The user who launched the process.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(MonitoringAgentProcessProps.__init__)
+            check_type(argname="argument instance_id", value=instance_id, expected_type=type_hints["instance_id"])
+            check_type(argname="argument process_name", value=process_name, expected_type=type_hints["process_name"])
+            check_type(argname="argument process_user", value=process_user, expected_type=type_hints["process_user"])
         self._values: typing.Dict[str, typing.Any] = {
             "instance_id": instance_id,
         }
         if process_name is not None:
             self._values["process_name"] = process_name
         if process_user is not None:
             self._values["process_user"] = process_user
@@ -1484,37 +1628,43 @@
 ):
     '''A ROS resource type:  ``ALIYUN::CMS::ResourceMetricRule``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "ResourceMetricRuleProps",
+        props: typing.Union["ResourceMetricRuleProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::CMS::ResourceMetricRule``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(ResourceMetricRule.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrRuleId")
     def attr_rule_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute RuleId: The ID of the alert rule.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrRuleId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrRuleName")
     def attr_rule_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute RuleName: The name of the alert rule.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrRuleName"))
 
 
 @jsii.data_type(
@@ -1543,28 +1693,28 @@
     },
 )
 class ResourceMetricRuleProps:
     def __init__(
         self,
         *,
         contact_groups: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]],
-        escalations: typing.Union[ros_cdk_core.IResolvable, "RosResourceMetricRule.EscalationsProperty"],
+        escalations: typing.Union[ros_cdk_core.IResolvable, typing.Union["RosResourceMetricRule.EscalationsProperty", typing.Dict[str, typing.Any]]],
         metric_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         namespace: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         resources: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Mapping[builtins.str, typing.Any]]],
-        composite_expression: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosResourceMetricRule.CompositeExpressionProperty"]] = None,
+        composite_expression: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosResourceMetricRule.CompositeExpressionProperty", typing.Dict[str, typing.Any]]]] = None,
         deletion_force: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         effective_interval: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         email_subject: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         interval: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
-        labels: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosResourceMetricRule.LabelsProperty"]]]] = None,
+        labels: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosResourceMetricRule.LabelsProperty", typing.Dict[str, typing.Any]]]]]] = None,
         no_data_policy: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         no_effective_interval: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         period: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
-        prometheus: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosResourceMetricRule.PrometheusProperty"]] = None,
+        prometheus: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosResourceMetricRule.PrometheusProperty", typing.Dict[str, typing.Any]]]] = None,
         rule_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         rule_name: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         silence_time: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         webhook: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::CMS::ResourceMetricRule``.
 
@@ -1584,14 +1734,35 @@
         :param period: Property period: The statistical period of the metric. Unit: seconds. The default value is the interval at which the monitoring data of the metric is collected. Note: For information about how to query the statistical period of a metric, see Appendix 1: Metrics.
         :param prometheus: Property prometheus: The Prometheus alert rule. Note: This parameter is required only when you create a Prometheus alert rule for Hybrid Cloud Monitoring.
         :param rule_id: Property ruleId: The ID of the alert rule. If not specified, ROS will generate one. You can specify a new ID or the ID of an existing alert rule. For information about how to query the ID of an alert rule, see DescribeMetricRuleList. Note: If you specify a new ID, a threshold-triggered alert rule is created.
         :param rule_name: Property ruleName: The name of the alert rule. If not specified and the rule is created by ROS, default to RuleId. You can specify a new name or the name of an existing alert rule. For information about how to query the name of an alert rule, see DescribeMetricRuleList. Note: If you specify a new name, a threshold-triggered alert rule is created.
         :param silence_time: Property silenceTime: The mute period during which new alerts are not sent even if the trigger conditions are met. Unit: seconds. Default value: 86400. Note: If an alert is not cleared within the mute period, a new alert notification is sent when the mute period ends.
         :param webhook: Property webhook: The callback URL to which a POST request is sent when an alert is triggered based on the alert rule.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(ResourceMetricRuleProps.__init__)
+            check_type(argname="argument contact_groups", value=contact_groups, expected_type=type_hints["contact_groups"])
+            check_type(argname="argument escalations", value=escalations, expected_type=type_hints["escalations"])
+            check_type(argname="argument metric_name", value=metric_name, expected_type=type_hints["metric_name"])
+            check_type(argname="argument namespace", value=namespace, expected_type=type_hints["namespace"])
+            check_type(argname="argument resources", value=resources, expected_type=type_hints["resources"])
+            check_type(argname="argument composite_expression", value=composite_expression, expected_type=type_hints["composite_expression"])
+            check_type(argname="argument deletion_force", value=deletion_force, expected_type=type_hints["deletion_force"])
+            check_type(argname="argument effective_interval", value=effective_interval, expected_type=type_hints["effective_interval"])
+            check_type(argname="argument email_subject", value=email_subject, expected_type=type_hints["email_subject"])
+            check_type(argname="argument interval", value=interval, expected_type=type_hints["interval"])
+            check_type(argname="argument labels", value=labels, expected_type=type_hints["labels"])
+            check_type(argname="argument no_data_policy", value=no_data_policy, expected_type=type_hints["no_data_policy"])
+            check_type(argname="argument no_effective_interval", value=no_effective_interval, expected_type=type_hints["no_effective_interval"])
+            check_type(argname="argument period", value=period, expected_type=type_hints["period"])
+            check_type(argname="argument prometheus", value=prometheus, expected_type=type_hints["prometheus"])
+            check_type(argname="argument rule_id", value=rule_id, expected_type=type_hints["rule_id"])
+            check_type(argname="argument rule_name", value=rule_name, expected_type=type_hints["rule_name"])
+            check_type(argname="argument silence_time", value=silence_time, expected_type=type_hints["silence_time"])
+            check_type(argname="argument webhook", value=webhook, expected_type=type_hints["webhook"])
         self._values: typing.Dict[str, typing.Any] = {
             "contact_groups": contact_groups,
             "escalations": escalations,
             "metric_name": metric_name,
             "namespace": namespace,
             "resources": resources,
         }
@@ -1850,109 +2021,130 @@
 ):
     '''A ROS template type:  ``ALIYUN::CMS::Contact``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosContactProps",
+        props: typing.Union["RosContactProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::CMS::Contact``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosContact.__init__)
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
+            type_hints = typing.get_type_hints(RosContact._render_properties)
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
     @jsii.member(jsii_name="attrContactName")
     def attr_contact_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ContactName: The name of the alarm contact.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrContactName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="channels")
     def channels(
         self,
     ) -> typing.Union["RosContact.ChannelsProperty", ros_cdk_core.IResolvable]:
         '''
         :Property: channels: undefined
         '''
         return typing.cast(typing.Union["RosContact.ChannelsProperty", ros_cdk_core.IResolvable], jsii.get(self, "channels"))
 
     @channels.setter
     def channels(
         self,
         value: typing.Union["RosContact.ChannelsProperty", ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosContact, "channels").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "channels", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="contactName")
     def contact_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: contactName: The name of the alarm contact.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "contactName"))
 
     @contact_name.setter
     def contact_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosContact, "contact_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "contactName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="describe")
     def describe(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: describe: The description of the alert contact.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "describe"))
 
     @describe.setter
     def describe(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosContact, "describe").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "describe", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosContact, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-cms.RosContact.ChannelsProperty",
         jsii_struct_bases=[],
         name_mapping={
             "ali_im": "aliIm",
@@ -1972,14 +2164,20 @@
         ) -> None:
             '''
             :param ali_im: 
             :param ding_web_hook: 
             :param mail: 
             :param sms: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosContact.ChannelsProperty.__init__)
+                check_type(argname="argument ali_im", value=ali_im, expected_type=type_hints["ali_im"])
+                check_type(argname="argument ding_web_hook", value=ding_web_hook, expected_type=type_hints["ding_web_hook"])
+                check_type(argname="argument mail", value=mail, expected_type=type_hints["mail"])
+                check_type(argname="argument sms", value=sms, expected_type=type_hints["sms"])
             self._values: typing.Dict[str, typing.Any] = {}
             if ali_im is not None:
                 self._values["ali_im"] = ali_im
             if ding_web_hook is not None:
                 self._values["ding_web_hook"] = ding_web_hook
             if mail is not None:
                 self._values["mail"] = mail
@@ -2045,111 +2243,132 @@
 ):
     '''A ROS template type:  ``ALIYUN::CMS::ContactGroup``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosContactGroupProps",
+        props: typing.Union["RosContactGroupProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::CMS::ContactGroup``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosContactGroup.__init__)
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
+            type_hints = typing.get_type_hints(RosContactGroup._render_properties)
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
     @jsii.member(jsii_name="attrContactGroupName")
     def attr_contact_group_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ContactGroupName: The name of the alert contact group.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrContactGroupName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="contactGroupName")
     def contact_group_name(
         self,
     ) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: contactGroupName: The name of the alert contact group.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "contactGroupName"))
 
     @contact_group_name.setter
     def contact_group_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosContactGroup, "contact_group_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "contactGroupName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="contactNames")
     def contact_names(
         self,
     ) -> typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]:
         '''
         :Property: contactNames: The name of the alert contact.
         '''
         return typing.cast(typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]], jsii.get(self, "contactNames"))
 
     @contact_names.setter
     def contact_names(
         self,
         value: typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosContactGroup, "contact_names").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "contactNames", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="describe")
     def describe(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: describe: The description of the alert contact group.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "describe"))
 
     @describe.setter
     def describe(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosContactGroup, "describe").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "describe", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosContactGroup, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-cms.RosContactGroupProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -2168,14 +2387,19 @@
     ) -> None:
         '''Properties for defining a ``ALIYUN::CMS::ContactGroup``.
 
         :param contact_group_name: 
         :param contact_names: 
         :param describe: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosContactGroupProps.__init__)
+            check_type(argname="argument contact_group_name", value=contact_group_name, expected_type=type_hints["contact_group_name"])
+            check_type(argname="argument contact_names", value=contact_names, expected_type=type_hints["contact_names"])
+            check_type(argname="argument describe", value=describe, expected_type=type_hints["describe"])
         self._values: typing.Dict[str, typing.Any] = {
             "contact_group_name": contact_group_name,
             "contact_names": contact_names,
             "describe": describe,
         }
 
     @builtins.property
@@ -2230,24 +2454,29 @@
         "describe": "describe",
     },
 )
 class RosContactProps:
     def __init__(
         self,
         *,
-        channels: typing.Union[RosContact.ChannelsProperty, ros_cdk_core.IResolvable],
+        channels: typing.Union[typing.Union[RosContact.ChannelsProperty, typing.Dict[str, typing.Any]], ros_cdk_core.IResolvable],
         contact_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         describe: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
         '''Properties for defining a ``ALIYUN::CMS::Contact``.
 
         :param channels: 
         :param contact_name: 
         :param describe: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosContactProps.__init__)
+            check_type(argname="argument channels", value=channels, expected_type=type_hints["channels"])
+            check_type(argname="argument contact_name", value=contact_name, expected_type=type_hints["contact_name"])
+            check_type(argname="argument describe", value=describe, expected_type=type_hints["describe"])
         self._values: typing.Dict[str, typing.Any] = {
             "channels": channels,
             "contact_name": contact_name,
             "describe": describe,
         }
 
     @builtins.property
@@ -2298,105 +2527,123 @@
 ):
     '''A ROS template type:  ``ALIYUN::CMS::DynamicTagGroup``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosDynamicTagGroupProps",
+        props: typing.Union["RosDynamicTagGroupProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::CMS::DynamicTagGroup``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosDynamicTagGroup.__init__)
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
+            type_hints = typing.get_type_hints(RosDynamicTagGroup._render_properties)
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
     @jsii.member(jsii_name="attrDynamicTagRuleId")
     def attr_dynamic_tag_rule_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: DynamicTagRuleId: Dynamic tag rule ID.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDynamicTagRuleId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTagKey")
     def attr_tag_key(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: TagKey: Tag key.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTagKey"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="contactGroupList")
     def contact_group_list(
         self,
     ) -> typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]:
         '''
         :Property: contactGroupList: Alarm contacts.
         '''
         return typing.cast(typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]], jsii.get(self, "contactGroupList"))
 
     @contact_group_list.setter
     def contact_group_list(
         self,
         value: typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDynamicTagGroup, "contact_group_list").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "contactGroupList", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDynamicTagGroup, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="tagKey")
     def tag_key(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: tagKey: Tag key.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "tagKey"))
 
     @tag_key.setter
     def tag_key(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDynamicTagGroup, "tag_key").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "tagKey", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableInstallAgent")
     def enable_install_agent(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -2408,17 +2655,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "enableInstallAgent"))
 
     @enable_install_agent.setter
     def enable_install_agent(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDynamicTagGroup, "enable_install_agent").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableInstallAgent", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableSubscribeEvent")
     def enable_subscribe_event(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -2429,34 +2679,40 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "enableSubscribeEvent"))
 
     @enable_subscribe_event.setter
     def enable_subscribe_event(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDynamicTagGroup, "enable_subscribe_event").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableSubscribeEvent", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="matchExpress")
     def match_express(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosDynamicTagGroup.MatchExpressProperty"]]]]:
         '''
         :Property: matchExpress: Matching list. Only supports one currently.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosDynamicTagGroup.MatchExpressProperty"]]]], jsii.get(self, "matchExpress"))
 
     @match_express.setter
     def match_express(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosDynamicTagGroup.MatchExpressProperty"]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDynamicTagGroup, "match_express").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "matchExpress", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="matchExpressFilterRelation")
     def match_express_filter_relation(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -2468,17 +2724,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "matchExpressFilterRelation"))
 
     @match_express_filter_relation.setter
     def match_express_filter_relation(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDynamicTagGroup, "match_express_filter_relation").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "matchExpressFilterRelation", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="templateIdList")
     def template_id_list(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]]:
         '''
         :Property:
 
@@ -2488,14 +2747,17 @@
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]], jsii.get(self, "templateIdList"))
 
     @template_id_list.setter
     def template_id_list(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDynamicTagGroup, "template_id_list").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "templateIdList", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-cms.RosDynamicTagGroup.MatchExpressProperty",
         jsii_struct_bases=[],
         name_mapping={
             "tag_value": "tagValue",
@@ -2509,14 +2771,18 @@
             tag_value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             tag_value_match_function: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         ) -> None:
             '''
             :param tag_value: 
             :param tag_value_match_function: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosDynamicTagGroup.MatchExpressProperty.__init__)
+                check_type(argname="argument tag_value", value=tag_value, expected_type=type_hints["tag_value"])
+                check_type(argname="argument tag_value_match_function", value=tag_value_match_function, expected_type=type_hints["tag_value_match_function"])
             self._values: typing.Dict[str, typing.Any] = {
                 "tag_value": tag_value,
                 "tag_value_match_function": tag_value_match_function,
             }
 
         @builtins.property
         def tag_value(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
@@ -2575,28 +2841,37 @@
     def __init__(
         self,
         *,
         contact_group_list: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]],
         tag_key: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         enable_install_agent: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         enable_subscribe_event: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
-        match_express: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosDynamicTagGroup.MatchExpressProperty]]]] = None,
+        match_express: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosDynamicTagGroup.MatchExpressProperty, typing.Dict[str, typing.Any]]]]]] = None,
         match_express_filter_relation: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         template_id_list: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::CMS::DynamicTagGroup``.
 
         :param contact_group_list: 
         :param tag_key: 
         :param enable_install_agent: 
         :param enable_subscribe_event: 
         :param match_express: 
         :param match_express_filter_relation: 
         :param template_id_list: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosDynamicTagGroupProps.__init__)
+            check_type(argname="argument contact_group_list", value=contact_group_list, expected_type=type_hints["contact_group_list"])
+            check_type(argname="argument tag_key", value=tag_key, expected_type=type_hints["tag_key"])
+            check_type(argname="argument enable_install_agent", value=enable_install_agent, expected_type=type_hints["enable_install_agent"])
+            check_type(argname="argument enable_subscribe_event", value=enable_subscribe_event, expected_type=type_hints["enable_subscribe_event"])
+            check_type(argname="argument match_express", value=match_express, expected_type=type_hints["match_express"])
+            check_type(argname="argument match_express_filter_relation", value=match_express_filter_relation, expected_type=type_hints["match_express_filter_relation"])
+            check_type(argname="argument template_id_list", value=template_id_list, expected_type=type_hints["template_id_list"])
         self._values: typing.Dict[str, typing.Any] = {
             "contact_group_list": contact_group_list,
             "tag_key": tag_key,
         }
         if enable_install_agent is not None:
             self._values["enable_install_agent"] = enable_install_agent
         if enable_subscribe_event is not None:
@@ -2714,114 +2989,135 @@
 ):
     '''A ROS template type:  ``ALIYUN::CMS::EventRule``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosEventRuleProps",
+        props: typing.Union["RosEventRuleProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::CMS::EventRule``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosEventRule.__init__)
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
+            type_hints = typing.get_type_hints(RosEventRule._render_properties)
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
     @jsii.member(jsii_name="attrData")
     def attr_data(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Data: Number of rows affected.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrData"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosEventRule, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="eventPattern")
     def event_pattern(
         self,
     ) -> typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosEventRule.EventPatternProperty"]]]:
         '''
         :Property: eventPattern: Event pattern configuration.A maximum of 20 event patterns.
         '''
         return typing.cast(typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosEventRule.EventPatternProperty"]]], jsii.get(self, "eventPattern"))
 
     @event_pattern.setter
     def event_pattern(
         self,
         value: typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosEventRule.EventPatternProperty"]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosEventRule, "event_pattern").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "eventPattern", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="ruleName")
     def rule_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: ruleName: The name of the alarm rule.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "ruleName"))
 
     @rule_name.setter
     def rule_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosEventRule, "rule_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "ruleName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="description")
     def description(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: description: The description of the alert rule.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "description"))
 
     @description.setter
     def description(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosEventRule, "description").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "description", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="eventType")
     def event_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -2832,34 +3128,40 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "eventType"))
 
     @event_type.setter
     def event_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosEventRule, "event_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "eventType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="groupId")
     def group_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: groupId: The ID of the application group.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "groupId"))
 
     @group_id.setter
     def group_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosEventRule, "group_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "groupId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="state")
     def state(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -2870,14 +3172,17 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "state"))
 
     @state.setter
     def state(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosEventRule, "state").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "state", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-cms.RosEventRule.EventPatternProperty",
         jsii_struct_bases=[],
         name_mapping={
             "event_type_list": "eventTypeList",
@@ -2900,14 +3205,21 @@
             '''
             :param event_type_list: 
             :param level_list: 
             :param name_list: 
             :param product: 
             :param status_list: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosEventRule.EventPatternProperty.__init__)
+                check_type(argname="argument event_type_list", value=event_type_list, expected_type=type_hints["event_type_list"])
+                check_type(argname="argument level_list", value=level_list, expected_type=type_hints["level_list"])
+                check_type(argname="argument name_list", value=name_list, expected_type=type_hints["name_list"])
+                check_type(argname="argument product", value=product, expected_type=type_hints["product"])
+                check_type(argname="argument status_list", value=status_list, expected_type=type_hints["status_list"])
             self._values: typing.Dict[str, typing.Any] = {}
             if event_type_list is not None:
                 self._values["event_type_list"] = event_type_list
             if level_list is not None:
                 self._values["level_list"] = level_list
             if name_list is not None:
                 self._values["name_list"] = name_list
@@ -2993,15 +3305,15 @@
         "state": "state",
     },
 )
 class RosEventRuleProps:
     def __init__(
         self,
         *,
-        event_pattern: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosEventRule.EventPatternProperty]]],
+        event_pattern: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosEventRule.EventPatternProperty, typing.Dict[str, typing.Any]]]]],
         rule_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         description: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         event_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         group_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         state: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::CMS::EventRule``.
@@ -3009,14 +3321,22 @@
         :param event_pattern: 
         :param rule_name: 
         :param description: 
         :param event_type: 
         :param group_id: 
         :param state: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosEventRuleProps.__init__)
+            check_type(argname="argument event_pattern", value=event_pattern, expected_type=type_hints["event_pattern"])
+            check_type(argname="argument rule_name", value=rule_name, expected_type=type_hints["rule_name"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument event_type", value=event_type, expected_type=type_hints["event_type"])
+            check_type(argname="argument group_id", value=group_id, expected_type=type_hints["group_id"])
+            check_type(argname="argument state", value=state, expected_type=type_hints["state"])
         self._values: typing.Dict[str, typing.Any] = {
             "event_pattern": event_pattern,
             "rule_name": rule_name,
         }
         if description is not None:
             self._values["description"] = description
         if event_type is not None:
@@ -3113,155 +3433,185 @@
 ):
     '''A ROS template type:  ``ALIYUN::CMS::EventRuleTargets``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosEventRuleTargetsProps",
+        props: typing.Union["RosEventRuleTargetsProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::CMS::EventRuleTargets``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosEventRuleTargets.__init__)
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
+            type_hints = typing.get_type_hints(RosEventRuleTargets._render_properties)
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
+            type_hints = typing.get_type_hints(getattr(RosEventRuleTargets, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="ruleName")
     def rule_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: ruleName: The name of the alert rule.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "ruleName"))
 
     @rule_name.setter
     def rule_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosEventRuleTargets, "rule_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "ruleName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="contactParameters")
     def contact_parameters(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosEventRuleTargets.ContactParametersProperty"]]]]:
         '''
         :Property: contactParameters: CONTACT configuration.A maximum of 5 parameters
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosEventRuleTargets.ContactParametersProperty"]]]], jsii.get(self, "contactParameters"))
 
     @contact_parameters.setter
     def contact_parameters(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosEventRuleTargets.ContactParametersProperty"]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosEventRuleTargets, "contact_parameters").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "contactParameters", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="fcParameters")
     def fc_parameters(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosEventRuleTargets.FcParametersProperty"]]]]:
         '''
         :Property: fcParameters: FC configuration.A maximum of 5 parameters.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosEventRuleTargets.FcParametersProperty"]]]], jsii.get(self, "fcParameters"))
 
     @fc_parameters.setter
     def fc_parameters(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosEventRuleTargets.FcParametersProperty"]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosEventRuleTargets, "fc_parameters").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "fcParameters", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="mnsParameters")
     def mns_parameters(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosEventRuleTargets.MnsParametersProperty"]]]]:
         '''
         :Property: mnsParameters: MNS configuration.A maximum of 5 parameters
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosEventRuleTargets.MnsParametersProperty"]]]], jsii.get(self, "mnsParameters"))
 
     @mns_parameters.setter
     def mns_parameters(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosEventRuleTargets.MnsParametersProperty"]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosEventRuleTargets, "mns_parameters").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "mnsParameters", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="slsParameters")
     def sls_parameters(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosEventRuleTargets.SlsParametersProperty"]]]]:
         '''
         :Property: slsParameters: SLS configuration.A maximum of 5 parameters.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosEventRuleTargets.SlsParametersProperty"]]]], jsii.get(self, "slsParameters"))
 
     @sls_parameters.setter
     def sls_parameters(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosEventRuleTargets.SlsParametersProperty"]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosEventRuleTargets, "sls_parameters").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "slsParameters", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="webhookParameters")
     def webhook_parameters(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosEventRuleTargets.WebhookParametersProperty"]]]]:
         '''
         :Property: webhookParameters: WEBHOOK configuration.A maximum of 5 parameters.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosEventRuleTargets.WebhookParametersProperty"]]]], jsii.get(self, "webhookParameters"))
 
     @webhook_parameters.setter
     def webhook_parameters(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosEventRuleTargets.WebhookParametersProperty"]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosEventRuleTargets, "webhook_parameters").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "webhookParameters", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-cms.RosEventRuleTargets.ContactParametersProperty",
         jsii_struct_bases=[],
         name_mapping={
             "contact_group_name": "contactGroupName",
@@ -3278,14 +3628,19 @@
             level: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param contact_group_name: 
             :param id: 
             :param level: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosEventRuleTargets.ContactParametersProperty.__init__)
+                check_type(argname="argument contact_group_name", value=contact_group_name, expected_type=type_hints["contact_group_name"])
+                check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+                check_type(argname="argument level", value=level, expected_type=type_hints["level"])
             self._values: typing.Dict[str, typing.Any] = {}
             if contact_group_name is not None:
                 self._values["contact_group_name"] = contact_group_name
             if id is not None:
                 self._values["id"] = id
             if level is not None:
                 self._values["level"] = level
@@ -3352,14 +3707,20 @@
         ) -> None:
             '''
             :param function_name: 
             :param id: 
             :param region: 
             :param service_name: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosEventRuleTargets.FcParametersProperty.__init__)
+                check_type(argname="argument function_name", value=function_name, expected_type=type_hints["function_name"])
+                check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+                check_type(argname="argument region", value=region, expected_type=type_hints["region"])
+                check_type(argname="argument service_name", value=service_name, expected_type=type_hints["service_name"])
             self._values: typing.Dict[str, typing.Any] = {}
             if function_name is not None:
                 self._values["function_name"] = function_name
             if id is not None:
                 self._values["id"] = id
             if region is not None:
                 self._values["region"] = region
@@ -3431,14 +3792,19 @@
             region: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param id: 
             :param queue: 
             :param region: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosEventRuleTargets.MnsParametersProperty.__init__)
+                check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+                check_type(argname="argument queue", value=queue, expected_type=type_hints["queue"])
+                check_type(argname="argument region", value=region, expected_type=type_hints["region"])
             self._values: typing.Dict[str, typing.Any] = {}
             if id is not None:
                 self._values["id"] = id
             if queue is not None:
                 self._values["queue"] = queue
             if region is not None:
                 self._values["region"] = region
@@ -3505,14 +3871,20 @@
         ) -> None:
             '''
             :param id: 
             :param log_store: 
             :param project: 
             :param region: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosEventRuleTargets.SlsParametersProperty.__init__)
+                check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+                check_type(argname="argument log_store", value=log_store, expected_type=type_hints["log_store"])
+                check_type(argname="argument project", value=project, expected_type=type_hints["project"])
+                check_type(argname="argument region", value=region, expected_type=type_hints["region"])
             self._values: typing.Dict[str, typing.Any] = {}
             if id is not None:
                 self._values["id"] = id
             if log_store is not None:
                 self._values["log_store"] = log_store
             if project is not None:
                 self._values["project"] = project
@@ -3591,14 +3963,20 @@
         ) -> None:
             '''
             :param id: 
             :param method: 
             :param protocol: 
             :param url: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosEventRuleTargets.WebhookParametersProperty.__init__)
+                check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+                check_type(argname="argument method", value=method, expected_type=type_hints["method"])
+                check_type(argname="argument protocol", value=protocol, expected_type=type_hints["protocol"])
+                check_type(argname="argument url", value=url, expected_type=type_hints["url"])
             self._values: typing.Dict[str, typing.Any] = {}
             if id is not None:
                 self._values["id"] = id
             if method is not None:
                 self._values["method"] = method
             if protocol is not None:
                 self._values["protocol"] = protocol
@@ -3670,29 +4048,37 @@
     },
 )
 class RosEventRuleTargetsProps:
     def __init__(
         self,
         *,
         rule_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
-        contact_parameters: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosEventRuleTargets.ContactParametersProperty]]]] = None,
-        fc_parameters: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosEventRuleTargets.FcParametersProperty]]]] = None,
-        mns_parameters: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosEventRuleTargets.MnsParametersProperty]]]] = None,
-        sls_parameters: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosEventRuleTargets.SlsParametersProperty]]]] = None,
-        webhook_parameters: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosEventRuleTargets.WebhookParametersProperty]]]] = None,
+        contact_parameters: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosEventRuleTargets.ContactParametersProperty, typing.Dict[str, typing.Any]]]]]] = None,
+        fc_parameters: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosEventRuleTargets.FcParametersProperty, typing.Dict[str, typing.Any]]]]]] = None,
+        mns_parameters: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosEventRuleTargets.MnsParametersProperty, typing.Dict[str, typing.Any]]]]]] = None,
+        sls_parameters: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosEventRuleTargets.SlsParametersProperty, typing.Dict[str, typing.Any]]]]]] = None,
+        webhook_parameters: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosEventRuleTargets.WebhookParametersProperty, typing.Dict[str, typing.Any]]]]]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::CMS::EventRuleTargets``.
 
         :param rule_name: 
         :param contact_parameters: 
         :param fc_parameters: 
         :param mns_parameters: 
         :param sls_parameters: 
         :param webhook_parameters: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosEventRuleTargetsProps.__init__)
+            check_type(argname="argument rule_name", value=rule_name, expected_type=type_hints["rule_name"])
+            check_type(argname="argument contact_parameters", value=contact_parameters, expected_type=type_hints["contact_parameters"])
+            check_type(argname="argument fc_parameters", value=fc_parameters, expected_type=type_hints["fc_parameters"])
+            check_type(argname="argument mns_parameters", value=mns_parameters, expected_type=type_hints["mns_parameters"])
+            check_type(argname="argument sls_parameters", value=sls_parameters, expected_type=type_hints["sls_parameters"])
+            check_type(argname="argument webhook_parameters", value=webhook_parameters, expected_type=type_hints["webhook_parameters"])
         self._values: typing.Dict[str, typing.Any] = {
             "rule_name": rule_name,
         }
         if contact_parameters is not None:
             self._values["contact_parameters"] = contact_parameters
         if fc_parameters is not None:
             self._values["fc_parameters"] = fc_parameters
@@ -3781,56 +4167,65 @@
 ):
     '''A ROS template type:  ``ALIYUN::CMS::GroupMetricRule``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosGroupMetricRuleProps",
+        props: typing.Union["RosGroupMetricRuleProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::CMS::GroupMetricRule``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosGroupMetricRule.__init__)
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
+            type_hints = typing.get_type_hints(RosGroupMetricRule._render_properties)
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
     @jsii.member(jsii_name="attrRuleId")
     def attr_rule_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: RuleId: Rule ID.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrRuleId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="category")
     def category(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         category: The abbreviation of the service name. Valid values:
         ECS (including Alibaba Cloud and non-Alibaba Cloud hosts)
@@ -3872,73 +4267,88 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "category"))
 
     @category.setter
     def category(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosGroupMetricRule, "category").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "category", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosGroupMetricRule, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="escalations")
     def escalations(
         self,
     ) -> typing.Union[ros_cdk_core.IResolvable, "RosGroupMetricRule.EscalationsProperty"]:
         '''
         :Property: escalations: undefined
         '''
         return typing.cast(typing.Union[ros_cdk_core.IResolvable, "RosGroupMetricRule.EscalationsProperty"], jsii.get(self, "escalations"))
 
     @escalations.setter
     def escalations(
         self,
         value: typing.Union[ros_cdk_core.IResolvable, "RosGroupMetricRule.EscalationsProperty"],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosGroupMetricRule, "escalations").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "escalations", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="groupId")
     def group_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: groupId: The ID of application group.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "groupId"))
 
     @group_id.setter
     def group_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosGroupMetricRule, "group_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "groupId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="metricName")
     def metric_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: metricName: The name of the metric. For more information, call DescribeMetricMetaList or see Preset metrics reference.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "metricName"))
 
     @metric_name.setter
     def metric_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosGroupMetricRule, "metric_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "metricName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="namespace")
     def namespace(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         namespace: The data namespace of the service. For more information, call DescribeMetricMetaList
         or see Preset metrics reference.
@@ -3946,17 +4356,20 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "namespace"))
 
     @namespace.setter
     def namespace(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosGroupMetricRule, "namespace").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "namespace", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="ruleId")
     def rule_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         ruleId: The ID of the alert rule. The IDs of alert rules are generated by callers to ensure
         uniqueness.
@@ -3964,134 +4377,158 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "ruleId"))
 
     @rule_id.setter
     def rule_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosGroupMetricRule, "rule_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "ruleId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="ruleName")
     def rule_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: ruleName: The name of the alert rule.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "ruleName"))
 
     @rule_name.setter
     def rule_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosGroupMetricRule, "rule_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "ruleName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dimensions")
     def dimensions(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: dimensions: The expended resource dimensions.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "dimensions"))
 
     @dimensions.setter
     def dimensions(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosGroupMetricRule, "dimensions").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dimensions", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="effectiveInterval")
     def effective_interval(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: effectiveInterval: The period when the alert rule is effective.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "effectiveInterval"))
 
     @effective_interval.setter
     def effective_interval(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosGroupMetricRule, "effective_interval").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "effectiveInterval", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="emailSubject")
     def email_subject(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: emailSubject: The subject of the alert notification email.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "emailSubject"))
 
     @email_subject.setter
     def email_subject(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosGroupMetricRule, "email_subject").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "emailSubject", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="interval")
     def interval(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: interval: The detection period of alerts.
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "interval"))
 
     @interval.setter
     def interval(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosGroupMetricRule, "interval").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "interval", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="noEffectiveInterval")
     def no_effective_interval(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: noEffectiveInterval: The period when the alert rule is ineffective.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "noEffectiveInterval"))
 
     @no_effective_interval.setter
     def no_effective_interval(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosGroupMetricRule, "no_effective_interval").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "noEffectiveInterval", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="period")
     def period(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: period: The aggregation period. Unite: second.
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "period"))
 
     @period.setter
     def period(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosGroupMetricRule, "period").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "period", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="silenceTime")
     def silence_time(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -4101,31 +4538,37 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "silenceTime"))
 
     @silence_time.setter
     def silence_time(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosGroupMetricRule, "silence_time").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "silenceTime", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="webhook")
     def webhook(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: webhook: The URL of the callback triggered when an alert occurs.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "webhook"))
 
     @webhook.setter
     def webhook(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosGroupMetricRule, "webhook").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "webhook", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-cms.RosGroupMetricRule.CriticalProperty",
         jsii_struct_bases=[],
         name_mapping={
             "comparison_operator": "comparisonOperator",
@@ -4145,14 +4588,20 @@
         ) -> None:
             '''
             :param comparison_operator: 
             :param statistics: 
             :param threshold: 
             :param times: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosGroupMetricRule.CriticalProperty.__init__)
+                check_type(argname="argument comparison_operator", value=comparison_operator, expected_type=type_hints["comparison_operator"])
+                check_type(argname="argument statistics", value=statistics, expected_type=type_hints["statistics"])
+                check_type(argname="argument threshold", value=threshold, expected_type=type_hints["threshold"])
+                check_type(argname="argument times", value=times, expected_type=type_hints["times"])
             self._values: typing.Dict[str, typing.Any] = {
                 "comparison_operator": comparison_operator,
                 "statistics": statistics,
                 "threshold": threshold,
                 "times": times,
             }
 
@@ -4229,23 +4678,28 @@
         jsii_struct_bases=[],
         name_mapping={"critical": "critical", "info": "info", "warn": "warn"},
     )
     class EscalationsProperty:
         def __init__(
             self,
             *,
-            critical: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosGroupMetricRule.CriticalProperty"]] = None,
-            info: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosGroupMetricRule.InfoProperty"]] = None,
-            warn: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosGroupMetricRule.WarnProperty"]] = None,
+            critical: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosGroupMetricRule.CriticalProperty", typing.Dict[str, typing.Any]]]] = None,
+            info: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosGroupMetricRule.InfoProperty", typing.Dict[str, typing.Any]]]] = None,
+            warn: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosGroupMetricRule.WarnProperty", typing.Dict[str, typing.Any]]]] = None,
         ) -> None:
             '''
             :param critical: 
             :param info: 
             :param warn: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosGroupMetricRule.EscalationsProperty.__init__)
+                check_type(argname="argument critical", value=critical, expected_type=type_hints["critical"])
+                check_type(argname="argument info", value=info, expected_type=type_hints["info"])
+                check_type(argname="argument warn", value=warn, expected_type=type_hints["warn"])
             self._values: typing.Dict[str, typing.Any] = {}
             if critical is not None:
                 self._values["critical"] = critical
             if info is not None:
                 self._values["info"] = info
             if warn is not None:
                 self._values["warn"] = warn
@@ -4312,14 +4766,20 @@
         ) -> None:
             '''
             :param comparison_operator: 
             :param statistics: 
             :param threshold: 
             :param times: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosGroupMetricRule.InfoProperty.__init__)
+                check_type(argname="argument comparison_operator", value=comparison_operator, expected_type=type_hints["comparison_operator"])
+                check_type(argname="argument statistics", value=statistics, expected_type=type_hints["statistics"])
+                check_type(argname="argument threshold", value=threshold, expected_type=type_hints["threshold"])
+                check_type(argname="argument times", value=times, expected_type=type_hints["times"])
             self._values: typing.Dict[str, typing.Any] = {
                 "comparison_operator": comparison_operator,
                 "statistics": statistics,
                 "threshold": threshold,
                 "times": times,
             }
 
@@ -4409,14 +4869,20 @@
         ) -> None:
             '''
             :param comparison_operator: 
             :param statistics: 
             :param threshold: 
             :param times: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosGroupMetricRule.WarnProperty.__init__)
+                check_type(argname="argument comparison_operator", value=comparison_operator, expected_type=type_hints["comparison_operator"])
+                check_type(argname="argument statistics", value=statistics, expected_type=type_hints["statistics"])
+                check_type(argname="argument threshold", value=threshold, expected_type=type_hints["threshold"])
+                check_type(argname="argument times", value=times, expected_type=type_hints["times"])
             self._values: typing.Dict[str, typing.Any] = {
                 "comparison_operator": comparison_operator,
                 "statistics": statistics,
                 "threshold": threshold,
                 "times": times,
             }
 
@@ -4508,15 +4974,15 @@
     },
 )
 class RosGroupMetricRuleProps:
     def __init__(
         self,
         *,
         category: typing.Union[builtins.str, ros_cdk_core.IResolvable],
-        escalations: typing.Union[ros_cdk_core.IResolvable, RosGroupMetricRule.EscalationsProperty],
+        escalations: typing.Union[ros_cdk_core.IResolvable, typing.Union[RosGroupMetricRule.EscalationsProperty, typing.Dict[str, typing.Any]]],
         group_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         metric_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         namespace: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         rule_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         rule_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         dimensions: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         effective_interval: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
@@ -4541,14 +5007,31 @@
         :param email_subject: 
         :param interval: 
         :param no_effective_interval: 
         :param period: 
         :param silence_time: 
         :param webhook: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosGroupMetricRuleProps.__init__)
+            check_type(argname="argument category", value=category, expected_type=type_hints["category"])
+            check_type(argname="argument escalations", value=escalations, expected_type=type_hints["escalations"])
+            check_type(argname="argument group_id", value=group_id, expected_type=type_hints["group_id"])
+            check_type(argname="argument metric_name", value=metric_name, expected_type=type_hints["metric_name"])
+            check_type(argname="argument namespace", value=namespace, expected_type=type_hints["namespace"])
+            check_type(argname="argument rule_id", value=rule_id, expected_type=type_hints["rule_id"])
+            check_type(argname="argument rule_name", value=rule_name, expected_type=type_hints["rule_name"])
+            check_type(argname="argument dimensions", value=dimensions, expected_type=type_hints["dimensions"])
+            check_type(argname="argument effective_interval", value=effective_interval, expected_type=type_hints["effective_interval"])
+            check_type(argname="argument email_subject", value=email_subject, expected_type=type_hints["email_subject"])
+            check_type(argname="argument interval", value=interval, expected_type=type_hints["interval"])
+            check_type(argname="argument no_effective_interval", value=no_effective_interval, expected_type=type_hints["no_effective_interval"])
+            check_type(argname="argument period", value=period, expected_type=type_hints["period"])
+            check_type(argname="argument silence_time", value=silence_time, expected_type=type_hints["silence_time"])
+            check_type(argname="argument webhook", value=webhook, expected_type=type_hints["webhook"])
         self._values: typing.Dict[str, typing.Any] = {
             "category": category,
             "escalations": escalations,
             "group_id": group_id,
             "metric_name": metric_name,
             "namespace": namespace,
             "rule_id": rule_id,
@@ -4781,102 +5264,120 @@
 ):
     '''A ROS template type:  ``ALIYUN::CMS::MetricRuleTargets``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosMetricRuleTargetsProps",
+        props: typing.Union["RosMetricRuleTargetsProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::CMS::MetricRuleTargets``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosMetricRuleTargets.__init__)
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
+            type_hints = typing.get_type_hints(RosMetricRuleTargets._render_properties)
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
     @jsii.member(jsii_name="attrArns")
     def attr_arns(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Arns: The ARN list of targets
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrArns"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrIds")
     def attr_ids(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Ids: The ID list of targets
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrIds"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosMetricRuleTargets, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="ruleId")
     def rule_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: ruleId: The ID of the alert rule.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "ruleId"))
 
     @rule_id.setter
     def rule_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosMetricRuleTargets, "rule_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "ruleId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="targets")
     def targets(
         self,
     ) -> typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosMetricRuleTargets.TargetsProperty"]]]:
         '''
         :Property: targets: undefined
         '''
         return typing.cast(typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosMetricRuleTargets.TargetsProperty"]]], jsii.get(self, "targets"))
 
     @targets.setter
     def targets(
         self,
         value: typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosMetricRuleTargets.TargetsProperty"]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosMetricRuleTargets, "targets").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "targets", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-cms.RosMetricRuleTargets.TargetsProperty",
         jsii_struct_bases=[],
         name_mapping={"arn": "arn", "id": "id", "level": "level"},
     )
@@ -4889,14 +5390,19 @@
             level: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param arn: 
             :param id: 
             :param level: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosMetricRuleTargets.TargetsProperty.__init__)
+                check_type(argname="argument arn", value=arn, expected_type=type_hints["arn"])
+                check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+                check_type(argname="argument level", value=level, expected_type=type_hints["level"])
             self._values: typing.Dict[str, typing.Any] = {
                 "arn": arn,
                 "id": id,
             }
             if level is not None:
                 self._values["level"] = level
 
@@ -4962,21 +5468,25 @@
     name_mapping={"rule_id": "ruleId", "targets": "targets"},
 )
 class RosMetricRuleTargetsProps:
     def __init__(
         self,
         *,
         rule_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
-        targets: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosMetricRuleTargets.TargetsProperty]]],
+        targets: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosMetricRuleTargets.TargetsProperty, typing.Dict[str, typing.Any]]]]],
     ) -> None:
         '''Properties for defining a ``ALIYUN::CMS::MetricRuleTargets``.
 
         :param rule_id: 
         :param targets: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosMetricRuleTargetsProps.__init__)
+            check_type(argname="argument rule_id", value=rule_id, expected_type=type_hints["rule_id"])
+            check_type(argname="argument targets", value=targets, expected_type=type_hints["targets"])
         self._values: typing.Dict[str, typing.Any] = {
             "rule_id": rule_id,
             "targets": targets,
         }
 
     @builtins.property
     def rule_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
@@ -5017,111 +5527,132 @@
 ):
     '''A ROS template type:  ``ALIYUN::CMS::MetricRuleTemplate``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosMetricRuleTemplateProps",
+        props: typing.Union["RosMetricRuleTemplateProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::CMS::MetricRuleTemplate``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosMetricRuleTemplate.__init__)
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
+            type_hints = typing.get_type_hints(RosMetricRuleTemplate._render_properties)
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
     @jsii.member(jsii_name="attrId")
     def attr_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Id: Alarm template ID.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrId"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosMetricRuleTemplate, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="name")
     def name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: name: The name of the alert template.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "name"))
 
     @name.setter
     def name(self, value: typing.Union[builtins.str, ros_cdk_core.IResolvable]) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosMetricRuleTemplate, "name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "name", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="alertTemplates")
     def alert_templates(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosMetricRuleTemplate.AlertTemplatesProperty"]]]]:
         '''
         :Property: alertTemplates: Valid values of N: 0 to 200.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosMetricRuleTemplate.AlertTemplatesProperty"]]]], jsii.get(self, "alertTemplates"))
 
     @alert_templates.setter
     def alert_templates(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosMetricRuleTemplate.AlertTemplatesProperty"]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosMetricRuleTemplate, "alert_templates").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "alertTemplates", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="description")
     def description(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: description: The description of the alert template.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "description"))
 
     @description.setter
     def description(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosMetricRuleTemplate, "description").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "description", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="restVersion")
     def rest_version(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -5132,31 +5663,37 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "restVersion"))
 
     @rest_version.setter
     def rest_version(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosMetricRuleTemplate, "rest_version").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "restVersion", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="templateId")
     def template_id(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: templateId: The ID of the alert template.
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "templateId"))
 
     @template_id.setter
     def template_id(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosMetricRuleTemplate, "template_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "templateId", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-cms.RosMetricRuleTemplate.AlertTemplatesProperty",
         jsii_struct_bases=[],
         name_mapping={
             "category": "category",
@@ -5173,29 +5710,39 @@
         def __init__(
             self,
             *,
             category: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             metric_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             namespace: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             rule_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
-            escalations: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosMetricRuleTemplate.EscalationsProperty"]] = None,
+            escalations: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosMetricRuleTemplate.EscalationsProperty", typing.Dict[str, typing.Any]]]] = None,
             period: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
             selector: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
             webhook: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param category: 
             :param metric_name: 
             :param namespace: 
             :param rule_name: 
             :param escalations: 
             :param period: 
             :param selector: 
             :param webhook: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosMetricRuleTemplate.AlertTemplatesProperty.__init__)
+                check_type(argname="argument category", value=category, expected_type=type_hints["category"])
+                check_type(argname="argument metric_name", value=metric_name, expected_type=type_hints["metric_name"])
+                check_type(argname="argument namespace", value=namespace, expected_type=type_hints["namespace"])
+                check_type(argname="argument rule_name", value=rule_name, expected_type=type_hints["rule_name"])
+                check_type(argname="argument escalations", value=escalations, expected_type=type_hints["escalations"])
+                check_type(argname="argument period", value=period, expected_type=type_hints["period"])
+                check_type(argname="argument selector", value=selector, expected_type=type_hints["selector"])
+                check_type(argname="argument webhook", value=webhook, expected_type=type_hints["webhook"])
             self._values: typing.Dict[str, typing.Any] = {
                 "category": category,
                 "metric_name": metric_name,
                 "namespace": namespace,
                 "rule_name": rule_name,
             }
             if escalations is not None:
@@ -5366,14 +5913,20 @@
         ) -> None:
             '''
             :param comparison_operator: 
             :param statistics: 
             :param threshold: 
             :param times: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosMetricRuleTemplate.CriticalProperty.__init__)
+                check_type(argname="argument comparison_operator", value=comparison_operator, expected_type=type_hints["comparison_operator"])
+                check_type(argname="argument statistics", value=statistics, expected_type=type_hints["statistics"])
+                check_type(argname="argument threshold", value=threshold, expected_type=type_hints["threshold"])
+                check_type(argname="argument times", value=times, expected_type=type_hints["times"])
             self._values: typing.Dict[str, typing.Any] = {
                 "comparison_operator": comparison_operator,
                 "statistics": statistics,
                 "threshold": threshold,
                 "times": times,
             }
 
@@ -5444,23 +5997,28 @@
         jsii_struct_bases=[],
         name_mapping={"critical": "critical", "info": "info", "warn": "warn"},
     )
     class EscalationsProperty:
         def __init__(
             self,
             *,
-            critical: typing.Union[ros_cdk_core.IResolvable, "RosMetricRuleTemplate.CriticalProperty"],
-            info: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosMetricRuleTemplate.InfoProperty"]] = None,
-            warn: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosMetricRuleTemplate.WarnProperty"]] = None,
+            critical: typing.Union[ros_cdk_core.IResolvable, typing.Union["RosMetricRuleTemplate.CriticalProperty", typing.Dict[str, typing.Any]]],
+            info: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosMetricRuleTemplate.InfoProperty", typing.Dict[str, typing.Any]]]] = None,
+            warn: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosMetricRuleTemplate.WarnProperty", typing.Dict[str, typing.Any]]]] = None,
         ) -> None:
             '''
             :param critical: 
             :param info: 
             :param warn: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosMetricRuleTemplate.EscalationsProperty.__init__)
+                check_type(argname="argument critical", value=critical, expected_type=type_hints["critical"])
+                check_type(argname="argument info", value=info, expected_type=type_hints["info"])
+                check_type(argname="argument warn", value=warn, expected_type=type_hints["warn"])
             self._values: typing.Dict[str, typing.Any] = {
                 "critical": critical,
             }
             if info is not None:
                 self._values["info"] = info
             if warn is not None:
                 self._values["warn"] = warn
@@ -5528,14 +6086,20 @@
         ) -> None:
             '''
             :param comparison_operator: 
             :param statistics: 
             :param threshold: 
             :param times: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosMetricRuleTemplate.InfoProperty.__init__)
+                check_type(argname="argument comparison_operator", value=comparison_operator, expected_type=type_hints["comparison_operator"])
+                check_type(argname="argument statistics", value=statistics, expected_type=type_hints["statistics"])
+                check_type(argname="argument threshold", value=threshold, expected_type=type_hints["threshold"])
+                check_type(argname="argument times", value=times, expected_type=type_hints["times"])
             self._values: typing.Dict[str, typing.Any] = {
                 "comparison_operator": comparison_operator,
                 "statistics": statistics,
                 "threshold": threshold,
                 "times": times,
             }
 
@@ -5622,14 +6186,20 @@
         ) -> None:
             '''
             :param comparison_operator: 
             :param statistics: 
             :param threshold: 
             :param times: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosMetricRuleTemplate.WarnProperty.__init__)
+                check_type(argname="argument comparison_operator", value=comparison_operator, expected_type=type_hints["comparison_operator"])
+                check_type(argname="argument statistics", value=statistics, expected_type=type_hints["statistics"])
+                check_type(argname="argument threshold", value=threshold, expected_type=type_hints["threshold"])
+                check_type(argname="argument times", value=times, expected_type=type_hints["times"])
             self._values: typing.Dict[str, typing.Any] = {
                 "comparison_operator": comparison_operator,
                 "statistics": statistics,
                 "threshold": threshold,
                 "times": times,
             }
 
@@ -5708,27 +6278,34 @@
     },
 )
 class RosMetricRuleTemplateProps:
     def __init__(
         self,
         *,
         name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
-        alert_templates: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosMetricRuleTemplate.AlertTemplatesProperty]]]] = None,
+        alert_templates: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosMetricRuleTemplate.AlertTemplatesProperty, typing.Dict[str, typing.Any]]]]]] = None,
         description: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         rest_version: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         template_id: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::CMS::MetricRuleTemplate``.
 
         :param name: 
         :param alert_templates: 
         :param description: 
         :param rest_version: 
         :param template_id: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosMetricRuleTemplateProps.__init__)
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+            check_type(argname="argument alert_templates", value=alert_templates, expected_type=type_hints["alert_templates"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument rest_version", value=rest_version, expected_type=type_hints["rest_version"])
+            check_type(argname="argument template_id", value=template_id, expected_type=type_hints["template_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "name": name,
         }
         if alert_templates is not None:
             self._values["alert_templates"] = alert_templates
         if description is not None:
             self._values["description"] = description
@@ -5809,80 +6386,95 @@
 ):
     '''A ROS template type:  ``ALIYUN::CMS::MonitorGroup``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosMonitorGroupProps",
+        props: typing.Union["RosMonitorGroupProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::CMS::MonitorGroup``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosMonitorGroup.__init__)
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
+            type_hints = typing.get_type_hints(RosMonitorGroup._render_properties)
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
         :Attribute: GroupId: Application group ID generated after the group is created.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrGroupId"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosMonitorGroup, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="groupName")
     def group_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: groupName: The name of the application group.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "groupName"))
 
     @group_name.setter
     def group_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosMonitorGroup, "group_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "groupName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="contactGroups")
     def contact_groups(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -5892,108 +6484,129 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "contactGroups"))
 
     @contact_groups.setter
     def contact_groups(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosMonitorGroup, "contact_groups").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "contactGroups", value)
 
 
 class RosMonitorGroupInstances(
     ros_cdk_core.RosResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@alicloud/ros-cdk-cms.RosMonitorGroupInstances",
 ):
     '''A ROS template type:  ``ALIYUN::CMS::MonitorGroupInstances``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosMonitorGroupInstancesProps",
+        props: typing.Union["RosMonitorGroupInstancesProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::CMS::MonitorGroupInstances``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosMonitorGroupInstances.__init__)
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
+            type_hints = typing.get_type_hints(RosMonitorGroupInstances._render_properties)
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
         :Attribute: GroupId: The ID of the application group.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrGroupId"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosMonitorGroupInstances, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="groupId")
     def group_id(self) -> typing.Union[jsii.Number, ros_cdk_core.IResolvable]:
         '''
         :Property: groupId: The ID of the application group.
         '''
         return typing.cast(typing.Union[jsii.Number, ros_cdk_core.IResolvable], jsii.get(self, "groupId"))
 
     @group_id.setter
     def group_id(
         self,
         value: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosMonitorGroupInstances, "group_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "groupId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="instances")
     def instances(
         self,
     ) -> typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosMonitorGroupInstances.InstancesProperty"]]]:
         '''
         :Property: instances:
         '''
         return typing.cast(typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosMonitorGroupInstances.InstancesProperty"]]], jsii.get(self, "instances"))
 
     @instances.setter
     def instances(
         self,
         value: typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosMonitorGroupInstances.InstancesProperty"]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosMonitorGroupInstances, "instances").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "instances", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-cms.RosMonitorGroupInstances.InstancesProperty",
         jsii_struct_bases=[],
         name_mapping={
             "category": "category",
@@ -6013,14 +6626,20 @@
         ) -> None:
             '''
             :param category: 
             :param instance_id: 
             :param instance_name: 
             :param region_id: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosMonitorGroupInstances.InstancesProperty.__init__)
+                check_type(argname="argument category", value=category, expected_type=type_hints["category"])
+                check_type(argname="argument instance_id", value=instance_id, expected_type=type_hints["instance_id"])
+                check_type(argname="argument instance_name", value=instance_name, expected_type=type_hints["instance_name"])
+                check_type(argname="argument region_id", value=region_id, expected_type=type_hints["region_id"])
             self._values: typing.Dict[str, typing.Any] = {
                 "category": category,
                 "instance_id": instance_id,
                 "instance_name": instance_name,
                 "region_id": region_id,
             }
 
@@ -6115,21 +6734,25 @@
     name_mapping={"group_id": "groupId", "instances": "instances"},
 )
 class RosMonitorGroupInstancesProps:
     def __init__(
         self,
         *,
         group_id: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
-        instances: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosMonitorGroupInstances.InstancesProperty]]],
+        instances: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosMonitorGroupInstances.InstancesProperty, typing.Dict[str, typing.Any]]]]],
     ) -> None:
         '''Properties for defining a ``ALIYUN::CMS::MonitorGroupInstances``.
 
         :param group_id: 
         :param instances: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosMonitorGroupInstancesProps.__init__)
+            check_type(argname="argument group_id", value=group_id, expected_type=type_hints["group_id"])
+            check_type(argname="argument instances", value=instances, expected_type=type_hints["instances"])
         self._values: typing.Dict[str, typing.Any] = {
             "group_id": group_id,
             "instances": instances,
         }
 
     @builtins.property
     def group_id(self) -> typing.Union[jsii.Number, ros_cdk_core.IResolvable]:
@@ -6176,14 +6799,18 @@
         contact_groups: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::CMS::MonitorGroup``.
 
         :param group_name: 
         :param contact_groups: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosMonitorGroupProps.__init__)
+            check_type(argname="argument group_name", value=group_name, expected_type=type_hints["group_name"])
+            check_type(argname="argument contact_groups", value=contact_groups, expected_type=type_hints["contact_groups"])
         self._values: typing.Dict[str, typing.Any] = {
             "group_name": group_name,
         }
         if contact_groups is not None:
             self._values["contact_groups"] = contact_groups
 
     @builtins.property
@@ -6227,111 +6854,132 @@
 ):
     '''A ROS template type:  ``ALIYUN::CMS::MonitoringAgentProcess``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosMonitoringAgentProcessProps",
+        props: typing.Union["RosMonitoringAgentProcessProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::CMS::MonitoringAgentProcess``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosMonitoringAgentProcess.__init__)
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
+            type_hints = typing.get_type_hints(RosMonitoringAgentProcess._render_properties)
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
     @jsii.member(jsii_name="attrId")
     def attr_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Id: The process ID.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrId"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosMonitoringAgentProcess, "enable_resource_property_constraint").fset)
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
+            type_hints = typing.get_type_hints(getattr(RosMonitoringAgentProcess, "instance_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "instanceId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="processName")
     def process_name(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: processName: The name of the process.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "processName"))
 
     @process_name.setter
     def process_name(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosMonitoringAgentProcess, "process_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "processName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="processUser")
     def process_user(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: processUser: The user who launched the process.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "processUser"))
 
     @process_user.setter
     def process_user(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosMonitoringAgentProcess, "process_user").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "processUser", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-cms.RosMonitoringAgentProcessProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -6350,14 +6998,19 @@
     ) -> None:
         '''Properties for defining a ``ALIYUN::CMS::MonitoringAgentProcess``.
 
         :param instance_id: 
         :param process_name: 
         :param process_user: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosMonitoringAgentProcessProps.__init__)
+            check_type(argname="argument instance_id", value=instance_id, expected_type=type_hints["instance_id"])
+            check_type(argname="argument process_name", value=process_name, expected_type=type_hints["process_name"])
+            check_type(argname="argument process_user", value=process_user, expected_type=type_hints["process_user"])
         self._values: typing.Dict[str, typing.Any] = {
             "instance_id": instance_id,
         }
         if process_name is not None:
             self._values["process_name"] = process_name
         if process_user is not None:
             self._values["process_user"] = process_user
@@ -6410,64 +7063,73 @@
 ):
     '''A ROS template type:  ``ALIYUN::CMS::ResourceMetricRule``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosResourceMetricRuleProps",
+        props: typing.Union["RosResourceMetricRuleProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::CMS::ResourceMetricRule``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosResourceMetricRule.__init__)
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
+            type_hints = typing.get_type_hints(RosResourceMetricRule._render_properties)
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
     @jsii.member(jsii_name="attrRuleId")
     def attr_rule_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: RuleId: The ID of the alert rule.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrRuleId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrRuleName")
     def attr_rule_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: RuleName: The name of the alert rule.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrRuleName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="contactGroups")
     def contact_groups(
         self,
     ) -> typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]:
         '''
         :Property:
 
@@ -6478,43 +7140,52 @@
         return typing.cast(typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]], jsii.get(self, "contactGroups"))
 
     @contact_groups.setter
     def contact_groups(
         self,
         value: typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosResourceMetricRule, "contact_groups").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "contactGroups", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosResourceMetricRule, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="escalations")
     def escalations(
         self,
     ) -> typing.Union[ros_cdk_core.IResolvable, "RosResourceMetricRule.EscalationsProperty"]:
         '''
         :Property: escalations: You must select at least one of the Critical, Warn, and Info alert levels.
         '''
         return typing.cast(typing.Union[ros_cdk_core.IResolvable, "RosResourceMetricRule.EscalationsProperty"], jsii.get(self, "escalations"))
 
     @escalations.setter
     def escalations(
         self,
         value: typing.Union[ros_cdk_core.IResolvable, "RosResourceMetricRule.EscalationsProperty"],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosResourceMetricRule, "escalations").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "escalations", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="metricName")
     def metric_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         metricName: The name of the metric.
         For information about how to query the name of a metric, see Appendix 1: Metrics.
@@ -6523,17 +7194,20 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "metricName"))
 
     @metric_name.setter
     def metric_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosResourceMetricRule, "metric_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "metricName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="namespace")
     def namespace(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         namespace: The namespace of the cloud service.
         For information about how to query the namespace of a cloud service, Appendix 1: Metrics.
@@ -6542,17 +7216,20 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "namespace"))
 
     @namespace.setter
     def namespace(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosResourceMetricRule, "namespace").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "namespace", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="resources")
     def resources(
         self,
     ) -> typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Mapping[builtins.str, typing.Any]]]:
         '''
         :Property:
 
@@ -6563,17 +7240,20 @@
         return typing.cast(typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Mapping[builtins.str, typing.Any]]], jsii.get(self, "resources"))
 
     @resources.setter
     def resources(
         self,
         value: typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Mapping[builtins.str, typing.Any]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosResourceMetricRule, "resources").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "resources", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="compositeExpression")
     def composite_expression(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosResourceMetricRule.CompositeExpressionProperty"]]:
         '''
         :Property:
 
@@ -6583,68 +7263,80 @@
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosResourceMetricRule.CompositeExpressionProperty"]], jsii.get(self, "compositeExpression"))
 
     @composite_expression.setter
     def composite_expression(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosResourceMetricRule.CompositeExpressionProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosResourceMetricRule, "composite_expression").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "compositeExpression", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="deletionForce")
     def deletion_force(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property: deletionForce: Whether to delete rule even if it is not created by ROS. Default is false
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "deletionForce"))
 
     @deletion_force.setter
     def deletion_force(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosResourceMetricRule, "deletion_force").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "deletionForce", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="effectiveInterval")
     def effective_interval(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: effectiveInterval: The time period during which the alert rule is effective.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "effectiveInterval"))
 
     @effective_interval.setter
     def effective_interval(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosResourceMetricRule, "effective_interval").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "effectiveInterval", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="emailSubject")
     def email_subject(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: emailSubject: The subject of the alert notification email.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "emailSubject"))
 
     @email_subject.setter
     def email_subject(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosResourceMetricRule, "email_subject").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "emailSubject", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="interval")
     def interval(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -6654,34 +7346,40 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "interval"))
 
     @interval.setter
     def interval(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosResourceMetricRule, "interval").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "interval", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="labels")
     def labels(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosResourceMetricRule.LabelsProperty"]]]]:
         '''
         :Property: labels:
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosResourceMetricRule.LabelsProperty"]]]], jsii.get(self, "labels"))
 
     @labels.setter
     def labels(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosResourceMetricRule.LabelsProperty"]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosResourceMetricRule, "labels").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "labels", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="noDataPolicy")
     def no_data_policy(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -6694,34 +7392,40 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "noDataPolicy"))
 
     @no_data_policy.setter
     def no_data_policy(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosResourceMetricRule, "no_data_policy").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "noDataPolicy", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="noEffectiveInterval")
     def no_effective_interval(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: noEffectiveInterval: The time period during which the alert rule is ineffective.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "noEffectiveInterval"))
 
     @no_effective_interval.setter
     def no_effective_interval(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosResourceMetricRule, "no_effective_interval").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "noEffectiveInterval", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="period")
     def period(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -6731,17 +7435,20 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "period"))
 
     @period.setter
     def period(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosResourceMetricRule, "period").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "period", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="prometheus")
     def prometheus(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosResourceMetricRule.PrometheusProperty"]]:
         '''
         :Property:
 
@@ -6751,17 +7458,20 @@
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosResourceMetricRule.PrometheusProperty"]], jsii.get(self, "prometheus"))
 
     @prometheus.setter
     def prometheus(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosResourceMetricRule.PrometheusProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosResourceMetricRule, "prometheus").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "prometheus", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="ruleId")
     def rule_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -6772,17 +7482,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "ruleId"))
 
     @rule_id.setter
     def rule_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosResourceMetricRule, "rule_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "ruleId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="ruleName")
     def rule_name(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -6793,17 +7506,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "ruleName"))
 
     @rule_name.setter
     def rule_name(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosResourceMetricRule, "rule_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "ruleName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="silenceTime")
     def silence_time(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -6813,31 +7529,37 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "silenceTime"))
 
     @silence_time.setter
     def silence_time(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosResourceMetricRule, "silence_time").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "silenceTime", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="webhook")
     def webhook(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: webhook: The callback URL to which a POST request is sent when an alert is triggered based on the alert rule.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "webhook"))
 
     @webhook.setter
     def webhook(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosResourceMetricRule, "webhook").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "webhook", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-cms.RosResourceMetricRule.AnnotationsProperty",
         jsii_struct_bases=[],
         name_mapping={"key": "key", "value": "value"},
     )
@@ -6848,14 +7570,18 @@
             key: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
             value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param key: 
             :param value: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosResourceMetricRule.AnnotationsProperty.__init__)
+                check_type(argname="argument key", value=key, expected_type=type_hints["key"])
+                check_type(argname="argument value", value=value, expected_type=type_hints["value"])
             self._values: typing.Dict[str, typing.Any] = {}
             if key is not None:
                 self._values["key"] = key
             if value is not None:
                 self._values["value"] = value
 
         @builtins.property
@@ -6902,25 +7628,32 @@
     )
     class CompositeExpressionProperty:
         def __init__(
             self,
             *,
             level: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             times: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
-            expression_list: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosResourceMetricRule.ExpressionListProperty"]]]] = None,
+            expression_list: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosResourceMetricRule.ExpressionListProperty", typing.Dict[str, typing.Any]]]]]] = None,
             expression_list_join: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
             expression_raw: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param level: 
             :param times: 
             :param expression_list: 
             :param expression_list_join: 
             :param expression_raw: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosResourceMetricRule.CompositeExpressionProperty.__init__)
+                check_type(argname="argument level", value=level, expected_type=type_hints["level"])
+                check_type(argname="argument times", value=times, expected_type=type_hints["times"])
+                check_type(argname="argument expression_list", value=expression_list, expected_type=type_hints["expression_list"])
+                check_type(argname="argument expression_list_join", value=expression_list_join, expected_type=type_hints["expression_list_join"])
+                check_type(argname="argument expression_raw", value=expression_raw, expected_type=type_hints["expression_raw"])
             self._values: typing.Dict[str, typing.Any] = {
                 "level": level,
                 "times": times,
             }
             if expression_list is not None:
                 self._values["expression_list"] = expression_list
             if expression_list_join is not None:
@@ -7025,14 +7758,20 @@
         ) -> None:
             '''
             :param comparison_operator: 
             :param statistics: 
             :param threshold: 
             :param times: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosResourceMetricRule.CriticalProperty.__init__)
+                check_type(argname="argument comparison_operator", value=comparison_operator, expected_type=type_hints["comparison_operator"])
+                check_type(argname="argument statistics", value=statistics, expected_type=type_hints["statistics"])
+                check_type(argname="argument threshold", value=threshold, expected_type=type_hints["threshold"])
+                check_type(argname="argument times", value=times, expected_type=type_hints["times"])
             self._values: typing.Dict[str, typing.Any] = {
                 "comparison_operator": comparison_operator,
                 "statistics": statistics,
                 "threshold": threshold,
                 "times": times,
             }
 
@@ -7111,23 +7850,28 @@
         jsii_struct_bases=[],
         name_mapping={"critical": "critical", "info": "info", "warn": "warn"},
     )
     class EscalationsProperty:
         def __init__(
             self,
             *,
-            critical: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosResourceMetricRule.CriticalProperty"]] = None,
-            info: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosResourceMetricRule.InfoProperty"]] = None,
-            warn: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosResourceMetricRule.WarnProperty"]] = None,
+            critical: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosResourceMetricRule.CriticalProperty", typing.Dict[str, typing.Any]]]] = None,
+            info: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosResourceMetricRule.InfoProperty", typing.Dict[str, typing.Any]]]] = None,
+            warn: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosResourceMetricRule.WarnProperty", typing.Dict[str, typing.Any]]]] = None,
         ) -> None:
             '''
             :param critical: 
             :param info: 
             :param warn: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosResourceMetricRule.EscalationsProperty.__init__)
+                check_type(argname="argument critical", value=critical, expected_type=type_hints["critical"])
+                check_type(argname="argument info", value=info, expected_type=type_hints["info"])
+                check_type(argname="argument warn", value=warn, expected_type=type_hints["warn"])
             self._values: typing.Dict[str, typing.Any] = {}
             if critical is not None:
                 self._values["critical"] = critical
             if info is not None:
                 self._values["info"] = info
             if warn is not None:
                 self._values["warn"] = warn
@@ -7197,14 +7941,21 @@
             '''
             :param comparison_operator: 
             :param metric_name: 
             :param period: 
             :param statistics: 
             :param threshold: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosResourceMetricRule.ExpressionListProperty.__init__)
+                check_type(argname="argument comparison_operator", value=comparison_operator, expected_type=type_hints["comparison_operator"])
+                check_type(argname="argument metric_name", value=metric_name, expected_type=type_hints["metric_name"])
+                check_type(argname="argument period", value=period, expected_type=type_hints["period"])
+                check_type(argname="argument statistics", value=statistics, expected_type=type_hints["statistics"])
+                check_type(argname="argument threshold", value=threshold, expected_type=type_hints["threshold"])
             self._values: typing.Dict[str, typing.Any] = {
                 "comparison_operator": comparison_operator,
                 "metric_name": metric_name,
                 "period": period,
                 "statistics": statistics,
                 "threshold": threshold,
             }
@@ -7312,14 +8063,20 @@
         ) -> None:
             '''
             :param comparison_operator: 
             :param statistics: 
             :param threshold: 
             :param times: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosResourceMetricRule.InfoProperty.__init__)
+                check_type(argname="argument comparison_operator", value=comparison_operator, expected_type=type_hints["comparison_operator"])
+                check_type(argname="argument statistics", value=statistics, expected_type=type_hints["statistics"])
+                check_type(argname="argument threshold", value=threshold, expected_type=type_hints["threshold"])
+                check_type(argname="argument times", value=times, expected_type=type_hints["times"])
             self._values: typing.Dict[str, typing.Any] = {
                 "comparison_operator": comparison_operator,
                 "statistics": statistics,
                 "threshold": threshold,
                 "times": times,
             }
 
@@ -7405,14 +8162,18 @@
             key: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param key: 
             :param value: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosResourceMetricRule.LabelsProperty.__init__)
+                check_type(argname="argument key", value=key, expected_type=type_hints["key"])
+                check_type(argname="argument value", value=value, expected_type=type_hints["value"])
             self._values: typing.Dict[str, typing.Any] = {
                 "key": key,
             }
             if value is not None:
                 self._values["value"] = value
 
         @builtins.property
@@ -7461,22 +8222,28 @@
     class PrometheusProperty:
         def __init__(
             self,
             *,
             level: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             prom_ql: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             times: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
-            annotations: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosResourceMetricRule.AnnotationsProperty"]]]] = None,
+            annotations: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosResourceMetricRule.AnnotationsProperty", typing.Dict[str, typing.Any]]]]]] = None,
         ) -> None:
             '''
             :param level: 
             :param prom_ql: 
             :param times: 
             :param annotations: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosResourceMetricRule.PrometheusProperty.__init__)
+                check_type(argname="argument level", value=level, expected_type=type_hints["level"])
+                check_type(argname="argument prom_ql", value=prom_ql, expected_type=type_hints["prom_ql"])
+                check_type(argname="argument times", value=times, expected_type=type_hints["times"])
+                check_type(argname="argument annotations", value=annotations, expected_type=type_hints["annotations"])
             self._values: typing.Dict[str, typing.Any] = {
                 "level": level,
                 "prom_ql": prom_ql,
                 "times": times,
             }
             if annotations is not None:
                 self._values["annotations"] = annotations
@@ -7562,14 +8329,20 @@
         ) -> None:
             '''
             :param comparison_operator: 
             :param statistics: 
             :param threshold: 
             :param times: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosResourceMetricRule.WarnProperty.__init__)
+                check_type(argname="argument comparison_operator", value=comparison_operator, expected_type=type_hints["comparison_operator"])
+                check_type(argname="argument statistics", value=statistics, expected_type=type_hints["statistics"])
+                check_type(argname="argument threshold", value=threshold, expected_type=type_hints["threshold"])
+                check_type(argname="argument times", value=times, expected_type=type_hints["times"])
             self._values: typing.Dict[str, typing.Any] = {
                 "comparison_operator": comparison_operator,
                 "statistics": statistics,
                 "threshold": threshold,
                 "times": times,
             }
 
@@ -7670,28 +8443,28 @@
     },
 )
 class RosResourceMetricRuleProps:
     def __init__(
         self,
         *,
         contact_groups: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]],
-        escalations: typing.Union[ros_cdk_core.IResolvable, RosResourceMetricRule.EscalationsProperty],
+        escalations: typing.Union[ros_cdk_core.IResolvable, typing.Union[RosResourceMetricRule.EscalationsProperty, typing.Dict[str, typing.Any]]],
         metric_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         namespace: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         resources: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Mapping[builtins.str, typing.Any]]],
-        composite_expression: typing.Optional[typing.Union[ros_cdk_core.IResolvable, RosResourceMetricRule.CompositeExpressionProperty]] = None,
+        composite_expression: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosResourceMetricRule.CompositeExpressionProperty, typing.Dict[str, typing.Any]]]] = None,
         deletion_force: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         effective_interval: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         email_subject: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         interval: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
-        labels: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosResourceMetricRule.LabelsProperty]]]] = None,
+        labels: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosResourceMetricRule.LabelsProperty, typing.Dict[str, typing.Any]]]]]] = None,
         no_data_policy: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         no_effective_interval: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         period: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
-        prometheus: typing.Optional[typing.Union[ros_cdk_core.IResolvable, RosResourceMetricRule.PrometheusProperty]] = None,
+        prometheus: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosResourceMetricRule.PrometheusProperty, typing.Dict[str, typing.Any]]]] = None,
         rule_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         rule_name: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         silence_time: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         webhook: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::CMS::ResourceMetricRule``.
 
@@ -7711,14 +8484,35 @@
         :param period: 
         :param prometheus: 
         :param rule_id: 
         :param rule_name: 
         :param silence_time: 
         :param webhook: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosResourceMetricRuleProps.__init__)
+            check_type(argname="argument contact_groups", value=contact_groups, expected_type=type_hints["contact_groups"])
+            check_type(argname="argument escalations", value=escalations, expected_type=type_hints["escalations"])
+            check_type(argname="argument metric_name", value=metric_name, expected_type=type_hints["metric_name"])
+            check_type(argname="argument namespace", value=namespace, expected_type=type_hints["namespace"])
+            check_type(argname="argument resources", value=resources, expected_type=type_hints["resources"])
+            check_type(argname="argument composite_expression", value=composite_expression, expected_type=type_hints["composite_expression"])
+            check_type(argname="argument deletion_force", value=deletion_force, expected_type=type_hints["deletion_force"])
+            check_type(argname="argument effective_interval", value=effective_interval, expected_type=type_hints["effective_interval"])
+            check_type(argname="argument email_subject", value=email_subject, expected_type=type_hints["email_subject"])
+            check_type(argname="argument interval", value=interval, expected_type=type_hints["interval"])
+            check_type(argname="argument labels", value=labels, expected_type=type_hints["labels"])
+            check_type(argname="argument no_data_policy", value=no_data_policy, expected_type=type_hints["no_data_policy"])
+            check_type(argname="argument no_effective_interval", value=no_effective_interval, expected_type=type_hints["no_effective_interval"])
+            check_type(argname="argument period", value=period, expected_type=type_hints["period"])
+            check_type(argname="argument prometheus", value=prometheus, expected_type=type_hints["prometheus"])
+            check_type(argname="argument rule_id", value=rule_id, expected_type=type_hints["rule_id"])
+            check_type(argname="argument rule_name", value=rule_name, expected_type=type_hints["rule_name"])
+            check_type(argname="argument silence_time", value=silence_time, expected_type=type_hints["silence_time"])
+            check_type(argname="argument webhook", value=webhook, expected_type=type_hints["webhook"])
         self._values: typing.Dict[str, typing.Any] = {
             "contact_groups": contact_groups,
             "escalations": escalations,
             "metric_name": metric_name,
             "namespace": namespace,
             "resources": resources,
         }
@@ -8006,80 +8800,95 @@
 ):
     '''A ROS template type:  ``ALIYUN::CMS::SiteMonitor``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosSiteMonitorProps",
+        props: typing.Union["RosSiteMonitorProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::CMS::SiteMonitor``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosSiteMonitor.__init__)
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
+            type_hints = typing.get_type_hints(RosSiteMonitor._render_properties)
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
     @jsii.member(jsii_name="attrTaskId")
     def attr_task_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: TaskId: The ID of the site monitoring task.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTaskId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="address")
     def address(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: address: The URL or IP address monitored by the monitoring task.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "address"))
 
     @address.setter
     def address(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSiteMonitor, "address").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "address", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSiteMonitor, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="taskName")
     def task_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         taskName: The name of the site monitoring task. The name must be 4 to 100 characters in length.
         It can contain letters, digits, and underscores (_).
@@ -8087,17 +8896,20 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "taskName"))
 
     @task_name.setter
     def task_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSiteMonitor, "task_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "taskName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="taskType")
     def task_type(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         taskType: The protocol used by the site monitoring task. Valid values: HTTP, HTTPS, PING, TCP,
         UDP, DNS, SMTP, POP3, and FTP.
@@ -8105,34 +8917,40 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "taskType"))
 
     @task_type.setter
     def task_type(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSiteMonitor, "task_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "taskType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="alertIds")
     def alert_ids(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]]:
         '''
         :Property: alertIds:
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]], jsii.get(self, "alertIds"))
 
     @alert_ids.setter
     def alert_ids(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSiteMonitor, "alert_ids").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "alertIds", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="interval")
     def interval(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -8142,17 +8960,20 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "interval"))
 
     @interval.setter
     def interval(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSiteMonitor, "interval").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "interval", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="ispCities")
     def isp_cities(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosSiteMonitor.IspCitiesProperty"]]]]:
         '''
         :Property:
 
@@ -8166,17 +8987,20 @@
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosSiteMonitor.IspCitiesProperty"]]]], jsii.get(self, "ispCities"))
 
     @isp_cities.setter
     def isp_cities(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosSiteMonitor.IspCitiesProperty"]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSiteMonitor, "isp_cities").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "ispCities", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="optionsJson")
     def options_json(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -8186,14 +9010,17 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "optionsJson"))
 
     @options_json.setter
     def options_json(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosSiteMonitor, "options_json").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "optionsJson", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-cms.RosSiteMonitor.IspCitiesProperty",
         jsii_struct_bases=[],
         name_mapping={"city": "city", "isp": "isp"},
     )
@@ -8204,14 +9031,18 @@
             city: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             isp: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         ) -> None:
             '''
             :param city: 
             :param isp: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosSiteMonitor.IspCitiesProperty.__init__)
+                check_type(argname="argument city", value=city, expected_type=type_hints["city"])
+                check_type(argname="argument isp", value=isp, expected_type=type_hints["isp"])
             self._values: typing.Dict[str, typing.Any] = {
                 "city": city,
                 "isp": isp,
             }
 
         @builtins.property
         def city(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
@@ -8261,27 +9092,36 @@
         self,
         *,
         address: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         task_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         task_type: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         alert_ids: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]] = None,
         interval: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
-        isp_cities: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosSiteMonitor.IspCitiesProperty]]]] = None,
+        isp_cities: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosSiteMonitor.IspCitiesProperty, typing.Dict[str, typing.Any]]]]]] = None,
         options_json: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::CMS::SiteMonitor``.
 
         :param address: 
         :param task_name: 
         :param task_type: 
         :param alert_ids: 
         :param interval: 
         :param isp_cities: 
         :param options_json: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosSiteMonitorProps.__init__)
+            check_type(argname="argument address", value=address, expected_type=type_hints["address"])
+            check_type(argname="argument task_name", value=task_name, expected_type=type_hints["task_name"])
+            check_type(argname="argument task_type", value=task_type, expected_type=type_hints["task_type"])
+            check_type(argname="argument alert_ids", value=alert_ids, expected_type=type_hints["alert_ids"])
+            check_type(argname="argument interval", value=interval, expected_type=type_hints["interval"])
+            check_type(argname="argument isp_cities", value=isp_cities, expected_type=type_hints["isp_cities"])
+            check_type(argname="argument options_json", value=options_json, expected_type=type_hints["options_json"])
         self._values: typing.Dict[str, typing.Any] = {
             "address": address,
             "task_name": task_name,
             "task_type": task_type,
         }
         if alert_ids is not None:
             self._values["alert_ids"] = alert_ids
@@ -8397,31 +9237,37 @@
 ):
     '''A ROS resource type:  ``ALIYUN::CMS::SiteMonitor``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "SiteMonitorProps",
+        props: typing.Union["SiteMonitorProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::CMS::SiteMonitor``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(SiteMonitor.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTaskId")
     def attr_task_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute TaskId: The ID of the site monitoring task.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTaskId"))
 
 
 @jsii.data_type(
@@ -8442,27 +9288,36 @@
         self,
         *,
         address: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         task_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         task_type: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         alert_ids: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]] = None,
         interval: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
-        isp_cities: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosSiteMonitor.IspCitiesProperty]]]] = None,
+        isp_cities: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosSiteMonitor.IspCitiesProperty, typing.Dict[str, typing.Any]]]]]] = None,
         options_json: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::CMS::SiteMonitor``.
 
         :param address: Property address: The URL or IP address monitored by the monitoring task.
         :param task_name: Property taskName: The name of the site monitoring task. The name must be 4 to 100 characters in length. It can contain letters, digits, and underscores (_).
         :param task_type: Property taskType: The protocol used by the site monitoring task. Valid values: HTTP, HTTPS, PING, TCP, UDP, DNS, SMTP, POP3, and FTP.
         :param alert_ids: Property alertIds:.
         :param interval: Property interval: The interval at which detection requests are sent. Valid values: 1, 5, and 15. Unit: minutes. Default value: 1.
         :param isp_cities: Property ispCities: The information about detection points, which is specified in a JSON array. Example: [{"city":"546","isp":"465"},{"city":"572","isp":"465"},{"city":"738","isp":"465"}]. The three city codes represent Beijing, Hangzhou, and Qingdao. Note You can call the DescribeSiteMonitorISPCityList API operation to query the detection points that can be used to create site monitoring tasks. For more information, see DescribeSiteMonitorISPCityList . If this parameter is not specified, the system randomly selects three detection points for site monitoring.
         :param options_json: Property optionsJson: The extended options of the protocol that is used by the site monitoring task. The options vary based on the protocol.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(SiteMonitorProps.__init__)
+            check_type(argname="argument address", value=address, expected_type=type_hints["address"])
+            check_type(argname="argument task_name", value=task_name, expected_type=type_hints["task_name"])
+            check_type(argname="argument task_type", value=task_type, expected_type=type_hints["task_type"])
+            check_type(argname="argument alert_ids", value=alert_ids, expected_type=type_hints["alert_ids"])
+            check_type(argname="argument interval", value=interval, expected_type=type_hints["interval"])
+            check_type(argname="argument isp_cities", value=isp_cities, expected_type=type_hints["isp_cities"])
+            check_type(argname="argument options_json", value=options_json, expected_type=type_hints["options_json"])
         self._values: typing.Dict[str, typing.Any] = {
             "address": address,
             "task_name": task_name,
             "task_type": task_type,
         }
         if alert_ids is not None:
             self._values["alert_ids"] = alert_ids
```

### Comparing `ros-cdk-cms-1.0.8/src/ros_cdk_cms.egg-info/PKG-INFO` & `ros-cdk-cms-1.0.9/src/ros_cdk_cms.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-cms
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS CMS Construct Library
```

