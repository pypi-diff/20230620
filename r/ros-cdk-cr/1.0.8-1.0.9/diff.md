# Comparing `tmp/ros-cdk-cr-1.0.8.tar.gz` & `tmp/ros-cdk-cr-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-cr-1.0.8.tar", last modified: Thu Jul 14 02:14:19 2022, max compression
+gzip compressed data, was "dist/ros-cdk-cr-1.0.9.tar", last modified: Fri Sep 23 12:28:04 2022, max compression
```

## Comparing `ros-cdk-cr-1.0.8.tar` & `ros-cdk-cr-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:14:19.000000 ros-cdk-cr-1.0.8/
--rw-r--r--   0 root         (0) root         (0)    10279 2022-07-14 02:14:19.000000 ros-cdk-cr-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2022-07-14 02:14:19.000000 ros-cdk-cr-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2022-07-14 02:14:19.000000 ros-cdk-cr-1.0.8/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1236 2022-07-14 02:14:19.000000 ros-cdk-cr-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      176 2022-07-14 02:14:19.000000 ros-cdk-cr-1.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)      106 2022-07-14 02:14:19.000000 ros-cdk-cr-1.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-07-14 02:14:19.000000 ros-cdk-cr-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1788 2022-07-14 02:14:19.000000 ros-cdk-cr-1.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:14:19.000000 ros-cdk-cr-1.0.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:14:19.000000 ros-cdk-cr-1.0.8/src/ros_cdk_cr/
--rw-r--r--   0 root         (0) root         (0)    70585 2022-07-14 02:14:19.000000 ros-cdk-cr-1.0.8/src/ros_cdk_cr/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:14:19.000000 ros-cdk-cr-1.0.8/src/ros_cdk_cr/_jsii/
--rw-r--r--   0 root         (0) root         (0)      368 2022-07-14 02:14:19.000000 ros-cdk-cr-1.0.8/src/ros_cdk_cr/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    47634 2022-07-14 02:14:19.000000 ros-cdk-cr-1.0.8/src/ros_cdk_cr/_jsii/ros-cdk-cr@1.0.8.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:14:19.000000 ros-cdk-cr-1.0.8/src/ros_cdk_cr/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:14:19.000000 ros-cdk-cr-1.0.8/src/ros_cdk_cr.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1236 2022-07-14 02:14:19.000000 ros-cdk-cr-1.0.8/src/ros_cdk_cr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      390 2022-07-14 02:14:19.000000 ros-cdk-cr-1.0.8/src/ros_cdk_cr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:14:19.000000 ros-cdk-cr-1.0.8/src/ros_cdk_cr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2022-07-14 02:14:19.000000 ros-cdk-cr-1.0.8/src/ros_cdk_cr.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2022-07-14 02:14:19.000000 ros-cdk-cr-1.0.8/src/ros_cdk_cr.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:28:04.000000 ros-cdk-cr-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)    10279 2022-09-23 12:28:03.000000 ros-cdk-cr-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-09-23 12:28:03.000000 ros-cdk-cr-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2022-09-23 12:28:03.000000 ros-cdk-cr-1.0.9/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1236 2022-09-23 12:28:04.000000 ros-cdk-cr-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      176 2022-09-23 12:28:03.000000 ros-cdk-cr-1.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      236 2022-09-23 12:28:03.000000 ros-cdk-cr-1.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-09-23 12:28:04.000000 ros-cdk-cr-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1817 2022-09-23 12:28:03.000000 ros-cdk-cr-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:28:04.000000 ros-cdk-cr-1.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:28:04.000000 ros-cdk-cr-1.0.9/src/ros_cdk_cr/
+-rw-r--r--   0 root         (0) root         (0)    86515 2022-09-23 12:28:03.000000 ros-cdk-cr-1.0.9/src/ros_cdk_cr/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:28:04.000000 ros-cdk-cr-1.0.9/src/ros_cdk_cr/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      402 2022-09-23 12:28:03.000000 ros-cdk-cr-1.0.9/src/ros_cdk_cr/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    47705 2022-09-23 12:28:03.000000 ros-cdk-cr-1.0.9/src/ros_cdk_cr/_jsii/ros-cdk-cr@1.0.9.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 12:28:03.000000 ros-cdk-cr-1.0.9/src/ros_cdk_cr/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:28:04.000000 ros-cdk-cr-1.0.9/src/ros_cdk_cr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1236 2022-09-23 12:28:03.000000 ros-cdk-cr-1.0.9/src/ros_cdk_cr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      390 2022-09-23 12:28:03.000000 ros-cdk-cr-1.0.9/src/ros_cdk_cr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 12:28:03.000000 ros-cdk-cr-1.0.9/src/ros_cdk_cr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2022-09-23 12:28:03.000000 ros-cdk-cr-1.0.9/src/ros_cdk_cr.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2022-09-23 12:28:03.000000 ros-cdk-cr-1.0.9/src/ros_cdk_cr.egg-info/top_level.txt
```

### Comparing `ros-cdk-cr-1.0.8/LICENSE` & `ros-cdk-cr-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-cr-1.0.8/PKG-INFO` & `ros-cdk-cr-1.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-cr
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS CR Construct Library
```

### Comparing `ros-cdk-cr-1.0.8/setup.py` & `ros-cdk-cr-1.0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-cr",
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
         "ros_cdk_cr",
         "ros_cdk_cr._jsii"
     ],
     "package_data": {
         "ros_cdk_cr._jsii": [
-            "ros-cdk-cr@1.0.8.jsii.tgz"
+            "ros-cdk-cr@1.0.9.jsii.tgz"
         ],
         "ros_cdk_cr": [
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

### Comparing `ros-cdk-cr-1.0.8/src/ros_cdk_cr/__init__.py` & `ros-cdk-cr-1.0.9/src/ros_cdk_cr/__init__.py`

 * *Files 19% similar despite different names*

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
 
 
 class InstanceEndpointAclPolicy(
     ros_cdk_core.Resource,
@@ -29,37 +31,43 @@
 ):
     '''A ROS resource type:  ``ALIYUN::CR::InstanceEndpointAclPolicy``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "InstanceEndpointAclPolicyProps",
+        props: typing.Union["InstanceEndpointAclPolicyProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::CR::InstanceEndpointAclPolicy``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(InstanceEndpointAclPolicy.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrEntry")
     def attr_entry(self) -> ros_cdk_core.IResolvable:
         '''Attribute Entry: The IP address range that is allowed to access the instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrEntry"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInstanceId")
     def attr_instance_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute InstanceId: The ID of the instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInstanceId"))
 
 
 @jsii.data_type(
@@ -90,14 +98,22 @@
         :param entry: Property entry: The IP address range that is allowed to access the instance.
         :param instance_id: Property instanceId: The ID of the instance.
         :param comment: Property comment: The description of the entry.
         :param endpoint_type: Property endpointType: The type of the endpoint.
         :param module_name: Property moduleName: The name of the module in the instance for which a whitelist is configured. Valid values: Registry and Chart.
         :param region_id: Property regionId: Region ID of instance. Default is current region.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(InstanceEndpointAclPolicyProps.__init__)
+            check_type(argname="argument entry", value=entry, expected_type=type_hints["entry"])
+            check_type(argname="argument instance_id", value=instance_id, expected_type=type_hints["instance_id"])
+            check_type(argname="argument comment", value=comment, expected_type=type_hints["comment"])
+            check_type(argname="argument endpoint_type", value=endpoint_type, expected_type=type_hints["endpoint_type"])
+            check_type(argname="argument module_name", value=module_name, expected_type=type_hints["module_name"])
+            check_type(argname="argument region_id", value=region_id, expected_type=type_hints["region_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "entry": entry,
             "instance_id": instance_id,
         }
         if comment is not None:
             self._values["comment"] = comment
         if endpoint_type is not None:
@@ -179,43 +195,49 @@
 ):
     '''A ROS resource type:  ``ALIYUN::CR::Namespace``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "NamespaceProps",
+        props: typing.Union["NamespaceProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::CR::Namespace``.
 
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
     @jsii.member(jsii_name="attrInstanceId")
     def attr_instance_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute InstanceId: The ID of the enterprise edition instance which namespace belongs to.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInstanceId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrNamespace")
     def attr_namespace(self) -> ros_cdk_core.IResolvable:
         '''Attribute Namespace: The namespace.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrNamespace"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrNamespaceId")
     def attr_namespace_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute NamespaceId: The namespace ID.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrNamespaceId"))
 
 
 @jsii.data_type(
@@ -240,14 +262,20 @@
         '''Properties for defining a ``ALIYUN::CR::Namespace``.
 
         :param namespace: Property namespace: The name of the namespace.
         :param auto_create: Property autoCreate: Specifies whether to automatically create an image repository.
         :param default_visibility: Property defaultVisibility: The default type of the repository that is automatically created. Valid values: PUBLIC, PRIVATE.
         :param instance_id: Property instanceId: The ID of the enterprise edition instance which namespace belongs to. If not provided, will use personal edition instance as default.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(NamespaceProps.__init__)
+            check_type(argname="argument namespace", value=namespace, expected_type=type_hints["namespace"])
+            check_type(argname="argument auto_create", value=auto_create, expected_type=type_hints["auto_create"])
+            check_type(argname="argument default_visibility", value=default_visibility, expected_type=type_hints["default_visibility"])
+            check_type(argname="argument instance_id", value=instance_id, expected_type=type_hints["instance_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "namespace": namespace,
         }
         if auto_create is not None:
             self._values["auto_create"] = auto_create
         if default_visibility is not None:
             self._values["default_visibility"] = default_visibility
@@ -310,55 +338,61 @@
 ):
     '''A ROS resource type:  ``ALIYUN::CR::Repository``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RepositoryProps",
+        props: typing.Union["RepositoryProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::CR::Repository``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(Repository.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInstanceId")
     def attr_instance_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute InstanceId: The ID of the enterprise edition instance which repository belongs to.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInstanceId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrRepoId")
     def attr_repo_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute RepoId: The repository ID.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrRepoId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrRepoName")
     def attr_repo_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute RepoName: The name of the repository.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrRepoName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrRepoNamespace")
     def attr_repo_namespace(self) -> ros_cdk_core.IResolvable:
         '''Attribute RepoNamespace: The name of the namespace to which the repository belongs.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrRepoNamespace"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrRepoType")
     def attr_repo_type(self) -> ros_cdk_core.IResolvable:
         '''Attribute RepoType: The type of the repository.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrRepoType"))
 
 
 @jsii.data_type(
@@ -381,28 +415,38 @@
         *,
         repo_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         repo_namespace: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         repo_type: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         summary: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         detail: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         instance_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        repo_source: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosRepository.RepoSourceProperty"]] = None,
+        repo_source: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosRepository.RepoSourceProperty", typing.Dict[str, typing.Any]]]] = None,
         tag_immutability: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::CR::Repository``.
 
         :param repo_name: Property repoName: The name of the repository.
         :param repo_namespace: Property repoNamespace: The name of the namespace to which the repository belongs.
         :param repo_type: Property repoType: The type of the repository. Valid values: PUBLIC, PRIVATE.
         :param summary: Property summary: The summary of the repository.
         :param detail: Property detail: The description of the repository.
         :param instance_id: Property instanceId: The ID of the enterprise edition instance which repository belongs to. If not provided, will use personal edition instance as default.
         :param repo_source: Property repoSource: Code Source message.
         :param tag_immutability: Property tagImmutability: Specifies whether the repository is immutable. Only takes effect when InstanceId is specified.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RepositoryProps.__init__)
+            check_type(argname="argument repo_name", value=repo_name, expected_type=type_hints["repo_name"])
+            check_type(argname="argument repo_namespace", value=repo_namespace, expected_type=type_hints["repo_namespace"])
+            check_type(argname="argument repo_type", value=repo_type, expected_type=type_hints["repo_type"])
+            check_type(argname="argument summary", value=summary, expected_type=type_hints["summary"])
+            check_type(argname="argument detail", value=detail, expected_type=type_hints["detail"])
+            check_type(argname="argument instance_id", value=instance_id, expected_type=type_hints["instance_id"])
+            check_type(argname="argument repo_source", value=repo_source, expected_type=type_hints["repo_source"])
+            check_type(argname="argument tag_immutability", value=tag_immutability, expected_type=type_hints["tag_immutability"])
         self._values: typing.Dict[str, typing.Any] = {
             "repo_name": repo_name,
             "repo_namespace": repo_namespace,
             "repo_type": repo_type,
             "summary": summary,
         }
         if detail is not None:
@@ -502,137 +546,161 @@
 ):
     '''A ROS template type:  ``ALIYUN::CR::InstanceEndpointAclPolicy``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosInstanceEndpointAclPolicyProps",
+        props: typing.Union["RosInstanceEndpointAclPolicyProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::CR::InstanceEndpointAclPolicy``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosInstanceEndpointAclPolicy.__init__)
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
+            type_hints = typing.get_type_hints(RosInstanceEndpointAclPolicy._render_properties)
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
     @jsii.member(jsii_name="attrEntry")
     def attr_entry(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Entry: The IP address range that is allowed to access the instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrEntry"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosInstanceEndpointAclPolicy, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="entry")
     def entry(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: entry: The IP address range that is allowed to access the instance.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "entry"))
 
     @entry.setter
     def entry(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstanceEndpointAclPolicy, "entry").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "entry", value)
 
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
+            type_hints = typing.get_type_hints(getattr(RosInstanceEndpointAclPolicy, "instance_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "instanceId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="comment")
     def comment(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: comment: The description of the entry.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "comment"))
 
     @comment.setter
     def comment(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstanceEndpointAclPolicy, "comment").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "comment", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="endpointType")
     def endpoint_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: endpointType: The type of the endpoint.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "endpointType"))
 
     @endpoint_type.setter
     def endpoint_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstanceEndpointAclPolicy, "endpoint_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "endpointType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="moduleName")
     def module_name(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -642,31 +710,37 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "moduleName"))
 
     @module_name.setter
     def module_name(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstanceEndpointAclPolicy, "module_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "moduleName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="regionId")
     def region_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: regionId: Region ID of instance. Default is current region.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "regionId"))
 
     @region_id.setter
     def region_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstanceEndpointAclPolicy, "region_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "regionId", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-cr.RosInstanceEndpointAclPolicyProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -694,14 +768,22 @@
         :param entry: 
         :param instance_id: 
         :param comment: 
         :param endpoint_type: 
         :param module_name: 
         :param region_id: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosInstanceEndpointAclPolicyProps.__init__)
+            check_type(argname="argument entry", value=entry, expected_type=type_hints["entry"])
+            check_type(argname="argument instance_id", value=instance_id, expected_type=type_hints["instance_id"])
+            check_type(argname="argument comment", value=comment, expected_type=type_hints["comment"])
+            check_type(argname="argument endpoint_type", value=endpoint_type, expected_type=type_hints["endpoint_type"])
+            check_type(argname="argument module_name", value=module_name, expected_type=type_hints["module_name"])
+            check_type(argname="argument region_id", value=region_id, expected_type=type_hints["region_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "entry": entry,
             "instance_id": instance_id,
         }
         if comment is not None:
             self._values["comment"] = comment
         if endpoint_type is not None:
@@ -791,144 +873,168 @@
 ):
     '''A ROS template type:  ``ALIYUN::CR::Namespace``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosNamespaceProps",
+        props: typing.Union["RosNamespaceProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::CR::Namespace``.
 
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
     @jsii.member(jsii_name="attrInstanceId")
     def attr_instance_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: InstanceId: The ID of the enterprise edition instance which namespace belongs to.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInstanceId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrNamespace")
     def attr_namespace(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Namespace: The namespace.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrNamespace"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrNamespaceId")
     def attr_namespace_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: NamespaceId: The namespace ID.
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
     @jsii.member(jsii_name="namespace")
     def namespace(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: namespace: The name of the namespace.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "namespace"))
 
     @namespace.setter
     def namespace(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosNamespace, "namespace").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "namespace", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="autoCreate")
     def auto_create(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property: autoCreate: Specifies whether to automatically create an image repository.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "autoCreate"))
 
     @auto_create.setter
     def auto_create(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosNamespace, "auto_create").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "autoCreate", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="defaultVisibility")
     def default_visibility(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: defaultVisibility: The default type of the repository that is automatically created. Valid values: PUBLIC, PRIVATE.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "defaultVisibility"))
 
     @default_visibility.setter
     def default_visibility(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosNamespace, "default_visibility").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "defaultVisibility", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="instanceId")
     def instance_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: instanceId: The ID of the enterprise edition instance which namespace belongs to. If not provided, will use personal edition instance as default.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "instanceId"))
 
     @instance_id.setter
     def instance_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosNamespace, "instance_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "instanceId", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-cr.RosNamespaceProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -950,14 +1056,20 @@
         '''Properties for defining a ``ALIYUN::CR::Namespace``.
 
         :param namespace: 
         :param auto_create: 
         :param default_visibility: 
         :param instance_id: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosNamespaceProps.__init__)
+            check_type(argname="argument namespace", value=namespace, expected_type=type_hints["namespace"])
+            check_type(argname="argument auto_create", value=auto_create, expected_type=type_hints["auto_create"])
+            check_type(argname="argument default_visibility", value=default_visibility, expected_type=type_hints["default_visibility"])
+            check_type(argname="argument instance_id", value=instance_id, expected_type=type_hints["instance_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "namespace": namespace,
         }
         if auto_create is not None:
             self._values["auto_create"] = auto_create
         if default_visibility is not None:
             self._values["default_visibility"] = default_visibility
@@ -1022,222 +1134,258 @@
 ):
     '''A ROS template type:  ``ALIYUN::CR::Repository``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosRepositoryProps",
+        props: typing.Union["RosRepositoryProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::CR::Repository``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosRepository.__init__)
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
+            type_hints = typing.get_type_hints(RosRepository._render_properties)
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
         :Attribute: InstanceId: The ID of the enterprise edition instance which repository belongs to.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInstanceId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrRepoId")
     def attr_repo_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: RepoId: The repository ID.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrRepoId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrRepoName")
     def attr_repo_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: RepoName: The name of the repository.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrRepoName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrRepoNamespace")
     def attr_repo_namespace(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: RepoNamespace: The name of the namespace to which the repository belongs.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrRepoNamespace"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrRepoType")
     def attr_repo_type(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: RepoType: The type of the repository.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrRepoType"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosRepository, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="repoName")
     def repo_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: repoName: The name of the repository.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "repoName"))
 
     @repo_name.setter
     def repo_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosRepository, "repo_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "repoName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="repoNamespace")
     def repo_namespace(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: repoNamespace: The name of the namespace to which the repository belongs.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "repoNamespace"))
 
     @repo_namespace.setter
     def repo_namespace(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosRepository, "repo_namespace").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "repoNamespace", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="repoType")
     def repo_type(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: repoType: The type of the repository. Valid values: PUBLIC, PRIVATE.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "repoType"))
 
     @repo_type.setter
     def repo_type(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosRepository, "repo_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "repoType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="summary")
     def summary(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: summary: The summary of the repository.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "summary"))
 
     @summary.setter
     def summary(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosRepository, "summary").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "summary", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="detail")
     def detail(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: detail: The description of the repository.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "detail"))
 
     @detail.setter
     def detail(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosRepository, "detail").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "detail", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="instanceId")
     def instance_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: instanceId: The ID of the enterprise edition instance which repository belongs to. If not provided, will use personal edition instance as default.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "instanceId"))
 
     @instance_id.setter
     def instance_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosRepository, "instance_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "instanceId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="repoSource")
     def repo_source(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosRepository.RepoSourceProperty"]]:
         '''
         :Property: repoSource: Code Source message.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosRepository.RepoSourceProperty"]], jsii.get(self, "repoSource"))
 
     @repo_source.setter
     def repo_source(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosRepository.RepoSourceProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosRepository, "repo_source").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "repoSource", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="tagImmutability")
     def tag_immutability(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property: tagImmutability: Specifies whether the repository is immutable. Only takes effect when InstanceId is specified.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "tagImmutability"))
 
     @tag_immutability.setter
     def tag_immutability(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosRepository, "tag_immutability").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "tagImmutability", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-cr.RosRepository.RepoSourceProperty",
         jsii_struct_bases=[],
         name_mapping={
             "is_auto_build": "isAutoBuild",
@@ -1263,14 +1411,22 @@
             :param is_auto_build: 
             :param is_disable_cache: 
             :param is_oversea: 
             :param source_repo_name: 
             :param source_repo_namespace: 
             :param source_repo_type: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosRepository.RepoSourceProperty.__init__)
+                check_type(argname="argument is_auto_build", value=is_auto_build, expected_type=type_hints["is_auto_build"])
+                check_type(argname="argument is_disable_cache", value=is_disable_cache, expected_type=type_hints["is_disable_cache"])
+                check_type(argname="argument is_oversea", value=is_oversea, expected_type=type_hints["is_oversea"])
+                check_type(argname="argument source_repo_name", value=source_repo_name, expected_type=type_hints["source_repo_name"])
+                check_type(argname="argument source_repo_namespace", value=source_repo_namespace, expected_type=type_hints["source_repo_namespace"])
+                check_type(argname="argument source_repo_type", value=source_repo_type, expected_type=type_hints["source_repo_type"])
             self._values: typing.Dict[str, typing.Any] = {
                 "is_auto_build": is_auto_build,
                 "is_disable_cache": is_disable_cache,
                 "is_oversea": is_oversea,
                 "source_repo_name": source_repo_name,
                 "source_repo_namespace": source_repo_namespace,
                 "source_repo_type": source_repo_type,
@@ -1375,28 +1531,38 @@
         *,
         repo_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         repo_namespace: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         repo_type: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         summary: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         detail: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         instance_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        repo_source: typing.Optional[typing.Union[ros_cdk_core.IResolvable, RosRepository.RepoSourceProperty]] = None,
+        repo_source: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosRepository.RepoSourceProperty, typing.Dict[str, typing.Any]]]] = None,
         tag_immutability: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::CR::Repository``.
 
         :param repo_name: 
         :param repo_namespace: 
         :param repo_type: 
         :param summary: 
         :param detail: 
         :param instance_id: 
         :param repo_source: 
         :param tag_immutability: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosRepositoryProps.__init__)
+            check_type(argname="argument repo_name", value=repo_name, expected_type=type_hints["repo_name"])
+            check_type(argname="argument repo_namespace", value=repo_namespace, expected_type=type_hints["repo_namespace"])
+            check_type(argname="argument repo_type", value=repo_type, expected_type=type_hints["repo_type"])
+            check_type(argname="argument summary", value=summary, expected_type=type_hints["summary"])
+            check_type(argname="argument detail", value=detail, expected_type=type_hints["detail"])
+            check_type(argname="argument instance_id", value=instance_id, expected_type=type_hints["instance_id"])
+            check_type(argname="argument repo_source", value=repo_source, expected_type=type_hints["repo_source"])
+            check_type(argname="argument tag_immutability", value=tag_immutability, expected_type=type_hints["tag_immutability"])
         self._values: typing.Dict[str, typing.Any] = {
             "repo_name": repo_name,
             "repo_namespace": repo_namespace,
             "repo_type": repo_type,
             "summary": summary,
         }
         if detail is not None:
@@ -1503,87 +1669,102 @@
 ):
     '''A ROS template type:  ``ALIYUN::CR::UserInfo``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosUserInfoProps",
+        props: typing.Union["RosUserInfoProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::CR::UserInfo``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosUserInfo.__init__)
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
+            type_hints = typing.get_type_hints(RosUserInfo._render_properties)
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
     @jsii.member(jsii_name="attrLoginName")
     def attr_login_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: LoginName: Login name.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrLoginName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrUserId")
     def attr_user_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: UserId: User ID.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrUserId"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosUserInfo, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="user")
     def user(
         self,
     ) -> typing.Union[ros_cdk_core.IResolvable, "RosUserInfo.UserProperty"]:
         '''
         :Property: user: User info. If user exists, will update user info.
         '''
         return typing.cast(typing.Union[ros_cdk_core.IResolvable, "RosUserInfo.UserProperty"], jsii.get(self, "user"))
 
     @user.setter
     def user(
         self,
         value: typing.Union[ros_cdk_core.IResolvable, "RosUserInfo.UserProperty"],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosUserInfo, "user").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "user", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-cr.RosUserInfo.UserProperty",
         jsii_struct_bases=[],
         name_mapping={"password": "password"},
     )
@@ -1592,14 +1773,17 @@
             self,
             *,
             password: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         ) -> None:
             '''
             :param password: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosUserInfo.UserProperty.__init__)
+                check_type(argname="argument password", value=password, expected_type=type_hints["password"])
             self._values: typing.Dict[str, typing.Any] = {
                 "password": password,
             }
 
         @builtins.property
         def password(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
             '''
@@ -1626,20 +1810,23 @@
     jsii_struct_bases=[],
     name_mapping={"user": "user"},
 )
 class RosUserInfoProps:
     def __init__(
         self,
         *,
-        user: typing.Union[ros_cdk_core.IResolvable, RosUserInfo.UserProperty],
+        user: typing.Union[ros_cdk_core.IResolvable, typing.Union[RosUserInfo.UserProperty, typing.Dict[str, typing.Any]]],
     ) -> None:
         '''Properties for defining a ``ALIYUN::CR::UserInfo``.
 
         :param user: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosUserInfoProps.__init__)
+            check_type(argname="argument user", value=user, expected_type=type_hints["user"])
         self._values: typing.Dict[str, typing.Any] = {
             "user": user,
         }
 
     @builtins.property
     def user(self) -> typing.Union[ros_cdk_core.IResolvable, RosUserInfo.UserProperty]:
         '''
@@ -1668,37 +1855,43 @@
 ):
     '''A ROS resource type:  ``ALIYUN::CR::UserInfo``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "UserInfoProps",
+        props: typing.Union["UserInfoProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::CR::UserInfo``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(UserInfo.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrLoginName")
     def attr_login_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute LoginName: Login name.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrLoginName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrUserId")
     def attr_user_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute UserId: User ID.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrUserId"))
 
 
 @jsii.data_type(
@@ -1706,20 +1899,23 @@
     jsii_struct_bases=[],
     name_mapping={"user": "user"},
 )
 class UserInfoProps:
     def __init__(
         self,
         *,
-        user: typing.Union[ros_cdk_core.IResolvable, RosUserInfo.UserProperty],
+        user: typing.Union[ros_cdk_core.IResolvable, typing.Union[RosUserInfo.UserProperty, typing.Dict[str, typing.Any]]],
     ) -> None:
         '''Properties for defining a ``ALIYUN::CR::UserInfo``.
 
         :param user: Property user: User info. If user exists, will update user info.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(UserInfoProps.__init__)
+            check_type(argname="argument user", value=user, expected_type=type_hints["user"])
         self._values: typing.Dict[str, typing.Any] = {
             "user": user,
         }
 
     @builtins.property
     def user(self) -> typing.Union[ros_cdk_core.IResolvable, RosUserInfo.UserProperty]:
         '''Property user: User info.
```

### Comparing `ros-cdk-cr-1.0.8/src/ros_cdk_cr.egg-info/PKG-INFO` & `ros-cdk-cr-1.0.9/src/ros_cdk_cr.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-cr
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS CR Construct Library
```

