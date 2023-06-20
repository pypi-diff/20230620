# Comparing `tmp/ros-cdk-tsdb-1.0.8.tar.gz` & `tmp/ros-cdk-tsdb-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-tsdb-1.0.8.tar", last modified: Thu Jul 14 02:22:23 2022, max compression
+gzip compressed data, was "dist/ros-cdk-tsdb-1.0.9.tar", last modified: Fri Sep 23 11:41:25 2022, max compression
```

## Comparing `ros-cdk-tsdb-1.0.8.tar` & `ros-cdk-tsdb-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:22:23.000000 ros-cdk-tsdb-1.0.8/
--rw-r--r--   0 root         (0) root         (0)    10279 2022-07-14 02:22:22.000000 ros-cdk-tsdb-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2022-07-14 02:22:22.000000 ros-cdk-tsdb-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2022-07-14 02:22:22.000000 ros-cdk-tsdb-1.0.8/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1244 2022-07-14 02:22:23.000000 ros-cdk-tsdb-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      182 2022-07-14 02:22:22.000000 ros-cdk-tsdb-1.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)      106 2022-07-14 02:22:22.000000 ros-cdk-tsdb-1.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-07-14 02:22:23.000000 ros-cdk-tsdb-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1800 2022-07-14 02:22:22.000000 ros-cdk-tsdb-1.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:22:23.000000 ros-cdk-tsdb-1.0.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:22:23.000000 ros-cdk-tsdb-1.0.8/src/ros_cdk_tsdb/
--rw-r--r--   0 root         (0) root         (0)    64186 2022-07-14 02:22:22.000000 ros-cdk-tsdb-1.0.8/src/ros_cdk_tsdb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:22:23.000000 ros-cdk-tsdb-1.0.8/src/ros_cdk_tsdb/_jsii/
--rw-r--r--   0 root         (0) root         (0)      372 2022-07-14 02:22:22.000000 ros-cdk-tsdb-1.0.8/src/ros_cdk_tsdb/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    47968 2022-07-14 02:22:22.000000 ros-cdk-tsdb-1.0.8/src/ros_cdk_tsdb/_jsii/ros-cdk-tsdb@1.0.8.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:22:22.000000 ros-cdk-tsdb-1.0.8/src/ros_cdk_tsdb/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:22:23.000000 ros-cdk-tsdb-1.0.8/src/ros_cdk_tsdb.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1244 2022-07-14 02:22:23.000000 ros-cdk-tsdb-1.0.8/src/ros_cdk_tsdb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      410 2022-07-14 02:22:23.000000 ros-cdk-tsdb-1.0.8/src/ros_cdk_tsdb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:22:23.000000 ros-cdk-tsdb-1.0.8/src/ros_cdk_tsdb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2022-07-14 02:22:23.000000 ros-cdk-tsdb-1.0.8/src/ros_cdk_tsdb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2022-07-14 02:22:23.000000 ros-cdk-tsdb-1.0.8/src/ros_cdk_tsdb.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:41:24.000000 ros-cdk-tsdb-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)    10279 2022-09-23 11:41:24.000000 ros-cdk-tsdb-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-09-23 11:41:24.000000 ros-cdk-tsdb-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2022-09-23 11:41:24.000000 ros-cdk-tsdb-1.0.9/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1244 2022-09-23 11:41:24.000000 ros-cdk-tsdb-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      182 2022-09-23 11:41:24.000000 ros-cdk-tsdb-1.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      236 2022-09-23 11:41:24.000000 ros-cdk-tsdb-1.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-09-23 11:41:24.000000 ros-cdk-tsdb-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1829 2022-09-23 11:41:24.000000 ros-cdk-tsdb-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:41:24.000000 ros-cdk-tsdb-1.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:41:24.000000 ros-cdk-tsdb-1.0.9/src/ros_cdk_tsdb/
+-rw-r--r--   0 root         (0) root         (0)    77178 2022-09-23 11:41:24.000000 ros-cdk-tsdb-1.0.9/src/ros_cdk_tsdb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:41:24.000000 ros-cdk-tsdb-1.0.9/src/ros_cdk_tsdb/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      406 2022-09-23 11:41:24.000000 ros-cdk-tsdb-1.0.9/src/ros_cdk_tsdb/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    48036 2022-09-23 11:41:24.000000 ros-cdk-tsdb-1.0.9/src/ros_cdk_tsdb/_jsii/ros-cdk-tsdb@1.0.9.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 11:41:24.000000 ros-cdk-tsdb-1.0.9/src/ros_cdk_tsdb/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:41:24.000000 ros-cdk-tsdb-1.0.9/src/ros_cdk_tsdb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1244 2022-09-23 11:41:24.000000 ros-cdk-tsdb-1.0.9/src/ros_cdk_tsdb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      410 2022-09-23 11:41:24.000000 ros-cdk-tsdb-1.0.9/src/ros_cdk_tsdb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 11:41:24.000000 ros-cdk-tsdb-1.0.9/src/ros_cdk_tsdb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2022-09-23 11:41:24.000000 ros-cdk-tsdb-1.0.9/src/ros_cdk_tsdb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2022-09-23 11:41:24.000000 ros-cdk-tsdb-1.0.9/src/ros_cdk_tsdb.egg-info/top_level.txt
```

### Comparing `ros-cdk-tsdb-1.0.8/LICENSE` & `ros-cdk-tsdb-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-tsdb-1.0.8/PKG-INFO` & `ros-cdk-tsdb-1.0.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-tsdb
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS TSDB Construct Library
```

### Comparing `ros-cdk-tsdb-1.0.8/setup.py` & `ros-cdk-tsdb-1.0.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-tsdb",
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
         "ros_cdk_tsdb",
         "ros_cdk_tsdb._jsii"
     ],
     "package_data": {
         "ros_cdk_tsdb._jsii": [
-            "ros-cdk-tsdb@1.0.8.jsii.tgz"
+            "ros-cdk-tsdb@1.0.9.jsii.tgz"
         ],
         "ros_cdk_tsdb": [
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

### Comparing `ros-cdk-tsdb-1.0.8/src/ros_cdk_tsdb/__init__.py` & `ros-cdk-tsdb-1.0.9/src/ros_cdk_tsdb/__init__.py`

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
 
 
 class HiTSDBInstance(
     ros_cdk_core.Resource,
@@ -29,67 +31,73 @@
 ):
     '''A ROS resource type:  ``ALIYUN::TSDB::HiTSDBInstance``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "HiTSDBInstanceProps",
+        props: typing.Union["HiTSDBInstanceProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::TSDB::HiTSDBInstance``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(HiTSDBInstance.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrConnectionString")
     def attr_connection_string(self) -> ros_cdk_core.IResolvable:
         '''Attribute ConnectionString: Connection string of the instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrConnectionString"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrEngineType")
     def attr_engine_type(self) -> ros_cdk_core.IResolvable:
         '''Attribute EngineType: Engine type of the instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrEngineType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInstanceId")
     def attr_instance_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute InstanceId: The ID of the instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInstanceId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrOrderId")
     def attr_order_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute OrderId: Order id of created instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrOrderId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPublicConnectionString")
     def attr_public_connection_string(self) -> ros_cdk_core.IResolvable:
         '''Attribute PublicConnectionString: Public connection string of the instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPublicConnectionString"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrReverseVpcIp")
     def attr_reverse_vpc_ip(self) -> ros_cdk_core.IResolvable:
         '''Attribute ReverseVpcIp: Reverse vpc ip of the instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrReverseVpcIp"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrReverseVpcPort")
     def attr_reverse_vpc_port(self) -> ros_cdk_core.IResolvable:
         '''Attribute ReverseVpcPort: Reverse vpc port of the instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrReverseVpcPort"))
 
 
 @jsii.data_type(
@@ -135,14 +143,27 @@
         :param disk_category: Property diskCategory: The category of disk.
         :param duration: Property duration: The validity period of the instance. This parameter is valid only when the PayType parameter is set to PREPAY. Default value: 1.
         :param instance_alias: Property instanceAlias: The alias of the instance.
         :param pay_type: Property payType: The billing method. Valid values: POSTPAY and PREPAY. The POSTPAY value indicates the pay-as-you-go method, and the PREPAY value indicates the subscription method. Default POSTPAY
         :param pricing_cycle: Property pricingCycle: The unit of the validity period. This parameter is valid only when the PayType parameter is set to PREPAY. Default value: Month.
         :param security_ip_list: Property securityIpList: List of the IP patterns.For example, ["127.0.0.1", "192.168.0.1/24"].
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(HiTSDBInstanceProps.__init__)
+            check_type(argname="argument instance_class", value=instance_class, expected_type=type_hints["instance_class"])
+            check_type(argname="argument instance_storage", value=instance_storage, expected_type=type_hints["instance_storage"])
+            check_type(argname="argument vpc_id", value=vpc_id, expected_type=type_hints["vpc_id"])
+            check_type(argname="argument v_switch_id", value=v_switch_id, expected_type=type_hints["v_switch_id"])
+            check_type(argname="argument zone_id", value=zone_id, expected_type=type_hints["zone_id"])
+            check_type(argname="argument disk_category", value=disk_category, expected_type=type_hints["disk_category"])
+            check_type(argname="argument duration", value=duration, expected_type=type_hints["duration"])
+            check_type(argname="argument instance_alias", value=instance_alias, expected_type=type_hints["instance_alias"])
+            check_type(argname="argument pay_type", value=pay_type, expected_type=type_hints["pay_type"])
+            check_type(argname="argument pricing_cycle", value=pricing_cycle, expected_type=type_hints["pricing_cycle"])
+            check_type(argname="argument security_ip_list", value=security_ip_list, expected_type=type_hints["security_ip_list"])
         self._values: typing.Dict[str, typing.Any] = {
             "instance_class": instance_class,
             "instance_storage": instance_storage,
             "vpc_id": vpc_id,
             "v_switch_id": v_switch_id,
             "zone_id": zone_id,
         }
@@ -283,37 +304,43 @@
 ):
     '''A ROS resource type:  ``ALIYUN::TSDB::InfluxDBDatabase``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "InfluxDBDatabaseProps",
+        props: typing.Union["InfluxDBDatabaseProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::TSDB::InfluxDBDatabase``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(InfluxDBDatabase.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDbName")
     def attr_db_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute DBName: The name of database.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDbName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInstanceId")
     def attr_instance_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute InstanceId: The ID of TSDB for InfluxDB.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInstanceId"))
 
 
 @jsii.data_type(
@@ -329,14 +356,18 @@
         instance_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
         '''Properties for defining a ``ALIYUN::TSDB::InfluxDBDatabase``.
 
         :param db_name: Property dbName: The name of database. The name can at most be 64 characters in length and can contain lowercase letters, digits, and underscores (_). It must start with a letter and end with a letter or digit.
         :param instance_id: Property instanceId: The ID of TSDB for InfluxDB.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(InfluxDBDatabaseProps.__init__)
+            check_type(argname="argument db_name", value=db_name, expected_type=type_hints["db_name"])
+            check_type(argname="argument instance_id", value=instance_id, expected_type=type_hints["instance_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "db_name": db_name,
             "instance_id": instance_id,
         }
 
     @builtins.property
     def db_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
@@ -374,43 +405,49 @@
 ):
     '''A ROS resource type:  ``ALIYUN::TSDB::InfluxDBUser``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "InfluxDBUserProps",
+        props: typing.Union["InfluxDBUserProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::TSDB::InfluxDBUser``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(InfluxDBUser.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInstanceId")
     def attr_instance_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute InstanceId: The ID of TSDB for InfluxDB.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInstanceId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrUserName")
     def attr_user_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute UserName: The name of user.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrUserName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrUserType")
     def attr_user_type(self) -> ros_cdk_core.IResolvable:
         '''Attribute UserType: The type of user.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrUserType"))
 
 
 @jsii.data_type(
@@ -428,24 +465,31 @@
     def __init__(
         self,
         *,
         instance_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         password: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         user_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         user_type: typing.Union[builtins.str, ros_cdk_core.IResolvable],
-        database_permissions: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosInfluxDBUser.DatabasePermissionsProperty"]]]] = None,
+        database_permissions: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosInfluxDBUser.DatabasePermissionsProperty", typing.Dict[str, typing.Any]]]]]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::TSDB::InfluxDBUser``.
 
         :param instance_id: Property instanceId: The ID of TSDB for InfluxDB.
         :param password: Property password: The password must be 8 to 32 characters in length and contain letters, digits, and special characters.!@#$%^&*()_+-=.
         :param user_name: Property userName: The name of user. The name can at must be 16 characters in length and can contain lowercase letters, digits, and underscores (_). It must start with a letter and end with a letter or digit.
         :param user_type: Property userType: The type of user. Valid values: normal: normal user admin: administrator user.
         :param database_permissions: Property databasePermissions: The list of databases that the user can access. If the user type is admin, do not specify this parameter.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(InfluxDBUserProps.__init__)
+            check_type(argname="argument instance_id", value=instance_id, expected_type=type_hints["instance_id"])
+            check_type(argname="argument password", value=password, expected_type=type_hints["password"])
+            check_type(argname="argument user_name", value=user_name, expected_type=type_hints["user_name"])
+            check_type(argname="argument user_type", value=user_type, expected_type=type_hints["user_type"])
+            check_type(argname="argument database_permissions", value=database_permissions, expected_type=type_hints["database_permissions"])
         self._values: typing.Dict[str, typing.Any] = {
             "instance_id": instance_id,
             "password": password,
             "user_name": user_name,
             "user_type": user_type,
         }
         if database_permissions is not None:
@@ -517,113 +561,125 @@
 ):
     '''A ROS template type:  ``ALIYUN::TSDB::HiTSDBInstance``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosHiTSDBInstanceProps",
+        props: typing.Union["RosHiTSDBInstanceProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::TSDB::HiTSDBInstance``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosHiTSDBInstance.__init__)
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
+            type_hints = typing.get_type_hints(RosHiTSDBInstance._render_properties)
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
     @jsii.member(jsii_name="attrConnectionString")
     def attr_connection_string(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ConnectionString: Connection string of the instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrConnectionString"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrEngineType")
     def attr_engine_type(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: EngineType: Engine type of the instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrEngineType"))
 
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
     @jsii.member(jsii_name="attrOrderId")
     def attr_order_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: OrderId: Order id of created instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrOrderId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPublicConnectionString")
     def attr_public_connection_string(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: PublicConnectionString: Public connection string of the instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPublicConnectionString"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrReverseVpcIp")
     def attr_reverse_vpc_ip(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ReverseVpcIp: Reverse vpc ip of the instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrReverseVpcIp"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrReverseVpcPort")
     def attr_reverse_vpc_port(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ReverseVpcPort: Reverse vpc port of the instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrReverseVpcPort"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosHiTSDBInstance, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="instanceClass")
     def instance_class(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         instanceClass: The type of the instance. For more information, see Instance types:
         tsdb.1x.basic: Basic Edition I
@@ -637,176 +693,209 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "instanceClass"))
 
     @instance_class.setter
     def instance_class(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosHiTSDBInstance, "instance_class").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "instanceClass", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="instanceStorage")
     def instance_storage(self) -> typing.Union[jsii.Number, ros_cdk_core.IResolvable]:
         '''
         :Property: instanceStorage: The storage capacity of the instance. Unit: GB. For example, the value 50 indicates 50 GB.
         '''
         return typing.cast(typing.Union[jsii.Number, ros_cdk_core.IResolvable], jsii.get(self, "instanceStorage"))
 
     @instance_storage.setter
     def instance_storage(
         self,
         value: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosHiTSDBInstance, "instance_storage").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "instanceStorage", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vpcId")
     def vpc_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: vpcId: The ID of the virtual private cloud (VPC) that is connected to the instance.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "vpcId"))
 
     @vpc_id.setter
     def vpc_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosHiTSDBInstance, "vpc_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "vpcId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vSwitchId")
     def v_switch_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: vSwitchId: The ID of the VSwitch in the specified VPC.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "vSwitchId"))
 
     @v_switch_id.setter
     def v_switch_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosHiTSDBInstance, "v_switch_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "vSwitchId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="zoneId")
     def zone_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: zoneId: The zone ID of the instance.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "zoneId"))
 
     @zone_id.setter
     def zone_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosHiTSDBInstance, "zone_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "zoneId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="diskCategory")
     def disk_category(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: diskCategory: The category of disk.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "diskCategory"))
 
     @disk_category.setter
     def disk_category(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosHiTSDBInstance, "disk_category").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "diskCategory", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="duration")
     def duration(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: duration: The validity period of the instance. This parameter is valid only when the PayType parameter is set to PREPAY. Default value: 1.
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "duration"))
 
     @duration.setter
     def duration(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosHiTSDBInstance, "duration").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "duration", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="instanceAlias")
     def instance_alias(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: instanceAlias: The alias of the instance.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "instanceAlias"))
 
     @instance_alias.setter
     def instance_alias(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosHiTSDBInstance, "instance_alias").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "instanceAlias", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="payType")
     def pay_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: payType: The billing method. Valid values: POSTPAY and PREPAY. The POSTPAY value indicates the pay-as-you-go method, and the PREPAY value indicates the subscription method. Default POSTPAY
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "payType"))
 
     @pay_type.setter
     def pay_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosHiTSDBInstance, "pay_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "payType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="pricingCycle")
     def pricing_cycle(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: pricingCycle: The unit of the validity period. This parameter is valid only when the PayType parameter is set to PREPAY. Default value: Month.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "pricingCycle"))
 
     @pricing_cycle.setter
     def pricing_cycle(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosHiTSDBInstance, "pricing_cycle").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "pricingCycle", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="securityIpList")
     def security_ip_list(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]]:
         '''
         :Property: securityIpList: List of the IP patterns.For example, ["127.0.0.1", "192.168.0.1/24"]
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]], jsii.get(self, "securityIpList"))
 
     @security_ip_list.setter
     def security_ip_list(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosHiTSDBInstance, "security_ip_list").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "securityIpList", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-tsdb.RosHiTSDBInstanceProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -849,14 +938,27 @@
         :param disk_category: 
         :param duration: 
         :param instance_alias: 
         :param pay_type: 
         :param pricing_cycle: 
         :param security_ip_list: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosHiTSDBInstanceProps.__init__)
+            check_type(argname="argument instance_class", value=instance_class, expected_type=type_hints["instance_class"])
+            check_type(argname="argument instance_storage", value=instance_storage, expected_type=type_hints["instance_storage"])
+            check_type(argname="argument vpc_id", value=vpc_id, expected_type=type_hints["vpc_id"])
+            check_type(argname="argument v_switch_id", value=v_switch_id, expected_type=type_hints["v_switch_id"])
+            check_type(argname="argument zone_id", value=zone_id, expected_type=type_hints["zone_id"])
+            check_type(argname="argument disk_category", value=disk_category, expected_type=type_hints["disk_category"])
+            check_type(argname="argument duration", value=duration, expected_type=type_hints["duration"])
+            check_type(argname="argument instance_alias", value=instance_alias, expected_type=type_hints["instance_alias"])
+            check_type(argname="argument pay_type", value=pay_type, expected_type=type_hints["pay_type"])
+            check_type(argname="argument pricing_cycle", value=pricing_cycle, expected_type=type_hints["pricing_cycle"])
+            check_type(argname="argument security_ip_list", value=security_ip_list, expected_type=type_hints["security_ip_list"])
         self._values: typing.Dict[str, typing.Any] = {
             "instance_class": instance_class,
             "instance_storage": instance_storage,
             "vpc_id": vpc_id,
             "v_switch_id": v_switch_id,
             "zone_id": zone_id,
         }
@@ -1006,100 +1108,118 @@
 ):
     '''A ROS template type:  ``ALIYUN::TSDB::InfluxDBDatabase``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosInfluxDBDatabaseProps",
+        props: typing.Union["RosInfluxDBDatabaseProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::TSDB::InfluxDBDatabase``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosInfluxDBDatabase.__init__)
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
+            type_hints = typing.get_type_hints(RosInfluxDBDatabase._render_properties)
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
     @jsii.member(jsii_name="attrDbName")
     def attr_db_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: DBName: The name of database.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDbName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInstanceId")
     def attr_instance_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: InstanceId: The ID of TSDB for InfluxDB.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInstanceId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dbName")
     def db_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: dbName: The name of database. The name can at most be 64 characters in length and can contain lowercase letters, digits, and underscores (_). It must start with a letter and end with a letter or digit.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "dbName"))
 
     @db_name.setter
     def db_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInfluxDBDatabase, "db_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dbName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInfluxDBDatabase, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="instanceId")
     def instance_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: instanceId: The ID of TSDB for InfluxDB.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "instanceId"))
 
     @instance_id.setter
     def instance_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInfluxDBDatabase, "instance_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "instanceId", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-tsdb.RosInfluxDBDatabaseProps",
     jsii_struct_bases=[],
     name_mapping={"db_name": "dbName", "instance_id": "instanceId"},
@@ -1112,14 +1232,18 @@
         instance_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
         '''Properties for defining a ``ALIYUN::TSDB::InfluxDBDatabase``.
 
         :param db_name: 
         :param instance_id: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosInfluxDBDatabaseProps.__init__)
+            check_type(argname="argument db_name", value=db_name, expected_type=type_hints["db_name"])
+            check_type(argname="argument instance_id", value=instance_id, expected_type=type_hints["instance_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "db_name": db_name,
             "instance_id": instance_id,
         }
 
     @builtins.property
     def db_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
@@ -1158,127 +1282,148 @@
 ):
     '''A ROS template type:  ``ALIYUN::TSDB::InfluxDBUser``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosInfluxDBUserProps",
+        props: typing.Union["RosInfluxDBUserProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::TSDB::InfluxDBUser``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosInfluxDBUser.__init__)
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
+            type_hints = typing.get_type_hints(RosInfluxDBUser._render_properties)
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
         :Attribute: InstanceId: The ID of TSDB for InfluxDB.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInstanceId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrUserName")
     def attr_user_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: UserName: The name of user.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrUserName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrUserType")
     def attr_user_type(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: UserType: The type of user.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrUserType"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosInfluxDBUser, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="instanceId")
     def instance_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: instanceId: The ID of TSDB for InfluxDB.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "instanceId"))
 
     @instance_id.setter
     def instance_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInfluxDBUser, "instance_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "instanceId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="password")
     def password(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :: #$%^&*()_+-=
         :Property: password: The password must be 8 to 32 characters in length and contain letters, digits, and special characters.!
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "password"))
 
     @password.setter
     def password(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInfluxDBUser, "password").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "password", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="userName")
     def user_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: userName: The name of user. The name can at must be 16 characters in length and can contain lowercase letters, digits, and underscores (_). It must start with a letter and end with a letter or digit.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "userName"))
 
     @user_name.setter
     def user_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInfluxDBUser, "user_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "userName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="userType")
     def user_type(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         userType: The type of user. Valid values:
         normal: normal user
@@ -1287,31 +1432,37 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "userType"))
 
     @user_type.setter
     def user_type(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInfluxDBUser, "user_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "userType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="databasePermissions")
     def database_permissions(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosInfluxDBUser.DatabasePermissionsProperty"]]]]:
         '''
         :Property: databasePermissions: The list of databases that the user can access. If the user type is admin, do not specify this parameter.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosInfluxDBUser.DatabasePermissionsProperty"]]]], jsii.get(self, "databasePermissions"))
 
     @database_permissions.setter
     def database_permissions(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosInfluxDBUser.DatabasePermissionsProperty"]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInfluxDBUser, "database_permissions").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "databasePermissions", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-tsdb.RosInfluxDBUser.DatabasePermissionsProperty",
         jsii_struct_bases=[],
         name_mapping={"db_name": "dbName", "permission": "permission"},
     )
@@ -1322,14 +1473,18 @@
             db_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             permission: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         ) -> None:
             '''
             :param db_name: 
             :param permission: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosInfluxDBUser.DatabasePermissionsProperty.__init__)
+                check_type(argname="argument db_name", value=db_name, expected_type=type_hints["db_name"])
+                check_type(argname="argument permission", value=permission, expected_type=type_hints["permission"])
             self._values: typing.Dict[str, typing.Any] = {
                 "db_name": db_name,
                 "permission": permission,
             }
 
         @builtins.property
         def db_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
@@ -1376,24 +1531,31 @@
     def __init__(
         self,
         *,
         instance_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         password: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         user_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         user_type: typing.Union[builtins.str, ros_cdk_core.IResolvable],
-        database_permissions: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosInfluxDBUser.DatabasePermissionsProperty]]]] = None,
+        database_permissions: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosInfluxDBUser.DatabasePermissionsProperty, typing.Dict[str, typing.Any]]]]]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::TSDB::InfluxDBUser``.
 
         :param instance_id: 
         :param password: 
         :param user_name: 
         :param user_type: 
         :param database_permissions: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosInfluxDBUserProps.__init__)
+            check_type(argname="argument instance_id", value=instance_id, expected_type=type_hints["instance_id"])
+            check_type(argname="argument password", value=password, expected_type=type_hints["password"])
+            check_type(argname="argument user_name", value=user_name, expected_type=type_hints["user_name"])
+            check_type(argname="argument user_type", value=user_type, expected_type=type_hints["user_type"])
+            check_type(argname="argument database_permissions", value=database_permissions, expected_type=type_hints["database_permissions"])
         self._values: typing.Dict[str, typing.Any] = {
             "instance_id": instance_id,
             "password": password,
             "user_name": user_name,
             "user_type": user_type,
         }
         if database_permissions is not None:
```

### Comparing `ros-cdk-tsdb-1.0.8/src/ros_cdk_tsdb.egg-info/PKG-INFO` & `ros-cdk-tsdb-1.0.9/src/ros_cdk_tsdb.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-tsdb
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS TSDB Construct Library
```

