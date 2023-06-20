# Comparing `tmp/ros-cdk-slb-1.0.8.tar.gz` & `tmp/ros-cdk-slb-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-slb-1.0.8.tar", last modified: Thu Jul 14 02:30:21 2022, max compression
+gzip compressed data, was "dist/ros-cdk-slb-1.0.9.tar", last modified: Fri Sep 23 11:21:02 2022, max compression
```

## Comparing `ros-cdk-slb-1.0.8.tar` & `ros-cdk-slb-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:30:21.000000 ros-cdk-slb-1.0.8/
--rw-r--r--   0 root         (0) root         (0)    10279 2022-07-14 02:30:21.000000 ros-cdk-slb-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2022-07-14 02:30:21.000000 ros-cdk-slb-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2022-07-14 02:30:21.000000 ros-cdk-slb-1.0.8/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1240 2022-07-14 02:30:21.000000 ros-cdk-slb-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      179 2022-07-14 02:30:21.000000 ros-cdk-slb-1.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)      106 2022-07-14 02:30:21.000000 ros-cdk-slb-1.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-07-14 02:30:21.000000 ros-cdk-slb-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1794 2022-07-14 02:30:21.000000 ros-cdk-slb-1.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:30:21.000000 ros-cdk-slb-1.0.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:30:21.000000 ros-cdk-slb-1.0.8/src/ros_cdk_slb/
--rw-r--r--   0 root         (0) root         (0)   343996 2022-07-14 02:30:21.000000 ros-cdk-slb-1.0.8/src/ros_cdk_slb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:30:21.000000 ros-cdk-slb-1.0.8/src/ros_cdk_slb/_jsii/
--rw-r--r--   0 root         (0) root         (0)      370 2022-07-14 02:30:21.000000 ros-cdk-slb-1.0.8/src/ros_cdk_slb/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)   135401 2022-07-14 02:30:21.000000 ros-cdk-slb-1.0.8/src/ros_cdk_slb/_jsii/ros-cdk-slb@1.0.8.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:30:21.000000 ros-cdk-slb-1.0.8/src/ros_cdk_slb/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:30:21.000000 ros-cdk-slb-1.0.8/src/ros_cdk_slb.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1240 2022-07-14 02:30:21.000000 ros-cdk-slb-1.0.8/src/ros_cdk_slb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      400 2022-07-14 02:30:21.000000 ros-cdk-slb-1.0.8/src/ros_cdk_slb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:30:21.000000 ros-cdk-slb-1.0.8/src/ros_cdk_slb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2022-07-14 02:30:21.000000 ros-cdk-slb-1.0.8/src/ros_cdk_slb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2022-07-14 02:30:21.000000 ros-cdk-slb-1.0.8/src/ros_cdk_slb.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:21:02.000000 ros-cdk-slb-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)    10279 2022-09-23 11:21:02.000000 ros-cdk-slb-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-09-23 11:21:02.000000 ros-cdk-slb-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2022-09-23 11:21:02.000000 ros-cdk-slb-1.0.9/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1240 2022-09-23 11:21:02.000000 ros-cdk-slb-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      179 2022-09-23 11:21:02.000000 ros-cdk-slb-1.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      236 2022-09-23 11:21:02.000000 ros-cdk-slb-1.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-09-23 11:21:02.000000 ros-cdk-slb-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1823 2022-09-23 11:21:02.000000 ros-cdk-slb-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:21:02.000000 ros-cdk-slb-1.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:21:02.000000 ros-cdk-slb-1.0.9/src/ros_cdk_slb/
+-rw-r--r--   0 root         (0) root         (0)   412132 2022-09-23 11:21:02.000000 ros-cdk-slb-1.0.9/src/ros_cdk_slb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:21:02.000000 ros-cdk-slb-1.0.9/src/ros_cdk_slb/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      404 2022-09-23 11:21:02.000000 ros-cdk-slb-1.0.9/src/ros_cdk_slb/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   136805 2022-09-23 11:21:02.000000 ros-cdk-slb-1.0.9/src/ros_cdk_slb/_jsii/ros-cdk-slb@1.0.9.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 11:21:02.000000 ros-cdk-slb-1.0.9/src/ros_cdk_slb/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:21:02.000000 ros-cdk-slb-1.0.9/src/ros_cdk_slb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1240 2022-09-23 11:21:02.000000 ros-cdk-slb-1.0.9/src/ros_cdk_slb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      400 2022-09-23 11:21:02.000000 ros-cdk-slb-1.0.9/src/ros_cdk_slb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 11:21:02.000000 ros-cdk-slb-1.0.9/src/ros_cdk_slb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2022-09-23 11:21:02.000000 ros-cdk-slb-1.0.9/src/ros_cdk_slb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2022-09-23 11:21:02.000000 ros-cdk-slb-1.0.9/src/ros_cdk_slb.egg-info/top_level.txt
```

### Comparing `ros-cdk-slb-1.0.8/LICENSE` & `ros-cdk-slb-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-slb-1.0.8/PKG-INFO` & `ros-cdk-slb-1.0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-slb
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS SLB Construct Library
```

### Comparing `ros-cdk-slb-1.0.8/setup.py` & `ros-cdk-slb-1.0.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-slb",
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
         "ros_cdk_slb",
         "ros_cdk_slb._jsii"
     ],
     "package_data": {
         "ros_cdk_slb._jsii": [
-            "ros-cdk-slb@1.0.8.jsii.tgz"
+            "ros-cdk-slb@1.0.9.jsii.tgz"
         ],
         "ros_cdk_slb": [
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

### Comparing `ros-cdk-slb-1.0.8/src/ros_cdk_slb/__init__.py` & `ros-cdk-slb-1.0.9/src/ros_cdk_slb/__init__.py`

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
 
 
 class AccessControl(
     ros_cdk_core.Resource,
@@ -29,31 +31,37 @@
 ):
     '''A ROS resource type:  ``ALIYUN::SLB::AccessControl``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "AccessControlProps",
+        props: typing.Union["AccessControlProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::SLB::AccessControl``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(AccessControl.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrAclId")
     def attr_acl_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute AclId: The ID of the access control list.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAclId"))
 
 
 @jsii.data_type(
@@ -68,27 +76,34 @@
     },
 )
 class AccessControlProps:
     def __init__(
         self,
         *,
         acl_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
-        acl_entrys: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosAccessControl.AclEntrysProperty"]]]] = None,
+        acl_entrys: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosAccessControl.AclEntrysProperty", typing.Dict[str, typing.Any]]]]]] = None,
         address_ip_version: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         resource_group_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        tags: typing.Optional[typing.Sequence["RosAccessControl.TagsProperty"]] = None,
+        tags: typing.Optional[typing.Sequence[typing.Union["RosAccessControl.TagsProperty", typing.Dict[str, typing.Any]]]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::SLB::AccessControl``.
 
         :param acl_name: Property aclName: The name of the access control list.
         :param acl_entrys: Property aclEntrys: A list of acl entrys. Each entry can be IP addresses or CIDR blocks. Max length: 50.
         :param address_ip_version: Property addressIpVersion: IP version. Could be "ipv4" or "ipv6".
         :param resource_group_id: Property resourceGroupId: Resource group id.
         :param tags: Property tags: Tags to attach to instance. Max support 20 tags to add during create instance. Each tag with two properties Key and Value, and Key is required.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(AccessControlProps.__init__)
+            check_type(argname="argument acl_name", value=acl_name, expected_type=type_hints["acl_name"])
+            check_type(argname="argument acl_entrys", value=acl_entrys, expected_type=type_hints["acl_entrys"])
+            check_type(argname="argument address_ip_version", value=address_ip_version, expected_type=type_hints["address_ip_version"])
+            check_type(argname="argument resource_group_id", value=resource_group_id, expected_type=type_hints["resource_group_id"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
         self._values: typing.Dict[str, typing.Any] = {
             "acl_name": acl_name,
         }
         if acl_entrys is not None:
             self._values["acl_entrys"] = acl_entrys
         if address_ip_version is not None:
             self._values["address_ip_version"] = address_ip_version
@@ -162,37 +177,43 @@
 ):
     '''A ROS resource type:  ``ALIYUN::SLB::BackendServerAttachment``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "BackendServerAttachmentProps",
+        props: typing.Union["BackendServerAttachmentProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::SLB::BackendServerAttachment``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(BackendServerAttachment.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrBackendServers")
     def attr_backend_servers(self) -> ros_cdk_core.IResolvable:
         '''Attribute BackendServers: The collection of attached backend server.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrBackendServers"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrLoadBalancerId")
     def attr_load_balancer_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute LoadBalancerId: The id of load balancer.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrLoadBalancerId"))
 
 
 @jsii.data_type(
@@ -207,24 +228,30 @@
 )
 class BackendServerAttachmentProps:
     def __init__(
         self,
         *,
         load_balancer_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         backend_server_list: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]] = None,
-        backend_servers: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosBackendServerAttachment.BackendServersProperty"]]]] = None,
+        backend_servers: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosBackendServerAttachment.BackendServersProperty", typing.Dict[str, typing.Any]]]]]] = None,
         backend_server_weight_list: typing.Optional[typing.Union[typing.Sequence[typing.Any], ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::SLB::BackendServerAttachment``.
 
         :param load_balancer_id: Property loadBalancerId: The id of load balancer.
         :param backend_server_list: Property backendServerList: The comma delimited instance id list.If the property "BackendServers" is setting, this property will be ignored.
         :param backend_servers: Property backendServers: The list of ECS instance, which will attached to load balancer.
         :param backend_server_weight_list: Property backendServerWeightList: The comma delimited weight list. If no value specified will use 100. If the length is small than "BackendServerList", it will copy the last one to fill the array.If the property "BackendServers" is setting, this property will be ignored.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(BackendServerAttachmentProps.__init__)
+            check_type(argname="argument load_balancer_id", value=load_balancer_id, expected_type=type_hints["load_balancer_id"])
+            check_type(argname="argument backend_server_list", value=backend_server_list, expected_type=type_hints["backend_server_list"])
+            check_type(argname="argument backend_servers", value=backend_servers, expected_type=type_hints["backend_servers"])
+            check_type(argname="argument backend_server_weight_list", value=backend_server_weight_list, expected_type=type_hints["backend_server_weight_list"])
         self._values: typing.Dict[str, typing.Any] = {
             "load_balancer_id": load_balancer_id,
         }
         if backend_server_list is not None:
             self._values["backend_server_list"] = backend_server_list
         if backend_servers is not None:
             self._values["backend_servers"] = backend_servers
@@ -284,31 +311,37 @@
 ):
     '''A ROS resource type:  ``ALIYUN::SLB::BackendServerToVServerGroupAddition``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "BackendServerToVServerGroupAdditionProps",
+        props: typing.Union["BackendServerToVServerGroupAdditionProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::SLB::BackendServerToVServerGroupAddition``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(BackendServerToVServerGroupAddition.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVServerGroupId")
     def attr_v_server_group_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute VServerGroupId: The ID of virtual server group.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVServerGroupId"))
 
 
 @jsii.data_type(
@@ -319,22 +352,26 @@
         "v_server_group_id": "vServerGroupId",
     },
 )
 class BackendServerToVServerGroupAdditionProps:
     def __init__(
         self,
         *,
-        backend_servers: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosBackendServerToVServerGroupAddition.BackendServersProperty"]]],
+        backend_servers: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosBackendServerToVServerGroupAddition.BackendServersProperty", typing.Dict[str, typing.Any]]]]],
         v_server_group_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
         '''Properties for defining a ``ALIYUN::SLB::BackendServerToVServerGroupAddition``.
 
         :param backend_servers: Property backendServers: The list of a combination of ECS Instance-Port-Weight.Same ecs instance with different port is allowed, but same ecs instance with same port isn't.
         :param v_server_group_id: Property vServerGroupId: The ID of virtual server group.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(BackendServerToVServerGroupAdditionProps.__init__)
+            check_type(argname="argument backend_servers", value=backend_servers, expected_type=type_hints["backend_servers"])
+            check_type(argname="argument v_server_group_id", value=v_server_group_id, expected_type=type_hints["v_server_group_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "backend_servers": backend_servers,
             "v_server_group_id": v_server_group_id,
         }
 
     @builtins.property
     def backend_servers(
@@ -371,37 +408,43 @@
 ):
     '''A ROS resource type:  ``ALIYUN::SLB::Certificate``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "CertificateProps",
+        props: typing.Union["CertificateProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::SLB::Certificate``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(Certificate.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrCertificateId")
     def attr_certificate_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute CertificateId: The ID of the certificate.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrCertificateId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrFingerprint")
     def attr_fingerprint(self) -> ros_cdk_core.IResolvable:
         '''Attribute Fingerprint: The fingerprint of the certificate.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrFingerprint"))
 
 
 @jsii.data_type(
@@ -425,27 +468,37 @@
         certificate: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         ali_cloud_certificate_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ali_cloud_certificate_name: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         certificate_name: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         certificate_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         private_key: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         resource_group_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        tags: typing.Optional[typing.Sequence["RosCertificate.TagsProperty"]] = None,
+        tags: typing.Optional[typing.Sequence[typing.Union["RosCertificate.TagsProperty", typing.Dict[str, typing.Any]]]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::SLB::Certificate``.
 
         :param certificate: Property certificate: The content of the certificate public key.
         :param ali_cloud_certificate_id: Property aliCloudCertificateId: The ID of the Alibaba Cloud certificate.
         :param ali_cloud_certificate_name: Property aliCloudCertificateName: The name of the Alibaba Cloud certificate.
         :param certificate_name: Property certificateName: The name of the certificate.
         :param certificate_type: Property certificateType: The type of the certificate.
         :param private_key: Property privateKey: The private key.
         :param resource_group_id: Property resourceGroupId: Resource group id.
         :param tags: Property tags: Tags to attach to instance. Max support 20 tags to add during create instance. Each tag with two properties Key and Value, and Key is required.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(CertificateProps.__init__)
+            check_type(argname="argument certificate", value=certificate, expected_type=type_hints["certificate"])
+            check_type(argname="argument ali_cloud_certificate_id", value=ali_cloud_certificate_id, expected_type=type_hints["ali_cloud_certificate_id"])
+            check_type(argname="argument ali_cloud_certificate_name", value=ali_cloud_certificate_name, expected_type=type_hints["ali_cloud_certificate_name"])
+            check_type(argname="argument certificate_name", value=certificate_name, expected_type=type_hints["certificate_name"])
+            check_type(argname="argument certificate_type", value=certificate_type, expected_type=type_hints["certificate_type"])
+            check_type(argname="argument private_key", value=private_key, expected_type=type_hints["private_key"])
+            check_type(argname="argument resource_group_id", value=resource_group_id, expected_type=type_hints["resource_group_id"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
         self._values: typing.Dict[str, typing.Any] = {
             "certificate": certificate,
         }
         if ali_cloud_certificate_id is not None:
             self._values["ali_cloud_certificate_id"] = ali_cloud_certificate_id
         if ali_cloud_certificate_name is not None:
             self._values["ali_cloud_certificate_name"] = ali_cloud_certificate_name
@@ -543,37 +596,43 @@
 ):
     '''A ROS resource type:  ``ALIYUN::SLB::DomainExtension``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "DomainExtensionProps",
+        props: typing.Union["DomainExtensionProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::SLB::DomainExtension``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(DomainExtension.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDomainExtensionId")
     def attr_domain_extension_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute DomainExtensionId: The ID of the created domain name extension.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDomainExtensionId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrListenerPort")
     def attr_listener_port(self) -> ros_cdk_core.IResolvable:
         '''Attribute ListenerPort: The front-end HTTPS listener port of the Server Load Balancer instance.
 
         Valid value:
         1-65535
         '''
@@ -602,14 +661,20 @@
         '''Properties for defining a ``ALIYUN::SLB::DomainExtension``.
 
         :param domain: Property domain: The domain name.
         :param listener_port: Property listenerPort: The front-end HTTPS listener port of the Server Load Balancer instance. Valid value: 1-65535
         :param load_balancer_id: Property loadBalancerId: The ID of Server Load Balancer instance.
         :param server_certificate_id: Property serverCertificateId: The ID of the certificate corresponding to the domain name.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(DomainExtensionProps.__init__)
+            check_type(argname="argument domain", value=domain, expected_type=type_hints["domain"])
+            check_type(argname="argument listener_port", value=listener_port, expected_type=type_hints["listener_port"])
+            check_type(argname="argument load_balancer_id", value=load_balancer_id, expected_type=type_hints["load_balancer_id"])
+            check_type(argname="argument server_certificate_id", value=server_certificate_id, expected_type=type_hints["server_certificate_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "domain": domain,
             "listener_port": listener_port,
             "load_balancer_id": load_balancer_id,
             "server_certificate_id": server_certificate_id,
         }
 
@@ -666,55 +731,61 @@
 ):
     '''A ROS resource type:  ``ALIYUN::SLB::Listener``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "ListenerProps",
+        props: typing.Union["ListenerProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::SLB::Listener``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(Listener.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrListenerPortsAndProtocol")
     def attr_listener_ports_and_protocol(self) -> ros_cdk_core.IResolvable:
         '''Attribute ListenerPortsAndProtocol: The collection of listener.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrListenerPortsAndProtocol"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrLoadBalancerId")
     def attr_load_balancer_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute LoadBalancerId: The id of load balancer.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrLoadBalancerId"))
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-slb.ListenerProps",
     jsii_struct_bases=[],
     name_mapping={
-        "backend_server_port": "backendServerPort",
         "bandwidth": "bandwidth",
         "listener_port": "listenerPort",
         "load_balancer_id": "loadBalancerId",
         "protocol": "protocol",
         "acl_id": "aclId",
         "acl_status": "aclStatus",
         "acl_type": "aclType",
+        "backend_server_port": "backendServerPort",
         "ca_certificate_id": "caCertificateId",
         "description": "description",
         "enable_http2": "enableHttp2",
         "health_check": "healthCheck",
         "http_config": "httpConfig",
         "idle_timeout": "idleTimeout",
         "master_slave_server_group_id": "masterSlaveServerGroupId",
@@ -727,47 +798,47 @@
         "v_server_group_id": "vServerGroupId",
     },
 )
 class ListenerProps:
     def __init__(
         self,
         *,
-        backend_server_port: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
         bandwidth: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
         listener_port: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
         load_balancer_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         protocol: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         acl_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         acl_status: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         acl_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
+        backend_server_port: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         ca_certificate_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         description: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         enable_http2: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        health_check: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosListener.HealthCheckProperty"]] = None,
-        http_config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosListener.HttpConfigProperty"]] = None,
+        health_check: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosListener.HealthCheckProperty", typing.Dict[str, typing.Any]]]] = None,
+        http_config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosListener.HttpConfigProperty", typing.Dict[str, typing.Any]]]] = None,
         idle_timeout: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         master_slave_server_group_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        persistence: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosListener.PersistenceProperty"]] = None,
-        port_range: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosListener.PortRangeProperty"]]]] = None,
+        persistence: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosListener.PersistenceProperty", typing.Dict[str, typing.Any]]]] = None,
+        port_range: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosListener.PortRangeProperty", typing.Dict[str, typing.Any]]]]]] = None,
         request_timeout: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         scheduler: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         server_certificate_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         start_listener: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         v_server_group_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::SLB::Listener``.
 
-        :param backend_server_port: Property backendServerPort: Backend server can listen on ports from 1 to 65535.
         :param bandwidth: Property bandwidth: The bandwidth of network, unit in Mbps(Million bits per second). If the specified load balancer with "LOAD_BALANCE_ID" is charged by "paybybandwidth" and is created in classic network, each Listener's bandwidth must be greater than 0 and the sum of all of its Listeners' bandwidth can't be greater than the bandwidth of the load balancer.
         :param listener_port: Property listenerPort: Port for front listener. Range from 0 to 65535.
         :param load_balancer_id: Property loadBalancerId: The id of load balancer to create listener.
         :param protocol: Property protocol: The load balancer transport protocol to use for routing: http, https, tcp, or udp.
         :param acl_id: Property aclId: The ID of the access control list associated with the listener to be created. If the value of the AclStatus parameter is on, this parameter is required.
         :param acl_status: Property aclStatus: Indicates whether to enable access control. Valid values: on | off. Default value: off
         :param acl_type: Property aclType: The access control type: * white: Indicates a whitelist. Only requests from IP addresses or CIDR blocks in the selected access control lists are forwarded. This applies to scenarios in which an application only allows access from specific IP addresses. Enabling a whitelist poses some risks to your services. After a whitelist is enabled, only the IP addresses in the list can access the listener. If you enable a whitelist without adding any IP addresses in the list, no requests are forwarded. - black: Indicates a blacklist. Requests from IP addresses or CIDR blocks in the selected access control lists are not forwarded (that is, they are blocked). This applies to scenarios in which an application only denies access from specific IP addresses. If you enable a blacklist without adding any IP addresses in the list, all requests are forwarded. If the value of the AclStatus parameter is on, this parameter is required.
+        :param backend_server_port: Property backendServerPort: Backend server can listen on ports from 1 to 65535.
         :param ca_certificate_id: Property caCertificateId: CA server certificate id, for https listener only.
         :param description: Property description: The description of the listener.It must be 1 to 80 characters in length and can contain letters, digits, hyphens (-), forward slashes (/), periods (.), and underscores (_). Chinese characters are supported.
         :param enable_http2: Property enableHttp2: Specifies whether to use HTTP/2. It takes effect when Protocol=https. Valid values: on: yes off: no
         :param health_check: Property healthCheck: The properties of health checking setting.
         :param http_config: Property httpConfig: Config for http protocol.
         :param idle_timeout: Property idleTimeout: Specify the idle connection timeout in seconds. Valid value: 1-60 If no request is received during the specified timeout period, Server Load Balancer will temporarily terminate the connection and restart the connection when the next request comes.
         :param master_slave_server_group_id: Property masterSlaveServerGroupId: The id of the MasterSlaveServerGroup which use in listener.
@@ -775,27 +846,52 @@
         :param port_range: Property portRange: Port range, only supports TCP or UDP listener. ListenerPort should be 0 when PortRange is specified.
         :param request_timeout: Property requestTimeout: Specify the request timeout in seconds. Valid value: 1-180 If no response is received from the backend server during the specified timeout period, Server Load Balancer will stop waiting and send an HTTP 504 error to the client.
         :param scheduler: Property scheduler: The scheduling algorithm. Valid values: wrr: Backend servers that have higher weights receive more requests than those that have lower weights. wlc: Requests are distributed based on the combination of the weights and connections to backend servers. If two backend servers have the same weight, the backend server that has fewer connections receives more requests. rr: Requests are distributed to backend servers in sequence. sch: specifies consistent hashing that is based on source IP addresses. Requests from the same source IP address are distributed to the same backend server. tch: specifies consistent hashing that is based on four factors: source IP address, destination IP address, source port number, and destination port number. Requests that contain the same preceding information are distributed to the same backend server. Default: wrr
         :param server_certificate_id: Property serverCertificateId: Server certificate id, for https listener only, this properties is required.
         :param start_listener: Property startListener: Whether start listener after listener created. Default True.
         :param v_server_group_id: Property vServerGroupId: The id of the VServerGroup which use in listener.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(ListenerProps.__init__)
+            check_type(argname="argument bandwidth", value=bandwidth, expected_type=type_hints["bandwidth"])
+            check_type(argname="argument listener_port", value=listener_port, expected_type=type_hints["listener_port"])
+            check_type(argname="argument load_balancer_id", value=load_balancer_id, expected_type=type_hints["load_balancer_id"])
+            check_type(argname="argument protocol", value=protocol, expected_type=type_hints["protocol"])
+            check_type(argname="argument acl_id", value=acl_id, expected_type=type_hints["acl_id"])
+            check_type(argname="argument acl_status", value=acl_status, expected_type=type_hints["acl_status"])
+            check_type(argname="argument acl_type", value=acl_type, expected_type=type_hints["acl_type"])
+            check_type(argname="argument backend_server_port", value=backend_server_port, expected_type=type_hints["backend_server_port"])
+            check_type(argname="argument ca_certificate_id", value=ca_certificate_id, expected_type=type_hints["ca_certificate_id"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument enable_http2", value=enable_http2, expected_type=type_hints["enable_http2"])
+            check_type(argname="argument health_check", value=health_check, expected_type=type_hints["health_check"])
+            check_type(argname="argument http_config", value=http_config, expected_type=type_hints["http_config"])
+            check_type(argname="argument idle_timeout", value=idle_timeout, expected_type=type_hints["idle_timeout"])
+            check_type(argname="argument master_slave_server_group_id", value=master_slave_server_group_id, expected_type=type_hints["master_slave_server_group_id"])
+            check_type(argname="argument persistence", value=persistence, expected_type=type_hints["persistence"])
+            check_type(argname="argument port_range", value=port_range, expected_type=type_hints["port_range"])
+            check_type(argname="argument request_timeout", value=request_timeout, expected_type=type_hints["request_timeout"])
+            check_type(argname="argument scheduler", value=scheduler, expected_type=type_hints["scheduler"])
+            check_type(argname="argument server_certificate_id", value=server_certificate_id, expected_type=type_hints["server_certificate_id"])
+            check_type(argname="argument start_listener", value=start_listener, expected_type=type_hints["start_listener"])
+            check_type(argname="argument v_server_group_id", value=v_server_group_id, expected_type=type_hints["v_server_group_id"])
         self._values: typing.Dict[str, typing.Any] = {
-            "backend_server_port": backend_server_port,
             "bandwidth": bandwidth,
             "listener_port": listener_port,
             "load_balancer_id": load_balancer_id,
             "protocol": protocol,
         }
         if acl_id is not None:
             self._values["acl_id"] = acl_id
         if acl_status is not None:
             self._values["acl_status"] = acl_status
         if acl_type is not None:
             self._values["acl_type"] = acl_type
+        if backend_server_port is not None:
+            self._values["backend_server_port"] = backend_server_port
         if ca_certificate_id is not None:
             self._values["ca_certificate_id"] = ca_certificate_id
         if description is not None:
             self._values["description"] = description
         if enable_http2 is not None:
             self._values["enable_http2"] = enable_http2
         if health_check is not None:
@@ -818,23 +914,14 @@
             self._values["server_certificate_id"] = server_certificate_id
         if start_listener is not None:
             self._values["start_listener"] = start_listener
         if v_server_group_id is not None:
             self._values["v_server_group_id"] = v_server_group_id
 
     @builtins.property
-    def backend_server_port(
-        self,
-    ) -> typing.Union[jsii.Number, ros_cdk_core.IResolvable]:
-        '''Property backendServerPort: Backend server can listen on ports from 1 to 65535.'''
-        result = self._values.get("backend_server_port")
-        assert result is not None, "Required property 'backend_server_port' is missing"
-        return typing.cast(typing.Union[jsii.Number, ros_cdk_core.IResolvable], result)
-
-    @builtins.property
     def bandwidth(self) -> typing.Union[jsii.Number, ros_cdk_core.IResolvable]:
         '''Property bandwidth: The bandwidth of network, unit in Mbps(Million bits per second).
 
         If the specified load balancer with "LOAD_BALANCE_ID" is charged by "paybybandwidth" and is created in classic network, each Listener's bandwidth must be greater than 0 and the sum of all of its Listeners' bandwidth can't be greater than the bandwidth of the load balancer.
         '''
         result = self._values.get("bandwidth")
         assert result is not None, "Required property 'bandwidth' is missing"
@@ -902,14 +989,22 @@
 
         If the value of the AclStatus parameter is on, this parameter is required.
         '''
         result = self._values.get("acl_type")
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], result)
 
     @builtins.property
+    def backend_server_port(
+        self,
+    ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
+        '''Property backendServerPort: Backend server can listen on ports from 1 to 65535.'''
+        result = self._values.get("backend_server_port")
+        return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], result)
+
+    @builtins.property
     def ca_certificate_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''Property caCertificateId: CA server certificate id, for https listener only.'''
         result = self._values.get("ca_certificate_id")
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], result)
 
@@ -1062,121 +1157,127 @@
 ):
     '''A ROS resource type:  ``ALIYUN::SLB::LoadBalancer``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: typing.Optional["LoadBalancerProps"] = None,
+        props: typing.Optional[typing.Union["LoadBalancerProps", typing.Dict[str, typing.Any]]] = None,
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::SLB::LoadBalancer``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(LoadBalancer.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrAddressIpVersion")
     def attr_address_ip_version(self) -> ros_cdk_core.IResolvable:
         '''Attribute AddressIPVersion: IP version.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAddressIpVersion"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrAddressType")
     def attr_address_type(self) -> ros_cdk_core.IResolvable:
         '''Attribute AddressType: The address type of the load balancer.
 
         "intranet" or "internet".
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAddressType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrBandwidth")
     def attr_bandwidth(self) -> ros_cdk_core.IResolvable:
         '''Attribute Bandwidth: The bandwidth for network.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrBandwidth"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrIpAddress")
     def attr_ip_address(self) -> ros_cdk_core.IResolvable:
         '''Attribute IpAddress: The ip address of the load balancer.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrIpAddress"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrLoadBalancerId")
     def attr_load_balancer_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute LoadBalancerId: The id of load balance created.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrLoadBalancerId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrLoadBalancerName")
     def attr_load_balancer_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute LoadBalancerName: Name of created load balancer.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrLoadBalancerName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrLoadBalancerSpec")
     def attr_load_balancer_spec(self) -> ros_cdk_core.IResolvable:
         '''Attribute LoadBalancerSpec: The specification of the Server Load Balancer instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrLoadBalancerSpec"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrMasterZoneId")
     def attr_master_zone_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute MasterZoneId: The master zone id to create load balancer instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrMasterZoneId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrNetworkType")
     def attr_network_type(self) -> ros_cdk_core.IResolvable:
         '''Attribute NetworkType: The network type of the load balancer.
 
         "vpc" or "classic" network.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrNetworkType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrOrderId")
     def attr_order_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute OrderId: The order ID.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrOrderId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPayType")
     def attr_pay_type(self) -> ros_cdk_core.IResolvable:
         '''Attribute PayType: The billing method of the instance to be created.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPayType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrResourceGroupId")
     def attr_resource_group_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute ResourceGroupId: Resource group id.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrResourceGroupId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrSlaveZoneId")
     def attr_slave_zone_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute SlaveZoneId: The slave zone id to create load balancer instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrSlaveZoneId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVpcId")
     def attr_vpc_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute VpcId: Vpc id.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVpcId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVSwitchId")
     def attr_v_switch_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute VSwitchId: VSwitch id.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVSwitchId"))
 
 
 class LoadBalancerClone(
@@ -1186,31 +1287,37 @@
 ):
     '''A ROS resource type:  ``ALIYUN::SLB::LoadBalancerClone``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "LoadBalancerCloneProps",
+        props: typing.Union["LoadBalancerCloneProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::SLB::LoadBalancerClone``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(LoadBalancerClone.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrLoadBalancerId")
     def attr_load_balancer_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute LoadBalancerId: The id of load balance generated.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrLoadBalancerId"))
 
 
 @jsii.data_type(
@@ -1230,21 +1337,21 @@
     },
 )
 class LoadBalancerCloneProps:
     def __init__(
         self,
         *,
         source_load_balancer_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
-        backend_servers: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosLoadBalancerClone.BackendServersProperty"]]]] = None,
+        backend_servers: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosLoadBalancerClone.BackendServersProperty", typing.Dict[str, typing.Any]]]]]] = None,
         backend_servers_policy: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         instance_charge_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         load_balancer_name: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         load_balancer_spec: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         resource_group_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        tags: typing.Optional[typing.Sequence["RosLoadBalancerClone.TagsProperty"]] = None,
+        tags: typing.Optional[typing.Sequence[typing.Union["RosLoadBalancerClone.TagsProperty", typing.Dict[str, typing.Any]]]] = None,
         tags_policy: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         v_switch_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::SLB::LoadBalancerClone``.
 
         :param source_load_balancer_id: Property sourceLoadBalancerId: Source load balancer id to clone.
         :param backend_servers: Property backendServers: The list of ECS instance, which will attached to load balancer.
@@ -1253,14 +1360,26 @@
         :param load_balancer_name: Property loadBalancerName: Name of created load balancer. Length is limited to 1-80 characters, allowed to contain letters, numbers, '-, /, _,.' When not specified, a default name will be assigned.
         :param load_balancer_spec: Property loadBalancerSpec: The specification of the load balancer. If not specified, it is same with the source load balancer. Note If InstanceChargeType is set to PayByCLCU, the LoadBalancerSpec parameter is invalid and you do not need to set this parameter.
         :param resource_group_id: Property resourceGroupId: Resource group id.
         :param tags: Property tags: Tags to attach to slb. Max support 5 tags to add during create slb. Each tag with two properties Key and Value, and Key is required.
         :param tags_policy: Property tagsPolicy: Solution for handle the tags. If select 'clone', it will clone from source load balancer. If select 'empty' it will not copy tags. If select 'append' it will append the new tags. If select 'replace' it will add new tags. Default is 'empty'.
         :param v_switch_id: Property vSwitchId: The new VSwitch ID to create load balancer instance. For VPC network only and the VSwitch should belong to the VPC which source load balancer is located.When not specified, source load balancer VSwitch ID will be used.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(LoadBalancerCloneProps.__init__)
+            check_type(argname="argument source_load_balancer_id", value=source_load_balancer_id, expected_type=type_hints["source_load_balancer_id"])
+            check_type(argname="argument backend_servers", value=backend_servers, expected_type=type_hints["backend_servers"])
+            check_type(argname="argument backend_servers_policy", value=backend_servers_policy, expected_type=type_hints["backend_servers_policy"])
+            check_type(argname="argument instance_charge_type", value=instance_charge_type, expected_type=type_hints["instance_charge_type"])
+            check_type(argname="argument load_balancer_name", value=load_balancer_name, expected_type=type_hints["load_balancer_name"])
+            check_type(argname="argument load_balancer_spec", value=load_balancer_spec, expected_type=type_hints["load_balancer_spec"])
+            check_type(argname="argument resource_group_id", value=resource_group_id, expected_type=type_hints["resource_group_id"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
+            check_type(argname="argument tags_policy", value=tags_policy, expected_type=type_hints["tags_policy"])
+            check_type(argname="argument v_switch_id", value=v_switch_id, expected_type=type_hints["v_switch_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "source_load_balancer_id": source_load_balancer_id,
         }
         if backend_servers is not None:
             self._values["backend_servers"] = backend_servers
         if backend_servers_policy is not None:
             self._values["backend_servers_policy"] = backend_servers_policy
@@ -1442,15 +1561,15 @@
         master_zone_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         modification_protection_reason: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         modification_protection_status: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         pay_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         pricing_cycle: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         resource_group_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         slave_zone_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        tags: typing.Optional[typing.Sequence["RosLoadBalancer.TagsProperty"]] = None,
+        tags: typing.Optional[typing.Sequence[typing.Union["RosLoadBalancer.TagsProperty", typing.Dict[str, typing.Any]]]] = None,
         vpc_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         v_switch_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::SLB::LoadBalancer``.
 
         :param address_ip_version: Property addressIpVersion: IP version, support 'ipv4' or 'ipv6'. If 'ipv6' is selected, please note that the zone and the specification are supported.
         :param address_type: Property addressType: Loader balancer address type. Support 'internet' and 'intranet' only, default is 'internet'.
@@ -1471,14 +1590,38 @@
         :param pricing_cycle: Property pricingCycle: Optional. The duration of the Subscription-billed Internet instance to be created. Valid values: month | year.
         :param resource_group_id: Property resourceGroupId: Resource group id.
         :param slave_zone_id: Property slaveZoneId: The slave zone id to create load balancer instance.
         :param tags: Property tags: Tags to attach to slb. Max support 5 tags to add during create slb. Each tag with two properties Key and Value, and Key is required.
         :param vpc_id: Property vpcId: The VPC id to create load balancer instance. For VPC network only.
         :param v_switch_id: Property vSwitchId: The VSwitch id to create load balancer instance. For VPC network only.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(LoadBalancerProps.__init__)
+            check_type(argname="argument address_ip_version", value=address_ip_version, expected_type=type_hints["address_ip_version"])
+            check_type(argname="argument address_type", value=address_type, expected_type=type_hints["address_type"])
+            check_type(argname="argument auto_pay", value=auto_pay, expected_type=type_hints["auto_pay"])
+            check_type(argname="argument auto_renew", value=auto_renew, expected_type=type_hints["auto_renew"])
+            check_type(argname="argument auto_renew_period", value=auto_renew_period, expected_type=type_hints["auto_renew_period"])
+            check_type(argname="argument bandwidth", value=bandwidth, expected_type=type_hints["bandwidth"])
+            check_type(argname="argument deletion_protection", value=deletion_protection, expected_type=type_hints["deletion_protection"])
+            check_type(argname="argument duration", value=duration, expected_type=type_hints["duration"])
+            check_type(argname="argument instance_charge_type", value=instance_charge_type, expected_type=type_hints["instance_charge_type"])
+            check_type(argname="argument internet_charge_type", value=internet_charge_type, expected_type=type_hints["internet_charge_type"])
+            check_type(argname="argument load_balancer_name", value=load_balancer_name, expected_type=type_hints["load_balancer_name"])
+            check_type(argname="argument load_balancer_spec", value=load_balancer_spec, expected_type=type_hints["load_balancer_spec"])
+            check_type(argname="argument master_zone_id", value=master_zone_id, expected_type=type_hints["master_zone_id"])
+            check_type(argname="argument modification_protection_reason", value=modification_protection_reason, expected_type=type_hints["modification_protection_reason"])
+            check_type(argname="argument modification_protection_status", value=modification_protection_status, expected_type=type_hints["modification_protection_status"])
+            check_type(argname="argument pay_type", value=pay_type, expected_type=type_hints["pay_type"])
+            check_type(argname="argument pricing_cycle", value=pricing_cycle, expected_type=type_hints["pricing_cycle"])
+            check_type(argname="argument resource_group_id", value=resource_group_id, expected_type=type_hints["resource_group_id"])
+            check_type(argname="argument slave_zone_id", value=slave_zone_id, expected_type=type_hints["slave_zone_id"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
+            check_type(argname="argument vpc_id", value=vpc_id, expected_type=type_hints["vpc_id"])
+            check_type(argname="argument v_switch_id", value=v_switch_id, expected_type=type_hints["v_switch_id"])
         self._values: typing.Dict[str, typing.Any] = {}
         if address_ip_version is not None:
             self._values["address_ip_version"] = address_ip_version
         if address_type is not None:
             self._values["address_type"] = address_type
         if auto_pay is not None:
             self._values["auto_pay"] = auto_pay
@@ -1771,31 +1914,37 @@
 ):
     '''A ROS resource type:  ``ALIYUN::SLB::MasterSlaveServerGroup``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "MasterSlaveServerGroupProps",
+        props: typing.Union["MasterSlaveServerGroupProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::SLB::MasterSlaveServerGroup``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(MasterSlaveServerGroup.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrMasterSlaveServerGroupId")
     def attr_master_slave_server_group_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute MasterSlaveServerGroupId: Active/standby server group ID.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrMasterSlaveServerGroupId"))
 
 
 @jsii.data_type(
@@ -1808,23 +1957,28 @@
     },
 )
 class MasterSlaveServerGroupProps:
     def __init__(
         self,
         *,
         load_balancer_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
-        master_slave_backend_servers: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosMasterSlaveServerGroup.MasterSlaveBackendServersProperty"]]],
+        master_slave_backend_servers: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosMasterSlaveServerGroup.MasterSlaveBackendServersProperty", typing.Dict[str, typing.Any]]]]],
         master_slave_server_group_name: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::SLB::MasterSlaveServerGroup``.
 
         :param load_balancer_id: Property loadBalancerId: The ID of the Server Load Balancer instance.
         :param master_slave_backend_servers: Property masterSlaveBackendServers: A list of active/standby server group. An active/standby server group can only contain two backend servers.
         :param master_slave_server_group_name: Property masterSlaveServerGroupName: The name of the active/standby server group.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(MasterSlaveServerGroupProps.__init__)
+            check_type(argname="argument load_balancer_id", value=load_balancer_id, expected_type=type_hints["load_balancer_id"])
+            check_type(argname="argument master_slave_backend_servers", value=master_slave_backend_servers, expected_type=type_hints["master_slave_backend_servers"])
+            check_type(argname="argument master_slave_server_group_name", value=master_slave_server_group_name, expected_type=type_hints["master_slave_server_group_name"])
         self._values: typing.Dict[str, typing.Any] = {
             "load_balancer_id": load_balancer_id,
             "master_slave_backend_servers": master_slave_backend_servers,
         }
         if master_slave_server_group_name is not None:
             self._values["master_slave_server_group_name"] = master_slave_server_group_name
 
@@ -1874,143 +2028,170 @@
 ):
     '''A ROS template type:  ``ALIYUN::SLB::AccessControl``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosAccessControlProps",
+        props: typing.Union["RosAccessControlProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::SLB::AccessControl``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosAccessControl.__init__)
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
+            type_hints = typing.get_type_hints(RosAccessControl._render_properties)
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
     @jsii.member(jsii_name="attrAclId")
     def attr_acl_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: AclId: The ID of the access control list.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAclId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="aclName")
     def acl_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: aclName: The name of the access control list.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "aclName"))
 
     @acl_name.setter
     def acl_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAccessControl, "acl_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "aclName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAccessControl, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="aclEntrys")
     def acl_entrys(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosAccessControl.AclEntrysProperty"]]]]:
         '''
         :Property: aclEntrys: A list of acl entrys. Each entry can be IP addresses or CIDR blocks. Max length: 50.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosAccessControl.AclEntrysProperty"]]]], jsii.get(self, "aclEntrys"))
 
     @acl_entrys.setter
     def acl_entrys(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosAccessControl.AclEntrysProperty"]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAccessControl, "acl_entrys").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "aclEntrys", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="addressIpVersion")
     def address_ip_version(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: addressIpVersion: IP version. Could be "ipv4" or "ipv6".
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "addressIpVersion"))
 
     @address_ip_version.setter
     def address_ip_version(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAccessControl, "address_ip_version").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "addressIpVersion", value)
 
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
+            type_hints = typing.get_type_hints(getattr(RosAccessControl, "resource_group_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "resourceGroupId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="tags")
     def tags(self) -> typing.Optional[typing.List["RosAccessControl.TagsProperty"]]:
         '''
         :Property: tags: Tags to attach to instance. Max support 20 tags to add during create instance. Each tag with two properties Key and Value, and Key is required.
         '''
         return typing.cast(typing.Optional[typing.List["RosAccessControl.TagsProperty"]], jsii.get(self, "tags"))
 
     @tags.setter
     def tags(
         self,
         value: typing.Optional[typing.List["RosAccessControl.TagsProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAccessControl, "tags").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "tags", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-slb.RosAccessControl.AclEntrysProperty",
         jsii_struct_bases=[],
         name_mapping={"entry": "entry", "comment": "comment"},
     )
@@ -2021,14 +2202,18 @@
             entry: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             comment: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param entry: 
             :param comment: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosAccessControl.AclEntrysProperty.__init__)
+                check_type(argname="argument entry", value=entry, expected_type=type_hints["entry"])
+                check_type(argname="argument comment", value=comment, expected_type=type_hints["comment"])
             self._values: typing.Dict[str, typing.Any] = {
                 "entry": entry,
             }
             if comment is not None:
                 self._values["comment"] = comment
 
         @builtins.property
@@ -2073,14 +2258,18 @@
             key: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param key: 
             :param value: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosAccessControl.TagsProperty.__init__)
+                check_type(argname="argument key", value=key, expected_type=type_hints["key"])
+                check_type(argname="argument value", value=value, expected_type=type_hints["value"])
             self._values: typing.Dict[str, typing.Any] = {
                 "key": key,
             }
             if value is not None:
                 self._values["value"] = value
 
         @builtins.property
@@ -2126,27 +2315,34 @@
     },
 )
 class RosAccessControlProps:
     def __init__(
         self,
         *,
         acl_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
-        acl_entrys: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosAccessControl.AclEntrysProperty]]]] = None,
+        acl_entrys: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosAccessControl.AclEntrysProperty, typing.Dict[str, typing.Any]]]]]] = None,
         address_ip_version: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         resource_group_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        tags: typing.Optional[typing.Sequence[RosAccessControl.TagsProperty]] = None,
+        tags: typing.Optional[typing.Sequence[typing.Union[RosAccessControl.TagsProperty, typing.Dict[str, typing.Any]]]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::SLB::AccessControl``.
 
         :param acl_name: 
         :param acl_entrys: 
         :param address_ip_version: 
         :param resource_group_id: 
         :param tags: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosAccessControlProps.__init__)
+            check_type(argname="argument acl_name", value=acl_name, expected_type=type_hints["acl_name"])
+            check_type(argname="argument acl_entrys", value=acl_entrys, expected_type=type_hints["acl_entrys"])
+            check_type(argname="argument address_ip_version", value=address_ip_version, expected_type=type_hints["address_ip_version"])
+            check_type(argname="argument resource_group_id", value=resource_group_id, expected_type=type_hints["resource_group_id"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
         self._values: typing.Dict[str, typing.Any] = {
             "acl_name": acl_name,
         }
         if acl_entrys is not None:
             self._values["acl_entrys"] = acl_entrys
         if address_ip_version is not None:
             self._values["address_ip_version"] = address_ip_version
@@ -2221,136 +2417,160 @@
 ):
     '''A ROS template type:  ``ALIYUN::SLB::BackendServerAttachment``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosBackendServerAttachmentProps",
+        props: typing.Union["RosBackendServerAttachmentProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::SLB::BackendServerAttachment``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosBackendServerAttachment.__init__)
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
+            type_hints = typing.get_type_hints(RosBackendServerAttachment._render_properties)
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
     @jsii.member(jsii_name="attrBackendServers")
     def attr_backend_servers(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: BackendServers: The collection of attached backend server.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrBackendServers"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrLoadBalancerId")
     def attr_load_balancer_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: LoadBalancerId: The id of load balancer.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrLoadBalancerId"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosBackendServerAttachment, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="loadBalancerId")
     def load_balancer_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: loadBalancerId: The id of load balancer.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "loadBalancerId"))
 
     @load_balancer_id.setter
     def load_balancer_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosBackendServerAttachment, "load_balancer_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "loadBalancerId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="backendServerList")
     def backend_server_list(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]]:
         '''
         :Property: backendServerList: The comma delimited instance id list.If the property "BackendServers" is setting, this property will be ignored.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]], jsii.get(self, "backendServerList"))
 
     @backend_server_list.setter
     def backend_server_list(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosBackendServerAttachment, "backend_server_list").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "backendServerList", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="backendServers")
     def backend_servers(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosBackendServerAttachment.BackendServersProperty"]]]]:
         '''
         :Property: backendServers: The list of ECS instance, which will attached to load balancer.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosBackendServerAttachment.BackendServersProperty"]]]], jsii.get(self, "backendServers"))
 
     @backend_servers.setter
     def backend_servers(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosBackendServerAttachment.BackendServersProperty"]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosBackendServerAttachment, "backend_servers").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "backendServers", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="backendServerWeightList")
     def backend_server_weight_list(
         self,
     ) -> typing.Optional[typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]]:
         '''
         :Property: backendServerWeightList: The comma delimited weight list. If no value specified will use 100. If the length is small than "BackendServerList", it will copy the last one to fill the array.If the property "BackendServers" is setting, this property will be ignored.
         '''
         return typing.cast(typing.Optional[typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]], jsii.get(self, "backendServerWeightList"))
 
     @backend_server_weight_list.setter
     def backend_server_weight_list(
         self,
         value: typing.Optional[typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosBackendServerAttachment, "backend_server_weight_list").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "backendServerWeightList", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-slb.RosBackendServerAttachment.BackendServersProperty",
         jsii_struct_bases=[],
         name_mapping={
             "server_id": "serverId",
@@ -2373,14 +2593,21 @@
             '''
             :param server_id: 
             :param weight: 
             :param description: 
             :param server_ip: 
             :param type: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosBackendServerAttachment.BackendServersProperty.__init__)
+                check_type(argname="argument server_id", value=server_id, expected_type=type_hints["server_id"])
+                check_type(argname="argument weight", value=weight, expected_type=type_hints["weight"])
+                check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+                check_type(argname="argument server_ip", value=server_ip, expected_type=type_hints["server_ip"])
+                check_type(argname="argument type", value=type, expected_type=type_hints["type"])
             self._values: typing.Dict[str, typing.Any] = {
                 "server_id": server_id,
                 "weight": weight,
             }
             if description is not None:
                 self._values["description"] = description
             if server_ip is not None:
@@ -2460,24 +2687,30 @@
 )
 class RosBackendServerAttachmentProps:
     def __init__(
         self,
         *,
         load_balancer_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         backend_server_list: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]] = None,
-        backend_servers: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosBackendServerAttachment.BackendServersProperty]]]] = None,
+        backend_servers: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosBackendServerAttachment.BackendServersProperty, typing.Dict[str, typing.Any]]]]]] = None,
         backend_server_weight_list: typing.Optional[typing.Union[typing.Sequence[typing.Any], ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::SLB::BackendServerAttachment``.
 
         :param load_balancer_id: 
         :param backend_server_list: 
         :param backend_servers: 
         :param backend_server_weight_list: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosBackendServerAttachmentProps.__init__)
+            check_type(argname="argument load_balancer_id", value=load_balancer_id, expected_type=type_hints["load_balancer_id"])
+            check_type(argname="argument backend_server_list", value=backend_server_list, expected_type=type_hints["backend_server_list"])
+            check_type(argname="argument backend_servers", value=backend_servers, expected_type=type_hints["backend_servers"])
+            check_type(argname="argument backend_server_weight_list", value=backend_server_weight_list, expected_type=type_hints["backend_server_weight_list"])
         self._values: typing.Dict[str, typing.Any] = {
             "load_balancer_id": load_balancer_id,
         }
         if backend_server_list is not None:
             self._values["backend_server_list"] = backend_server_list
         if backend_servers is not None:
             self._values["backend_servers"] = backend_servers
@@ -2542,94 +2775,112 @@
 ):
     '''A ROS template type:  ``ALIYUN::SLB::BackendServerToVServerGroupAddition``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosBackendServerToVServerGroupAdditionProps",
+        props: typing.Union["RosBackendServerToVServerGroupAdditionProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::SLB::BackendServerToVServerGroupAddition``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosBackendServerToVServerGroupAddition.__init__)
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
+            type_hints = typing.get_type_hints(RosBackendServerToVServerGroupAddition._render_properties)
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
     @jsii.member(jsii_name="attrVServerGroupId")
     def attr_v_server_group_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: VServerGroupId: The ID of virtual server group.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVServerGroupId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="backendServers")
     def backend_servers(
         self,
     ) -> typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosBackendServerToVServerGroupAddition.BackendServersProperty"]]]:
         '''
         :Property: backendServers: The list of a combination of ECS Instance-Port-Weight.Same ecs instance with different port is allowed, but same ecs instance with same port isn't.
         '''
         return typing.cast(typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosBackendServerToVServerGroupAddition.BackendServersProperty"]]], jsii.get(self, "backendServers"))
 
     @backend_servers.setter
     def backend_servers(
         self,
         value: typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosBackendServerToVServerGroupAddition.BackendServersProperty"]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosBackendServerToVServerGroupAddition, "backend_servers").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "backendServers", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosBackendServerToVServerGroupAddition, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vServerGroupId")
     def v_server_group_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: vServerGroupId: The ID of virtual server group.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "vServerGroupId"))
 
     @v_server_group_id.setter
     def v_server_group_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosBackendServerToVServerGroupAddition, "v_server_group_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "vServerGroupId", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-slb.RosBackendServerToVServerGroupAddition.BackendServersProperty",
         jsii_struct_bases=[],
         name_mapping={
             "port": "port",
@@ -2655,14 +2906,22 @@
             :param port: 
             :param server_id: 
             :param description: 
             :param server_ip: 
             :param type: 
             :param weight: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosBackendServerToVServerGroupAddition.BackendServersProperty.__init__)
+                check_type(argname="argument port", value=port, expected_type=type_hints["port"])
+                check_type(argname="argument server_id", value=server_id, expected_type=type_hints["server_id"])
+                check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+                check_type(argname="argument server_ip", value=server_ip, expected_type=type_hints["server_ip"])
+                check_type(argname="argument type", value=type, expected_type=type_hints["type"])
+                check_type(argname="argument weight", value=weight, expected_type=type_hints["weight"])
             self._values: typing.Dict[str, typing.Any] = {
                 "port": port,
                 "server_id": server_id,
             }
             if description is not None:
                 self._values["description"] = description
             if server_ip is not None:
@@ -2755,22 +3014,26 @@
         "v_server_group_id": "vServerGroupId",
     },
 )
 class RosBackendServerToVServerGroupAdditionProps:
     def __init__(
         self,
         *,
-        backend_servers: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosBackendServerToVServerGroupAddition.BackendServersProperty]]],
+        backend_servers: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosBackendServerToVServerGroupAddition.BackendServersProperty, typing.Dict[str, typing.Any]]]]],
         v_server_group_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
         '''Properties for defining a ``ALIYUN::SLB::BackendServerToVServerGroupAddition``.
 
         :param backend_servers: 
         :param v_server_group_id: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosBackendServerToVServerGroupAdditionProps.__init__)
+            check_type(argname="argument backend_servers", value=backend_servers, expected_type=type_hints["backend_servers"])
+            check_type(argname="argument v_server_group_id", value=v_server_group_id, expected_type=type_hints["v_server_group_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "backend_servers": backend_servers,
             "v_server_group_id": v_server_group_id,
         }
 
     @builtins.property
     def backend_servers(
@@ -2811,202 +3074,238 @@
 ):
     '''A ROS template type:  ``ALIYUN::SLB::Certificate``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosCertificateProps",
+        props: typing.Union["RosCertificateProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::SLB::Certificate``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosCertificate.__init__)
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
+            type_hints = typing.get_type_hints(RosCertificate._render_properties)
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
     @jsii.member(jsii_name="attrCertificateId")
     def attr_certificate_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: CertificateId: The ID of the certificate.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrCertificateId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrFingerprint")
     def attr_fingerprint(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Fingerprint: The fingerprint of the certificate.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrFingerprint"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="certificate")
     def certificate(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: certificate: The content of the certificate public key.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "certificate"))
 
     @certificate.setter
     def certificate(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCertificate, "certificate").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "certificate", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCertificate, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="aliCloudCertificateId")
     def ali_cloud_certificate_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: aliCloudCertificateId: The ID of the Alibaba Cloud certificate.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "aliCloudCertificateId"))
 
     @ali_cloud_certificate_id.setter
     def ali_cloud_certificate_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCertificate, "ali_cloud_certificate_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "aliCloudCertificateId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="aliCloudCertificateName")
     def ali_cloud_certificate_name(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: aliCloudCertificateName: The name of the Alibaba Cloud certificate.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "aliCloudCertificateName"))
 
     @ali_cloud_certificate_name.setter
     def ali_cloud_certificate_name(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCertificate, "ali_cloud_certificate_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "aliCloudCertificateName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="certificateName")
     def certificate_name(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: certificateName: The name of the certificate.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "certificateName"))
 
     @certificate_name.setter
     def certificate_name(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCertificate, "certificate_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "certificateName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="certificateType")
     def certificate_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: certificateType: The type of the certificate.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "certificateType"))
 
     @certificate_type.setter
     def certificate_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCertificate, "certificate_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "certificateType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="privateKey")
     def private_key(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: privateKey: The private key.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "privateKey"))
 
     @private_key.setter
     def private_key(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCertificate, "private_key").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "privateKey", value)
 
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
+            type_hints = typing.get_type_hints(getattr(RosCertificate, "resource_group_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "resourceGroupId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="tags")
     def tags(self) -> typing.Optional[typing.List["RosCertificate.TagsProperty"]]:
         '''
         :Property: tags: Tags to attach to instance. Max support 20 tags to add during create instance. Each tag with two properties Key and Value, and Key is required.
         '''
         return typing.cast(typing.Optional[typing.List["RosCertificate.TagsProperty"]], jsii.get(self, "tags"))
 
     @tags.setter
     def tags(
         self,
         value: typing.Optional[typing.List["RosCertificate.TagsProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCertificate, "tags").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "tags", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-slb.RosCertificate.TagsProperty",
         jsii_struct_bases=[],
         name_mapping={"key": "key", "value": "value"},
     )
@@ -3017,14 +3316,18 @@
             key: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param key: 
             :param value: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosCertificate.TagsProperty.__init__)
+                check_type(argname="argument key", value=key, expected_type=type_hints["key"])
+                check_type(argname="argument value", value=value, expected_type=type_hints["value"])
             self._values: typing.Dict[str, typing.Any] = {
                 "key": key,
             }
             if value is not None:
                 self._values["value"] = value
 
         @builtins.property
@@ -3079,27 +3382,37 @@
         certificate: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         ali_cloud_certificate_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ali_cloud_certificate_name: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         certificate_name: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         certificate_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         private_key: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         resource_group_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        tags: typing.Optional[typing.Sequence[RosCertificate.TagsProperty]] = None,
+        tags: typing.Optional[typing.Sequence[typing.Union[RosCertificate.TagsProperty, typing.Dict[str, typing.Any]]]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::SLB::Certificate``.
 
         :param certificate: 
         :param ali_cloud_certificate_id: 
         :param ali_cloud_certificate_name: 
         :param certificate_name: 
         :param certificate_type: 
         :param private_key: 
         :param resource_group_id: 
         :param tags: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosCertificateProps.__init__)
+            check_type(argname="argument certificate", value=certificate, expected_type=type_hints["certificate"])
+            check_type(argname="argument ali_cloud_certificate_id", value=ali_cloud_certificate_id, expected_type=type_hints["ali_cloud_certificate_id"])
+            check_type(argname="argument ali_cloud_certificate_name", value=ali_cloud_certificate_name, expected_type=type_hints["ali_cloud_certificate_name"])
+            check_type(argname="argument certificate_name", value=certificate_name, expected_type=type_hints["certificate_name"])
+            check_type(argname="argument certificate_type", value=certificate_type, expected_type=type_hints["certificate_type"])
+            check_type(argname="argument private_key", value=private_key, expected_type=type_hints["private_key"])
+            check_type(argname="argument resource_group_id", value=resource_group_id, expected_type=type_hints["resource_group_id"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
         self._values: typing.Dict[str, typing.Any] = {
             "certificate": certificate,
         }
         if ali_cloud_certificate_id is not None:
             self._values["ali_cloud_certificate_id"] = ali_cloud_certificate_id
         if ali_cloud_certificate_name is not None:
             self._values["ali_cloud_certificate_name"] = ali_cloud_certificate_name
@@ -3210,91 +3523,106 @@
 ):
     '''A ROS template type:  ``ALIYUN::SLB::DomainExtension``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosDomainExtensionProps",
+        props: typing.Union["RosDomainExtensionProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::SLB::DomainExtension``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosDomainExtension.__init__)
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
+            type_hints = typing.get_type_hints(RosDomainExtension._render_properties)
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
     @jsii.member(jsii_name="attrDomainExtensionId")
     def attr_domain_extension_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: DomainExtensionId: The ID of the created domain name extension.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDomainExtensionId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrListenerPort")
     def attr_listener_port(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute:
 
         ListenerPort: The front-end HTTPS listener port of the Server Load Balancer instance. Valid value:
         1-65535
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrListenerPort"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="domain")
     def domain(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: domain: The domain name.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "domain"))
 
     @domain.setter
     def domain(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDomainExtension, "domain").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "domain", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDomainExtension, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="listenerPort")
     def listener_port(self) -> typing.Union[jsii.Number, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         listenerPort: The front-end HTTPS listener port of the Server Load Balancer instance. Valid value:
         1-65535
@@ -3302,46 +3630,55 @@
         return typing.cast(typing.Union[jsii.Number, ros_cdk_core.IResolvable], jsii.get(self, "listenerPort"))
 
     @listener_port.setter
     def listener_port(
         self,
         value: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDomainExtension, "listener_port").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "listenerPort", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="loadBalancerId")
     def load_balancer_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: loadBalancerId: The ID of Server Load Balancer instance.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "loadBalancerId"))
 
     @load_balancer_id.setter
     def load_balancer_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDomainExtension, "load_balancer_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "loadBalancerId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="serverCertificateId")
     def server_certificate_id(
         self,
     ) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: serverCertificateId: The ID of the certificate corresponding to the domain name.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "serverCertificateId"))
 
     @server_certificate_id.setter
     def server_certificate_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDomainExtension, "server_certificate_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "serverCertificateId", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-slb.RosDomainExtensionProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -3363,14 +3700,20 @@
         '''Properties for defining a ``ALIYUN::SLB::DomainExtension``.
 
         :param domain: 
         :param listener_port: 
         :param load_balancer_id: 
         :param server_certificate_id: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosDomainExtensionProps.__init__)
+            check_type(argname="argument domain", value=domain, expected_type=type_hints["domain"])
+            check_type(argname="argument listener_port", value=listener_port, expected_type=type_hints["listener_port"])
+            check_type(argname="argument load_balancer_id", value=load_balancer_id, expected_type=type_hints["load_balancer_id"])
+            check_type(argname="argument server_certificate_id", value=server_certificate_id, expected_type=type_hints["server_certificate_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "domain": domain,
             "listener_port": listener_port,
             "load_balancer_id": load_balancer_id,
             "server_certificate_id": server_certificate_id,
         }
 
@@ -3434,150 +3777,157 @@
 ):
     '''A ROS template type:  ``ALIYUN::SLB::Listener``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosListenerProps",
+        props: typing.Union["RosListenerProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::SLB::Listener``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosListener.__init__)
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
+            type_hints = typing.get_type_hints(RosListener._render_properties)
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
     @jsii.member(jsii_name="attrListenerPortsAndProtocol")
     def attr_listener_ports_and_protocol(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ListenerPortsAndProtocol: The collection of listener.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrListenerPortsAndProtocol"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrLoadBalancerId")
     def attr_load_balancer_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: LoadBalancerId: The id of load balancer
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrLoadBalancerId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
-    @jsii.member(jsii_name="backendServerPort")
-    def backend_server_port(
-        self,
-    ) -> typing.Union[jsii.Number, ros_cdk_core.IResolvable]:
-        '''
-        :Property: backendServerPort: Backend server can listen on ports from 1 to 65535.
-        '''
-        return typing.cast(typing.Union[jsii.Number, ros_cdk_core.IResolvable], jsii.get(self, "backendServerPort"))
-
-    @backend_server_port.setter
-    def backend_server_port(
-        self,
-        value: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
-    ) -> None:
-        jsii.set(self, "backendServerPort", value)
-
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="bandwidth")
     def bandwidth(self) -> typing.Union[jsii.Number, ros_cdk_core.IResolvable]:
         '''
         :Property: bandwidth: The bandwidth of network, unit in Mbps(Million bits per second). If the specified load balancer with "LOAD_BALANCE_ID" is charged by "paybybandwidth" and is created in classic network, each Listener's bandwidth must be greater than 0 and the sum of all of its Listeners' bandwidth can't be greater than the bandwidth of the load balancer.
         '''
         return typing.cast(typing.Union[jsii.Number, ros_cdk_core.IResolvable], jsii.get(self, "bandwidth"))
 
     @bandwidth.setter
     def bandwidth(
         self,
         value: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosListener, "bandwidth").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "bandwidth", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosListener, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="listenerPort")
     def listener_port(self) -> typing.Union[jsii.Number, ros_cdk_core.IResolvable]:
         '''
         :Property: listenerPort: Port for front listener. Range from 0 to 65535.
         '''
         return typing.cast(typing.Union[jsii.Number, ros_cdk_core.IResolvable], jsii.get(self, "listenerPort"))
 
     @listener_port.setter
     def listener_port(
         self,
         value: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosListener, "listener_port").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "listenerPort", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="loadBalancerId")
     def load_balancer_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: loadBalancerId: The id of load balancer to create listener.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "loadBalancerId"))
 
     @load_balancer_id.setter
     def load_balancer_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosListener, "load_balancer_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "loadBalancerId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="protocol")
     def protocol(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: protocol: The load balancer transport protocol to use for routing: http, https, tcp, or udp.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "protocol"))
 
     @protocol.setter
     def protocol(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosListener, "protocol").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "protocol", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="aclId")
     def acl_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -3587,17 +3937,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "aclId"))
 
     @acl_id.setter
     def acl_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosListener, "acl_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "aclId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="aclStatus")
     def acl_status(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -3607,17 +3960,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "aclStatus"))
 
     @acl_status.setter
     def acl_status(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosListener, "acl_status").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "aclStatus", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="aclType")
     def acl_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -3635,51 +3991,80 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "aclType"))
 
     @acl_type.setter
     def acl_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosListener, "acl_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "aclType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
+    @jsii.member(jsii_name="backendServerPort")
+    def backend_server_port(
+        self,
+    ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
+        '''
+        :Property: backendServerPort: Backend server can listen on ports from 1 to 65535.
+        '''
+        return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "backendServerPort"))
+
+    @backend_server_port.setter
+    def backend_server_port(
+        self,
+        value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosListener, "backend_server_port").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "backendServerPort", value)
+
+    @builtins.property
     @jsii.member(jsii_name="caCertificateId")
     def ca_certificate_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: caCertificateId: CA server certificate id, for https listener only.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "caCertificateId"))
 
     @ca_certificate_id.setter
     def ca_certificate_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosListener, "ca_certificate_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "caCertificateId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="description")
     def description(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: description: The description of the listener.It must be 1 to 80 characters in length and can contain letters, digits, hyphens (-), forward slashes (/), periods (.), and underscores (_). Chinese characters are supported.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "description"))
 
     @description.setter
     def description(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosListener, "description").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "description", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableHttp2")
     def enable_http2(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -3690,136 +4075,160 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "enableHttp2"))
 
     @enable_http2.setter
     def enable_http2(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosListener, "enable_http2").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableHttp2", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="healthCheck")
     def health_check(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosListener.HealthCheckProperty"]]:
         '''
         :Property: healthCheck: The properties of health checking setting.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosListener.HealthCheckProperty"]], jsii.get(self, "healthCheck"))
 
     @health_check.setter
     def health_check(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosListener.HealthCheckProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosListener, "health_check").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "healthCheck", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="httpConfig")
     def http_config(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosListener.HttpConfigProperty"]]:
         '''
         :Property: httpConfig: Config for http protocol.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosListener.HttpConfigProperty"]], jsii.get(self, "httpConfig"))
 
     @http_config.setter
     def http_config(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosListener.HttpConfigProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosListener, "http_config").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "httpConfig", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="idleTimeout")
     def idle_timeout(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: idleTimeout: Specify the idle connection timeout in seconds. Valid value: 1-60 If no request is received during the specified timeout period, Server Load Balancer will temporarily terminate the connection and restart the connection when the next request comes.
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "idleTimeout"))
 
     @idle_timeout.setter
     def idle_timeout(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosListener, "idle_timeout").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "idleTimeout", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="masterSlaveServerGroupId")
     def master_slave_server_group_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: masterSlaveServerGroupId: The id of the MasterSlaveServerGroup which use in listener.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "masterSlaveServerGroupId"))
 
     @master_slave_server_group_id.setter
     def master_slave_server_group_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosListener, "master_slave_server_group_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "masterSlaveServerGroupId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="persistence")
     def persistence(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosListener.PersistenceProperty"]]:
         '''
         :Property: persistence: The properties of persistence.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosListener.PersistenceProperty"]], jsii.get(self, "persistence"))
 
     @persistence.setter
     def persistence(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosListener.PersistenceProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosListener, "persistence").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "persistence", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="portRange")
     def port_range(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosListener.PortRangeProperty"]]]]:
         '''
         :Property: portRange: Port range, only supports TCP or UDP listener. ListenerPort should be 0 when PortRange is specified.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosListener.PortRangeProperty"]]]], jsii.get(self, "portRange"))
 
     @port_range.setter
     def port_range(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosListener.PortRangeProperty"]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosListener, "port_range").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "portRange", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="requestTimeout")
     def request_timeout(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: requestTimeout: Specify the request timeout in seconds. Valid value: 1-180 If no response is received from the backend server during the specified timeout period, Server Load Balancer will stop waiting and send an HTTP 504 error to the client.
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "requestTimeout"))
 
     @request_timeout.setter
     def request_timeout(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosListener, "request_timeout").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "requestTimeout", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="scheduler")
     def scheduler(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -3834,65 +4243,77 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "scheduler"))
 
     @scheduler.setter
     def scheduler(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosListener, "scheduler").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "scheduler", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="serverCertificateId")
     def server_certificate_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: serverCertificateId: Server certificate id, for https listener only, this properties is required.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "serverCertificateId"))
 
     @server_certificate_id.setter
     def server_certificate_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosListener, "server_certificate_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "serverCertificateId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="startListener")
     def start_listener(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property: startListener: Whether start listener after listener created. Default True.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "startListener"))
 
     @start_listener.setter
     def start_listener(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosListener, "start_listener").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "startListener", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vServerGroupId")
     def v_server_group_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: vServerGroupId: The id of the VServerGroup which use in listener.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "vServerGroupId"))
 
     @v_server_group_id.setter
     def v_server_group_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosListener, "v_server_group_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "vServerGroupId", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-slb.RosListener.HealthCheckProperty",
         jsii_struct_bases=[],
         name_mapping={
             "domain": "domain",
@@ -3933,14 +4354,27 @@
             :param interval: 
             :param port: 
             :param switch: 
             :param timeout: 
             :param unhealthy_threshold: 
             :param uri: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosListener.HealthCheckProperty.__init__)
+                check_type(argname="argument domain", value=domain, expected_type=type_hints["domain"])
+                check_type(argname="argument health_check_method", value=health_check_method, expected_type=type_hints["health_check_method"])
+                check_type(argname="argument health_check_type", value=health_check_type, expected_type=type_hints["health_check_type"])
+                check_type(argname="argument healthy_threshold", value=healthy_threshold, expected_type=type_hints["healthy_threshold"])
+                check_type(argname="argument http_code", value=http_code, expected_type=type_hints["http_code"])
+                check_type(argname="argument interval", value=interval, expected_type=type_hints["interval"])
+                check_type(argname="argument port", value=port, expected_type=type_hints["port"])
+                check_type(argname="argument switch", value=switch, expected_type=type_hints["switch"])
+                check_type(argname="argument timeout", value=timeout, expected_type=type_hints["timeout"])
+                check_type(argname="argument unhealthy_threshold", value=unhealthy_threshold, expected_type=type_hints["unhealthy_threshold"])
+                check_type(argname="argument uri", value=uri, expected_type=type_hints["uri"])
             self._values: typing.Dict[str, typing.Any] = {}
             if domain is not None:
                 self._values["domain"] = domain
             if health_check_method is not None:
                 self._values["health_check_method"] = health_check_method
             if health_check_type is not None:
                 self._values["health_check_type"] = health_check_type
@@ -4100,14 +4534,18 @@
             forward_port: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
             listener_forward: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param forward_port: 
             :param listener_forward: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosListener.HttpConfigProperty.__init__)
+                check_type(argname="argument forward_port", value=forward_port, expected_type=type_hints["forward_port"])
+                check_type(argname="argument listener_forward", value=listener_forward, expected_type=type_hints["listener_forward"])
             self._values: typing.Dict[str, typing.Any] = {}
             if forward_port is not None:
                 self._values["forward_port"] = forward_port
             if listener_forward is not None:
                 self._values["listener_forward"] = listener_forward
 
         @builtins.property
@@ -4189,14 +4627,27 @@
             :param x_forwarded_for: 
             :param x_forwarded_for_client_src_port: 
             :param x_forwarded_for_proto: 
             :param x_forwarded_for_slbid: 
             :param x_forwarded_for_slbip: 
             :param x_forwarded_for_slbport: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosListener.PersistenceProperty.__init__)
+                check_type(argname="argument cookie", value=cookie, expected_type=type_hints["cookie"])
+                check_type(argname="argument cookie_timeout", value=cookie_timeout, expected_type=type_hints["cookie_timeout"])
+                check_type(argname="argument persistence_timeout", value=persistence_timeout, expected_type=type_hints["persistence_timeout"])
+                check_type(argname="argument sticky_session", value=sticky_session, expected_type=type_hints["sticky_session"])
+                check_type(argname="argument sticky_session_type", value=sticky_session_type, expected_type=type_hints["sticky_session_type"])
+                check_type(argname="argument x_forwarded_for", value=x_forwarded_for, expected_type=type_hints["x_forwarded_for"])
+                check_type(argname="argument x_forwarded_for_client_src_port", value=x_forwarded_for_client_src_port, expected_type=type_hints["x_forwarded_for_client_src_port"])
+                check_type(argname="argument x_forwarded_for_proto", value=x_forwarded_for_proto, expected_type=type_hints["x_forwarded_for_proto"])
+                check_type(argname="argument x_forwarded_for_slbid", value=x_forwarded_for_slbid, expected_type=type_hints["x_forwarded_for_slbid"])
+                check_type(argname="argument x_forwarded_for_slbip", value=x_forwarded_for_slbip, expected_type=type_hints["x_forwarded_for_slbip"])
+                check_type(argname="argument x_forwarded_for_slbport", value=x_forwarded_for_slbport, expected_type=type_hints["x_forwarded_for_slbport"])
             self._values: typing.Dict[str, typing.Any] = {}
             if cookie is not None:
                 self._values["cookie"] = cookie
             if cookie_timeout is not None:
                 self._values["cookie_timeout"] = cookie_timeout
             if persistence_timeout is not None:
                 self._values["persistence_timeout"] = persistence_timeout
@@ -4350,14 +4801,18 @@
             end_port: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
             start_port: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
         ) -> None:
             '''
             :param end_port: 
             :param start_port: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosListener.PortRangeProperty.__init__)
+                check_type(argname="argument end_port", value=end_port, expected_type=type_hints["end_port"])
+                check_type(argname="argument start_port", value=start_port, expected_type=type_hints["start_port"])
             self._values: typing.Dict[str, typing.Any] = {
                 "end_port": end_port,
                 "start_port": start_port,
             }
 
         @builtins.property
         def end_port(self) -> typing.Union[jsii.Number, ros_cdk_core.IResolvable]:
@@ -4389,22 +4844,22 @@
             )
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-slb.RosListenerProps",
     jsii_struct_bases=[],
     name_mapping={
-        "backend_server_port": "backendServerPort",
         "bandwidth": "bandwidth",
         "listener_port": "listenerPort",
         "load_balancer_id": "loadBalancerId",
         "protocol": "protocol",
         "acl_id": "aclId",
         "acl_status": "aclStatus",
         "acl_type": "aclType",
+        "backend_server_port": "backendServerPort",
         "ca_certificate_id": "caCertificateId",
         "description": "description",
         "enable_http2": "enableHttp2",
         "health_check": "healthCheck",
         "http_config": "httpConfig",
         "idle_timeout": "idleTimeout",
         "master_slave_server_group_id": "masterSlaveServerGroupId",
@@ -4417,47 +4872,47 @@
         "v_server_group_id": "vServerGroupId",
     },
 )
 class RosListenerProps:
     def __init__(
         self,
         *,
-        backend_server_port: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
         bandwidth: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
         listener_port: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
         load_balancer_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         protocol: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         acl_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         acl_status: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         acl_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
+        backend_server_port: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         ca_certificate_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         description: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         enable_http2: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        health_check: typing.Optional[typing.Union[ros_cdk_core.IResolvable, RosListener.HealthCheckProperty]] = None,
-        http_config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, RosListener.HttpConfigProperty]] = None,
+        health_check: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosListener.HealthCheckProperty, typing.Dict[str, typing.Any]]]] = None,
+        http_config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosListener.HttpConfigProperty, typing.Dict[str, typing.Any]]]] = None,
         idle_timeout: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         master_slave_server_group_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        persistence: typing.Optional[typing.Union[ros_cdk_core.IResolvable, RosListener.PersistenceProperty]] = None,
-        port_range: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosListener.PortRangeProperty]]]] = None,
+        persistence: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosListener.PersistenceProperty, typing.Dict[str, typing.Any]]]] = None,
+        port_range: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosListener.PortRangeProperty, typing.Dict[str, typing.Any]]]]]] = None,
         request_timeout: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         scheduler: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         server_certificate_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         start_listener: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         v_server_group_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::SLB::Listener``.
 
-        :param backend_server_port: 
         :param bandwidth: 
         :param listener_port: 
         :param load_balancer_id: 
         :param protocol: 
         :param acl_id: 
         :param acl_status: 
         :param acl_type: 
+        :param backend_server_port: 
         :param ca_certificate_id: 
         :param description: 
         :param enable_http2: 
         :param health_check: 
         :param http_config: 
         :param idle_timeout: 
         :param master_slave_server_group_id: 
@@ -4465,27 +4920,52 @@
         :param port_range: 
         :param request_timeout: 
         :param scheduler: 
         :param server_certificate_id: 
         :param start_listener: 
         :param v_server_group_id: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosListenerProps.__init__)
+            check_type(argname="argument bandwidth", value=bandwidth, expected_type=type_hints["bandwidth"])
+            check_type(argname="argument listener_port", value=listener_port, expected_type=type_hints["listener_port"])
+            check_type(argname="argument load_balancer_id", value=load_balancer_id, expected_type=type_hints["load_balancer_id"])
+            check_type(argname="argument protocol", value=protocol, expected_type=type_hints["protocol"])
+            check_type(argname="argument acl_id", value=acl_id, expected_type=type_hints["acl_id"])
+            check_type(argname="argument acl_status", value=acl_status, expected_type=type_hints["acl_status"])
+            check_type(argname="argument acl_type", value=acl_type, expected_type=type_hints["acl_type"])
+            check_type(argname="argument backend_server_port", value=backend_server_port, expected_type=type_hints["backend_server_port"])
+            check_type(argname="argument ca_certificate_id", value=ca_certificate_id, expected_type=type_hints["ca_certificate_id"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument enable_http2", value=enable_http2, expected_type=type_hints["enable_http2"])
+            check_type(argname="argument health_check", value=health_check, expected_type=type_hints["health_check"])
+            check_type(argname="argument http_config", value=http_config, expected_type=type_hints["http_config"])
+            check_type(argname="argument idle_timeout", value=idle_timeout, expected_type=type_hints["idle_timeout"])
+            check_type(argname="argument master_slave_server_group_id", value=master_slave_server_group_id, expected_type=type_hints["master_slave_server_group_id"])
+            check_type(argname="argument persistence", value=persistence, expected_type=type_hints["persistence"])
+            check_type(argname="argument port_range", value=port_range, expected_type=type_hints["port_range"])
+            check_type(argname="argument request_timeout", value=request_timeout, expected_type=type_hints["request_timeout"])
+            check_type(argname="argument scheduler", value=scheduler, expected_type=type_hints["scheduler"])
+            check_type(argname="argument server_certificate_id", value=server_certificate_id, expected_type=type_hints["server_certificate_id"])
+            check_type(argname="argument start_listener", value=start_listener, expected_type=type_hints["start_listener"])
+            check_type(argname="argument v_server_group_id", value=v_server_group_id, expected_type=type_hints["v_server_group_id"])
         self._values: typing.Dict[str, typing.Any] = {
-            "backend_server_port": backend_server_port,
             "bandwidth": bandwidth,
             "listener_port": listener_port,
             "load_balancer_id": load_balancer_id,
             "protocol": protocol,
         }
         if acl_id is not None:
             self._values["acl_id"] = acl_id
         if acl_status is not None:
             self._values["acl_status"] = acl_status
         if acl_type is not None:
             self._values["acl_type"] = acl_type
+        if backend_server_port is not None:
+            self._values["backend_server_port"] = backend_server_port
         if ca_certificate_id is not None:
             self._values["ca_certificate_id"] = ca_certificate_id
         if description is not None:
             self._values["description"] = description
         if enable_http2 is not None:
             self._values["enable_http2"] = enable_http2
         if health_check is not None:
@@ -4508,25 +4988,14 @@
             self._values["server_certificate_id"] = server_certificate_id
         if start_listener is not None:
             self._values["start_listener"] = start_listener
         if v_server_group_id is not None:
             self._values["v_server_group_id"] = v_server_group_id
 
     @builtins.property
-    def backend_server_port(
-        self,
-    ) -> typing.Union[jsii.Number, ros_cdk_core.IResolvable]:
-        '''
-        :Property: backendServerPort: Backend server can listen on ports from 1 to 65535.
-        '''
-        result = self._values.get("backend_server_port")
-        assert result is not None, "Required property 'backend_server_port' is missing"
-        return typing.cast(typing.Union[jsii.Number, ros_cdk_core.IResolvable], result)
-
-    @builtins.property
     def bandwidth(self) -> typing.Union[jsii.Number, ros_cdk_core.IResolvable]:
         '''
         :Property: bandwidth: The bandwidth of network, unit in Mbps(Million bits per second). If the specified load balancer with "LOAD_BALANCE_ID" is charged by "paybybandwidth" and is created in classic network, each Listener's bandwidth must be greater than 0 and the sum of all of its Listeners' bandwidth can't be greater than the bandwidth of the load balancer.
         '''
         result = self._values.get("bandwidth")
         assert result is not None, "Required property 'bandwidth' is missing"
         return typing.cast(typing.Union[jsii.Number, ros_cdk_core.IResolvable], result)
@@ -4602,14 +5071,24 @@
 
         If the value of the AclStatus parameter is on, this parameter is required.
         '''
         result = self._values.get("acl_type")
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], result)
 
     @builtins.property
+    def backend_server_port(
+        self,
+    ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
+        '''
+        :Property: backendServerPort: Backend server can listen on ports from 1 to 65535.
+        '''
+        result = self._values.get("backend_server_port")
+        return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], result)
+
+    @builtins.property
     def ca_certificate_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: caCertificateId: CA server certificate id, for https listener only.
         '''
         result = self._values.get("ca_certificate_id")
@@ -4776,211 +5255,229 @@
 ):
     '''A ROS template type:  ``ALIYUN::SLB::LoadBalancer``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosLoadBalancerProps",
+        props: typing.Union["RosLoadBalancerProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::SLB::LoadBalancer``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosLoadBalancer.__init__)
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
+            type_hints = typing.get_type_hints(RosLoadBalancer._render_properties)
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
     @jsii.member(jsii_name="attrAddressIpVersion")
     def attr_address_ip_version(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: AddressIPVersion: IP version
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAddressIpVersion"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrAddressType")
     def attr_address_type(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: AddressType: The address type of the load balancer. "intranet" or "internet".
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAddressType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrBandwidth")
     def attr_bandwidth(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Bandwidth: The bandwidth for network
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrBandwidth"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrIpAddress")
     def attr_ip_address(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: IpAddress: The ip address of the load balancer.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrIpAddress"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrLoadBalancerId")
     def attr_load_balancer_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: LoadBalancerId: The id of load balance created.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrLoadBalancerId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrLoadBalancerName")
     def attr_load_balancer_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: LoadBalancerName: Name of created load balancer.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrLoadBalancerName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrLoadBalancerSpec")
     def attr_load_balancer_spec(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: LoadBalancerSpec: The specification of the Server Load Balancer instance
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrLoadBalancerSpec"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrMasterZoneId")
     def attr_master_zone_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: MasterZoneId: The master zone id to create load balancer instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrMasterZoneId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrNetworkType")
     def attr_network_type(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: NetworkType: The network type of the load balancer. "vpc" or "classic" network.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrNetworkType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrOrderId")
     def attr_order_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: OrderId: The order ID.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrOrderId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPayType")
     def attr_pay_type(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: PayType: The billing method of the instance to be created.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPayType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrResourceGroupId")
     def attr_resource_group_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ResourceGroupId: Resource group id.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrResourceGroupId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrSlaveZoneId")
     def attr_slave_zone_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: SlaveZoneId: The slave zone id to create load balancer instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrSlaveZoneId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVpcId")
     def attr_vpc_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: VpcId: Vpc id
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVpcId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVSwitchId")
     def attr_v_switch_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: VSwitchId: VSwitch id
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVSwitchId"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosLoadBalancer, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="addressIpVersion")
     def address_ip_version(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: addressIpVersion: IP version, support 'ipv4' or 'ipv6'. If 'ipv6' is selected, please note that the zone and the specification are supported.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "addressIpVersion"))
 
     @address_ip_version.setter
     def address_ip_version(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosLoadBalancer, "address_ip_version").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "addressIpVersion", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="addressType")
     def address_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: addressType: Loader balancer address type. Support 'internet' and 'intranet' only, default is 'internet'.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "addressType"))
 
     @address_type.setter
     def address_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosLoadBalancer, "address_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "addressType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="autoPay")
     def auto_pay(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -4990,34 +5487,40 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "autoPay"))
 
     @auto_pay.setter
     def auto_pay(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosLoadBalancer, "auto_pay").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "autoPay", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="autoRenew")
     def auto_renew(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property: autoRenew: Indicates whether automatic renewal is enabled for the instance. Valid values:true: Automatic renewal is enabled.false: Automatic renewal is not enabled. You must renew the instance manually.Default value: false.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "autoRenew"))
 
     @auto_renew.setter
     def auto_renew(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosLoadBalancer, "auto_renew").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "autoRenew", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="autoRenewPeriod")
     def auto_renew_period(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -5028,51 +5531,60 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "autoRenewPeriod"))
 
     @auto_renew_period.setter
     def auto_renew_period(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosLoadBalancer, "auto_renew_period").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "autoRenewPeriod", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="bandwidth")
     def bandwidth(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: bandwidth: The bandwidth for network, unit in Mbps(Mega bit per second). Default is 1. If InternetChargeType is specified as "paybytraffic", this property will be ignore and please specify the "Bandwidth" in ALIYUN::SLB::Listener.
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "bandwidth"))
 
     @bandwidth.setter
     def bandwidth(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosLoadBalancer, "bandwidth").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "bandwidth", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="deletionProtection")
     def deletion_protection(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property: deletionProtection: Whether to enable deletion protection.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "deletionProtection"))
 
     @deletion_protection.setter
     def deletion_protection(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosLoadBalancer, "deletion_protection").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "deletionProtection", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="duration")
     def duration(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -5084,17 +5596,20 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "duration"))
 
     @duration.setter
     def duration(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosLoadBalancer, "duration").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "duration", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="instanceChargeType")
     def instance_charge_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -5105,85 +5620,100 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "instanceChargeType"))
 
     @instance_charge_type.setter
     def instance_charge_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosLoadBalancer, "instance_charge_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "instanceChargeType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="internetChargeType")
     def internet_charge_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: internetChargeType: Instance internet access charge type.Support 'paybybandwidth' and 'paybytraffic' only. Default is 'paybytraffic'. If load balancer is created in VPC, the charge type will be set as 'paybytraffic' by default.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "internetChargeType"))
 
     @internet_charge_type.setter
     def internet_charge_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosLoadBalancer, "internet_charge_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "internetChargeType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="loadBalancerName")
     def load_balancer_name(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: loadBalancerName: Name of created load balancer. Length is limited to 1-80 characters, allowed to contain letters, numbers, '-, /, _,.' When not specified, a default name will be assigned.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "loadBalancerName"))
 
     @load_balancer_name.setter
     def load_balancer_name(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosLoadBalancer, "load_balancer_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "loadBalancerName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="loadBalancerSpec")
     def load_balancer_spec(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: loadBalancerSpec: The specification of the Server Load Balancer instance. Allowed value: slb.s1.small|slb.s2.small|slb.s2.medium|slb.s3.small|slb.s3.medium|slb.s3.large|slb.s3.xlarge|slb.s3.xxlarge. Default value: slb.s1.small. The supported performance specification in each region is different, two specifications are supported in the US East 1 region. If the region does not support the performance-guaranteed instances, the value will not take effect.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "loadBalancerSpec"))
 
     @load_balancer_spec.setter
     def load_balancer_spec(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosLoadBalancer, "load_balancer_spec").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "loadBalancerSpec", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="masterZoneId")
     def master_zone_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: masterZoneId: The master zone id to create load balancer instance.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "masterZoneId"))
 
     @master_zone_id.setter
     def master_zone_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosLoadBalancer, "master_zone_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "masterZoneId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="modificationProtectionReason")
     def modification_protection_reason(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -5193,17 +5723,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "modificationProtectionReason"))
 
     @modification_protection_reason.setter
     def modification_protection_reason(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosLoadBalancer, "modification_protection_reason").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "modificationProtectionReason", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="modificationProtectionStatus")
     def modification_protection_status(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -5214,17 +5747,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "modificationProtectionStatus"))
 
     @modification_protection_status.setter
     def modification_protection_status(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosLoadBalancer, "modification_protection_status").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "modificationProtectionStatus", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="payType")
     def pay_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -5234,17 +5770,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "payType"))
 
     @pay_type.setter
     def pay_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosLoadBalancer, "pay_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "payType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="pricingCycle")
     def pricing_cycle(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -5254,97 +5793,115 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "pricingCycle"))
 
     @pricing_cycle.setter
     def pricing_cycle(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosLoadBalancer, "pricing_cycle").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "pricingCycle", value)
 
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
+            type_hints = typing.get_type_hints(getattr(RosLoadBalancer, "resource_group_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "resourceGroupId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="slaveZoneId")
     def slave_zone_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: slaveZoneId: The slave zone id to create load balancer instance.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "slaveZoneId"))
 
     @slave_zone_id.setter
     def slave_zone_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosLoadBalancer, "slave_zone_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "slaveZoneId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="tags")
     def tags(self) -> typing.Optional[typing.List["RosLoadBalancer.TagsProperty"]]:
         '''
         :Property: tags: Tags to attach to slb. Max support 5 tags to add during create slb. Each tag with two properties Key and Value, and Key is required.
         '''
         return typing.cast(typing.Optional[typing.List["RosLoadBalancer.TagsProperty"]], jsii.get(self, "tags"))
 
     @tags.setter
     def tags(
         self,
         value: typing.Optional[typing.List["RosLoadBalancer.TagsProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosLoadBalancer, "tags").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "tags", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vpcId")
     def vpc_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: vpcId: The VPC id to create load balancer instance. For VPC network only.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "vpcId"))
 
     @vpc_id.setter
     def vpc_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosLoadBalancer, "vpc_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "vpcId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vSwitchId")
     def v_switch_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: vSwitchId: The VSwitch id to create load balancer instance. For VPC network only.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "vSwitchId"))
 
     @v_switch_id.setter
     def v_switch_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosLoadBalancer, "v_switch_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "vSwitchId", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-slb.RosLoadBalancer.TagsProperty",
         jsii_struct_bases=[],
         name_mapping={"key": "key", "value": "value"},
     )
@@ -5355,14 +5912,18 @@
             key: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param key: 
             :param value: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosLoadBalancer.TagsProperty.__init__)
+                check_type(argname="argument key", value=key, expected_type=type_hints["key"])
+                check_type(argname="argument value", value=value, expected_type=type_hints["value"])
             self._values: typing.Dict[str, typing.Any] = {
                 "key": key,
             }
             if value is not None:
                 self._values["value"] = value
 
         @builtins.property
@@ -5403,116 +5964,137 @@
 ):
     '''A ROS template type:  ``ALIYUN::SLB::LoadBalancerClone``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosLoadBalancerCloneProps",
+        props: typing.Union["RosLoadBalancerCloneProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::SLB::LoadBalancerClone``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosLoadBalancerClone.__init__)
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
+            type_hints = typing.get_type_hints(RosLoadBalancerClone._render_properties)
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
     @jsii.member(jsii_name="attrLoadBalancerId")
     def attr_load_balancer_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: LoadBalancerId: The id of load balance generated
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrLoadBalancerId"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosLoadBalancerClone, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="sourceLoadBalancerId")
     def source_load_balancer_id(
         self,
     ) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: sourceLoadBalancerId: Source load balancer id to clone
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "sourceLoadBalancerId"))
 
     @source_load_balancer_id.setter
     def source_load_balancer_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosLoadBalancerClone, "source_load_balancer_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "sourceLoadBalancerId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="backendServers")
     def backend_servers(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosLoadBalancerClone.BackendServersProperty"]]]]:
         '''
         :Property: backendServers: The list of ECS instance, which will attached to load balancer.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosLoadBalancerClone.BackendServersProperty"]]]], jsii.get(self, "backendServers"))
 
     @backend_servers.setter
     def backend_servers(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosLoadBalancerClone.BackendServersProperty"]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosLoadBalancerClone, "backend_servers").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "backendServers", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="backendServersPolicy")
     def backend_servers_policy(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: backendServersPolicy: Solution for handle the backend server and weights. If select 'clone', it will clone from source load balancer. If select 'empty' it will not attach any backend servers. If select 'append' it will append the new backend server list to source backed servers. If select 'replace' it will only attach new backend server list. Default is 'clone'.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "backendServersPolicy"))
 
     @backend_servers_policy.setter
     def backend_servers_policy(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosLoadBalancerClone, "backend_servers_policy").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "backendServersPolicy", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="instanceChargeType")
     def instance_charge_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -5523,34 +6105,40 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "instanceChargeType"))
 
     @instance_charge_type.setter
     def instance_charge_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosLoadBalancerClone, "instance_charge_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "instanceChargeType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="loadBalancerName")
     def load_balancer_name(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: loadBalancerName: Name of created load balancer. Length is limited to 1-80 characters, allowed to contain letters, numbers, '-, /, _,.' When not specified, a default name will be assigned.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "loadBalancerName"))
 
     @load_balancer_name.setter
     def load_balancer_name(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosLoadBalancerClone, "load_balancer_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "loadBalancerName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="loadBalancerSpec")
     def load_balancer_spec(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -5560,49 +6148,58 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "loadBalancerSpec"))
 
     @load_balancer_spec.setter
     def load_balancer_spec(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosLoadBalancerClone, "load_balancer_spec").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "loadBalancerSpec", value)
 
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
+            type_hints = typing.get_type_hints(getattr(RosLoadBalancerClone, "resource_group_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "resourceGroupId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="tags")
     def tags(self) -> typing.Optional[typing.List["RosLoadBalancerClone.TagsProperty"]]:
         '''
         :Property: tags: Tags to attach to slb. Max support 5 tags to add during create slb. Each tag with two properties Key and Value, and Key is required.
         '''
         return typing.cast(typing.Optional[typing.List["RosLoadBalancerClone.TagsProperty"]], jsii.get(self, "tags"))
 
     @tags.setter
     def tags(
         self,
         value: typing.Optional[typing.List["RosLoadBalancerClone.TagsProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosLoadBalancerClone, "tags").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "tags", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="tagsPolicy")
     def tags_policy(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -5612,31 +6209,37 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "tagsPolicy"))
 
     @tags_policy.setter
     def tags_policy(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosLoadBalancerClone, "tags_policy").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "tagsPolicy", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vSwitchId")
     def v_switch_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: vSwitchId: The new VSwitch ID to create load balancer instance. For VPC network only and the VSwitch should belong to the VPC which source load balancer is located.When not specified, source load balancer VSwitch ID will be used.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "vSwitchId"))
 
     @v_switch_id.setter
     def v_switch_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosLoadBalancerClone, "v_switch_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "vSwitchId", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-slb.RosLoadBalancerClone.BackendServersProperty",
         jsii_struct_bases=[],
         name_mapping={
             "server_id": "serverId",
@@ -5659,14 +6262,21 @@
             '''
             :param server_id: 
             :param weight: 
             :param description: 
             :param server_ip: 
             :param type: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosLoadBalancerClone.BackendServersProperty.__init__)
+                check_type(argname="argument server_id", value=server_id, expected_type=type_hints["server_id"])
+                check_type(argname="argument weight", value=weight, expected_type=type_hints["weight"])
+                check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+                check_type(argname="argument server_ip", value=server_ip, expected_type=type_hints["server_ip"])
+                check_type(argname="argument type", value=type, expected_type=type_hints["type"])
             self._values: typing.Dict[str, typing.Any] = {
                 "server_id": server_id,
                 "weight": weight,
             }
             if description is not None:
                 self._values["description"] = description
             if server_ip is not None:
@@ -5745,14 +6355,18 @@
             key: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param key: 
             :param value: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosLoadBalancerClone.TagsProperty.__init__)
+                check_type(argname="argument key", value=key, expected_type=type_hints["key"])
+                check_type(argname="argument value", value=value, expected_type=type_hints["value"])
             self._values: typing.Dict[str, typing.Any] = {
                 "key": key,
             }
             if value is not None:
                 self._values["value"] = value
 
         @builtins.property
@@ -5803,21 +6417,21 @@
     },
 )
 class RosLoadBalancerCloneProps:
     def __init__(
         self,
         *,
         source_load_balancer_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
-        backend_servers: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosLoadBalancerClone.BackendServersProperty]]]] = None,
+        backend_servers: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosLoadBalancerClone.BackendServersProperty, typing.Dict[str, typing.Any]]]]]] = None,
         backend_servers_policy: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         instance_charge_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         load_balancer_name: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         load_balancer_spec: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         resource_group_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        tags: typing.Optional[typing.Sequence[RosLoadBalancerClone.TagsProperty]] = None,
+        tags: typing.Optional[typing.Sequence[typing.Union[RosLoadBalancerClone.TagsProperty, typing.Dict[str, typing.Any]]]] = None,
         tags_policy: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         v_switch_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::SLB::LoadBalancerClone``.
 
         :param source_load_balancer_id: 
         :param backend_servers: 
@@ -5826,14 +6440,26 @@
         :param load_balancer_name: 
         :param load_balancer_spec: 
         :param resource_group_id: 
         :param tags: 
         :param tags_policy: 
         :param v_switch_id: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosLoadBalancerCloneProps.__init__)
+            check_type(argname="argument source_load_balancer_id", value=source_load_balancer_id, expected_type=type_hints["source_load_balancer_id"])
+            check_type(argname="argument backend_servers", value=backend_servers, expected_type=type_hints["backend_servers"])
+            check_type(argname="argument backend_servers_policy", value=backend_servers_policy, expected_type=type_hints["backend_servers_policy"])
+            check_type(argname="argument instance_charge_type", value=instance_charge_type, expected_type=type_hints["instance_charge_type"])
+            check_type(argname="argument load_balancer_name", value=load_balancer_name, expected_type=type_hints["load_balancer_name"])
+            check_type(argname="argument load_balancer_spec", value=load_balancer_spec, expected_type=type_hints["load_balancer_spec"])
+            check_type(argname="argument resource_group_id", value=resource_group_id, expected_type=type_hints["resource_group_id"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
+            check_type(argname="argument tags_policy", value=tags_policy, expected_type=type_hints["tags_policy"])
+            check_type(argname="argument v_switch_id", value=v_switch_id, expected_type=type_hints["v_switch_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "source_load_balancer_id": source_load_balancer_id,
         }
         if backend_servers is not None:
             self._values["backend_servers"] = backend_servers
         if backend_servers_policy is not None:
             self._values["backend_servers_policy"] = backend_servers_policy
@@ -6020,15 +6646,15 @@
         master_zone_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         modification_protection_reason: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         modification_protection_status: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         pay_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         pricing_cycle: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         resource_group_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         slave_zone_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        tags: typing.Optional[typing.Sequence[RosLoadBalancer.TagsProperty]] = None,
+        tags: typing.Optional[typing.Sequence[typing.Union[RosLoadBalancer.TagsProperty, typing.Dict[str, typing.Any]]]] = None,
         vpc_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         v_switch_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::SLB::LoadBalancer``.
 
         :param address_ip_version: 
         :param address_type: 
@@ -6049,14 +6675,38 @@
         :param pricing_cycle: 
         :param resource_group_id: 
         :param slave_zone_id: 
         :param tags: 
         :param vpc_id: 
         :param v_switch_id: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosLoadBalancerProps.__init__)
+            check_type(argname="argument address_ip_version", value=address_ip_version, expected_type=type_hints["address_ip_version"])
+            check_type(argname="argument address_type", value=address_type, expected_type=type_hints["address_type"])
+            check_type(argname="argument auto_pay", value=auto_pay, expected_type=type_hints["auto_pay"])
+            check_type(argname="argument auto_renew", value=auto_renew, expected_type=type_hints["auto_renew"])
+            check_type(argname="argument auto_renew_period", value=auto_renew_period, expected_type=type_hints["auto_renew_period"])
+            check_type(argname="argument bandwidth", value=bandwidth, expected_type=type_hints["bandwidth"])
+            check_type(argname="argument deletion_protection", value=deletion_protection, expected_type=type_hints["deletion_protection"])
+            check_type(argname="argument duration", value=duration, expected_type=type_hints["duration"])
+            check_type(argname="argument instance_charge_type", value=instance_charge_type, expected_type=type_hints["instance_charge_type"])
+            check_type(argname="argument internet_charge_type", value=internet_charge_type, expected_type=type_hints["internet_charge_type"])
+            check_type(argname="argument load_balancer_name", value=load_balancer_name, expected_type=type_hints["load_balancer_name"])
+            check_type(argname="argument load_balancer_spec", value=load_balancer_spec, expected_type=type_hints["load_balancer_spec"])
+            check_type(argname="argument master_zone_id", value=master_zone_id, expected_type=type_hints["master_zone_id"])
+            check_type(argname="argument modification_protection_reason", value=modification_protection_reason, expected_type=type_hints["modification_protection_reason"])
+            check_type(argname="argument modification_protection_status", value=modification_protection_status, expected_type=type_hints["modification_protection_status"])
+            check_type(argname="argument pay_type", value=pay_type, expected_type=type_hints["pay_type"])
+            check_type(argname="argument pricing_cycle", value=pricing_cycle, expected_type=type_hints["pricing_cycle"])
+            check_type(argname="argument resource_group_id", value=resource_group_id, expected_type=type_hints["resource_group_id"])
+            check_type(argname="argument slave_zone_id", value=slave_zone_id, expected_type=type_hints["slave_zone_id"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
+            check_type(argname="argument vpc_id", value=vpc_id, expected_type=type_hints["vpc_id"])
+            check_type(argname="argument v_switch_id", value=v_switch_id, expected_type=type_hints["v_switch_id"])
         self._values: typing.Dict[str, typing.Any] = {}
         if address_ip_version is not None:
             self._values["address_ip_version"] = address_ip_version
         if address_type is not None:
             self._values["address_type"] = address_type
         if auto_pay is not None:
             self._values["auto_pay"] = auto_pay
@@ -6365,80 +7015,95 @@
 ):
     '''A ROS template type:  ``ALIYUN::SLB::MasterSlaveServerGroup``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosMasterSlaveServerGroupProps",
+        props: typing.Union["RosMasterSlaveServerGroupProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::SLB::MasterSlaveServerGroup``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosMasterSlaveServerGroup.__init__)
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
+            type_hints = typing.get_type_hints(RosMasterSlaveServerGroup._render_properties)
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
     @jsii.member(jsii_name="attrMasterSlaveServerGroupId")
     def attr_master_slave_server_group_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: MasterSlaveServerGroupId: Active/standby server group ID.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrMasterSlaveServerGroupId"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosMasterSlaveServerGroup, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="loadBalancerId")
     def load_balancer_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: loadBalancerId: The ID of the Server Load Balancer instance.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "loadBalancerId"))
 
     @load_balancer_id.setter
     def load_balancer_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosMasterSlaveServerGroup, "load_balancer_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "loadBalancerId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="masterSlaveBackendServers")
     def master_slave_backend_servers(
         self,
     ) -> typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosMasterSlaveServerGroup.MasterSlaveBackendServersProperty"]]]:
         '''
         :Property:
 
@@ -6448,31 +7113,37 @@
         return typing.cast(typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosMasterSlaveServerGroup.MasterSlaveBackendServersProperty"]]], jsii.get(self, "masterSlaveBackendServers"))
 
     @master_slave_backend_servers.setter
     def master_slave_backend_servers(
         self,
         value: typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosMasterSlaveServerGroup.MasterSlaveBackendServersProperty"]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosMasterSlaveServerGroup, "master_slave_backend_servers").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "masterSlaveBackendServers", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="masterSlaveServerGroupName")
     def master_slave_server_group_name(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: masterSlaveServerGroupName: The name of the active/standby server group.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "masterSlaveServerGroupName"))
 
     @master_slave_server_group_name.setter
     def master_slave_server_group_name(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosMasterSlaveServerGroup, "master_slave_server_group_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "masterSlaveServerGroupName", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-slb.RosMasterSlaveServerGroup.MasterSlaveBackendServersProperty",
         jsii_struct_bases=[],
         name_mapping={
             "port": "port",
@@ -6492,14 +7163,20 @@
         ) -> None:
             '''
             :param port: 
             :param server_id: 
             :param weight: 
             :param server_type: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosMasterSlaveServerGroup.MasterSlaveBackendServersProperty.__init__)
+                check_type(argname="argument port", value=port, expected_type=type_hints["port"])
+                check_type(argname="argument server_id", value=server_id, expected_type=type_hints["server_id"])
+                check_type(argname="argument weight", value=weight, expected_type=type_hints["weight"])
+                check_type(argname="argument server_type", value=server_type, expected_type=type_hints["server_type"])
             self._values: typing.Dict[str, typing.Any] = {
                 "port": port,
                 "server_id": server_id,
                 "weight": weight,
             }
             if server_type is not None:
                 self._values["server_type"] = server_type
@@ -6563,23 +7240,28 @@
     },
 )
 class RosMasterSlaveServerGroupProps:
     def __init__(
         self,
         *,
         load_balancer_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
-        master_slave_backend_servers: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosMasterSlaveServerGroup.MasterSlaveBackendServersProperty]]],
+        master_slave_backend_servers: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosMasterSlaveServerGroup.MasterSlaveBackendServersProperty, typing.Dict[str, typing.Any]]]]],
         master_slave_server_group_name: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::SLB::MasterSlaveServerGroup``.
 
         :param load_balancer_id: 
         :param master_slave_backend_servers: 
         :param master_slave_server_group_name: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosMasterSlaveServerGroupProps.__init__)
+            check_type(argname="argument load_balancer_id", value=load_balancer_id, expected_type=type_hints["load_balancer_id"])
+            check_type(argname="argument master_slave_backend_servers", value=master_slave_backend_servers, expected_type=type_hints["master_slave_backend_servers"])
+            check_type(argname="argument master_slave_server_group_name", value=master_slave_server_group_name, expected_type=type_hints["master_slave_server_group_name"])
         self._values: typing.Dict[str, typing.Any] = {
             "load_balancer_id": load_balancer_id,
             "master_slave_backend_servers": master_slave_backend_servers,
         }
         if master_slave_server_group_name is not None:
             self._values["master_slave_server_group_name"] = master_slave_server_group_name
 
@@ -6635,65 +7317,77 @@
 ):
     '''A ROS template type:  ``ALIYUN::SLB::Rule``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosRuleProps",
+        props: typing.Union["RosRuleProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::SLB::Rule``.
 
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
     @jsii.member(jsii_name="attrRules")
     def attr_rules(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Rules: A list of forwarding rules. Each element of rules contains "RuleId".
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrRules"))
 
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
     @jsii.member(jsii_name="listenerPort")
     def listener_port(self) -> typing.Union[jsii.Number, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         listenerPort: The front-end HTTPS listener port of the Server Load Balancer instance. Valid value:
         1-65535
@@ -6701,46 +7395,55 @@
         return typing.cast(typing.Union[jsii.Number, ros_cdk_core.IResolvable], jsii.get(self, "listenerPort"))
 
     @listener_port.setter
     def listener_port(
         self,
         value: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosRule, "listener_port").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "listenerPort", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="loadBalancerId")
     def load_balancer_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: loadBalancerId: The ID of Server Load Balancer instance.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "loadBalancerId"))
 
     @load_balancer_id.setter
     def load_balancer_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosRule, "load_balancer_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "loadBalancerId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="ruleList")
     def rule_list(
         self,
     ) -> typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosRule.RuleListProperty"]]]:
         '''
         :Property: ruleList: The forwarding rules to add.
         '''
         return typing.cast(typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosRule.RuleListProperty"]]], jsii.get(self, "ruleList"))
 
     @rule_list.setter
     def rule_list(
         self,
         value: typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosRule.RuleListProperty"]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosRule, "rule_list").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "ruleList", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-slb.RosRule.RuleListProperty",
         jsii_struct_bases=[],
         name_mapping={
             "rule_name": "ruleName",
@@ -6760,14 +7463,20 @@
         ) -> None:
             '''
             :param rule_name: 
             :param v_server_group_id: 
             :param domain: 
             :param url: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosRule.RuleListProperty.__init__)
+                check_type(argname="argument rule_name", value=rule_name, expected_type=type_hints["rule_name"])
+                check_type(argname="argument v_server_group_id", value=v_server_group_id, expected_type=type_hints["v_server_group_id"])
+                check_type(argname="argument domain", value=domain, expected_type=type_hints["domain"])
+                check_type(argname="argument url", value=url, expected_type=type_hints["url"])
             self._values: typing.Dict[str, typing.Any] = {
                 "rule_name": rule_name,
                 "v_server_group_id": v_server_group_id,
             }
             if domain is not None:
                 self._values["domain"] = domain
             if url is not None:
@@ -6836,22 +7545,27 @@
 )
 class RosRuleProps:
     def __init__(
         self,
         *,
         listener_port: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
         load_balancer_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
-        rule_list: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosRule.RuleListProperty]]],
+        rule_list: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosRule.RuleListProperty, typing.Dict[str, typing.Any]]]]],
     ) -> None:
         '''Properties for defining a ``ALIYUN::SLB::Rule``.
 
         :param listener_port: 
         :param load_balancer_id: 
         :param rule_list: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosRuleProps.__init__)
+            check_type(argname="argument listener_port", value=listener_port, expected_type=type_hints["listener_port"])
+            check_type(argname="argument load_balancer_id", value=load_balancer_id, expected_type=type_hints["load_balancer_id"])
+            check_type(argname="argument rule_list", value=rule_list, expected_type=type_hints["rule_list"])
         self._values: typing.Dict[str, typing.Any] = {
             "listener_port": listener_port,
             "load_balancer_id": load_balancer_id,
             "rule_list": rule_list,
         }
 
     @builtins.property
@@ -6905,119 +7619,140 @@
 ):
     '''A ROS template type:  ``ALIYUN::SLB::VServerGroup``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosVServerGroupProps",
+        props: typing.Union["RosVServerGroupProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::SLB::VServerGroup``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosVServerGroup.__init__)
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
+            type_hints = typing.get_type_hints(RosVServerGroup._render_properties)
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
     @jsii.member(jsii_name="attrBackendServers")
     def attr_backend_servers(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: BackendServers: Backend server list in this VServerGroup.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrBackendServers"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVServerGroupId")
     def attr_v_server_group_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: VServerGroupId: The id of VServerGroup created.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVServerGroupId"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosVServerGroup, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="loadBalancerId")
     def load_balancer_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: loadBalancerId: The id of load balancer.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "loadBalancerId"))
 
     @load_balancer_id.setter
     def load_balancer_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosVServerGroup, "load_balancer_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "loadBalancerId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vServerGroupName")
     def v_server_group_name(
         self,
     ) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: vServerGroupName: Display name of the VServerGroup.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "vServerGroupName"))
 
     @v_server_group_name.setter
     def v_server_group_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosVServerGroup, "v_server_group_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "vServerGroupName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="backendServers")
     def backend_servers(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosVServerGroup.BackendServersProperty"]]]]:
         '''
         :Property: backendServers: The list of a combination of ECS Instance-Port-Weight.Same ecs instance with different port is allowed, but same ecs instance with same port isn't.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosVServerGroup.BackendServersProperty"]]]], jsii.get(self, "backendServers"))
 
     @backend_servers.setter
     def backend_servers(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosVServerGroup.BackendServersProperty"]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosVServerGroup, "backend_servers").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "backendServers", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-slb.RosVServerGroup.BackendServersProperty",
         jsii_struct_bases=[],
         name_mapping={
             "port": "port",
@@ -7043,14 +7778,22 @@
             :param port: 
             :param server_id: 
             :param description: 
             :param server_ip: 
             :param type: 
             :param weight: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosVServerGroup.BackendServersProperty.__init__)
+                check_type(argname="argument port", value=port, expected_type=type_hints["port"])
+                check_type(argname="argument server_id", value=server_id, expected_type=type_hints["server_id"])
+                check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+                check_type(argname="argument server_ip", value=server_ip, expected_type=type_hints["server_ip"])
+                check_type(argname="argument type", value=type, expected_type=type_hints["type"])
+                check_type(argname="argument weight", value=weight, expected_type=type_hints["weight"])
             self._values: typing.Dict[str, typing.Any] = {
                 "port": port,
                 "server_id": server_id,
             }
             if description is not None:
                 self._values["description"] = description
             if server_ip is not None:
@@ -7146,22 +7889,27 @@
 )
 class RosVServerGroupProps:
     def __init__(
         self,
         *,
         load_balancer_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         v_server_group_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
-        backend_servers: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosVServerGroup.BackendServersProperty]]]] = None,
+        backend_servers: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosVServerGroup.BackendServersProperty, typing.Dict[str, typing.Any]]]]]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::SLB::VServerGroup``.
 
         :param load_balancer_id: 
         :param v_server_group_name: 
         :param backend_servers: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosVServerGroupProps.__init__)
+            check_type(argname="argument load_balancer_id", value=load_balancer_id, expected_type=type_hints["load_balancer_id"])
+            check_type(argname="argument v_server_group_name", value=v_server_group_name, expected_type=type_hints["v_server_group_name"])
+            check_type(argname="argument backend_servers", value=backend_servers, expected_type=type_hints["backend_servers"])
         self._values: typing.Dict[str, typing.Any] = {
             "load_balancer_id": load_balancer_id,
             "v_server_group_name": v_server_group_name,
         }
         if backend_servers is not None:
             self._values["backend_servers"] = backend_servers
 
@@ -7214,31 +7962,37 @@
 ):
     '''A ROS resource type:  ``ALIYUN::SLB::Rule``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RuleProps",
+        props: typing.Union["RuleProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::SLB::Rule``.
 
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
     @jsii.member(jsii_name="attrRules")
     def attr_rules(self) -> ros_cdk_core.IResolvable:
         '''Attribute Rules: A list of forwarding rules.
 
         Each element of rules contains "RuleId".
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrRules"))
@@ -7255,22 +8009,27 @@
 )
 class RuleProps:
     def __init__(
         self,
         *,
         listener_port: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
         load_balancer_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
-        rule_list: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosRule.RuleListProperty]]],
+        rule_list: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosRule.RuleListProperty, typing.Dict[str, typing.Any]]]]],
     ) -> None:
         '''Properties for defining a ``ALIYUN::SLB::Rule``.
 
         :param listener_port: Property listenerPort: The front-end HTTPS listener port of the Server Load Balancer instance. Valid value: 1-65535
         :param load_balancer_id: Property loadBalancerId: The ID of Server Load Balancer instance.
         :param rule_list: Property ruleList: The forwarding rules to add.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RuleProps.__init__)
+            check_type(argname="argument listener_port", value=listener_port, expected_type=type_hints["listener_port"])
+            check_type(argname="argument load_balancer_id", value=load_balancer_id, expected_type=type_hints["load_balancer_id"])
+            check_type(argname="argument rule_list", value=rule_list, expected_type=type_hints["rule_list"])
         self._values: typing.Dict[str, typing.Any] = {
             "listener_port": listener_port,
             "load_balancer_id": load_balancer_id,
             "rule_list": rule_list,
         }
 
     @builtins.property
@@ -7319,37 +8078,43 @@
 ):
     '''A ROS resource type:  ``ALIYUN::SLB::VServerGroup``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "VServerGroupProps",
+        props: typing.Union["VServerGroupProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::SLB::VServerGroup``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(VServerGroup.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrBackendServers")
     def attr_backend_servers(self) -> ros_cdk_core.IResolvable:
         '''Attribute BackendServers: Backend server list in this VServerGroup.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrBackendServers"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVServerGroupId")
     def attr_v_server_group_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute VServerGroupId: The id of VServerGroup created.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVServerGroupId"))
 
 
 @jsii.data_type(
@@ -7363,22 +8128,27 @@
 )
 class VServerGroupProps:
     def __init__(
         self,
         *,
         load_balancer_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         v_server_group_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
-        backend_servers: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosVServerGroup.BackendServersProperty]]]] = None,
+        backend_servers: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosVServerGroup.BackendServersProperty, typing.Dict[str, typing.Any]]]]]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::SLB::VServerGroup``.
 
         :param load_balancer_id: Property loadBalancerId: The id of load balancer.
         :param v_server_group_name: Property vServerGroupName: Display name of the VServerGroup.
         :param backend_servers: Property backendServers: The list of a combination of ECS Instance-Port-Weight.Same ecs instance with different port is allowed, but same ecs instance with same port isn't.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(VServerGroupProps.__init__)
+            check_type(argname="argument load_balancer_id", value=load_balancer_id, expected_type=type_hints["load_balancer_id"])
+            check_type(argname="argument v_server_group_name", value=v_server_group_name, expected_type=type_hints["v_server_group_name"])
+            check_type(argname="argument backend_servers", value=backend_servers, expected_type=type_hints["backend_servers"])
         self._values: typing.Dict[str, typing.Any] = {
             "load_balancer_id": load_balancer_id,
             "v_server_group_name": v_server_group_name,
         }
         if backend_servers is not None:
             self._values["backend_servers"] = backend_servers
```

### Comparing `ros-cdk-slb-1.0.8/src/ros_cdk_slb.egg-info/PKG-INFO` & `ros-cdk-slb-1.0.9/src/ros_cdk_slb.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-slb
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS SLB Construct Library
```

