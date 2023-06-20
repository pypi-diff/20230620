# Comparing `tmp/ros-cdk-gpdb-1.0.8.tar.gz` & `tmp/ros-cdk-gpdb-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-gpdb-1.0.8.tar", last modified: Thu Jul 14 02:29:28 2022, max compression
+gzip compressed data, was "dist/ros-cdk-gpdb-1.0.9.tar", last modified: Fri Sep 23 11:16:59 2022, max compression
```

## Comparing `ros-cdk-gpdb-1.0.8.tar` & `ros-cdk-gpdb-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:29:28.000000 ros-cdk-gpdb-1.0.8/
--rw-r--r--   0 root         (0) root         (0)    10279 2022-07-14 02:29:27.000000 ros-cdk-gpdb-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2022-07-14 02:29:27.000000 ros-cdk-gpdb-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2022-07-14 02:29:27.000000 ros-cdk-gpdb-1.0.8/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1244 2022-07-14 02:29:28.000000 ros-cdk-gpdb-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      182 2022-07-14 02:29:27.000000 ros-cdk-gpdb-1.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)      106 2022-07-14 02:29:27.000000 ros-cdk-gpdb-1.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-07-14 02:29:28.000000 ros-cdk-gpdb-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1800 2022-07-14 02:29:27.000000 ros-cdk-gpdb-1.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:29:28.000000 ros-cdk-gpdb-1.0.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:29:28.000000 ros-cdk-gpdb-1.0.8/src/ros_cdk_gpdb/
--rw-r--r--   0 root         (0) root         (0)   113266 2022-07-14 02:29:27.000000 ros-cdk-gpdb-1.0.8/src/ros_cdk_gpdb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:29:28.000000 ros-cdk-gpdb-1.0.8/src/ros_cdk_gpdb/_jsii/
--rw-r--r--   0 root         (0) root         (0)      372 2022-07-14 02:29:27.000000 ros-cdk-gpdb-1.0.8/src/ros_cdk_gpdb/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    60731 2022-07-14 02:29:27.000000 ros-cdk-gpdb-1.0.8/src/ros_cdk_gpdb/_jsii/ros-cdk-gpdb@1.0.8.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:29:27.000000 ros-cdk-gpdb-1.0.8/src/ros_cdk_gpdb/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:29:28.000000 ros-cdk-gpdb-1.0.8/src/ros_cdk_gpdb.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1244 2022-07-14 02:29:27.000000 ros-cdk-gpdb-1.0.8/src/ros_cdk_gpdb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      410 2022-07-14 02:29:27.000000 ros-cdk-gpdb-1.0.8/src/ros_cdk_gpdb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:29:27.000000 ros-cdk-gpdb-1.0.8/src/ros_cdk_gpdb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2022-07-14 02:29:27.000000 ros-cdk-gpdb-1.0.8/src/ros_cdk_gpdb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2022-07-14 02:29:27.000000 ros-cdk-gpdb-1.0.8/src/ros_cdk_gpdb.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:16:59.000000 ros-cdk-gpdb-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)    10279 2022-09-23 11:16:59.000000 ros-cdk-gpdb-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-09-23 11:16:59.000000 ros-cdk-gpdb-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2022-09-23 11:16:59.000000 ros-cdk-gpdb-1.0.9/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1244 2022-09-23 11:16:59.000000 ros-cdk-gpdb-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      182 2022-09-23 11:16:59.000000 ros-cdk-gpdb-1.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      236 2022-09-23 11:16:59.000000 ros-cdk-gpdb-1.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-09-23 11:16:59.000000 ros-cdk-gpdb-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1829 2022-09-23 11:16:59.000000 ros-cdk-gpdb-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:16:59.000000 ros-cdk-gpdb-1.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:16:59.000000 ros-cdk-gpdb-1.0.9/src/ros_cdk_gpdb/
+-rw-r--r--   0 root         (0) root         (0)   136913 2022-09-23 11:16:59.000000 ros-cdk-gpdb-1.0.9/src/ros_cdk_gpdb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:16:59.000000 ros-cdk-gpdb-1.0.9/src/ros_cdk_gpdb/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      406 2022-09-23 11:16:59.000000 ros-cdk-gpdb-1.0.9/src/ros_cdk_gpdb/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    60493 2022-09-23 11:16:59.000000 ros-cdk-gpdb-1.0.9/src/ros_cdk_gpdb/_jsii/ros-cdk-gpdb@1.0.9.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 11:16:59.000000 ros-cdk-gpdb-1.0.9/src/ros_cdk_gpdb/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:16:59.000000 ros-cdk-gpdb-1.0.9/src/ros_cdk_gpdb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1244 2022-09-23 11:16:59.000000 ros-cdk-gpdb-1.0.9/src/ros_cdk_gpdb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      410 2022-09-23 11:16:59.000000 ros-cdk-gpdb-1.0.9/src/ros_cdk_gpdb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 11:16:59.000000 ros-cdk-gpdb-1.0.9/src/ros_cdk_gpdb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2022-09-23 11:16:59.000000 ros-cdk-gpdb-1.0.9/src/ros_cdk_gpdb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2022-09-23 11:16:59.000000 ros-cdk-gpdb-1.0.9/src/ros_cdk_gpdb.egg-info/top_level.txt
```

### Comparing `ros-cdk-gpdb-1.0.8/LICENSE` & `ros-cdk-gpdb-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-gpdb-1.0.8/PKG-INFO` & `ros-cdk-gpdb-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-gpdb
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS GPDB Construct Library
```

### Comparing `ros-cdk-gpdb-1.0.8/setup.py` & `ros-cdk-gpdb-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-gpdb",
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
         "ros_cdk_gpdb",
         "ros_cdk_gpdb._jsii"
     ],
     "package_data": {
         "ros_cdk_gpdb._jsii": [
-            "ros-cdk-gpdb@1.0.8.jsii.tgz"
+            "ros-cdk-gpdb@1.0.9.jsii.tgz"
         ],
         "ros_cdk_gpdb": [
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

### Comparing `ros-cdk-gpdb-1.0.8/src/ros_cdk_gpdb/__init__.py` & `ros-cdk-gpdb-1.0.9/src/ros_cdk_gpdb/__init__.py`

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
 
 
 class Account(
     ros_cdk_core.Resource,
@@ -29,37 +31,43 @@
 ):
     '''A ROS resource type:  ``ALIYUN::GPDB::Account``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "AccountProps",
+        props: typing.Union["AccountProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::GPDB::Account``.
 
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
     @jsii.member(jsii_name="attrDbInstanceId")
     def attr_db_instance_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute DBInstanceId: The ID of the instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDbInstanceId"))
 
 
 @jsii.data_type(
@@ -84,14 +92,20 @@
         '''Properties for defining a ``ALIYUN::GPDB::Account``.
 
         :param account_name: Property accountName: The name of the privileged account. The name can contain lowercase letters, digits, and underscores (_). The name must start with a lowercase letter and end with a lowercase letter or a digit. The name cannot start with gp. The name must be 2 to 16 characters in length.
         :param account_password: Property accountPassword: The password of the privileged account. The password must contain at least three of the following character types: uppercase letters, lowercase letters, digits, and special characters. Special characters include ! @ # $ % ^ & * ( ) _ + - = The password must be 8 to 32 characters in length.
         :param db_instance_id: Property dbInstanceId: The ID of the instance. Note You can call the DescribeDBInstances operation to query details of all AnalyticDB for PostgreSQL instances in a specific region, including instance IDs.
         :param account_description: Property accountDescription: The description of the privileged account.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(AccountProps.__init__)
+            check_type(argname="argument account_name", value=account_name, expected_type=type_hints["account_name"])
+            check_type(argname="argument account_password", value=account_password, expected_type=type_hints["account_password"])
+            check_type(argname="argument db_instance_id", value=db_instance_id, expected_type=type_hints["db_instance_id"])
+            check_type(argname="argument account_description", value=account_description, expected_type=type_hints["account_description"])
         self._values: typing.Dict[str, typing.Any] = {
             "account_name": account_name,
             "account_password": account_password,
             "db_instance_id": db_instance_id,
         }
         if account_description is not None:
             self._values["account_description"] = account_description
@@ -160,49 +174,55 @@
 ):
     '''A ROS resource type:  ``ALIYUN::GPDB::DBInstance``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "DBInstanceProps",
+        props: typing.Union["DBInstanceProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::GPDB::DBInstance``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(DBInstance.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrConnectionString")
     def attr_connection_string(self) -> ros_cdk_core.IResolvable:
         '''Attribute ConnectionString: The endpoint of the instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrConnectionString"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDbInstanceId")
     def attr_db_instance_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute DBInstanceId: The ID of the instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDbInstanceId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrOrderId")
     def attr_order_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute OrderId: The order ID of the instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrOrderId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPort")
     def attr_port(self) -> ros_cdk_core.IResolvable:
         '''Attribute Port: The port used to connect to the instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPort"))
 
 
 @jsii.data_type(
@@ -233,15 +253,15 @@
         v_switch_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         zone_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         db_instance_description: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         pay_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         period: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         period_unit: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         security_ip_list: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        tags: typing.Optional[typing.Sequence["RosDBInstance.TagsProperty"]] = None,
+        tags: typing.Optional[typing.Sequence[typing.Union["RosDBInstance.TagsProperty", typing.Dict[str, typing.Any]]]] = None,
         vpc_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::GPDB::DBInstance``.
 
         :param db_instance_class: Property dbInstanceClass: The instance type.
         :param db_instance_group_count: Property dbInstanceGroupCount: The number of compute nodes in the instance.
         :param engine_version: Property engineVersion: The version of the database engine.
@@ -251,14 +271,28 @@
         :param pay_type: Property payType: The billing method of the instance. Default value: Postpaid. Valid values: Postpaid: pay-as-you-go Prepaid: subscription
         :param period: Property period: The subscription period. While choose by pay by month, it could be from 1 to 11. While choose pay by year, it could be from 1 to 3.
         :param period_unit: Property periodUnit: Unit of subscription period, it could be Month/Year. Default value is Month.
         :param security_ip_list: Property securityIpList: The whitelist of IP addresses that are allowed to access the instance. Default value: 127.0.0.1.
         :param tags: Property tags: Tags to attach to instance. Max support 20 tags to add during create instance. Each tag with two properties Key and Value, and Key is required.
         :param vpc_id: Property vpcId: The VPC ID of the instance. If you set the InstanceNetworkType parameter to VPC, you must also specify the VPCId parameter. The specified region of the VPC must be the same as the RegionId value.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(DBInstanceProps.__init__)
+            check_type(argname="argument db_instance_class", value=db_instance_class, expected_type=type_hints["db_instance_class"])
+            check_type(argname="argument db_instance_group_count", value=db_instance_group_count, expected_type=type_hints["db_instance_group_count"])
+            check_type(argname="argument engine_version", value=engine_version, expected_type=type_hints["engine_version"])
+            check_type(argname="argument v_switch_id", value=v_switch_id, expected_type=type_hints["v_switch_id"])
+            check_type(argname="argument zone_id", value=zone_id, expected_type=type_hints["zone_id"])
+            check_type(argname="argument db_instance_description", value=db_instance_description, expected_type=type_hints["db_instance_description"])
+            check_type(argname="argument pay_type", value=pay_type, expected_type=type_hints["pay_type"])
+            check_type(argname="argument period", value=period, expected_type=type_hints["period"])
+            check_type(argname="argument period_unit", value=period_unit, expected_type=type_hints["period_unit"])
+            check_type(argname="argument security_ip_list", value=security_ip_list, expected_type=type_hints["security_ip_list"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
+            check_type(argname="argument vpc_id", value=vpc_id, expected_type=type_hints["vpc_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "db_instance_class": db_instance_class,
             "db_instance_group_count": db_instance_group_count,
             "engine_version": engine_version,
             "v_switch_id": v_switch_id,
             "zone_id": zone_id,
         }
@@ -417,49 +451,55 @@
 ):
     '''A ROS resource type:  ``ALIYUN::GPDB::ElasticDBInstance``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "ElasticDBInstanceProps",
+        props: typing.Union["ElasticDBInstanceProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::GPDB::ElasticDBInstance``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(ElasticDBInstance.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrConnectionString")
     def attr_connection_string(self) -> ros_cdk_core.IResolvable:
         '''Attribute ConnectionString: The endpoint of the instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrConnectionString"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDbInstanceId")
     def attr_db_instance_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute DBInstanceId: The ID of the instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDbInstanceId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrOrderId")
     def attr_order_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute OrderId: The order ID of the instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrOrderId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPort")
     def attr_port(self) -> ros_cdk_core.IResolvable:
         '''Attribute Port: The port used to connect to the instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPort"))
 
 
 @jsii.data_type(
@@ -502,15 +542,15 @@
         encryption_key: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         encryption_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         master_node_num: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         pay_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         period: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         period_unit: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         security_ip_list: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        tags: typing.Optional[typing.Sequence["RosElasticDBInstance.TagsProperty"]] = None,
+        tags: typing.Optional[typing.Sequence[typing.Union["RosElasticDBInstance.TagsProperty", typing.Dict[str, typing.Any]]]] = None,
         vpc_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::GPDB::ElasticDBInstance``.
 
         :param engine_version: Property engineVersion: The version of the database engine.
         :param instance_spec: Property instanceSpec: The specification of segment nodes. For example: 2C16G, 4C32G, 16C128G.
         :param seg_node_num: Property segNodeNum: The number of segment nodes. Minimum is 4, max is 512, step is 4.
@@ -526,14 +566,34 @@
         :param pay_type: Property payType: The billing method of the instance. Default value: Postpaid. Valid values: Postpaid: pay-as-you-go Prepaid: subscription
         :param period: Property period: The subscription period. While choose by pay by month, it could be from 1 to 11. While choose pay by year, it could be from 1 to 3.
         :param period_unit: Property periodUnit: Unit of subscription period, it could be Month/Year. Default value is Month.
         :param security_ip_list: Property securityIpList: The whitelist of IP addresses that are allowed to access the instance. Default value: 127.0.0.1.
         :param tags: Property tags: Tags to attach to instance. Max support 20 tags to add during create instance. Each tag with two properties Key and Value, and Key is required.
         :param vpc_id: Property vpcId: The VPC ID of the instance. If you set the InstanceNetworkType parameter to VPC, you must also specify the VPCId parameter. The specified region of the VPC must be the same as the RegionId value.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(ElasticDBInstanceProps.__init__)
+            check_type(argname="argument engine_version", value=engine_version, expected_type=type_hints["engine_version"])
+            check_type(argname="argument instance_spec", value=instance_spec, expected_type=type_hints["instance_spec"])
+            check_type(argname="argument seg_node_num", value=seg_node_num, expected_type=type_hints["seg_node_num"])
+            check_type(argname="argument seg_storage_type", value=seg_storage_type, expected_type=type_hints["seg_storage_type"])
+            check_type(argname="argument storage_size", value=storage_size, expected_type=type_hints["storage_size"])
+            check_type(argname="argument v_switch_id", value=v_switch_id, expected_type=type_hints["v_switch_id"])
+            check_type(argname="argument zone_id", value=zone_id, expected_type=type_hints["zone_id"])
+            check_type(argname="argument db_instance_category", value=db_instance_category, expected_type=type_hints["db_instance_category"])
+            check_type(argname="argument db_instance_description", value=db_instance_description, expected_type=type_hints["db_instance_description"])
+            check_type(argname="argument encryption_key", value=encryption_key, expected_type=type_hints["encryption_key"])
+            check_type(argname="argument encryption_type", value=encryption_type, expected_type=type_hints["encryption_type"])
+            check_type(argname="argument master_node_num", value=master_node_num, expected_type=type_hints["master_node_num"])
+            check_type(argname="argument pay_type", value=pay_type, expected_type=type_hints["pay_type"])
+            check_type(argname="argument period", value=period, expected_type=type_hints["period"])
+            check_type(argname="argument period_unit", value=period_unit, expected_type=type_hints["period_unit"])
+            check_type(argname="argument security_ip_list", value=security_ip_list, expected_type=type_hints["security_ip_list"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
+            check_type(argname="argument vpc_id", value=vpc_id, expected_type=type_hints["vpc_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "engine_version": engine_version,
             "instance_spec": instance_spec,
             "seg_node_num": seg_node_num,
             "seg_storage_type": seg_storage_type,
             "storage_size": storage_size,
             "v_switch_id": v_switch_id,
@@ -770,37 +830,43 @@
 ):
     '''A ROS resource type:  ``ALIYUN::GPDB::InstancePublicConnection``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "InstancePublicConnectionProps",
+        props: typing.Union["InstancePublicConnectionProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::GPDB::InstancePublicConnection``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(InstancePublicConnection.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrConnectionString")
     def attr_connection_string(self) -> ros_cdk_core.IResolvable:
         '''Attribute ConnectionString: The connection string of the instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrConnectionString"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDbInstanceId")
     def attr_db_instance_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute DBInstanceId: The ID of the instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDbInstanceId"))
 
 
 @jsii.data_type(
@@ -822,14 +888,19 @@
     ) -> None:
         '''Properties for defining a ``ALIYUN::GPDB::InstancePublicConnection``.
 
         :param connection_string_prefix: Property connectionStringPrefix: The endpoint that is used to connect to the specified database.
         :param db_instance_id: Property dbInstanceId: The ID of the instance.
         :param port: Property port: The port number of the instance.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(InstancePublicConnectionProps.__init__)
+            check_type(argname="argument connection_string_prefix", value=connection_string_prefix, expected_type=type_hints["connection_string_prefix"])
+            check_type(argname="argument db_instance_id", value=db_instance_id, expected_type=type_hints["db_instance_id"])
+            check_type(argname="argument port", value=port, expected_type=type_hints["port"])
         self._values: typing.Dict[str, typing.Any] = {
             "connection_string_prefix": connection_string_prefix,
             "db_instance_id": db_instance_id,
             "port": port,
         }
 
     @builtins.property
@@ -874,64 +945,73 @@
 ):
     '''A ROS template type:  ``ALIYUN::GPDB::Account``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosAccountProps",
+        props: typing.Union["RosAccountProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::GPDB::Account``.
 
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
     @jsii.member(jsii_name="attrDbInstanceId")
     def attr_db_instance_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: DBInstanceId: The ID of the instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDbInstanceId"))
 
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
 
         accountName: The name of the privileged account.
         The name can contain lowercase letters, digits, and underscores (_).
@@ -942,17 +1022,20 @@
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
 
 
 
@@ -969,17 +1052,20 @@
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
     @jsii.member(jsii_name="dbInstanceId")
     def db_instance_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         dbInstanceId: The ID of the instance.
         Note You can call the DescribeDBInstances operation to query details of all AnalyticDB for PostgreSQL instances in a specific
@@ -988,40 +1074,49 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "dbInstanceId"))
 
     @db_instance_id.setter
     def db_instance_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAccount, "db_instance_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dbInstanceId", value)
 
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
     @jsii.member(jsii_name="accountDescription")
     def account_description(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: accountDescription: The description of the privileged account.
         '''
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
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-gpdb.RosAccountProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -1043,14 +1138,20 @@
         '''Properties for defining a ``ALIYUN::GPDB::Account``.
 
         :param account_name: 
         :param account_password: 
         :param db_instance_id: 
         :param account_description: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosAccountProps.__init__)
+            check_type(argname="argument account_name", value=account_name, expected_type=type_hints["account_name"])
+            check_type(argname="argument account_password", value=account_password, expected_type=type_hints["account_password"])
+            check_type(argname="argument db_instance_id", value=db_instance_id, expected_type=type_hints["db_instance_id"])
+            check_type(argname="argument account_description", value=account_description, expected_type=type_hints["account_description"])
         self._values: typing.Dict[str, typing.Any] = {
             "account_name": account_name,
             "account_password": account_password,
             "db_instance_id": db_instance_id,
         }
         if account_description is not None:
             self._values["account_description"] = account_description
@@ -1133,151 +1234,175 @@
 ):
     '''A ROS template type:  ``ALIYUN::GPDB::DBInstance``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosDBInstanceProps",
+        props: typing.Union["RosDBInstanceProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::GPDB::DBInstance``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosDBInstance.__init__)
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
+            type_hints = typing.get_type_hints(RosDBInstance._render_properties)
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
         :Attribute: ConnectionString: The endpoint of the instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrConnectionString"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDbInstanceId")
     def attr_db_instance_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: DBInstanceId: The ID of the instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDbInstanceId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrOrderId")
     def attr_order_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: OrderId: The order ID of the instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrOrderId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPort")
     def attr_port(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Port: The port used to connect to the instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPort"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dbInstanceClass")
     def db_instance_class(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: dbInstanceClass: The instance type.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "dbInstanceClass"))
 
     @db_instance_class.setter
     def db_instance_class(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstance, "db_instance_class").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dbInstanceClass", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dbInstanceGroupCount")
     def db_instance_group_count(
         self,
     ) -> typing.Union[jsii.Number, ros_cdk_core.IResolvable]:
         '''
         :Property: dbInstanceGroupCount: The number of compute nodes in the instance.
         '''
         return typing.cast(typing.Union[jsii.Number, ros_cdk_core.IResolvable], jsii.get(self, "dbInstanceGroupCount"))
 
     @db_instance_group_count.setter
     def db_instance_group_count(
         self,
         value: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstance, "db_instance_group_count").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dbInstanceGroupCount", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstance, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="engineVersion")
     def engine_version(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: engineVersion: The version of the database engine.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "engineVersion"))
 
     @engine_version.setter
     def engine_version(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstance, "engine_version").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "engineVersion", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vSwitchId")
     def v_switch_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: vSwitchId: The vSwitch ID of the instance.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "vSwitchId"))
 
     @v_switch_id.setter
     def v_switch_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstance, "v_switch_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "vSwitchId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="zoneId")
     def zone_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         zoneId: The zone ID of the instance, such as cn-hangzhou-d. You can call the DescribeRegions
         operation to query the most recent zone list.
@@ -1285,34 +1410,40 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "zoneId"))
 
     @zone_id.setter
     def zone_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstance, "zone_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "zoneId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dbInstanceDescription")
     def db_instance_description(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: dbInstanceDescription: The description of the instance. The description cannot exceed 256 characters in length.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "dbInstanceDescription"))
 
     @db_instance_description.setter
     def db_instance_description(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstance, "db_instance_description").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dbInstanceDescription", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="payType")
     def pay_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -1323,51 +1454,60 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "payType"))
 
     @pay_type.setter
     def pay_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstance, "pay_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "payType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="period")
     def period(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: period: The subscription period. While choose by pay by month, it could be from 1 to 11. While choose pay by year, it could be from 1 to 3.
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "period"))
 
     @period.setter
     def period(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstance, "period").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "period", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="periodUnit")
     def period_unit(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: periodUnit: Unit of subscription period, it could be Month/Year. Default value is Month.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "periodUnit"))
 
     @period_unit.setter
     def period_unit(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstance, "period_unit").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "periodUnit", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="securityIpList")
     def security_ip_list(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -1377,32 +1517,38 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "securityIpList"))
 
     @security_ip_list.setter
     def security_ip_list(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstance, "security_ip_list").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "securityIpList", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="tags")
     def tags(self) -> typing.Optional[typing.List["RosDBInstance.TagsProperty"]]:
         '''
         :Property: tags: Tags to attach to instance. Max support 20 tags to add during create instance. Each tag with two properties Key and Value, and Key is required.
         '''
         return typing.cast(typing.Optional[typing.List["RosDBInstance.TagsProperty"]], jsii.get(self, "tags"))
 
     @tags.setter
     def tags(
         self,
         value: typing.Optional[typing.List["RosDBInstance.TagsProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstance, "tags").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "tags", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vpcId")
     def vpc_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -1413,14 +1559,17 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "vpcId"))
 
     @vpc_id.setter
     def vpc_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstance, "vpc_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "vpcId", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-gpdb.RosDBInstance.TagsProperty",
         jsii_struct_bases=[],
         name_mapping={"key": "key", "value": "value"},
     )
@@ -1431,14 +1580,18 @@
             key: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param key: 
             :param value: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosDBInstance.TagsProperty.__init__)
+                check_type(argname="argument key", value=key, expected_type=type_hints["key"])
+                check_type(argname="argument value", value=value, expected_type=type_hints["value"])
             self._values: typing.Dict[str, typing.Any] = {
                 "key": key,
             }
             if value is not None:
                 self._values["value"] = value
 
         @builtins.property
@@ -1500,15 +1653,15 @@
         v_switch_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         zone_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         db_instance_description: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         pay_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         period: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         period_unit: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         security_ip_list: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        tags: typing.Optional[typing.Sequence[RosDBInstance.TagsProperty]] = None,
+        tags: typing.Optional[typing.Sequence[typing.Union[RosDBInstance.TagsProperty, typing.Dict[str, typing.Any]]]] = None,
         vpc_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::GPDB::DBInstance``.
 
         :param db_instance_class: 
         :param db_instance_group_count: 
         :param engine_version: 
@@ -1518,14 +1671,28 @@
         :param pay_type: 
         :param period: 
         :param period_unit: 
         :param security_ip_list: 
         :param tags: 
         :param vpc_id: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosDBInstanceProps.__init__)
+            check_type(argname="argument db_instance_class", value=db_instance_class, expected_type=type_hints["db_instance_class"])
+            check_type(argname="argument db_instance_group_count", value=db_instance_group_count, expected_type=type_hints["db_instance_group_count"])
+            check_type(argname="argument engine_version", value=engine_version, expected_type=type_hints["engine_version"])
+            check_type(argname="argument v_switch_id", value=v_switch_id, expected_type=type_hints["v_switch_id"])
+            check_type(argname="argument zone_id", value=zone_id, expected_type=type_hints["zone_id"])
+            check_type(argname="argument db_instance_description", value=db_instance_description, expected_type=type_hints["db_instance_description"])
+            check_type(argname="argument pay_type", value=pay_type, expected_type=type_hints["pay_type"])
+            check_type(argname="argument period", value=period, expected_type=type_hints["period"])
+            check_type(argname="argument period_unit", value=period_unit, expected_type=type_hints["period_unit"])
+            check_type(argname="argument security_ip_list", value=security_ip_list, expected_type=type_hints["security_ip_list"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
+            check_type(argname="argument vpc_id", value=vpc_id, expected_type=type_hints["vpc_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "db_instance_class": db_instance_class,
             "db_instance_group_count": db_instance_group_count,
             "engine_version": engine_version,
             "v_switch_id": v_switch_id,
             "zone_id": zone_id,
         }
@@ -1692,179 +1859,209 @@
 ):
     '''A ROS template type:  ``ALIYUN::GPDB::ElasticDBInstance``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosElasticDBInstanceProps",
+        props: typing.Union["RosElasticDBInstanceProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::GPDB::ElasticDBInstance``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosElasticDBInstance.__init__)
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
+            type_hints = typing.get_type_hints(RosElasticDBInstance._render_properties)
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
         :Attribute: ConnectionString: The endpoint of the instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrConnectionString"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDbInstanceId")
     def attr_db_instance_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: DBInstanceId: The ID of the instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDbInstanceId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrOrderId")
     def attr_order_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: OrderId: The order ID of the instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrOrderId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPort")
     def attr_port(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Port: The port used to connect to the instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPort"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosElasticDBInstance, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="engineVersion")
     def engine_version(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: engineVersion: The version of the database engine.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "engineVersion"))
 
     @engine_version.setter
     def engine_version(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosElasticDBInstance, "engine_version").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "engineVersion", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="instanceSpec")
     def instance_spec(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: instanceSpec: The specification of segment nodes. For example: 2C16G, 4C32G, 16C128G.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "instanceSpec"))
 
     @instance_spec.setter
     def instance_spec(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosElasticDBInstance, "instance_spec").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "instanceSpec", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="segNodeNum")
     def seg_node_num(self) -> typing.Union[jsii.Number, ros_cdk_core.IResolvable]:
         '''
         :Property: segNodeNum: The number of segment nodes. Minimum is 4, max is 512, step is 4.
         '''
         return typing.cast(typing.Union[jsii.Number, ros_cdk_core.IResolvable], jsii.get(self, "segNodeNum"))
 
     @seg_node_num.setter
     def seg_node_num(
         self,
         value: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosElasticDBInstance, "seg_node_num").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "segNodeNum", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="segStorageType")
     def seg_storage_type(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: segStorageType: The disk type of segment nodes. For example: cloud_essd, cloud_efficiency.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "segStorageType"))
 
     @seg_storage_type.setter
     def seg_storage_type(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosElasticDBInstance, "seg_storage_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "segStorageType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="storageSize")
     def storage_size(self) -> typing.Union[jsii.Number, ros_cdk_core.IResolvable]:
         '''
         :Property: storageSize: The storage capacity of per segment node. Unit: GB. Minimum is 50, max is 4000, step is 50.
         '''
         return typing.cast(typing.Union[jsii.Number, ros_cdk_core.IResolvable], jsii.get(self, "storageSize"))
 
     @storage_size.setter
     def storage_size(
         self,
         value: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosElasticDBInstance, "storage_size").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "storageSize", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vSwitchId")
     def v_switch_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: vSwitchId: The vSwitch ID of the instance.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "vSwitchId"))
 
     @v_switch_id.setter
     def v_switch_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosElasticDBInstance, "v_switch_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "vSwitchId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="zoneId")
     def zone_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         zoneId: The zone ID of the instance, such as cn-hangzhou-d. You can call the DescribeRegions
         operation to query the most recent zone list.
@@ -1872,68 +2069,80 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "zoneId"))
 
     @zone_id.setter
     def zone_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosElasticDBInstance, "zone_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "zoneId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dbInstanceCategory")
     def db_instance_category(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: dbInstanceCategory: DB instance category, valid values: Basic, HighAvailability
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "dbInstanceCategory"))
 
     @db_instance_category.setter
     def db_instance_category(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosElasticDBInstance, "db_instance_category").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dbInstanceCategory", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dbInstanceDescription")
     def db_instance_description(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: dbInstanceDescription: The description of the instance. The description cannot exceed 256 characters in length.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "dbInstanceDescription"))
 
     @db_instance_description.setter
     def db_instance_description(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosElasticDBInstance, "db_instance_description").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dbInstanceDescription", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="encryptionKey")
     def encryption_key(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: encryptionKey: If the EncryptionType parameter is set to CloudDisk, you must specify this parameter to the encryption key that is in the same region with the disks that is specified by the EncryptionType parameter. Otherwise, leave this parameter empty.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "encryptionKey"))
 
     @encryption_key.setter
     def encryption_key(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosElasticDBInstance, "encryption_key").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "encryptionKey", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="encryptionType")
     def encryption_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -1945,34 +2154,40 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "encryptionType"))
 
     @encryption_type.setter
     def encryption_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosElasticDBInstance, "encryption_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "encryptionType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="masterNodeNum")
     def master_node_num(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: masterNodeNum: The number of master nodes. Minimum is 1, max is 2.
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "masterNodeNum"))
 
     @master_node_num.setter
     def master_node_num(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosElasticDBInstance, "master_node_num").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "masterNodeNum", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="payType")
     def pay_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -1983,51 +2198,60 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "payType"))
 
     @pay_type.setter
     def pay_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosElasticDBInstance, "pay_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "payType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="period")
     def period(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: period: The subscription period. While choose by pay by month, it could be from 1 to 11. While choose pay by year, it could be from 1 to 3.
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "period"))
 
     @period.setter
     def period(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosElasticDBInstance, "period").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "period", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="periodUnit")
     def period_unit(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: periodUnit: Unit of subscription period, it could be Month/Year. Default value is Month.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "periodUnit"))
 
     @period_unit.setter
     def period_unit(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosElasticDBInstance, "period_unit").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "periodUnit", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="securityIpList")
     def security_ip_list(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -2037,32 +2261,38 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "securityIpList"))
 
     @security_ip_list.setter
     def security_ip_list(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosElasticDBInstance, "security_ip_list").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "securityIpList", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="tags")
     def tags(self) -> typing.Optional[typing.List["RosElasticDBInstance.TagsProperty"]]:
         '''
         :Property: tags: Tags to attach to instance. Max support 20 tags to add during create instance. Each tag with two properties Key and Value, and Key is required.
         '''
         return typing.cast(typing.Optional[typing.List["RosElasticDBInstance.TagsProperty"]], jsii.get(self, "tags"))
 
     @tags.setter
     def tags(
         self,
         value: typing.Optional[typing.List["RosElasticDBInstance.TagsProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosElasticDBInstance, "tags").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "tags", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vpcId")
     def vpc_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -2073,14 +2303,17 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "vpcId"))
 
     @vpc_id.setter
     def vpc_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosElasticDBInstance, "vpc_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "vpcId", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-gpdb.RosElasticDBInstance.TagsProperty",
         jsii_struct_bases=[],
         name_mapping={"key": "key", "value": "value"},
     )
@@ -2091,14 +2324,18 @@
             key: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param key: 
             :param value: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosElasticDBInstance.TagsProperty.__init__)
+                check_type(argname="argument key", value=key, expected_type=type_hints["key"])
+                check_type(argname="argument value", value=value, expected_type=type_hints["value"])
             self._values: typing.Dict[str, typing.Any] = {
                 "key": key,
             }
             if value is not None:
                 self._values["value"] = value
 
         @builtins.property
@@ -2172,15 +2409,15 @@
         encryption_key: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         encryption_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         master_node_num: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         pay_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         period: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         period_unit: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         security_ip_list: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        tags: typing.Optional[typing.Sequence[RosElasticDBInstance.TagsProperty]] = None,
+        tags: typing.Optional[typing.Sequence[typing.Union[RosElasticDBInstance.TagsProperty, typing.Dict[str, typing.Any]]]] = None,
         vpc_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::GPDB::ElasticDBInstance``.
 
         :param engine_version: 
         :param instance_spec: 
         :param seg_node_num: 
@@ -2196,14 +2433,34 @@
         :param pay_type: 
         :param period: 
         :param period_unit: 
         :param security_ip_list: 
         :param tags: 
         :param vpc_id: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosElasticDBInstanceProps.__init__)
+            check_type(argname="argument engine_version", value=engine_version, expected_type=type_hints["engine_version"])
+            check_type(argname="argument instance_spec", value=instance_spec, expected_type=type_hints["instance_spec"])
+            check_type(argname="argument seg_node_num", value=seg_node_num, expected_type=type_hints["seg_node_num"])
+            check_type(argname="argument seg_storage_type", value=seg_storage_type, expected_type=type_hints["seg_storage_type"])
+            check_type(argname="argument storage_size", value=storage_size, expected_type=type_hints["storage_size"])
+            check_type(argname="argument v_switch_id", value=v_switch_id, expected_type=type_hints["v_switch_id"])
+            check_type(argname="argument zone_id", value=zone_id, expected_type=type_hints["zone_id"])
+            check_type(argname="argument db_instance_category", value=db_instance_category, expected_type=type_hints["db_instance_category"])
+            check_type(argname="argument db_instance_description", value=db_instance_description, expected_type=type_hints["db_instance_description"])
+            check_type(argname="argument encryption_key", value=encryption_key, expected_type=type_hints["encryption_key"])
+            check_type(argname="argument encryption_type", value=encryption_type, expected_type=type_hints["encryption_type"])
+            check_type(argname="argument master_node_num", value=master_node_num, expected_type=type_hints["master_node_num"])
+            check_type(argname="argument pay_type", value=pay_type, expected_type=type_hints["pay_type"])
+            check_type(argname="argument period", value=period, expected_type=type_hints["period"])
+            check_type(argname="argument period_unit", value=period_unit, expected_type=type_hints["period_unit"])
+            check_type(argname="argument security_ip_list", value=security_ip_list, expected_type=type_hints["security_ip_list"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
+            check_type(argname="argument vpc_id", value=vpc_id, expected_type=type_hints["vpc_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "engine_version": engine_version,
             "instance_spec": instance_spec,
             "seg_node_num": seg_node_num,
             "seg_storage_type": seg_storage_type,
             "storage_size": storage_size,
             "v_switch_id": v_switch_id,
@@ -2441,114 +2698,135 @@
 ):
     '''A ROS template type:  ``ALIYUN::GPDB::InstancePublicConnection``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosInstancePublicConnectionProps",
+        props: typing.Union["RosInstancePublicConnectionProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::GPDB::InstancePublicConnection``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosInstancePublicConnection.__init__)
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
+            type_hints = typing.get_type_hints(RosInstancePublicConnection._render_properties)
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
         :Attribute: ConnectionString: The connection string of the instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrConnectionString"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDbInstanceId")
     def attr_db_instance_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: DBInstanceId: The ID of the instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDbInstanceId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="connectionStringPrefix")
     def connection_string_prefix(
         self,
     ) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: connectionStringPrefix: The endpoint that is used to connect to the specified database.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "connectionStringPrefix"))
 
     @connection_string_prefix.setter
     def connection_string_prefix(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstancePublicConnection, "connection_string_prefix").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "connectionStringPrefix", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dbInstanceId")
     def db_instance_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: dbInstanceId: The ID of the instance.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "dbInstanceId"))
 
     @db_instance_id.setter
     def db_instance_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstancePublicConnection, "db_instance_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dbInstanceId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstancePublicConnection, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="port")
     def port(self) -> typing.Union[jsii.Number, ros_cdk_core.IResolvable]:
         '''
         :Property: port: The port number of the instance.
         '''
         return typing.cast(typing.Union[jsii.Number, ros_cdk_core.IResolvable], jsii.get(self, "port"))
 
     @port.setter
     def port(self, value: typing.Union[jsii.Number, ros_cdk_core.IResolvable]) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosInstancePublicConnection, "port").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "port", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-gpdb.RosInstancePublicConnectionProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -2567,14 +2845,19 @@
     ) -> None:
         '''Properties for defining a ``ALIYUN::GPDB::InstancePublicConnection``.
 
         :param connection_string_prefix: 
         :param db_instance_id: 
         :param port: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosInstancePublicConnectionProps.__init__)
+            check_type(argname="argument connection_string_prefix", value=connection_string_prefix, expected_type=type_hints["connection_string_prefix"])
+            check_type(argname="argument db_instance_id", value=db_instance_id, expected_type=type_hints["db_instance_id"])
+            check_type(argname="argument port", value=port, expected_type=type_hints["port"])
         self._values: typing.Dict[str, typing.Any] = {
             "connection_string_prefix": connection_string_prefix,
             "db_instance_id": db_instance_id,
             "port": port,
         }
 
     @builtins.property
```

### Comparing `ros-cdk-gpdb-1.0.8/src/ros_cdk_gpdb.egg-info/PKG-INFO` & `ros-cdk-gpdb-1.0.9/src/ros_cdk_gpdb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-gpdb
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS GPDB Construct Library
```

