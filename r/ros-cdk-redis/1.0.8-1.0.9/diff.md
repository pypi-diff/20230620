# Comparing `tmp/ros-cdk-redis-1.0.8.tar.gz` & `tmp/ros-cdk-redis-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-redis-1.0.8.tar", last modified: Thu Jul 14 02:42:10 2022, max compression
+gzip compressed data, was "dist/ros-cdk-redis-1.0.9.tar", last modified: Fri Sep 23 11:30:57 2022, max compression
```

## Comparing `ros-cdk-redis-1.0.8.tar` & `ros-cdk-redis-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:42:10.000000 ros-cdk-redis-1.0.8/
--rw-r--r--   0 root         (0) root         (0)    10279 2022-07-14 02:42:10.000000 ros-cdk-redis-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2022-07-14 02:42:10.000000 ros-cdk-redis-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2022-07-14 02:42:10.000000 ros-cdk-redis-1.0.8/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1248 2022-07-14 02:42:10.000000 ros-cdk-redis-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      185 2022-07-14 02:42:10.000000 ros-cdk-redis-1.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)      106 2022-07-14 02:42:10.000000 ros-cdk-redis-1.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-07-14 02:42:10.000000 ros-cdk-redis-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1806 2022-07-14 02:42:10.000000 ros-cdk-redis-1.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:42:10.000000 ros-cdk-redis-1.0.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:42:10.000000 ros-cdk-redis-1.0.8/src/ros_cdk_redis/
--rw-r--r--   0 root         (0) root         (0)   234506 2022-07-14 02:42:10.000000 ros-cdk-redis-1.0.8/src/ros_cdk_redis/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:42:10.000000 ros-cdk-redis-1.0.8/src/ros_cdk_redis/_jsii/
--rw-r--r--   0 root         (0) root         (0)      374 2022-07-14 02:42:10.000000 ros-cdk-redis-1.0.8/src/ros_cdk_redis/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    96810 2022-07-14 02:42:10.000000 ros-cdk-redis-1.0.8/src/ros_cdk_redis/_jsii/ros-cdk-redis@1.0.8.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:42:10.000000 ros-cdk-redis-1.0.8/src/ros_cdk_redis/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:42:10.000000 ros-cdk-redis-1.0.8/src/ros_cdk_redis.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1248 2022-07-14 02:42:10.000000 ros-cdk-redis-1.0.8/src/ros_cdk_redis.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      420 2022-07-14 02:42:10.000000 ros-cdk-redis-1.0.8/src/ros_cdk_redis.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:42:10.000000 ros-cdk-redis-1.0.8/src/ros_cdk_redis.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2022-07-14 02:42:10.000000 ros-cdk-redis-1.0.8/src/ros_cdk_redis.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2022-07-14 02:42:10.000000 ros-cdk-redis-1.0.8/src/ros_cdk_redis.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:30:57.000000 ros-cdk-redis-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)    10279 2022-09-23 11:30:56.000000 ros-cdk-redis-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-09-23 11:30:56.000000 ros-cdk-redis-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2022-09-23 11:30:56.000000 ros-cdk-redis-1.0.9/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1248 2022-09-23 11:30:57.000000 ros-cdk-redis-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      185 2022-09-23 11:30:56.000000 ros-cdk-redis-1.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      236 2022-09-23 11:30:56.000000 ros-cdk-redis-1.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-09-23 11:30:57.000000 ros-cdk-redis-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1835 2022-09-23 11:30:56.000000 ros-cdk-redis-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:30:57.000000 ros-cdk-redis-1.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:30:57.000000 ros-cdk-redis-1.0.9/src/ros_cdk_redis/
+-rw-r--r--   0 root         (0) root         (0)   275852 2022-09-23 11:30:56.000000 ros-cdk-redis-1.0.9/src/ros_cdk_redis/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:30:57.000000 ros-cdk-redis-1.0.9/src/ros_cdk_redis/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      408 2022-09-23 11:30:56.000000 ros-cdk-redis-1.0.9/src/ros_cdk_redis/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    99418 2022-09-23 11:30:56.000000 ros-cdk-redis-1.0.9/src/ros_cdk_redis/_jsii/ros-cdk-redis@1.0.9.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 11:30:56.000000 ros-cdk-redis-1.0.9/src/ros_cdk_redis/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:30:57.000000 ros-cdk-redis-1.0.9/src/ros_cdk_redis.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1248 2022-09-23 11:30:56.000000 ros-cdk-redis-1.0.9/src/ros_cdk_redis.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      420 2022-09-23 11:30:56.000000 ros-cdk-redis-1.0.9/src/ros_cdk_redis.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 11:30:56.000000 ros-cdk-redis-1.0.9/src/ros_cdk_redis.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2022-09-23 11:30:56.000000 ros-cdk-redis-1.0.9/src/ros_cdk_redis.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2022-09-23 11:30:56.000000 ros-cdk-redis-1.0.9/src/ros_cdk_redis.egg-info/top_level.txt
```

### Comparing `ros-cdk-redis-1.0.8/LICENSE` & `ros-cdk-redis-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-redis-1.0.8/PKG-INFO` & `ros-cdk-redis-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-redis
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS REDIS Construct Library
```

### Comparing `ros-cdk-redis-1.0.8/setup.py` & `ros-cdk-redis-1.0.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-redis",
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
         "ros_cdk_redis",
         "ros_cdk_redis._jsii"
     ],
     "package_data": {
         "ros_cdk_redis._jsii": [
-            "ros-cdk-redis@1.0.8.jsii.tgz"
+            "ros-cdk-redis@1.0.9.jsii.tgz"
         ],
         "ros_cdk_redis": [
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

### Comparing `ros-cdk-redis-1.0.8/src/ros_cdk_redis/__init__.py` & `ros-cdk-redis-1.0.9/src/ros_cdk_redis/__init__.py`

 * *Files 8% similar despite different names*

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
 
 
 class Account(
     ros_cdk_core.Resource,
@@ -29,37 +31,43 @@
 ):
     '''A ROS resource type:  ``ALIYUN::REDIS::Account``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "AccountProps",
+        props: typing.Union["AccountProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::REDIS::Account``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(Account.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrAccountName")
     def attr_account_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute AccountName: The name of the account.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAccountName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInstanceId")
     def attr_instance_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute InstanceId: The name of the instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInstanceId"))
 
 
 @jsii.data_type(
@@ -90,14 +98,22 @@
         :param account_name: Property accountName: The name of the account. The name must start with a lowercase letter and can contain lowercase letters, digits, and underscores (_). The name can be 1 to 16 characters in length.
         :param account_password: Property accountPassword: The password of the account. The password can be 8 to 32 characters in length and must contain at least three types of the following characters: uppercase letters, lowercase letters, digits, and special characters. Special characters include ! at signs (@), number signs (#), dollar signs ($), percent signs (%), carets (^), ampersands (&), asterisks (*), parentheses (()), underscores (_), plus signs (+), hyphens (-), and equal signs (=).
         :param instance_id: Property instanceId: The ID of the instance for which you want to create the account.
         :param account_description: Property accountDescription: The description of the account. The description must start with a letter, and cannot start with http:// or https://. The description can contain letters, underscores (_), hyphens (-), and digits. It can be 2 to 256 characters in length.
         :param account_privilege: Property accountPrivilege: The permission of the account. Valid values: RoleReadOnly RoleReadWrite (default value) RoleRepl Note In addition to reading data from and writing data to the ApsaraDB for Redis instance, an account with the RoleRepl permission can run the SYNC and PSYNC commands. The RoleRepl permission can be granted to an account only in an ApsaraDB for Redis instance of the standard edition in Redis 4.0.
         :param account_type: Property accountType: The type of the account. Set this parameter to Normal.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(AccountProps.__init__)
+            check_type(argname="argument account_name", value=account_name, expected_type=type_hints["account_name"])
+            check_type(argname="argument account_password", value=account_password, expected_type=type_hints["account_password"])
+            check_type(argname="argument instance_id", value=instance_id, expected_type=type_hints["instance_id"])
+            check_type(argname="argument account_description", value=account_description, expected_type=type_hints["account_description"])
+            check_type(argname="argument account_privilege", value=account_privilege, expected_type=type_hints["account_privilege"])
+            check_type(argname="argument account_type", value=account_type, expected_type=type_hints["account_type"])
         self._values: typing.Dict[str, typing.Any] = {
             "account_name": account_name,
             "account_password": account_password,
             "instance_id": instance_id,
         }
         if account_description is not None:
             self._values["account_description"] = account_description
@@ -200,217 +216,223 @@
 ):
     '''A ROS resource type:  ``ALIYUN::REDIS::Instance``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: typing.Optional["InstanceProps"] = None,
+        props: typing.Optional[typing.Union["InstanceProps", typing.Dict[str, typing.Any]]] = None,
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::REDIS::Instance``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(Instance.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrArchitectureType")
     def attr_architecture_type(self) -> ros_cdk_core.IResolvable:
         '''Attribute ArchitectureType: The architecture.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrArchitectureType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrBandwidth")
     def attr_bandwidth(self) -> ros_cdk_core.IResolvable:
         '''Attribute Bandwidth: The bandwidth of the instance.
 
         Unit: Mbit/s.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrBandwidth"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrCapacity")
     def attr_capacity(self) -> ros_cdk_core.IResolvable:
         '''Attribute Capacity: The storage capacity of the instance.
 
         Unit: MB.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrCapacity"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrChargeType")
     def attr_charge_type(self) -> ros_cdk_core.IResolvable:
         '''Attribute ChargeType: The billing method of the instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrChargeType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrClassicInnerConnectionPort")
     def attr_classic_inner_connection_port(self) -> ros_cdk_core.IResolvable:
         '''Attribute ClassicInnerConnectionPort: The classic inner connection port of the instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrClassicInnerConnectionPort"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrClassicInnerConnectionString")
     def attr_classic_inner_connection_string(self) -> ros_cdk_core.IResolvable:
         '''Attribute ClassicInnerConnectionString: The classic inner connection string of the instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrClassicInnerConnectionString"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrConnectionDomain")
     def attr_connection_domain(self) -> ros_cdk_core.IResolvable:
         '''Attribute ConnectionDomain: Connection domain of created instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrConnectionDomain"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrConnections")
     def attr_connections(self) -> ros_cdk_core.IResolvable:
         '''Attribute Connections: The maximum number of connections supported by the instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrConnections"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDirectConnectionPort")
     def attr_direct_connection_port(self) -> ros_cdk_core.IResolvable:
         '''Attribute DirectConnectionPort: The direct connection port of the instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDirectConnectionPort"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDirectConnectionString")
     def attr_direct_connection_string(self) -> ros_cdk_core.IResolvable:
         '''Attribute DirectConnectionString: The direct connection string of the instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDirectConnectionString"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrEngineVersion")
     def attr_engine_version(self) -> ros_cdk_core.IResolvable:
         '''Attribute EngineVersion: The engine version of the instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrEngineVersion"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrHasRenewChangeOrder")
     def attr_has_renew_change_order(self) -> ros_cdk_core.IResolvable:
         '''Attribute HasRenewChangeOrder: Indicates whether the Alibaba Cloud account has pending renewal or scaling orders.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrHasRenewChangeOrder"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInstanceClass")
     def attr_instance_class(self) -> ros_cdk_core.IResolvable:
         '''Attribute InstanceClass: Redis instance type.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInstanceClass"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInstanceId")
     def attr_instance_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute InstanceId: Instance id of created redis instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInstanceId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInstanceName")
     def attr_instance_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute InstanceName: Name of created redis instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInstanceName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInstanceType")
     def attr_instance_type(self) -> ros_cdk_core.IResolvable:
         '''Attribute InstanceType: The engine type of the instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInstanceType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrNetworkType")
     def attr_network_type(self) -> ros_cdk_core.IResolvable:
         '''Attribute NetworkType: The network type.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrNetworkType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrNodeType")
     def attr_node_type(self) -> ros_cdk_core.IResolvable:
         '''Attribute NodeType: The type of node.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrNodeType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrOrderId")
     def attr_order_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute OrderId: Order Id of created instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrOrderId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPackageType")
     def attr_package_type(self) -> ros_cdk_core.IResolvable:
         '''Attribute PackageType: The plan type.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPackageType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPort")
     def attr_port(self) -> ros_cdk_core.IResolvable:
         '''Attribute Port: Port of created instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPort"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPrivateIp")
     def attr_private_ip(self) -> ros_cdk_core.IResolvable:
         '''Attribute PrivateIp: The internal IP address of the instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPrivateIp"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPublicConnectionPort")
     def attr_public_connection_port(self) -> ros_cdk_core.IResolvable:
         '''Attribute PublicConnectionPort: The public connection port of the instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPublicConnectionPort"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPublicConnectionString")
     def attr_public_connection_string(self) -> ros_cdk_core.IResolvable:
         '''Attribute PublicConnectionString: The public connection string of the instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPublicConnectionString"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrQps")
     def attr_qps(self) -> ros_cdk_core.IResolvable:
         '''Attribute QPS: The queries per second (QPS) supported by the instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrQps"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrResourceGroupId")
     def attr_resource_group_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute ResourceGroupId: The ID of the resource group to which the instance belongs.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrResourceGroupId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVpcId")
     def attr_vpc_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute VpcId: The ID of the VPC.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVpcId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVpcPrivateConnectionPort")
     def attr_vpc_private_connection_port(self) -> ros_cdk_core.IResolvable:
         '''Attribute VpcPrivateConnectionPort: The vpc private connection port of the instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVpcPrivateConnectionPort"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVpcPrivateConnectionString")
     def attr_vpc_private_connection_string(self) -> ros_cdk_core.IResolvable:
         '''Attribute VpcPrivateConnectionString: The vpc private connection string of the instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVpcPrivateConnectionString"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVSwitchId")
     def attr_v_switch_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute VSwitchId: The ID of the vSwitch.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVSwitchId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrZoneId")
     def attr_zone_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute ZoneId: The ID of the zone.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrZoneId"))
 
 
 @jsii.data_type(
@@ -425,14 +447,15 @@
         "engine_version": "engineVersion",
         "eviction_policy": "evictionPolicy",
         "instance_class": "instanceClass",
         "instance_maintain_time": "instanceMaintainTime",
         "instance_name": "instanceName",
         "password": "password",
         "period": "period",
+        "period_unit": "periodUnit",
         "product_type": "productType",
         "resource_group_id": "resourceGroupId",
         "secondary_zone_id": "secondaryZoneId",
         "security_group_id": "securityGroupId",
         "ssl_enabled": "sslEnabled",
         "tags": "tags",
         "vpc_id": "vpcId",
@@ -442,31 +465,32 @@
     },
 )
 class InstanceProps:
     def __init__(
         self,
         *,
         auto_renew_duration: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
-        backup_policy: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosInstance.BackupPolicyProperty"]] = None,
+        backup_policy: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosInstance.BackupPolicyProperty", typing.Dict[str, typing.Any]]]] = None,
         charge_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        connections: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosInstance.ConnectionsProperty"]] = None,
+        connections: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosInstance.ConnectionsProperty", typing.Dict[str, typing.Any]]]] = None,
         deletion_force: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         engine_version: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         eviction_policy: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         instance_class: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        instance_maintain_time: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosInstance.InstanceMaintainTimeProperty"]] = None,
+        instance_maintain_time: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosInstance.InstanceMaintainTimeProperty", typing.Dict[str, typing.Any]]]] = None,
         instance_name: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         password: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         period: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
+        period_unit: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         product_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         resource_group_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         secondary_zone_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         security_group_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ssl_enabled: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        tags: typing.Optional[typing.Sequence["RosInstance.TagsProperty"]] = None,
+        tags: typing.Optional[typing.Sequence[typing.Union["RosInstance.TagsProperty", typing.Dict[str, typing.Any]]]] = None,
         vpc_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         vpc_password_free: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         v_switch_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         zone_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::REDIS::Instance``.
 
@@ -478,25 +502,51 @@
         :param engine_version: Property engineVersion: Engine version. Supported values: 2.8, 4.0 and 5.0.
         :param eviction_policy: Property evictionPolicy: The eviction policy of cache data storage.
         :param instance_class: Property instanceClass: Redis instance type. Refer the Redis instance type reference, such as 'redis.master.small.default', 'redis.master.4xlarge.default', 'redis.sharding.mid.default' etc
         :param instance_maintain_time: Property instanceMaintainTime: Instance maintain time.
         :param instance_name: Property instanceName: Display name of the instance, [2, 128] English or Chinese characters, must start with a letter or Chinese in size, can contain numbers, '_' or '.', '-'.
         :param password: Property password: The password of redis instance.length 8 to 30 characters, need to contain both uppercase and lowercase letters and numbers.
         :param period: Property period: The period of order, when choose Prepaid required.optional value 1-9, 12, 24, 36, 60 Unit in month.
+        :param period_unit: Property periodUnit: The unit of the subscription duration. Valid values: Month Year Default value: Month.
         :param product_type: Property productType: Product type. Valid values:Local: Community Edition(Local) or Enhanced Edition(Local)Tair_rdb: Performance Enhanced(Cloud Disk)Tair_scm: Persistent Memory(Cloud Disk)Tair_essd: Capacity Storage(Cloud Disk)OnECS: Community Edition(Cloud Disk)
         :param resource_group_id: Property resourceGroupId: Resource group id.
         :param secondary_zone_id: Property secondaryZoneId: The secondary zone ID of the instance.
         :param security_group_id: Property securityGroupId: The IDs of security groups. Separate multiple security group IDs with commas (,) and up to 10 can be set.
         :param ssl_enabled: Property sslEnabled: Modifies the SSL status. Valid values: Disable: disables SSL encryption. Enable: enables SSL encryption. Update: updates the SSL certificate.
         :param tags: Property tags: Tags to attach to redis. Max support 20 tags to add during create redis. Each tag with two properties Key and Value, and Key is required.
         :param vpc_id: Property vpcId: The VPC id to create ecs instance.
         :param vpc_password_free: Property vpcPasswordFree: Specifies whether to enable password free for access within the VPC. If set to: - true: enables password free. - false: disables password free.
         :param v_switch_id: Property vSwitchId: The vSwitch Id to create ecs instance.
         :param zone_id: Property zoneId: The zone id of input region.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(InstanceProps.__init__)
+            check_type(argname="argument auto_renew_duration", value=auto_renew_duration, expected_type=type_hints["auto_renew_duration"])
+            check_type(argname="argument backup_policy", value=backup_policy, expected_type=type_hints["backup_policy"])
+            check_type(argname="argument charge_type", value=charge_type, expected_type=type_hints["charge_type"])
+            check_type(argname="argument connections", value=connections, expected_type=type_hints["connections"])
+            check_type(argname="argument deletion_force", value=deletion_force, expected_type=type_hints["deletion_force"])
+            check_type(argname="argument engine_version", value=engine_version, expected_type=type_hints["engine_version"])
+            check_type(argname="argument eviction_policy", value=eviction_policy, expected_type=type_hints["eviction_policy"])
+            check_type(argname="argument instance_class", value=instance_class, expected_type=type_hints["instance_class"])
+            check_type(argname="argument instance_maintain_time", value=instance_maintain_time, expected_type=type_hints["instance_maintain_time"])
+            check_type(argname="argument instance_name", value=instance_name, expected_type=type_hints["instance_name"])
+            check_type(argname="argument password", value=password, expected_type=type_hints["password"])
+            check_type(argname="argument period", value=period, expected_type=type_hints["period"])
+            check_type(argname="argument period_unit", value=period_unit, expected_type=type_hints["period_unit"])
+            check_type(argname="argument product_type", value=product_type, expected_type=type_hints["product_type"])
+            check_type(argname="argument resource_group_id", value=resource_group_id, expected_type=type_hints["resource_group_id"])
+            check_type(argname="argument secondary_zone_id", value=secondary_zone_id, expected_type=type_hints["secondary_zone_id"])
+            check_type(argname="argument security_group_id", value=security_group_id, expected_type=type_hints["security_group_id"])
+            check_type(argname="argument ssl_enabled", value=ssl_enabled, expected_type=type_hints["ssl_enabled"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
+            check_type(argname="argument vpc_id", value=vpc_id, expected_type=type_hints["vpc_id"])
+            check_type(argname="argument vpc_password_free", value=vpc_password_free, expected_type=type_hints["vpc_password_free"])
+            check_type(argname="argument v_switch_id", value=v_switch_id, expected_type=type_hints["v_switch_id"])
+            check_type(argname="argument zone_id", value=zone_id, expected_type=type_hints["zone_id"])
         self._values: typing.Dict[str, typing.Any] = {}
         if auto_renew_duration is not None:
             self._values["auto_renew_duration"] = auto_renew_duration
         if backup_policy is not None:
             self._values["backup_policy"] = backup_policy
         if charge_type is not None:
             self._values["charge_type"] = charge_type
@@ -514,14 +564,16 @@
             self._values["instance_maintain_time"] = instance_maintain_time
         if instance_name is not None:
             self._values["instance_name"] = instance_name
         if password is not None:
             self._values["password"] = password
         if period is not None:
             self._values["period"] = period
+        if period_unit is not None:
+            self._values["period_unit"] = period_unit
         if product_type is not None:
             self._values["product_type"] = product_type
         if resource_group_id is not None:
             self._values["resource_group_id"] = resource_group_id
         if secondary_zone_id is not None:
             self._values["secondary_zone_id"] = secondary_zone_id
         if security_group_id is not None:
@@ -647,14 +699,28 @@
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''Property period: The period of order, when choose Prepaid required.optional value 1-9, 12, 24, 36, 60 Unit in month.'''
         result = self._values.get("period")
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], result)
 
     @builtins.property
+    def period_unit(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
+        '''Property periodUnit: The unit of the subscription duration.
+
+        Valid values:
+        Month
+        Year
+        Default value: Month.
+        '''
+        result = self._values.get("period_unit")
+        return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], result)
+
+    @builtins.property
     def product_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''Property productType: Product type.
 
         Valid values:Local: Community Edition(Local) or Enhanced Edition(Local)Tair_rdb: Performance Enhanced(Cloud Disk)Tair_scm: Persistent Memory(Cloud Disk)Tair_essd: Capacity Storage(Cloud Disk)OnECS: Community Edition(Cloud Disk)
         '''
@@ -768,217 +834,223 @@
 ):
     '''A ROS resource type:  ``ALIYUN::REDIS::PrepayInstance``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: typing.Optional["PrepayInstanceProps"] = None,
+        props: typing.Optional[typing.Union["PrepayInstanceProps", typing.Dict[str, typing.Any]]] = None,
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::REDIS::PrepayInstance``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(PrepayInstance.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrArchitectureType")
     def attr_architecture_type(self) -> ros_cdk_core.IResolvable:
         '''Attribute ArchitectureType: The architecture.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrArchitectureType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrBandwidth")
     def attr_bandwidth(self) -> ros_cdk_core.IResolvable:
         '''Attribute Bandwidth: The bandwidth of the instance.
 
         Unit: Mbit/s.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrBandwidth"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrCapacity")
     def attr_capacity(self) -> ros_cdk_core.IResolvable:
         '''Attribute Capacity: The storage capacity of the instance.
 
         Unit: MB.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrCapacity"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrChargeType")
     def attr_charge_type(self) -> ros_cdk_core.IResolvable:
         '''Attribute ChargeType: The billing method of the instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrChargeType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrClassicInnerConnectionPort")
     def attr_classic_inner_connection_port(self) -> ros_cdk_core.IResolvable:
         '''Attribute ClassicInnerConnectionPort: The classic inner connection port of the instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrClassicInnerConnectionPort"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrClassicInnerConnectionString")
     def attr_classic_inner_connection_string(self) -> ros_cdk_core.IResolvable:
         '''Attribute ClassicInnerConnectionString: The classic inner connection string of the instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrClassicInnerConnectionString"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrConnectionDomain")
     def attr_connection_domain(self) -> ros_cdk_core.IResolvable:
         '''Attribute ConnectionDomain: Connection domain of created instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrConnectionDomain"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrConnections")
     def attr_connections(self) -> ros_cdk_core.IResolvable:
         '''Attribute Connections: The maximum number of connections supported by the instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrConnections"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDirectConnectionPort")
     def attr_direct_connection_port(self) -> ros_cdk_core.IResolvable:
         '''Attribute DirectConnectionPort: The direct connection port of the instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDirectConnectionPort"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDirectConnectionString")
     def attr_direct_connection_string(self) -> ros_cdk_core.IResolvable:
         '''Attribute DirectConnectionString: The direct connection string of the instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDirectConnectionString"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrEngineVersion")
     def attr_engine_version(self) -> ros_cdk_core.IResolvable:
         '''Attribute EngineVersion: The engine version of the instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrEngineVersion"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrHasRenewChangeOrder")
     def attr_has_renew_change_order(self) -> ros_cdk_core.IResolvable:
         '''Attribute HasRenewChangeOrder: Indicates whether the Alibaba Cloud account has pending renewal or scaling orders.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrHasRenewChangeOrder"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInstanceClass")
     def attr_instance_class(self) -> ros_cdk_core.IResolvable:
         '''Attribute InstanceClass: Redis instance type.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInstanceClass"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInstanceId")
     def attr_instance_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute InstanceId: Instance id of created redis instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInstanceId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInstanceName")
     def attr_instance_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute InstanceName: Name of created redis instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInstanceName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInstanceType")
     def attr_instance_type(self) -> ros_cdk_core.IResolvable:
         '''Attribute InstanceType: The engine type of the instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInstanceType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrNetworkType")
     def attr_network_type(self) -> ros_cdk_core.IResolvable:
         '''Attribute NetworkType: The network type.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrNetworkType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrNodeType")
     def attr_node_type(self) -> ros_cdk_core.IResolvable:
         '''Attribute NodeType: The type of node.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrNodeType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrOrderId")
     def attr_order_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute OrderId: Order Id of created instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrOrderId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPackageType")
     def attr_package_type(self) -> ros_cdk_core.IResolvable:
         '''Attribute PackageType: The plan type.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPackageType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPort")
     def attr_port(self) -> ros_cdk_core.IResolvable:
         '''Attribute Port: Port of created instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPort"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPrivateIp")
     def attr_private_ip(self) -> ros_cdk_core.IResolvable:
         '''Attribute PrivateIp: The internal IP address of the instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPrivateIp"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPublicConnectionPort")
     def attr_public_connection_port(self) -> ros_cdk_core.IResolvable:
         '''Attribute PublicConnectionPort: The public connection port of the instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPublicConnectionPort"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPublicConnectionString")
     def attr_public_connection_string(self) -> ros_cdk_core.IResolvable:
         '''Attribute PublicConnectionString: The public connection string of the instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPublicConnectionString"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrQps")
     def attr_qps(self) -> ros_cdk_core.IResolvable:
         '''Attribute QPS: The queries per second (QPS) supported by the instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrQps"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrResourceGroupId")
     def attr_resource_group_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute ResourceGroupId: The ID of the resource group to which the instance belongs.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrResourceGroupId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVpcId")
     def attr_vpc_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute VpcId: The ID of the VPC.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVpcId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVpcPrivateConnectionPort")
     def attr_vpc_private_connection_port(self) -> ros_cdk_core.IResolvable:
         '''Attribute VpcPrivateConnectionPort: The vpc private connection port of the instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVpcPrivateConnectionPort"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVpcPrivateConnectionString")
     def attr_vpc_private_connection_string(self) -> ros_cdk_core.IResolvable:
         '''Attribute VpcPrivateConnectionString: The vpc private connection string of the instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVpcPrivateConnectionString"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVSwitchId")
     def attr_v_switch_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute VSwitchId: The ID of the vSwitch.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVSwitchId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrZoneId")
     def attr_zone_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute ZoneId: The ID of the zone.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrZoneId"))
 
 
 @jsii.data_type(
@@ -993,14 +1065,15 @@
         "engine_version": "engineVersion",
         "eviction_policy": "evictionPolicy",
         "instance_class": "instanceClass",
         "instance_maintain_time": "instanceMaintainTime",
         "instance_name": "instanceName",
         "password": "password",
         "period": "period",
+        "period_unit": "periodUnit",
         "product_type": "productType",
         "resource_group_id": "resourceGroupId",
         "secondary_zone_id": "secondaryZoneId",
         "security_group_id": "securityGroupId",
         "ssl_enabled": "sslEnabled",
         "tags": "tags",
         "vpc_id": "vpcId",
@@ -1011,30 +1084,31 @@
 )
 class PrepayInstanceProps:
     def __init__(
         self,
         *,
         auto_pay: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         auto_renew_duration: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
-        backup_policy: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosPrepayInstance.BackupPolicyProperty"]] = None,
-        connections: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosPrepayInstance.ConnectionsProperty"]] = None,
+        backup_policy: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosPrepayInstance.BackupPolicyProperty", typing.Dict[str, typing.Any]]]] = None,
+        connections: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosPrepayInstance.ConnectionsProperty", typing.Dict[str, typing.Any]]]] = None,
         deletion_force: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         engine_version: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         eviction_policy: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         instance_class: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        instance_maintain_time: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosPrepayInstance.InstanceMaintainTimeProperty"]] = None,
+        instance_maintain_time: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosPrepayInstance.InstanceMaintainTimeProperty", typing.Dict[str, typing.Any]]]] = None,
         instance_name: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         password: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         period: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
+        period_unit: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         product_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         resource_group_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         secondary_zone_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         security_group_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ssl_enabled: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        tags: typing.Optional[typing.Sequence["RosPrepayInstance.TagsProperty"]] = None,
+        tags: typing.Optional[typing.Sequence[typing.Union["RosPrepayInstance.TagsProperty", typing.Dict[str, typing.Any]]]] = None,
         vpc_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         vpc_password_free: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         v_switch_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         zone_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::REDIS::PrepayInstance``.
 
@@ -1046,25 +1120,51 @@
         :param engine_version: Property engineVersion: Engine version. Supported values: 2.8, 4.0 and 5.0.
         :param eviction_policy: Property evictionPolicy: The eviction policy of cache data storage.
         :param instance_class: Property instanceClass: Redis instance type. Refer the Redis instance type reference, such as 'redis.master.small.default', 'redis.master.4xlarge.default', 'redis.sharding.mid.default' etc
         :param instance_maintain_time: Property instanceMaintainTime: Instance maintain time.
         :param instance_name: Property instanceName: Display name of the instance, [2, 128] English or Chinese characters, must start with a letter or Chinese in size, can contain numbers, '_' or '.', '-'.
         :param password: Property password: The password of redis instance.length 8 to 30 characters, need to contain both uppercase and lowercase letters and numbers.
         :param period: Property period: The period of order, when choose Prepaid required.optional value 1-9, 12, 24, 36, 60 Unit in month.
+        :param period_unit: Property periodUnit: The unit of the subscription duration. Valid values: Month Year Default value: Month.
         :param product_type: Property productType: Product type. Valid values:Local: Community Edition(Local) or Enhanced Edition(Local)Tair_rdb: Performance Enhanced(Cloud Disk)Tair_scm: Persistent Memory(Cloud Disk)Tair_essd: Capacity Storage(Cloud Disk)OnECS: Community Edition(Cloud Disk)
         :param resource_group_id: Property resourceGroupId: Resource group id.
         :param secondary_zone_id: Property secondaryZoneId: The secondary zone ID of the instance.
         :param security_group_id: Property securityGroupId: The IDs of security groups. Separate multiple security group IDs with commas (,) and up to 10 can be set.
         :param ssl_enabled: Property sslEnabled: Modifies the SSL status. Valid values: Disable: disables SSL encryption. Enable: enables SSL encryption. Update: updates the SSL certificate.
         :param tags: Property tags: Tags to attach to redis. Max support 20 tags to add during create redis. Each tag with two properties Key and Value, and Key is required.
         :param vpc_id: Property vpcId: The VPC id to create ecs instance.
         :param vpc_password_free: Property vpcPasswordFree: Specifies whether to enable password free for access within the VPC. If set to: - true: enables password free. - false: disables password free.
         :param v_switch_id: Property vSwitchId: The vSwitch Id to create ecs instance.
         :param zone_id: Property zoneId: The zone id of input region.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(PrepayInstanceProps.__init__)
+            check_type(argname="argument auto_pay", value=auto_pay, expected_type=type_hints["auto_pay"])
+            check_type(argname="argument auto_renew_duration", value=auto_renew_duration, expected_type=type_hints["auto_renew_duration"])
+            check_type(argname="argument backup_policy", value=backup_policy, expected_type=type_hints["backup_policy"])
+            check_type(argname="argument connections", value=connections, expected_type=type_hints["connections"])
+            check_type(argname="argument deletion_force", value=deletion_force, expected_type=type_hints["deletion_force"])
+            check_type(argname="argument engine_version", value=engine_version, expected_type=type_hints["engine_version"])
+            check_type(argname="argument eviction_policy", value=eviction_policy, expected_type=type_hints["eviction_policy"])
+            check_type(argname="argument instance_class", value=instance_class, expected_type=type_hints["instance_class"])
+            check_type(argname="argument instance_maintain_time", value=instance_maintain_time, expected_type=type_hints["instance_maintain_time"])
+            check_type(argname="argument instance_name", value=instance_name, expected_type=type_hints["instance_name"])
+            check_type(argname="argument password", value=password, expected_type=type_hints["password"])
+            check_type(argname="argument period", value=period, expected_type=type_hints["period"])
+            check_type(argname="argument period_unit", value=period_unit, expected_type=type_hints["period_unit"])
+            check_type(argname="argument product_type", value=product_type, expected_type=type_hints["product_type"])
+            check_type(argname="argument resource_group_id", value=resource_group_id, expected_type=type_hints["resource_group_id"])
+            check_type(argname="argument secondary_zone_id", value=secondary_zone_id, expected_type=type_hints["secondary_zone_id"])
+            check_type(argname="argument security_group_id", value=security_group_id, expected_type=type_hints["security_group_id"])
+            check_type(argname="argument ssl_enabled", value=ssl_enabled, expected_type=type_hints["ssl_enabled"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
+            check_type(argname="argument vpc_id", value=vpc_id, expected_type=type_hints["vpc_id"])
+            check_type(argname="argument vpc_password_free", value=vpc_password_free, expected_type=type_hints["vpc_password_free"])
+            check_type(argname="argument v_switch_id", value=v_switch_id, expected_type=type_hints["v_switch_id"])
+            check_type(argname="argument zone_id", value=zone_id, expected_type=type_hints["zone_id"])
         self._values: typing.Dict[str, typing.Any] = {}
         if auto_pay is not None:
             self._values["auto_pay"] = auto_pay
         if auto_renew_duration is not None:
             self._values["auto_renew_duration"] = auto_renew_duration
         if backup_policy is not None:
             self._values["backup_policy"] = backup_policy
@@ -1082,14 +1182,16 @@
             self._values["instance_maintain_time"] = instance_maintain_time
         if instance_name is not None:
             self._values["instance_name"] = instance_name
         if password is not None:
             self._values["password"] = password
         if period is not None:
             self._values["period"] = period
+        if period_unit is not None:
+            self._values["period_unit"] = period_unit
         if product_type is not None:
             self._values["product_type"] = product_type
         if resource_group_id is not None:
             self._values["resource_group_id"] = resource_group_id
         if secondary_zone_id is not None:
             self._values["secondary_zone_id"] = secondary_zone_id
         if security_group_id is not None:
@@ -1221,14 +1323,28 @@
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''Property period: The period of order, when choose Prepaid required.optional value 1-9, 12, 24, 36, 60 Unit in month.'''
         result = self._values.get("period")
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], result)
 
     @builtins.property
+    def period_unit(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
+        '''Property periodUnit: The unit of the subscription duration.
+
+        Valid values:
+        Month
+        Year
+        Default value: Month.
+        '''
+        result = self._values.get("period_unit")
+        return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], result)
+
+    @builtins.property
     def product_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''Property productType: Product type.
 
         Valid values:Local: Community Edition(Local) or Enhanced Edition(Local)Tair_rdb: Performance Enhanced(Cloud Disk)Tair_scm: Persistent Memory(Cloud Disk)Tair_essd: Capacity Storage(Cloud Disk)OnECS: Community Edition(Cloud Disk)
         '''
@@ -1342,64 +1458,73 @@
 ):
     '''A ROS template type:  ``ALIYUN::REDIS::Account``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosAccountProps",
+        props: typing.Union["RosAccountProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::REDIS::Account``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosAccount.__init__)
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
+            type_hints = typing.get_type_hints(RosAccount._render_properties)
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
     @jsii.member(jsii_name="attrAccountName")
     def attr_account_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: AccountName: The name of the account.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAccountName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInstanceId")
     def attr_instance_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: InstanceId: The name of the instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInstanceId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="accountName")
     def account_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         accountName: The name of the account. The name must start with a lowercase letter and can contain
         lowercase letters, digits, and underscores (_). The name can be 1 to 16 characters
@@ -1408,17 +1533,20 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "accountName"))
 
     @account_name.setter
     def account_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAccount, "account_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "accountName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="accountPassword")
     def account_password(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         ::
 
         ), number signs (#), dollar signs ($), percent signs (%), carets (^),
         ampersands (&), asterisks (*), parentheses (()), underscores (_), plus signs (+),
@@ -1432,41 +1560,50 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "accountPassword"))
 
     @account_password.setter
     def account_password(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAccount, "account_password").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "accountPassword", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAccount, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="instanceId")
     def instance_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: instanceId: The ID of the instance for which you want to create the account.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "instanceId"))
 
     @instance_id.setter
     def instance_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAccount, "instance_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "instanceId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="accountDescription")
     def account_description(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -1478,17 +1615,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "accountDescription"))
 
     @account_description.setter
     def account_description(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAccount, "account_description").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "accountDescription", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="accountPrivilege")
     def account_privilege(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -1504,31 +1644,37 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "accountPrivilege"))
 
     @account_privilege.setter
     def account_privilege(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAccount, "account_privilege").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "accountPrivilege", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="accountType")
     def account_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: accountType: The type of the account. Set this parameter to Normal.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "accountType"))
 
     @account_type.setter
     def account_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAccount, "account_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "accountType", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-redis.RosAccountProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -1556,14 +1702,22 @@
         :param account_name: 
         :param account_password: 
         :param instance_id: 
         :param account_description: 
         :param account_privilege: 
         :param account_type: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosAccountProps.__init__)
+            check_type(argname="argument account_name", value=account_name, expected_type=type_hints["account_name"])
+            check_type(argname="argument account_password", value=account_password, expected_type=type_hints["account_password"])
+            check_type(argname="argument instance_id", value=instance_id, expected_type=type_hints["instance_id"])
+            check_type(argname="argument account_description", value=account_description, expected_type=type_hints["account_description"])
+            check_type(argname="argument account_privilege", value=account_privilege, expected_type=type_hints["account_privilege"])
+            check_type(argname="argument account_type", value=account_type, expected_type=type_hints["account_type"])
         self._values: typing.Dict[str, typing.Any] = {
             "account_name": account_name,
             "account_password": account_password,
             "instance_id": instance_id,
         }
         if account_description is not None:
             self._values["account_description"] = account_description
@@ -1675,305 +1829,317 @@
 ):
     '''A ROS template type:  ``ALIYUN::REDIS::Instance``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosInstanceProps",
+        props: typing.Union["RosInstanceProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::REDIS::Instance``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosInstance.__init__)
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
+            type_hints = typing.get_type_hints(RosInstance._render_properties)
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
     @jsii.member(jsii_name="attrArchitectureType")
     def attr_architecture_type(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ArchitectureType: The architecture.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrArchitectureType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrBandwidth")
     def attr_bandwidth(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Bandwidth: The bandwidth of the instance. Unit: Mbit/s.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrBandwidth"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrCapacity")
     def attr_capacity(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Capacity: The storage capacity of the instance. Unit: MB.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrCapacity"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrChargeType")
     def attr_charge_type(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ChargeType: The billing method of the instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrChargeType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrClassicInnerConnectionPort")
     def attr_classic_inner_connection_port(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ClassicInnerConnectionPort: The classic inner connection port of the instance
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrClassicInnerConnectionPort"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrClassicInnerConnectionString")
     def attr_classic_inner_connection_string(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ClassicInnerConnectionString: The classic inner connection string of the instance
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrClassicInnerConnectionString"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrConnectionDomain")
     def attr_connection_domain(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ConnectionDomain: Connection domain of created instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrConnectionDomain"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrConnections")
     def attr_connections(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Connections: The maximum number of connections supported by the instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrConnections"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDirectConnectionPort")
     def attr_direct_connection_port(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: DirectConnectionPort: The direct connection port of the instance
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDirectConnectionPort"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDirectConnectionString")
     def attr_direct_connection_string(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: DirectConnectionString: The direct connection string of the instance
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDirectConnectionString"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrEngineVersion")
     def attr_engine_version(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: EngineVersion: The engine version of the instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrEngineVersion"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrHasRenewChangeOrder")
     def attr_has_renew_change_order(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: HasRenewChangeOrder: Indicates whether the Alibaba Cloud account has pending renewal or scaling orders
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrHasRenewChangeOrder"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInstanceClass")
     def attr_instance_class(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: InstanceClass: Redis instance type.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInstanceClass"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInstanceId")
     def attr_instance_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: InstanceId: Instance id of created redis instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInstanceId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInstanceName")
     def attr_instance_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: InstanceName: Name of created redis instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInstanceName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInstanceType")
     def attr_instance_type(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: InstanceType: The engine type of the instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInstanceType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrNetworkType")
     def attr_network_type(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: NetworkType: The network type.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrNetworkType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrNodeType")
     def attr_node_type(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: NodeType: The type of node.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrNodeType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrOrderId")
     def attr_order_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: OrderId: Order Id of created instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrOrderId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPackageType")
     def attr_package_type(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: PackageType: The plan type.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPackageType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPort")
     def attr_port(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Port: Port of created instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPort"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPrivateIp")
     def attr_private_ip(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: PrivateIp: The internal IP address of the instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPrivateIp"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPublicConnectionPort")
     def attr_public_connection_port(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: PublicConnectionPort: The public connection port of the instance
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPublicConnectionPort"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPublicConnectionString")
     def attr_public_connection_string(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: PublicConnectionString: The public connection string of the instance
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPublicConnectionString"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrQps")
     def attr_qps(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: QPS: The queries per second (QPS) supported by the instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrQps"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrResourceGroupId")
     def attr_resource_group_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ResourceGroupId: The ID of the resource group to which the instance belongs.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrResourceGroupId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVpcId")
     def attr_vpc_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: VpcId: The ID of the VPC.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVpcId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVpcPrivateConnectionPort")
     def attr_vpc_private_connection_port(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: VpcPrivateConnectionPort: The vpc private connection port of the instance
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVpcPrivateConnectionPort"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVpcPrivateConnectionString")
     def attr_vpc_private_connection_string(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: VpcPrivateConnectionString: The vpc private connection string of the instance
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVpcPrivateConnectionString"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVSwitchId")
     def attr_v_switch_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: VSwitchId: The ID of the vSwitch.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVSwitchId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrZoneId")
     def attr_zone_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ZoneId: The ID of the zone.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrZoneId"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosInstance, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="autoRenewDuration")
     def auto_renew_duration(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -1985,272 +2151,345 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "autoRenewDuration"))
 
     @auto_renew_duration.setter
     def auto_renew_duration(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "auto_renew_duration").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "autoRenewDuration", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="backupPolicy")
     def backup_policy(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosInstance.BackupPolicyProperty"]]:
         '''
         :Property: backupPolicy: Backup policy
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosInstance.BackupPolicyProperty"]], jsii.get(self, "backupPolicy"))
 
     @backup_policy.setter
     def backup_policy(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosInstance.BackupPolicyProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "backup_policy").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "backupPolicy", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="chargeType")
     def charge_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: chargeType: The billing method of the ApsaraDB for Redis instance.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "chargeType"))
 
     @charge_type.setter
     def charge_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "charge_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "chargeType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="connections")
     def connections(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosInstance.ConnectionsProperty"]]:
         '''
         :Property: connections: Connection address
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosInstance.ConnectionsProperty"]], jsii.get(self, "connections"))
 
     @connections.setter
     def connections(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosInstance.ConnectionsProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "connections").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "connections", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="deletionForce")
     def deletion_force(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property: deletionForce: Whether destroy instance when it is in recycle. Default is false
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "deletionForce"))
 
     @deletion_force.setter
     def deletion_force(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "deletion_force").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "deletionForce", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="engineVersion")
     def engine_version(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: engineVersion: Engine version. Supported values: 2.8, 4.0 and 5.0.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "engineVersion"))
 
     @engine_version.setter
     def engine_version(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "engine_version").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "engineVersion", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="evictionPolicy")
     def eviction_policy(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: evictionPolicy: The eviction policy of cache data storage.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "evictionPolicy"))
 
     @eviction_policy.setter
     def eviction_policy(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "eviction_policy").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "evictionPolicy", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="instanceClass")
     def instance_class(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: instanceClass: Redis instance type. Refer the Redis instance type reference, such as 'redis.master.small.default', 'redis.master.4xlarge.default', 'redis.sharding.mid.default' etc
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "instanceClass"))
 
     @instance_class.setter
     def instance_class(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "instance_class").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "instanceClass", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="instanceMaintainTime")
     def instance_maintain_time(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosInstance.InstanceMaintainTimeProperty"]]:
         '''
         :Property: instanceMaintainTime: Instance maintain time.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosInstance.InstanceMaintainTimeProperty"]], jsii.get(self, "instanceMaintainTime"))
 
     @instance_maintain_time.setter
     def instance_maintain_time(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosInstance.InstanceMaintainTimeProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "instance_maintain_time").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "instanceMaintainTime", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="instanceName")
     def instance_name(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: instanceName: Display name of the instance, [2, 128] English or Chinese characters, must start with a letter or Chinese in size, can contain numbers, '_' or '.', '-'
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "instanceName"))
 
     @instance_name.setter
     def instance_name(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "instance_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "instanceName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="password")
     def password(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: password: The password of redis instance.length 8 to 30 characters, need to contain both uppercase and lowercase letters and numbers
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "password"))
 
     @password.setter
     def password(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "password").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "password", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="period")
     def period(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: period: The period of order, when choose Prepaid required.optional value 1-9, 12, 24, 36, 60 Unit in month.
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "period"))
 
     @period.setter
     def period(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "period").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "period", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
+    @jsii.member(jsii_name="periodUnit")
+    def period_unit(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
+        '''
+        :Property:
+
+        periodUnit: The unit of the subscription duration. Valid values:
+        Month
+        Year
+        Default value: Month.
+        '''
+        return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "periodUnit"))
+
+    @period_unit.setter
+    def period_unit(
+        self,
+        value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "period_unit").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "periodUnit", value)
+
+    @builtins.property
     @jsii.member(jsii_name="productType")
     def product_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: productType: Product type. Valid values:Local: Community Edition(Local) or Enhanced Edition(Local)Tair_rdb: Performance Enhanced(Cloud Disk)Tair_scm: Persistent Memory(Cloud Disk)Tair_essd: Capacity Storage(Cloud Disk)OnECS: Community Edition(Cloud Disk)
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "productType"))
 
     @product_type.setter
     def product_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "product_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "productType", value)
 
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
+            type_hints = typing.get_type_hints(getattr(RosInstance, "resource_group_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "resourceGroupId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="secondaryZoneId")
     def secondary_zone_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: secondaryZoneId: The secondary zone ID of the instance.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "secondaryZoneId"))
 
     @secondary_zone_id.setter
     def secondary_zone_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "secondary_zone_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "secondaryZoneId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="securityGroupId")
     def security_group_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: securityGroupId: The IDs of security groups. Separate multiple security group IDs with commas (,) and up to 10 can be set.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "securityGroupId"))
 
     @security_group_id.setter
     def security_group_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "security_group_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "securityGroupId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="sslEnabled")
     def ssl_enabled(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -2262,49 +2501,58 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "sslEnabled"))
 
     @ssl_enabled.setter
     def ssl_enabled(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "ssl_enabled").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "sslEnabled", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="tags")
     def tags(self) -> typing.Optional[typing.List["RosInstance.TagsProperty"]]:
         '''
         :Property: tags: Tags to attach to redis. Max support 20 tags to add during create redis. Each tag with two properties Key and Value, and Key is required.
         '''
         return typing.cast(typing.Optional[typing.List["RosInstance.TagsProperty"]], jsii.get(self, "tags"))
 
     @tags.setter
     def tags(
         self,
         value: typing.Optional[typing.List["RosInstance.TagsProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "tags").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "tags", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vpcId")
     def vpc_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: vpcId: The VPC id to create ecs instance.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "vpcId"))
 
     @vpc_id.setter
     def vpc_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "vpc_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "vpcId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vpcPasswordFree")
     def vpc_password_free(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -2316,48 +2564,57 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "vpcPasswordFree"))
 
     @vpc_password_free.setter
     def vpc_password_free(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "vpc_password_free").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "vpcPasswordFree", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vSwitchId")
     def v_switch_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: vSwitchId: The vSwitch Id to create ecs instance.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "vSwitchId"))
 
     @v_switch_id.setter
     def v_switch_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "v_switch_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "vSwitchId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="zoneId")
     def zone_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: zoneId: The zone id of input region.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "zoneId"))
 
     @zone_id.setter
     def zone_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstance, "zone_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "zoneId", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-redis.RosInstance.BackupPolicyProperty",
         jsii_struct_bases=[],
         name_mapping={
             "preferred_backup_period": "preferredBackupPeriod",
@@ -2374,14 +2631,19 @@
             enable_backup_log: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param preferred_backup_period: 
             :param preferred_backup_time: 
             :param enable_backup_log: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosInstance.BackupPolicyProperty.__init__)
+                check_type(argname="argument preferred_backup_period", value=preferred_backup_period, expected_type=type_hints["preferred_backup_period"])
+                check_type(argname="argument preferred_backup_time", value=preferred_backup_time, expected_type=type_hints["preferred_backup_time"])
+                check_type(argname="argument enable_backup_log", value=enable_backup_log, expected_type=type_hints["enable_backup_log"])
             self._values: typing.Dict[str, typing.Any] = {
                 "preferred_backup_period": preferred_backup_period,
                 "preferred_backup_time": preferred_backup_time,
             }
             if enable_backup_log is not None:
                 self._values["enable_backup_log"] = enable_backup_log
 
@@ -2447,14 +2709,18 @@
             connection_port: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
             connection_string: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         ) -> None:
             '''
             :param connection_port: 
             :param connection_string: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosInstance.ClassicInnerConnectionProperty.__init__)
+                check_type(argname="argument connection_port", value=connection_port, expected_type=type_hints["connection_port"])
+                check_type(argname="argument connection_string", value=connection_string, expected_type=type_hints["connection_string"])
             self._values: typing.Dict[str, typing.Any] = {
                 "connection_port": connection_port,
                 "connection_string": connection_string,
             }
 
         @builtins.property
         def connection_port(
@@ -2504,25 +2770,31 @@
             "vpc_private_connection": "vpcPrivateConnection",
         },
     )
     class ConnectionsProperty:
         def __init__(
             self,
             *,
-            classic_inner_connection: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosInstance.ClassicInnerConnectionProperty"]] = None,
-            direct_connection: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosInstance.DirectConnectionProperty"]] = None,
-            public_connection: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosInstance.PublicConnectionProperty"]] = None,
-            vpc_private_connection: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosInstance.VpcPrivateConnectionProperty"]] = None,
+            classic_inner_connection: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosInstance.ClassicInnerConnectionProperty", typing.Dict[str, typing.Any]]]] = None,
+            direct_connection: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosInstance.DirectConnectionProperty", typing.Dict[str, typing.Any]]]] = None,
+            public_connection: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosInstance.PublicConnectionProperty", typing.Dict[str, typing.Any]]]] = None,
+            vpc_private_connection: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosInstance.VpcPrivateConnectionProperty", typing.Dict[str, typing.Any]]]] = None,
         ) -> None:
             '''
             :param classic_inner_connection: 
             :param direct_connection: 
             :param public_connection: 
             :param vpc_private_connection: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosInstance.ConnectionsProperty.__init__)
+                check_type(argname="argument classic_inner_connection", value=classic_inner_connection, expected_type=type_hints["classic_inner_connection"])
+                check_type(argname="argument direct_connection", value=direct_connection, expected_type=type_hints["direct_connection"])
+                check_type(argname="argument public_connection", value=public_connection, expected_type=type_hints["public_connection"])
+                check_type(argname="argument vpc_private_connection", value=vpc_private_connection, expected_type=type_hints["vpc_private_connection"])
             self._values: typing.Dict[str, typing.Any] = {}
             if classic_inner_connection is not None:
                 self._values["classic_inner_connection"] = classic_inner_connection
             if direct_connection is not None:
                 self._values["direct_connection"] = direct_connection
             if public_connection is not None:
                 self._values["public_connection"] = public_connection
@@ -2598,14 +2870,18 @@
             connection_port: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
             connection_string: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         ) -> None:
             '''
             :param connection_port: 
             :param connection_string: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosInstance.DirectConnectionProperty.__init__)
+                check_type(argname="argument connection_port", value=connection_port, expected_type=type_hints["connection_port"])
+                check_type(argname="argument connection_string", value=connection_string, expected_type=type_hints["connection_string"])
             self._values: typing.Dict[str, typing.Any] = {
                 "connection_port": connection_port,
                 "connection_string": connection_string,
             }
 
         @builtins.property
         def connection_port(
@@ -2660,14 +2936,18 @@
             maintain_end_time: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
             maintain_start_time: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param maintain_end_time: 
             :param maintain_start_time: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosInstance.InstanceMaintainTimeProperty.__init__)
+                check_type(argname="argument maintain_end_time", value=maintain_end_time, expected_type=type_hints["maintain_end_time"])
+                check_type(argname="argument maintain_start_time", value=maintain_start_time, expected_type=type_hints["maintain_start_time"])
             self._values: typing.Dict[str, typing.Any] = {}
             if maintain_end_time is not None:
                 self._values["maintain_end_time"] = maintain_end_time
             if maintain_start_time is not None:
                 self._values["maintain_start_time"] = maintain_start_time
 
         @builtins.property
@@ -2726,14 +3006,18 @@
             connection_port: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
             connection_string: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         ) -> None:
             '''
             :param connection_port: 
             :param connection_string: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosInstance.PublicConnectionProperty.__init__)
+                check_type(argname="argument connection_port", value=connection_port, expected_type=type_hints["connection_port"])
+                check_type(argname="argument connection_string", value=connection_string, expected_type=type_hints["connection_string"])
             self._values: typing.Dict[str, typing.Any] = {
                 "connection_port": connection_port,
                 "connection_string": connection_string,
             }
 
         @builtins.property
         def connection_port(
@@ -2785,14 +3069,18 @@
             key: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param key: 
             :param value: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosInstance.TagsProperty.__init__)
+                check_type(argname="argument key", value=key, expected_type=type_hints["key"])
+                check_type(argname="argument value", value=value, expected_type=type_hints["value"])
             self._values: typing.Dict[str, typing.Any] = {
                 "key": key,
             }
             if value is not None:
                 self._values["value"] = value
 
         @builtins.property
@@ -2840,14 +3128,18 @@
             connection_port: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
             connection_string: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         ) -> None:
             '''
             :param connection_port: 
             :param connection_string: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosInstance.VpcPrivateConnectionProperty.__init__)
+                check_type(argname="argument connection_port", value=connection_port, expected_type=type_hints["connection_port"])
+                check_type(argname="argument connection_string", value=connection_string, expected_type=type_hints["connection_string"])
             self._values: typing.Dict[str, typing.Any] = {
                 "connection_port": connection_port,
                 "connection_string": connection_string,
             }
 
         @builtins.property
         def connection_port(
@@ -2900,14 +3192,15 @@
         "engine_version": "engineVersion",
         "eviction_policy": "evictionPolicy",
         "instance_class": "instanceClass",
         "instance_maintain_time": "instanceMaintainTime",
         "instance_name": "instanceName",
         "password": "password",
         "period": "period",
+        "period_unit": "periodUnit",
         "product_type": "productType",
         "resource_group_id": "resourceGroupId",
         "secondary_zone_id": "secondaryZoneId",
         "security_group_id": "securityGroupId",
         "ssl_enabled": "sslEnabled",
         "tags": "tags",
         "vpc_id": "vpcId",
@@ -2917,31 +3210,32 @@
     },
 )
 class RosInstanceProps:
     def __init__(
         self,
         *,
         auto_renew_duration: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
-        backup_policy: typing.Optional[typing.Union[ros_cdk_core.IResolvable, RosInstance.BackupPolicyProperty]] = None,
+        backup_policy: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosInstance.BackupPolicyProperty, typing.Dict[str, typing.Any]]]] = None,
         charge_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        connections: typing.Optional[typing.Union[ros_cdk_core.IResolvable, RosInstance.ConnectionsProperty]] = None,
+        connections: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosInstance.ConnectionsProperty, typing.Dict[str, typing.Any]]]] = None,
         deletion_force: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         engine_version: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         eviction_policy: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         instance_class: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        instance_maintain_time: typing.Optional[typing.Union[ros_cdk_core.IResolvable, RosInstance.InstanceMaintainTimeProperty]] = None,
+        instance_maintain_time: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosInstance.InstanceMaintainTimeProperty, typing.Dict[str, typing.Any]]]] = None,
         instance_name: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         password: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         period: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
+        period_unit: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         product_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         resource_group_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         secondary_zone_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         security_group_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ssl_enabled: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        tags: typing.Optional[typing.Sequence[RosInstance.TagsProperty]] = None,
+        tags: typing.Optional[typing.Sequence[typing.Union[RosInstance.TagsProperty, typing.Dict[str, typing.Any]]]] = None,
         vpc_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         vpc_password_free: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         v_switch_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         zone_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::REDIS::Instance``.
 
@@ -2953,25 +3247,51 @@
         :param engine_version: 
         :param eviction_policy: 
         :param instance_class: 
         :param instance_maintain_time: 
         :param instance_name: 
         :param password: 
         :param period: 
+        :param period_unit: 
         :param product_type: 
         :param resource_group_id: 
         :param secondary_zone_id: 
         :param security_group_id: 
         :param ssl_enabled: 
         :param tags: 
         :param vpc_id: 
         :param vpc_password_free: 
         :param v_switch_id: 
         :param zone_id: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosInstanceProps.__init__)
+            check_type(argname="argument auto_renew_duration", value=auto_renew_duration, expected_type=type_hints["auto_renew_duration"])
+            check_type(argname="argument backup_policy", value=backup_policy, expected_type=type_hints["backup_policy"])
+            check_type(argname="argument charge_type", value=charge_type, expected_type=type_hints["charge_type"])
+            check_type(argname="argument connections", value=connections, expected_type=type_hints["connections"])
+            check_type(argname="argument deletion_force", value=deletion_force, expected_type=type_hints["deletion_force"])
+            check_type(argname="argument engine_version", value=engine_version, expected_type=type_hints["engine_version"])
+            check_type(argname="argument eviction_policy", value=eviction_policy, expected_type=type_hints["eviction_policy"])
+            check_type(argname="argument instance_class", value=instance_class, expected_type=type_hints["instance_class"])
+            check_type(argname="argument instance_maintain_time", value=instance_maintain_time, expected_type=type_hints["instance_maintain_time"])
+            check_type(argname="argument instance_name", value=instance_name, expected_type=type_hints["instance_name"])
+            check_type(argname="argument password", value=password, expected_type=type_hints["password"])
+            check_type(argname="argument period", value=period, expected_type=type_hints["period"])
+            check_type(argname="argument period_unit", value=period_unit, expected_type=type_hints["period_unit"])
+            check_type(argname="argument product_type", value=product_type, expected_type=type_hints["product_type"])
+            check_type(argname="argument resource_group_id", value=resource_group_id, expected_type=type_hints["resource_group_id"])
+            check_type(argname="argument secondary_zone_id", value=secondary_zone_id, expected_type=type_hints["secondary_zone_id"])
+            check_type(argname="argument security_group_id", value=security_group_id, expected_type=type_hints["security_group_id"])
+            check_type(argname="argument ssl_enabled", value=ssl_enabled, expected_type=type_hints["ssl_enabled"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
+            check_type(argname="argument vpc_id", value=vpc_id, expected_type=type_hints["vpc_id"])
+            check_type(argname="argument vpc_password_free", value=vpc_password_free, expected_type=type_hints["vpc_password_free"])
+            check_type(argname="argument v_switch_id", value=v_switch_id, expected_type=type_hints["v_switch_id"])
+            check_type(argname="argument zone_id", value=zone_id, expected_type=type_hints["zone_id"])
         self._values: typing.Dict[str, typing.Any] = {}
         if auto_renew_duration is not None:
             self._values["auto_renew_duration"] = auto_renew_duration
         if backup_policy is not None:
             self._values["backup_policy"] = backup_policy
         if charge_type is not None:
             self._values["charge_type"] = charge_type
@@ -2989,14 +3309,16 @@
             self._values["instance_maintain_time"] = instance_maintain_time
         if instance_name is not None:
             self._values["instance_name"] = instance_name
         if password is not None:
             self._values["password"] = password
         if period is not None:
             self._values["period"] = period
+        if period_unit is not None:
+            self._values["period_unit"] = period_unit
         if product_type is not None:
             self._values["product_type"] = product_type
         if resource_group_id is not None:
             self._values["resource_group_id"] = resource_group_id
         if secondary_zone_id is not None:
             self._values["secondary_zone_id"] = secondary_zone_id
         if security_group_id is not None:
@@ -3136,14 +3458,29 @@
         '''
         :Property: period: The period of order, when choose Prepaid required.optional value 1-9, 12, 24, 36, 60 Unit in month.
         '''
         result = self._values.get("period")
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], result)
 
     @builtins.property
+    def period_unit(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
+        '''
+        :Property:
+
+        periodUnit: The unit of the subscription duration. Valid values:
+        Month
+        Year
+        Default value: Month.
+        '''
+        result = self._values.get("period_unit")
+        return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], result)
+
+    @builtins.property
     def product_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: productType: Product type. Valid values:Local: Community Edition(Local) or Enhanced Edition(Local)Tair_rdb: Performance Enhanced(Cloud Disk)Tair_scm: Persistent Memory(Cloud Disk)Tair_essd: Capacity Storage(Cloud Disk)OnECS: Community Edition(Cloud Disk)
         '''
         result = self._values.get("product_type")
@@ -3266,305 +3603,317 @@
 ):
     '''A ROS template type:  ``ALIYUN::REDIS::PrepayInstance``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosPrepayInstanceProps",
+        props: typing.Union["RosPrepayInstanceProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::REDIS::PrepayInstance``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosPrepayInstance.__init__)
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
+            type_hints = typing.get_type_hints(RosPrepayInstance._render_properties)
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
     @jsii.member(jsii_name="attrArchitectureType")
     def attr_architecture_type(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ArchitectureType: The architecture.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrArchitectureType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrBandwidth")
     def attr_bandwidth(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Bandwidth: The bandwidth of the instance. Unit: Mbit/s.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrBandwidth"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrCapacity")
     def attr_capacity(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Capacity: The storage capacity of the instance. Unit: MB.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrCapacity"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrChargeType")
     def attr_charge_type(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ChargeType: The billing method of the instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrChargeType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrClassicInnerConnectionPort")
     def attr_classic_inner_connection_port(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ClassicInnerConnectionPort: The classic inner connection port of the instance
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrClassicInnerConnectionPort"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrClassicInnerConnectionString")
     def attr_classic_inner_connection_string(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ClassicInnerConnectionString: The classic inner connection string of the instance
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrClassicInnerConnectionString"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrConnectionDomain")
     def attr_connection_domain(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ConnectionDomain: Connection domain of created instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrConnectionDomain"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrConnections")
     def attr_connections(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Connections: The maximum number of connections supported by the instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrConnections"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDirectConnectionPort")
     def attr_direct_connection_port(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: DirectConnectionPort: The direct connection port of the instance
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDirectConnectionPort"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDirectConnectionString")
     def attr_direct_connection_string(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: DirectConnectionString: The direct connection string of the instance
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDirectConnectionString"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrEngineVersion")
     def attr_engine_version(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: EngineVersion: The engine version of the instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrEngineVersion"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrHasRenewChangeOrder")
     def attr_has_renew_change_order(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: HasRenewChangeOrder: Indicates whether the Alibaba Cloud account has pending renewal or scaling orders
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrHasRenewChangeOrder"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInstanceClass")
     def attr_instance_class(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: InstanceClass: Redis instance type.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInstanceClass"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInstanceId")
     def attr_instance_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: InstanceId: Instance id of created redis instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInstanceId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInstanceName")
     def attr_instance_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: InstanceName: Name of created redis instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInstanceName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInstanceType")
     def attr_instance_type(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: InstanceType: The engine type of the instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInstanceType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrNetworkType")
     def attr_network_type(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: NetworkType: The network type.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrNetworkType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrNodeType")
     def attr_node_type(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: NodeType: The type of node.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrNodeType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrOrderId")
     def attr_order_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: OrderId: Order Id of created instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrOrderId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPackageType")
     def attr_package_type(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: PackageType: The plan type.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPackageType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPort")
     def attr_port(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Port: Port of created instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPort"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPrivateIp")
     def attr_private_ip(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: PrivateIp: The internal IP address of the instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPrivateIp"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPublicConnectionPort")
     def attr_public_connection_port(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: PublicConnectionPort: The public connection port of the instance
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPublicConnectionPort"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPublicConnectionString")
     def attr_public_connection_string(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: PublicConnectionString: The public connection string of the instance
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPublicConnectionString"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrQps")
     def attr_qps(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: QPS: The queries per second (QPS) supported by the instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrQps"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrResourceGroupId")
     def attr_resource_group_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ResourceGroupId: The ID of the resource group to which the instance belongs.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrResourceGroupId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVpcId")
     def attr_vpc_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: VpcId: The ID of the VPC.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVpcId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVpcPrivateConnectionPort")
     def attr_vpc_private_connection_port(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: VpcPrivateConnectionPort: The vpc private connection port of the instance
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVpcPrivateConnectionPort"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVpcPrivateConnectionString")
     def attr_vpc_private_connection_string(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: VpcPrivateConnectionString: The vpc private connection string of the instance
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVpcPrivateConnectionString"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVSwitchId")
     def attr_v_switch_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: VSwitchId: The ID of the vSwitch.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVSwitchId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrZoneId")
     def attr_zone_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ZoneId: The ID of the zone.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrZoneId"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosPrepayInstance, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="autoPay")
     def auto_pay(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -3576,17 +3925,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "autoPay"))
 
     @auto_pay.setter
     def auto_pay(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPrepayInstance, "auto_pay").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "autoPay", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="autoRenewDuration")
     def auto_renew_duration(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -3598,255 +3950,325 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "autoRenewDuration"))
 
     @auto_renew_duration.setter
     def auto_renew_duration(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPrepayInstance, "auto_renew_duration").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "autoRenewDuration", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="backupPolicy")
     def backup_policy(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosPrepayInstance.BackupPolicyProperty"]]:
         '''
         :Property: backupPolicy: Backup policy
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosPrepayInstance.BackupPolicyProperty"]], jsii.get(self, "backupPolicy"))
 
     @backup_policy.setter
     def backup_policy(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosPrepayInstance.BackupPolicyProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPrepayInstance, "backup_policy").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "backupPolicy", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="connections")
     def connections(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosPrepayInstance.ConnectionsProperty"]]:
         '''
         :Property: connections: Connection address
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosPrepayInstance.ConnectionsProperty"]], jsii.get(self, "connections"))
 
     @connections.setter
     def connections(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosPrepayInstance.ConnectionsProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPrepayInstance, "connections").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "connections", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="deletionForce")
     def deletion_force(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property: deletionForce: Whether destroy instance when it is in recycle. Default is false
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "deletionForce"))
 
     @deletion_force.setter
     def deletion_force(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPrepayInstance, "deletion_force").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "deletionForce", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="engineVersion")
     def engine_version(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: engineVersion: Engine version. Supported values: 2.8, 4.0 and 5.0.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "engineVersion"))
 
     @engine_version.setter
     def engine_version(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPrepayInstance, "engine_version").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "engineVersion", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="evictionPolicy")
     def eviction_policy(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: evictionPolicy: The eviction policy of cache data storage.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "evictionPolicy"))
 
     @eviction_policy.setter
     def eviction_policy(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPrepayInstance, "eviction_policy").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "evictionPolicy", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="instanceClass")
     def instance_class(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: instanceClass: Redis instance type. Refer the Redis instance type reference, such as 'redis.master.small.default', 'redis.master.4xlarge.default', 'redis.sharding.mid.default' etc
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "instanceClass"))
 
     @instance_class.setter
     def instance_class(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPrepayInstance, "instance_class").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "instanceClass", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="instanceMaintainTime")
     def instance_maintain_time(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosPrepayInstance.InstanceMaintainTimeProperty"]]:
         '''
         :Property: instanceMaintainTime: Instance maintain time.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosPrepayInstance.InstanceMaintainTimeProperty"]], jsii.get(self, "instanceMaintainTime"))
 
     @instance_maintain_time.setter
     def instance_maintain_time(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosPrepayInstance.InstanceMaintainTimeProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPrepayInstance, "instance_maintain_time").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "instanceMaintainTime", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="instanceName")
     def instance_name(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: instanceName: Display name of the instance, [2, 128] English or Chinese characters, must start with a letter or Chinese in size, can contain numbers, '_' or '.', '-'
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "instanceName"))
 
     @instance_name.setter
     def instance_name(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPrepayInstance, "instance_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "instanceName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="password")
     def password(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: password: The password of redis instance.length 8 to 30 characters, need to contain both uppercase and lowercase letters and numbers
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "password"))
 
     @password.setter
     def password(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPrepayInstance, "password").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "password", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="period")
     def period(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: period: The period of order, when choose Prepaid required.optional value 1-9, 12, 24, 36, 60 Unit in month.
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "period"))
 
     @period.setter
     def period(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPrepayInstance, "period").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "period", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
+    @jsii.member(jsii_name="periodUnit")
+    def period_unit(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
+        '''
+        :Property:
+
+        periodUnit: The unit of the subscription duration. Valid values:
+        Month
+        Year
+        Default value: Month.
+        '''
+        return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "periodUnit"))
+
+    @period_unit.setter
+    def period_unit(
+        self,
+        value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPrepayInstance, "period_unit").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "periodUnit", value)
+
+    @builtins.property
     @jsii.member(jsii_name="productType")
     def product_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: productType: Product type. Valid values:Local: Community Edition(Local) or Enhanced Edition(Local)Tair_rdb: Performance Enhanced(Cloud Disk)Tair_scm: Persistent Memory(Cloud Disk)Tair_essd: Capacity Storage(Cloud Disk)OnECS: Community Edition(Cloud Disk)
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "productType"))
 
     @product_type.setter
     def product_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPrepayInstance, "product_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "productType", value)
 
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
+            type_hints = typing.get_type_hints(getattr(RosPrepayInstance, "resource_group_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "resourceGroupId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="secondaryZoneId")
     def secondary_zone_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: secondaryZoneId: The secondary zone ID of the instance.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "secondaryZoneId"))
 
     @secondary_zone_id.setter
     def secondary_zone_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPrepayInstance, "secondary_zone_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "secondaryZoneId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="securityGroupId")
     def security_group_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: securityGroupId: The IDs of security groups. Separate multiple security group IDs with commas (,) and up to 10 can be set.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "securityGroupId"))
 
     @security_group_id.setter
     def security_group_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPrepayInstance, "security_group_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "securityGroupId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="sslEnabled")
     def ssl_enabled(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -3858,49 +4280,58 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "sslEnabled"))
 
     @ssl_enabled.setter
     def ssl_enabled(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPrepayInstance, "ssl_enabled").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "sslEnabled", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="tags")
     def tags(self) -> typing.Optional[typing.List["RosPrepayInstance.TagsProperty"]]:
         '''
         :Property: tags: Tags to attach to redis. Max support 20 tags to add during create redis. Each tag with two properties Key and Value, and Key is required.
         '''
         return typing.cast(typing.Optional[typing.List["RosPrepayInstance.TagsProperty"]], jsii.get(self, "tags"))
 
     @tags.setter
     def tags(
         self,
         value: typing.Optional[typing.List["RosPrepayInstance.TagsProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPrepayInstance, "tags").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "tags", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vpcId")
     def vpc_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: vpcId: The VPC id to create ecs instance.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "vpcId"))
 
     @vpc_id.setter
     def vpc_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPrepayInstance, "vpc_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "vpcId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vpcPasswordFree")
     def vpc_password_free(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -3912,48 +4343,57 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "vpcPasswordFree"))
 
     @vpc_password_free.setter
     def vpc_password_free(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPrepayInstance, "vpc_password_free").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "vpcPasswordFree", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vSwitchId")
     def v_switch_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: vSwitchId: The vSwitch Id to create ecs instance.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "vSwitchId"))
 
     @v_switch_id.setter
     def v_switch_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPrepayInstance, "v_switch_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "vSwitchId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="zoneId")
     def zone_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: zoneId: The zone id of input region.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "zoneId"))
 
     @zone_id.setter
     def zone_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPrepayInstance, "zone_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "zoneId", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-redis.RosPrepayInstance.BackupPolicyProperty",
         jsii_struct_bases=[],
         name_mapping={
             "preferred_backup_period": "preferredBackupPeriod",
@@ -3970,14 +4410,19 @@
             enable_backup_log: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param preferred_backup_period: 
             :param preferred_backup_time: 
             :param enable_backup_log: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosPrepayInstance.BackupPolicyProperty.__init__)
+                check_type(argname="argument preferred_backup_period", value=preferred_backup_period, expected_type=type_hints["preferred_backup_period"])
+                check_type(argname="argument preferred_backup_time", value=preferred_backup_time, expected_type=type_hints["preferred_backup_time"])
+                check_type(argname="argument enable_backup_log", value=enable_backup_log, expected_type=type_hints["enable_backup_log"])
             self._values: typing.Dict[str, typing.Any] = {
                 "preferred_backup_period": preferred_backup_period,
                 "preferred_backup_time": preferred_backup_time,
             }
             if enable_backup_log is not None:
                 self._values["enable_backup_log"] = enable_backup_log
 
@@ -4043,14 +4488,18 @@
             connection_port: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
             connection_string: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         ) -> None:
             '''
             :param connection_port: 
             :param connection_string: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosPrepayInstance.ClassicInnerConnectionProperty.__init__)
+                check_type(argname="argument connection_port", value=connection_port, expected_type=type_hints["connection_port"])
+                check_type(argname="argument connection_string", value=connection_string, expected_type=type_hints["connection_string"])
             self._values: typing.Dict[str, typing.Any] = {
                 "connection_port": connection_port,
                 "connection_string": connection_string,
             }
 
         @builtins.property
         def connection_port(
@@ -4100,25 +4549,31 @@
             "vpc_private_connection": "vpcPrivateConnection",
         },
     )
     class ConnectionsProperty:
         def __init__(
             self,
             *,
-            classic_inner_connection: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosPrepayInstance.ClassicInnerConnectionProperty"]] = None,
-            direct_connection: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosPrepayInstance.DirectConnectionProperty"]] = None,
-            public_connection: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosPrepayInstance.PublicConnectionProperty"]] = None,
-            vpc_private_connection: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosPrepayInstance.VpcPrivateConnectionProperty"]] = None,
+            classic_inner_connection: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosPrepayInstance.ClassicInnerConnectionProperty", typing.Dict[str, typing.Any]]]] = None,
+            direct_connection: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosPrepayInstance.DirectConnectionProperty", typing.Dict[str, typing.Any]]]] = None,
+            public_connection: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosPrepayInstance.PublicConnectionProperty", typing.Dict[str, typing.Any]]]] = None,
+            vpc_private_connection: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosPrepayInstance.VpcPrivateConnectionProperty", typing.Dict[str, typing.Any]]]] = None,
         ) -> None:
             '''
             :param classic_inner_connection: 
             :param direct_connection: 
             :param public_connection: 
             :param vpc_private_connection: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosPrepayInstance.ConnectionsProperty.__init__)
+                check_type(argname="argument classic_inner_connection", value=classic_inner_connection, expected_type=type_hints["classic_inner_connection"])
+                check_type(argname="argument direct_connection", value=direct_connection, expected_type=type_hints["direct_connection"])
+                check_type(argname="argument public_connection", value=public_connection, expected_type=type_hints["public_connection"])
+                check_type(argname="argument vpc_private_connection", value=vpc_private_connection, expected_type=type_hints["vpc_private_connection"])
             self._values: typing.Dict[str, typing.Any] = {}
             if classic_inner_connection is not None:
                 self._values["classic_inner_connection"] = classic_inner_connection
             if direct_connection is not None:
                 self._values["direct_connection"] = direct_connection
             if public_connection is not None:
                 self._values["public_connection"] = public_connection
@@ -4194,14 +4649,18 @@
             connection_port: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
             connection_string: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         ) -> None:
             '''
             :param connection_port: 
             :param connection_string: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosPrepayInstance.DirectConnectionProperty.__init__)
+                check_type(argname="argument connection_port", value=connection_port, expected_type=type_hints["connection_port"])
+                check_type(argname="argument connection_string", value=connection_string, expected_type=type_hints["connection_string"])
             self._values: typing.Dict[str, typing.Any] = {
                 "connection_port": connection_port,
                 "connection_string": connection_string,
             }
 
         @builtins.property
         def connection_port(
@@ -4256,14 +4715,18 @@
             maintain_end_time: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
             maintain_start_time: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param maintain_end_time: 
             :param maintain_start_time: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosPrepayInstance.InstanceMaintainTimeProperty.__init__)
+                check_type(argname="argument maintain_end_time", value=maintain_end_time, expected_type=type_hints["maintain_end_time"])
+                check_type(argname="argument maintain_start_time", value=maintain_start_time, expected_type=type_hints["maintain_start_time"])
             self._values: typing.Dict[str, typing.Any] = {}
             if maintain_end_time is not None:
                 self._values["maintain_end_time"] = maintain_end_time
             if maintain_start_time is not None:
                 self._values["maintain_start_time"] = maintain_start_time
 
         @builtins.property
@@ -4322,14 +4785,18 @@
             connection_port: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
             connection_string: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         ) -> None:
             '''
             :param connection_port: 
             :param connection_string: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosPrepayInstance.PublicConnectionProperty.__init__)
+                check_type(argname="argument connection_port", value=connection_port, expected_type=type_hints["connection_port"])
+                check_type(argname="argument connection_string", value=connection_string, expected_type=type_hints["connection_string"])
             self._values: typing.Dict[str, typing.Any] = {
                 "connection_port": connection_port,
                 "connection_string": connection_string,
             }
 
         @builtins.property
         def connection_port(
@@ -4381,14 +4848,18 @@
             key: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param key: 
             :param value: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosPrepayInstance.TagsProperty.__init__)
+                check_type(argname="argument key", value=key, expected_type=type_hints["key"])
+                check_type(argname="argument value", value=value, expected_type=type_hints["value"])
             self._values: typing.Dict[str, typing.Any] = {
                 "key": key,
             }
             if value is not None:
                 self._values["value"] = value
 
         @builtins.property
@@ -4436,14 +4907,18 @@
             connection_port: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
             connection_string: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         ) -> None:
             '''
             :param connection_port: 
             :param connection_string: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosPrepayInstance.VpcPrivateConnectionProperty.__init__)
+                check_type(argname="argument connection_port", value=connection_port, expected_type=type_hints["connection_port"])
+                check_type(argname="argument connection_string", value=connection_string, expected_type=type_hints["connection_string"])
             self._values: typing.Dict[str, typing.Any] = {
                 "connection_port": connection_port,
                 "connection_string": connection_string,
             }
 
         @builtins.property
         def connection_port(
@@ -4496,14 +4971,15 @@
         "engine_version": "engineVersion",
         "eviction_policy": "evictionPolicy",
         "instance_class": "instanceClass",
         "instance_maintain_time": "instanceMaintainTime",
         "instance_name": "instanceName",
         "password": "password",
         "period": "period",
+        "period_unit": "periodUnit",
         "product_type": "productType",
         "resource_group_id": "resourceGroupId",
         "secondary_zone_id": "secondaryZoneId",
         "security_group_id": "securityGroupId",
         "ssl_enabled": "sslEnabled",
         "tags": "tags",
         "vpc_id": "vpcId",
@@ -4514,30 +4990,31 @@
 )
 class RosPrepayInstanceProps:
     def __init__(
         self,
         *,
         auto_pay: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         auto_renew_duration: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
-        backup_policy: typing.Optional[typing.Union[ros_cdk_core.IResolvable, RosPrepayInstance.BackupPolicyProperty]] = None,
-        connections: typing.Optional[typing.Union[ros_cdk_core.IResolvable, RosPrepayInstance.ConnectionsProperty]] = None,
+        backup_policy: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosPrepayInstance.BackupPolicyProperty, typing.Dict[str, typing.Any]]]] = None,
+        connections: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosPrepayInstance.ConnectionsProperty, typing.Dict[str, typing.Any]]]] = None,
         deletion_force: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         engine_version: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         eviction_policy: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         instance_class: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        instance_maintain_time: typing.Optional[typing.Union[ros_cdk_core.IResolvable, RosPrepayInstance.InstanceMaintainTimeProperty]] = None,
+        instance_maintain_time: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosPrepayInstance.InstanceMaintainTimeProperty, typing.Dict[str, typing.Any]]]] = None,
         instance_name: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         password: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         period: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
+        period_unit: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         product_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         resource_group_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         secondary_zone_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         security_group_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ssl_enabled: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        tags: typing.Optional[typing.Sequence[RosPrepayInstance.TagsProperty]] = None,
+        tags: typing.Optional[typing.Sequence[typing.Union[RosPrepayInstance.TagsProperty, typing.Dict[str, typing.Any]]]] = None,
         vpc_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         vpc_password_free: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         v_switch_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         zone_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::REDIS::PrepayInstance``.
 
@@ -4549,25 +5026,51 @@
         :param engine_version: 
         :param eviction_policy: 
         :param instance_class: 
         :param instance_maintain_time: 
         :param instance_name: 
         :param password: 
         :param period: 
+        :param period_unit: 
         :param product_type: 
         :param resource_group_id: 
         :param secondary_zone_id: 
         :param security_group_id: 
         :param ssl_enabled: 
         :param tags: 
         :param vpc_id: 
         :param vpc_password_free: 
         :param v_switch_id: 
         :param zone_id: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosPrepayInstanceProps.__init__)
+            check_type(argname="argument auto_pay", value=auto_pay, expected_type=type_hints["auto_pay"])
+            check_type(argname="argument auto_renew_duration", value=auto_renew_duration, expected_type=type_hints["auto_renew_duration"])
+            check_type(argname="argument backup_policy", value=backup_policy, expected_type=type_hints["backup_policy"])
+            check_type(argname="argument connections", value=connections, expected_type=type_hints["connections"])
+            check_type(argname="argument deletion_force", value=deletion_force, expected_type=type_hints["deletion_force"])
+            check_type(argname="argument engine_version", value=engine_version, expected_type=type_hints["engine_version"])
+            check_type(argname="argument eviction_policy", value=eviction_policy, expected_type=type_hints["eviction_policy"])
+            check_type(argname="argument instance_class", value=instance_class, expected_type=type_hints["instance_class"])
+            check_type(argname="argument instance_maintain_time", value=instance_maintain_time, expected_type=type_hints["instance_maintain_time"])
+            check_type(argname="argument instance_name", value=instance_name, expected_type=type_hints["instance_name"])
+            check_type(argname="argument password", value=password, expected_type=type_hints["password"])
+            check_type(argname="argument period", value=period, expected_type=type_hints["period"])
+            check_type(argname="argument period_unit", value=period_unit, expected_type=type_hints["period_unit"])
+            check_type(argname="argument product_type", value=product_type, expected_type=type_hints["product_type"])
+            check_type(argname="argument resource_group_id", value=resource_group_id, expected_type=type_hints["resource_group_id"])
+            check_type(argname="argument secondary_zone_id", value=secondary_zone_id, expected_type=type_hints["secondary_zone_id"])
+            check_type(argname="argument security_group_id", value=security_group_id, expected_type=type_hints["security_group_id"])
+            check_type(argname="argument ssl_enabled", value=ssl_enabled, expected_type=type_hints["ssl_enabled"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
+            check_type(argname="argument vpc_id", value=vpc_id, expected_type=type_hints["vpc_id"])
+            check_type(argname="argument vpc_password_free", value=vpc_password_free, expected_type=type_hints["vpc_password_free"])
+            check_type(argname="argument v_switch_id", value=v_switch_id, expected_type=type_hints["v_switch_id"])
+            check_type(argname="argument zone_id", value=zone_id, expected_type=type_hints["zone_id"])
         self._values: typing.Dict[str, typing.Any] = {}
         if auto_pay is not None:
             self._values["auto_pay"] = auto_pay
         if auto_renew_duration is not None:
             self._values["auto_renew_duration"] = auto_renew_duration
         if backup_policy is not None:
             self._values["backup_policy"] = backup_policy
@@ -4585,14 +5088,16 @@
             self._values["instance_maintain_time"] = instance_maintain_time
         if instance_name is not None:
             self._values["instance_name"] = instance_name
         if password is not None:
             self._values["password"] = password
         if period is not None:
             self._values["period"] = period
+        if period_unit is not None:
+            self._values["period_unit"] = period_unit
         if product_type is not None:
             self._values["product_type"] = product_type
         if resource_group_id is not None:
             self._values["resource_group_id"] = resource_group_id
         if secondary_zone_id is not None:
             self._values["secondary_zone_id"] = secondary_zone_id
         if security_group_id is not None:
@@ -4737,14 +5242,29 @@
         '''
         :Property: period: The period of order, when choose Prepaid required.optional value 1-9, 12, 24, 36, 60 Unit in month.
         '''
         result = self._values.get("period")
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], result)
 
     @builtins.property
+    def period_unit(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
+        '''
+        :Property:
+
+        periodUnit: The unit of the subscription duration. Valid values:
+        Month
+        Year
+        Default value: Month.
+        '''
+        result = self._values.get("period_unit")
+        return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], result)
+
+    @builtins.property
     def product_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: productType: Product type. Valid values:Local: Community Edition(Local) or Enhanced Edition(Local)Tair_rdb: Performance Enhanced(Cloud Disk)Tair_scm: Persistent Memory(Cloud Disk)Tair_essd: Capacity Storage(Cloud Disk)OnECS: Community Edition(Cloud Disk)
         '''
         result = self._values.get("product_type")
@@ -4867,142 +5387,166 @@
 ):
     '''A ROS template type:  ``ALIYUN::REDIS::Whitelist``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosWhitelistProps",
+        props: typing.Union["RosWhitelistProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::REDIS::Whitelist``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosWhitelist.__init__)
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
+            type_hints = typing.get_type_hints(RosWhitelist._render_properties)
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
     @jsii.member(jsii_name="attrSecurityIpGroupAttribute")
     def attr_security_ip_group_attribute(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: SecurityIpGroupAttribute: The default is empty. For distinguishing between different attribute values, the console will not display the value of hidden whitelist packet.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrSecurityIpGroupAttribute"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrSecurityIpGroupName")
     def attr_security_ip_group_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: SecurityIpGroupName: Whitelist group
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrSecurityIpGroupName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrSecurityIps")
     def attr_security_ips(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: SecurityIps: IP address whitelist to be modified
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrSecurityIps"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosWhitelist, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="instanceId")
     def instance_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: instanceId: Instance ID (globally unique)
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "instanceId"))
 
     @instance_id.setter
     def instance_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosWhitelist, "instance_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "instanceId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="securityIps")
     def security_ips(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: securityIps: IP address whitelist to be modified
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "securityIps"))
 
     @security_ips.setter
     def security_ips(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosWhitelist, "security_ips").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "securityIps", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="securityIpGroupAttribute")
     def security_ip_group_attribute(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: securityIpGroupAttribute: The default is empty. For distinguishing between different attribute values, the console will not display the value of hidden whitelist packet.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "securityIpGroupAttribute"))
 
     @security_ip_group_attribute.setter
     def security_ip_group_attribute(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosWhitelist, "security_ip_group_attribute").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "securityIpGroupAttribute", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="securityIpGroupName")
     def security_ip_group_name(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: securityIpGroupName: Whitelist group
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "securityIpGroupName"))
 
     @security_ip_group_name.setter
     def security_ip_group_name(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosWhitelist, "security_ip_group_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "securityIpGroupName", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-redis.RosWhitelistProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -5024,14 +5568,20 @@
         '''Properties for defining a ``ALIYUN::REDIS::Whitelist``.
 
         :param instance_id: 
         :param security_ips: 
         :param security_ip_group_attribute: 
         :param security_ip_group_name: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosWhitelistProps.__init__)
+            check_type(argname="argument instance_id", value=instance_id, expected_type=type_hints["instance_id"])
+            check_type(argname="argument security_ips", value=security_ips, expected_type=type_hints["security_ips"])
+            check_type(argname="argument security_ip_group_attribute", value=security_ip_group_attribute, expected_type=type_hints["security_ip_group_attribute"])
+            check_type(argname="argument security_ip_group_name", value=security_ip_group_name, expected_type=type_hints["security_ip_group_name"])
         self._values: typing.Dict[str, typing.Any] = {
             "instance_id": instance_id,
             "security_ips": security_ips,
         }
         if security_ip_group_attribute is not None:
             self._values["security_ip_group_attribute"] = security_ip_group_attribute
         if security_ip_group_name is not None:
@@ -5094,46 +5644,52 @@
 ):
     '''A ROS resource type:  ``ALIYUN::REDIS::Whitelist``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "WhitelistProps",
+        props: typing.Union["WhitelistProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::REDIS::Whitelist``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(Whitelist.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrSecurityIpGroupAttribute")
     def attr_security_ip_group_attribute(self) -> ros_cdk_core.IResolvable:
         '''Attribute SecurityIpGroupAttribute: The default is empty.
 
         For distinguishing between different attribute values, the console will not display the value of hidden whitelist packet.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrSecurityIpGroupAttribute"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrSecurityIpGroupName")
     def attr_security_ip_group_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute SecurityIpGroupName: Whitelist group.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrSecurityIpGroupName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrSecurityIps")
     def attr_security_ips(self) -> ros_cdk_core.IResolvable:
         '''Attribute SecurityIps: IP address whitelist to be modified.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrSecurityIps"))
 
 
 @jsii.data_type(
@@ -5158,14 +5714,20 @@
         '''Properties for defining a ``ALIYUN::REDIS::Whitelist``.
 
         :param instance_id: Property instanceId: Instance ID (globally unique).
         :param security_ips: Property securityIps: IP address whitelist to be modified.
         :param security_ip_group_attribute: Property securityIpGroupAttribute: The default is empty. For distinguishing between different attribute values, the console will not display the value of hidden whitelist packet.
         :param security_ip_group_name: Property securityIpGroupName: Whitelist group.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(WhitelistProps.__init__)
+            check_type(argname="argument instance_id", value=instance_id, expected_type=type_hints["instance_id"])
+            check_type(argname="argument security_ips", value=security_ips, expected_type=type_hints["security_ips"])
+            check_type(argname="argument security_ip_group_attribute", value=security_ip_group_attribute, expected_type=type_hints["security_ip_group_attribute"])
+            check_type(argname="argument security_ip_group_name", value=security_ip_group_name, expected_type=type_hints["security_ip_group_name"])
         self._values: typing.Dict[str, typing.Any] = {
             "instance_id": instance_id,
             "security_ips": security_ips,
         }
         if security_ip_group_attribute is not None:
             self._values["security_ip_group_attribute"] = security_ip_group_attribute
         if security_ip_group_name is not None:
```

### Comparing `ros-cdk-redis-1.0.8/src/ros_cdk_redis.egg-info/PKG-INFO` & `ros-cdk-redis-1.0.9/src/ros_cdk_redis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-redis
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS REDIS Construct Library
```

