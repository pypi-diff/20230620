# Comparing `tmp/ros-cdk-cdn-1.0.8.tar.gz` & `tmp/ros-cdk-cdn-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-cdn-1.0.8.tar", last modified: Thu Jul 14 02:25:06 2022, max compression
+gzip compressed data, was "dist/ros-cdk-cdn-1.0.9.tar", last modified: Fri Sep 23 12:11:36 2022, max compression
```

## Comparing `ros-cdk-cdn-1.0.8.tar` & `ros-cdk-cdn-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:25:06.000000 ros-cdk-cdn-1.0.8/
--rw-r--r--   0 root         (0) root         (0)    10279 2022-07-14 02:25:06.000000 ros-cdk-cdn-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2022-07-14 02:25:06.000000 ros-cdk-cdn-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2022-07-14 02:25:06.000000 ros-cdk-cdn-1.0.8/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1240 2022-07-14 02:25:06.000000 ros-cdk-cdn-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      179 2022-07-14 02:25:06.000000 ros-cdk-cdn-1.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)      106 2022-07-14 02:25:06.000000 ros-cdk-cdn-1.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-07-14 02:25:06.000000 ros-cdk-cdn-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1794 2022-07-14 02:25:06.000000 ros-cdk-cdn-1.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:25:06.000000 ros-cdk-cdn-1.0.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:25:06.000000 ros-cdk-cdn-1.0.8/src/ros_cdk_cdn/
--rw-r--r--   0 root         (0) root         (0)    34410 2022-07-14 02:25:06.000000 ros-cdk-cdn-1.0.8/src/ros_cdk_cdn/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:25:06.000000 ros-cdk-cdn-1.0.8/src/ros_cdk_cdn/_jsii/
--rw-r--r--   0 root         (0) root         (0)      370 2022-07-14 02:25:06.000000 ros-cdk-cdn-1.0.8/src/ros_cdk_cdn/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    37392 2022-07-14 02:25:06.000000 ros-cdk-cdn-1.0.8/src/ros_cdk_cdn/_jsii/ros-cdk-cdn@1.0.8.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:25:06.000000 ros-cdk-cdn-1.0.8/src/ros_cdk_cdn/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:25:06.000000 ros-cdk-cdn-1.0.8/src/ros_cdk_cdn.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1240 2022-07-14 02:25:06.000000 ros-cdk-cdn-1.0.8/src/ros_cdk_cdn.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      400 2022-07-14 02:25:06.000000 ros-cdk-cdn-1.0.8/src/ros_cdk_cdn.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:25:06.000000 ros-cdk-cdn-1.0.8/src/ros_cdk_cdn.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2022-07-14 02:25:06.000000 ros-cdk-cdn-1.0.8/src/ros_cdk_cdn.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2022-07-14 02:25:06.000000 ros-cdk-cdn-1.0.8/src/ros_cdk_cdn.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:11:36.000000 ros-cdk-cdn-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)    10279 2022-09-23 12:11:36.000000 ros-cdk-cdn-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-09-23 12:11:36.000000 ros-cdk-cdn-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2022-09-23 12:11:36.000000 ros-cdk-cdn-1.0.9/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1240 2022-09-23 12:11:36.000000 ros-cdk-cdn-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      179 2022-09-23 12:11:36.000000 ros-cdk-cdn-1.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      236 2022-09-23 12:11:36.000000 ros-cdk-cdn-1.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-09-23 12:11:36.000000 ros-cdk-cdn-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1823 2022-09-23 12:11:36.000000 ros-cdk-cdn-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:11:36.000000 ros-cdk-cdn-1.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:11:36.000000 ros-cdk-cdn-1.0.9/src/ros_cdk_cdn/
+-rw-r--r--   0 root         (0) root         (0)    42366 2022-09-23 12:11:36.000000 ros-cdk-cdn-1.0.9/src/ros_cdk_cdn/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:11:36.000000 ros-cdk-cdn-1.0.9/src/ros_cdk_cdn/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      404 2022-09-23 12:11:36.000000 ros-cdk-cdn-1.0.9/src/ros_cdk_cdn/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    37457 2022-09-23 12:11:36.000000 ros-cdk-cdn-1.0.9/src/ros_cdk_cdn/_jsii/ros-cdk-cdn@1.0.9.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 12:11:36.000000 ros-cdk-cdn-1.0.9/src/ros_cdk_cdn/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:11:36.000000 ros-cdk-cdn-1.0.9/src/ros_cdk_cdn.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1240 2022-09-23 12:11:36.000000 ros-cdk-cdn-1.0.9/src/ros_cdk_cdn.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      400 2022-09-23 12:11:36.000000 ros-cdk-cdn-1.0.9/src/ros_cdk_cdn.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 12:11:36.000000 ros-cdk-cdn-1.0.9/src/ros_cdk_cdn.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2022-09-23 12:11:36.000000 ros-cdk-cdn-1.0.9/src/ros_cdk_cdn.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2022-09-23 12:11:36.000000 ros-cdk-cdn-1.0.9/src/ros_cdk_cdn.egg-info/top_level.txt
```

### Comparing `ros-cdk-cdn-1.0.8/LICENSE` & `ros-cdk-cdn-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-cdn-1.0.8/PKG-INFO` & `ros-cdk-cdn-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-cdn
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS CDN Construct Library
```

### Comparing `ros-cdk-cdn-1.0.8/setup.py` & `ros-cdk-cdn-1.0.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-cdn",
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
         "ros_cdk_cdn",
         "ros_cdk_cdn._jsii"
     ],
     "package_data": {
         "ros_cdk_cdn._jsii": [
-            "ros-cdk-cdn@1.0.8.jsii.tgz"
+            "ros-cdk-cdn@1.0.9.jsii.tgz"
         ],
         "ros_cdk_cdn": [
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

### Comparing `ros-cdk-cdn-1.0.8/src/ros_cdk_cdn/__init__.py` & `ros-cdk-cdn-1.0.9/src/ros_cdk_cdn/__init__.py`

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
 
 
 class Domain(
     ros_cdk_core.Resource,
@@ -29,37 +31,43 @@
 ):
     '''A ROS resource type:  ``ALIYUN::CDN::Domain``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "DomainProps",
+        props: typing.Union["DomainProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::CDN::Domain``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(Domain.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrCname")
     def attr_cname(self) -> ros_cdk_core.IResolvable:
         '''Attribute Cname: The CNAME generated for the CDN domain.You must add a CNAME record with your DNS provider to map the CDN domain name to the CNAME.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrCname"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDomainName")
     def attr_domain_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute DomainName: The CDN domain name.
 
         Wildcard domain names that start with periods (.) are supported. For example, .a.com.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDomainName"))
@@ -72,28 +80,34 @@
 ):
     '''A ROS resource type:  ``ALIYUN::CDN::DomainConfig``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "DomainConfigProps",
+        props: typing.Union["DomainConfigProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::CDN::DomainConfig``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(DomainConfig.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-cdn.DomainConfigProps",
     jsii_struct_bases=[],
     name_mapping={"domain_names": "domainNames", "functions": "functions"},
@@ -106,14 +120,18 @@
         functions: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
         '''Properties for defining a ``ALIYUN::CDN::DomainConfig``.
 
         :param domain_names: Property domainNames: Your accelerated domain name, separated by commas in English.
         :param functions: Property functions: function list, please refer to the CDN documentation for details.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(DomainConfigProps.__init__)
+            check_type(argname="argument domain_names", value=domain_names, expected_type=type_hints["domain_names"])
+            check_type(argname="argument functions", value=functions, expected_type=type_hints["functions"])
         self._values: typing.Dict[str, typing.Any] = {
             "domain_names": domain_names,
             "functions": functions,
         }
 
     @builtins.property
     def domain_names(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
@@ -161,28 +179,38 @@
         *,
         cdn_type: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         domain_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         check_url: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         resource_group_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         scope: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         sources: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        tags: typing.Optional[typing.Sequence["RosDomain.TagsProperty"]] = None,
+        tags: typing.Optional[typing.Sequence[typing.Union["RosDomain.TagsProperty", typing.Dict[str, typing.Any]]]] = None,
         top_level_domain: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::CDN::Domain``.
 
         :param cdn_type: Property cdnType: The business type. Valid values: web, download, video, livestream, and httpsdelivery. web: acceleration of images and small files download. download: acceleration of large file downloads. video: live streaming acceleration. httpsdelivery: SSL acceleration for HTTPS.
         :param domain_name: Property domainName: The CDN domain name. Wildcard domain names that start with periods (.) are supported. For example, .a.com.
         :param check_url: Property checkUrl: The validation of the origin.
         :param resource_group_id: Property resourceGroupId: The ID of the resource group. If this is left blank, the system automatically fills in the ID of the default resource group.
         :param scope: Property scope: Valid values: domestic, overseas, and global. Default value: domestic. The setting is supported for users outside mainland China, users in mainland China of level 3 or above.
         :param sources: Property sources: The list of origin URLs.
         :param tags: Property tags: Tags to attach to instance. Max support 20 tags to add during create instance. Each tag with two properties Key and Value, and Key is required.
         :param top_level_domain: Property topLevelDomain: The top-level domain, which can only be configured by users on the whitelist.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(DomainProps.__init__)
+            check_type(argname="argument cdn_type", value=cdn_type, expected_type=type_hints["cdn_type"])
+            check_type(argname="argument domain_name", value=domain_name, expected_type=type_hints["domain_name"])
+            check_type(argname="argument check_url", value=check_url, expected_type=type_hints["check_url"])
+            check_type(argname="argument resource_group_id", value=resource_group_id, expected_type=type_hints["resource_group_id"])
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument sources", value=sources, expected_type=type_hints["sources"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
+            check_type(argname="argument top_level_domain", value=top_level_domain, expected_type=type_hints["top_level_domain"])
         self._values: typing.Dict[str, typing.Any] = {
             "cdn_type": cdn_type,
             "domain_name": domain_name,
         }
         if check_url is not None:
             self._values["check_url"] = check_url
         if resource_group_id is not None:
@@ -290,200 +318,236 @@
 ):
     '''A ROS template type:  ``ALIYUN::CDN::Domain``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosDomainProps",
+        props: typing.Union["RosDomainProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::CDN::Domain``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosDomain.__init__)
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
+            type_hints = typing.get_type_hints(RosDomain._render_properties)
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
     @jsii.member(jsii_name="attrCname")
     def attr_cname(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Cname: The CNAME generated for the CDN domain.You must add a CNAME record with your DNS provider to map the CDN domain name to the CNAME.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrCname"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDomainName")
     def attr_domain_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: DomainName: The CDN domain name. Wildcard domain names that start with periods (.) are supported. For example, .a.com.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDomainName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="cdnType")
     def cdn_type(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: cdnType: The business type. Valid values: web, download, video, livestream, and httpsdelivery. web: acceleration of images and small files download. download: acceleration of large file downloads. video: live streaming acceleration. httpsdelivery: SSL acceleration for HTTPS.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "cdnType"))
 
     @cdn_type.setter
     def cdn_type(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDomain, "cdn_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "cdnType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="domainName")
     def domain_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: domainName: The CDN domain name. Wildcard domain names that start with periods (.) are supported. For example, .a.com.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "domainName"))
 
     @domain_name.setter
     def domain_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDomain, "domain_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "domainName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDomain, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="checkUrl")
     def check_url(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: checkUrl: The validation of the origin.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "checkUrl"))
 
     @check_url.setter
     def check_url(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDomain, "check_url").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "checkUrl", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="resourceGroupId")
     def resource_group_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: resourceGroupId: The ID of the resource group. If this is left blank, the system automatically fills in the ID of the default resource group.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "resourceGroupId"))
 
     @resource_group_id.setter
     def resource_group_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDomain, "resource_group_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "resourceGroupId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="scope")
     def scope(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: scope: Valid values: domestic, overseas, and global. Default value: domestic. The setting is supported for users outside mainland China, users in mainland China of level 3 or above.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "scope"))
 
     @scope.setter
     def scope(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDomain, "scope").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "scope", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="sources")
     def sources(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: sources: The list of origin URLs.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "sources"))
 
     @sources.setter
     def sources(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDomain, "sources").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "sources", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="tags")
     def tags(self) -> typing.Optional[typing.List["RosDomain.TagsProperty"]]:
         '''
         :Property: tags: Tags to attach to instance. Max support 20 tags to add during create instance. Each tag with two properties Key and Value, and Key is required.
         '''
         return typing.cast(typing.Optional[typing.List["RosDomain.TagsProperty"]], jsii.get(self, "tags"))
 
     @tags.setter
     def tags(
         self,
         value: typing.Optional[typing.List["RosDomain.TagsProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDomain, "tags").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "tags", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="topLevelDomain")
     def top_level_domain(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: topLevelDomain: The top-level domain, which can only be configured by users on the whitelist.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "topLevelDomain"))
 
     @top_level_domain.setter
     def top_level_domain(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDomain, "top_level_domain").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "topLevelDomain", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-cdn.RosDomain.TagsProperty",
         jsii_struct_bases=[],
         name_mapping={"key": "key", "value": "value"},
     )
@@ -494,14 +558,18 @@
             key: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param key: 
             :param value: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosDomain.TagsProperty.__init__)
+                check_type(argname="argument key", value=key, expected_type=type_hints["key"])
+                check_type(argname="argument value", value=value, expected_type=type_hints["value"])
             self._values: typing.Dict[str, typing.Any] = {
                 "key": key,
             }
             if value is not None:
                 self._values["value"] = value
 
         @builtins.property
@@ -542,85 +610,103 @@
 ):
     '''A ROS template type:  ``ALIYUN::CDN::DomainConfig``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosDomainConfigProps",
+        props: typing.Union["RosDomainConfigProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::CDN::DomainConfig``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosDomainConfig.__init__)
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
+            type_hints = typing.get_type_hints(RosDomainConfig._render_properties)
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
     @jsii.member(jsii_name="domainNames")
     def domain_names(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: domainNames: Your accelerated domain name, separated by commas in English.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "domainNames"))
 
     @domain_names.setter
     def domain_names(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDomainConfig, "domain_names").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "domainNames", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         '''A factory method that creates a new instance of this class from an object containing the properties of this ROS resource.'''
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDomainConfig, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="functions")
     def functions(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: functions: function list, please refer to the CDN documentation for details.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "functions"))
 
     @functions.setter
     def functions(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDomainConfig, "functions").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "functions", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-cdn.RosDomainConfigProps",
     jsii_struct_bases=[],
     name_mapping={"domain_names": "domainNames", "functions": "functions"},
@@ -633,14 +719,18 @@
         functions: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
         '''Properties for defining a ``ALIYUN::CDN::DomainConfig``.
 
         :param domain_names: 
         :param functions: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosDomainConfigProps.__init__)
+            check_type(argname="argument domain_names", value=domain_names, expected_type=type_hints["domain_names"])
+            check_type(argname="argument functions", value=functions, expected_type=type_hints["functions"])
         self._values: typing.Dict[str, typing.Any] = {
             "domain_names": domain_names,
             "functions": functions,
         }
 
     @builtins.property
     def domain_names(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
@@ -692,28 +782,38 @@
         *,
         cdn_type: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         domain_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         check_url: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         resource_group_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         scope: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         sources: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        tags: typing.Optional[typing.Sequence[RosDomain.TagsProperty]] = None,
+        tags: typing.Optional[typing.Sequence[typing.Union[RosDomain.TagsProperty, typing.Dict[str, typing.Any]]]] = None,
         top_level_domain: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::CDN::Domain``.
 
         :param cdn_type: 
         :param domain_name: 
         :param check_url: 
         :param resource_group_id: 
         :param scope: 
         :param sources: 
         :param tags: 
         :param top_level_domain: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosDomainProps.__init__)
+            check_type(argname="argument cdn_type", value=cdn_type, expected_type=type_hints["cdn_type"])
+            check_type(argname="argument domain_name", value=domain_name, expected_type=type_hints["domain_name"])
+            check_type(argname="argument check_url", value=check_url, expected_type=type_hints["check_url"])
+            check_type(argname="argument resource_group_id", value=resource_group_id, expected_type=type_hints["resource_group_id"])
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument sources", value=sources, expected_type=type_hints["sources"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
+            check_type(argname="argument top_level_domain", value=top_level_domain, expected_type=type_hints["top_level_domain"])
         self._values: typing.Dict[str, typing.Any] = {
             "cdn_type": cdn_type,
             "domain_name": domain_name,
         }
         if check_url is not None:
             self._values["check_url"] = check_url
         if resource_group_id is not None:
```

### Comparing `ros-cdk-cdn-1.0.8/src/ros_cdk_cdn.egg-info/PKG-INFO` & `ros-cdk-cdn-1.0.9/src/ros_cdk_cdn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-cdn
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS CDN Construct Library
```

