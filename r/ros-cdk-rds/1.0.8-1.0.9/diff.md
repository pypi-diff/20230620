# Comparing `tmp/ros-cdk-rds-1.0.8.tar.gz` & `tmp/ros-cdk-rds-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-rds-1.0.8.tar", last modified: Thu Jul 14 02:12:28 2022, max compression
+gzip compressed data, was "dist/ros-cdk-rds-1.0.9.tar", last modified: Fri Sep 23 10:57:28 2022, max compression
```

## Comparing `ros-cdk-rds-1.0.8.tar` & `ros-cdk-rds-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:12:28.000000 ros-cdk-rds-1.0.8/
--rw-r--r--   0 root         (0) root         (0)    10279 2022-07-14 02:12:28.000000 ros-cdk-rds-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2022-07-14 02:12:28.000000 ros-cdk-rds-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2022-07-14 02:12:28.000000 ros-cdk-rds-1.0.8/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1240 2022-07-14 02:12:28.000000 ros-cdk-rds-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      179 2022-07-14 02:12:28.000000 ros-cdk-rds-1.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)      106 2022-07-14 02:12:28.000000 ros-cdk-rds-1.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-07-14 02:12:28.000000 ros-cdk-rds-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1794 2022-07-14 02:12:28.000000 ros-cdk-rds-1.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:12:28.000000 ros-cdk-rds-1.0.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:12:28.000000 ros-cdk-rds-1.0.8/src/ros_cdk_rds/
--rw-r--r--   0 root         (0) root         (0)   614378 2022-07-14 02:12:28.000000 ros-cdk-rds-1.0.8/src/ros_cdk_rds/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:12:28.000000 ros-cdk-rds-1.0.8/src/ros_cdk_rds/_jsii/
--rw-r--r--   0 root         (0) root         (0)      370 2022-07-14 02:12:28.000000 ros-cdk-rds-1.0.8/src/ros_cdk_rds/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)   221254 2022-07-14 02:12:28.000000 ros-cdk-rds-1.0.8/src/ros_cdk_rds/_jsii/ros-cdk-rds@1.0.8.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:12:28.000000 ros-cdk-rds-1.0.8/src/ros_cdk_rds/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:12:28.000000 ros-cdk-rds-1.0.8/src/ros_cdk_rds.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1240 2022-07-14 02:12:28.000000 ros-cdk-rds-1.0.8/src/ros_cdk_rds.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      400 2022-07-14 02:12:28.000000 ros-cdk-rds-1.0.8/src/ros_cdk_rds.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:12:28.000000 ros-cdk-rds-1.0.8/src/ros_cdk_rds.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2022-07-14 02:12:28.000000 ros-cdk-rds-1.0.8/src/ros_cdk_rds.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2022-07-14 02:12:28.000000 ros-cdk-rds-1.0.8/src/ros_cdk_rds.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 10:57:28.000000 ros-cdk-rds-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)    10279 2022-09-23 10:57:28.000000 ros-cdk-rds-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-09-23 10:57:28.000000 ros-cdk-rds-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2022-09-23 10:57:28.000000 ros-cdk-rds-1.0.9/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1240 2022-09-23 10:57:28.000000 ros-cdk-rds-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      179 2022-09-23 10:57:28.000000 ros-cdk-rds-1.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      236 2022-09-23 10:57:28.000000 ros-cdk-rds-1.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-09-23 10:57:28.000000 ros-cdk-rds-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1823 2022-09-23 10:57:28.000000 ros-cdk-rds-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 10:57:28.000000 ros-cdk-rds-1.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 10:57:28.000000 ros-cdk-rds-1.0.9/src/ros_cdk_rds/
+-rw-r--r--   0 root         (0) root         (0)   758397 2022-09-23 10:57:28.000000 ros-cdk-rds-1.0.9/src/ros_cdk_rds/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 10:57:28.000000 ros-cdk-rds-1.0.9/src/ros_cdk_rds/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      404 2022-09-23 10:57:28.000000 ros-cdk-rds-1.0.9/src/ros_cdk_rds/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   231855 2022-09-23 10:57:28.000000 ros-cdk-rds-1.0.9/src/ros_cdk_rds/_jsii/ros-cdk-rds@1.0.9.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 10:57:28.000000 ros-cdk-rds-1.0.9/src/ros_cdk_rds/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 10:57:28.000000 ros-cdk-rds-1.0.9/src/ros_cdk_rds.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1240 2022-09-23 10:57:28.000000 ros-cdk-rds-1.0.9/src/ros_cdk_rds.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      400 2022-09-23 10:57:28.000000 ros-cdk-rds-1.0.9/src/ros_cdk_rds.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 10:57:28.000000 ros-cdk-rds-1.0.9/src/ros_cdk_rds.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2022-09-23 10:57:28.000000 ros-cdk-rds-1.0.9/src/ros_cdk_rds.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2022-09-23 10:57:28.000000 ros-cdk-rds-1.0.9/src/ros_cdk_rds.egg-info/top_level.txt
```

### Comparing `ros-cdk-rds-1.0.8/LICENSE` & `ros-cdk-rds-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-rds-1.0.8/PKG-INFO` & `ros-cdk-rds-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-rds
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS RDS Construct Library
```

### Comparing `ros-cdk-rds-1.0.8/setup.py` & `ros-cdk-rds-1.0.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-rds",
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
         "ros_cdk_rds",
         "ros_cdk_rds._jsii"
     ],
     "package_data": {
         "ros_cdk_rds._jsii": [
-            "ros-cdk-rds@1.0.8.jsii.tgz"
+            "ros-cdk-rds@1.0.9.jsii.tgz"
         ],
         "ros_cdk_rds": [
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

### Comparing `ros-cdk-rds-1.0.8/src/ros_cdk_rds/__init__.py` & `ros-cdk-rds-1.0.9/src/ros_cdk_rds/__init__.py`

 * *Files 17% similar despite different names*

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
 
 
 class ADInfo(
     ros_cdk_core.Resource,
@@ -29,37 +31,43 @@
 ):
     '''A ROS resource type:  ``ALIYUN::RDS::ADInfo``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "ADInfoProps",
+        props: typing.Union["ADInfoProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::RDS::ADInfo``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(ADInfo.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrAddns")
     def attr_addns(self) -> ros_cdk_core.IResolvable:
         '''Attribute ADDNS: Active directory domain name.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAddns"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDbInstanceId")
     def attr_db_instance_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute DBInstanceId: The ID of the instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDbInstanceId"))
 
 
 @jsii.data_type(
@@ -87,14 +95,21 @@
 
         :param ad_account_name: Property adAccountName: Domain account name.
         :param addns: Property addns: Active directory domain name.
         :param ad_password: Property adPassword: Domain password.
         :param ad_server_ip_address: Property adServerIpAddress: The IP address of the AD server, it must be in the same VPC as the RDS.
         :param db_instance_id: Property dbInstanceId: The ID of the instance.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(ADInfoProps.__init__)
+            check_type(argname="argument ad_account_name", value=ad_account_name, expected_type=type_hints["ad_account_name"])
+            check_type(argname="argument addns", value=addns, expected_type=type_hints["addns"])
+            check_type(argname="argument ad_password", value=ad_password, expected_type=type_hints["ad_password"])
+            check_type(argname="argument ad_server_ip_address", value=ad_server_ip_address, expected_type=type_hints["ad_server_ip_address"])
+            check_type(argname="argument db_instance_id", value=db_instance_id, expected_type=type_hints["db_instance_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "ad_account_name": ad_account_name,
             "addns": addns,
             "ad_password": ad_password,
             "ad_server_ip_address": ad_server_ip_address,
             "db_instance_id": db_instance_id,
         }
@@ -155,31 +170,37 @@
 ):
     '''A ROS resource type:  ``ALIYUN::RDS::Account``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "AccountProps",
+        props: typing.Union["AccountProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::RDS::Account``.
 
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
         '''Attribute AccountName: Account name.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAccountName"))
 
 
 class AccountPrivilege(
@@ -189,28 +210,34 @@
 ):
     '''A ROS resource type:  ``ALIYUN::RDS::AccountPrivilege``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "AccountPrivilegeProps",
+        props: typing.Union["AccountPrivilegeProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::RDS::AccountPrivilege``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(AccountPrivilege.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-rds.AccountPrivilegeProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -232,14 +259,20 @@
         '''Properties for defining a ``ALIYUN::RDS::AccountPrivilege``.
 
         :param account_name: Property accountName: RDS account name.
         :param account_privilege: Property accountPrivilege: RDS account privilege.
         :param db_instance_id: Property dbInstanceId: RDS instance ID.
         :param db_name: Property dbName: RDS database name.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(AccountPrivilegeProps.__init__)
+            check_type(argname="argument account_name", value=account_name, expected_type=type_hints["account_name"])
+            check_type(argname="argument account_privilege", value=account_privilege, expected_type=type_hints["account_privilege"])
+            check_type(argname="argument db_instance_id", value=db_instance_id, expected_type=type_hints["db_instance_id"])
+            check_type(argname="argument db_name", value=db_name, expected_type=type_hints["db_name"])
         self._values: typing.Dict[str, typing.Any] = {
             "account_name": account_name,
             "account_privilege": account_privilege,
             "db_instance_id": db_instance_id,
             "db_name": db_name,
         }
 
@@ -308,14 +341,21 @@
 
         :param account_name: Property accountName: Account name, which must be unique and meet the following requirements: Start with a letter; Consist of lower-case letters, digits, and underscores (_); Contain no more than 16 characters. For other invalid characters, see Forbidden keywords table.
         :param account_password: Property accountPassword: The account password for the database instance. It may consist of letters, digits, or underlines, with a length of 8 to 32 characters.
         :param db_instance_id: Property dbInstanceId: RDS instance ID.
         :param account_description: Property accountDescription: Account remarks. It cannot begin with http:// or https://. It must start with a Chinese character or English letter. It can include Chinese and English characters/letters, underscores (_), hyphens (-), and digits. The length may be 2-256 characters.
         :param account_type: Property accountType: Privilege type of account. Normal: Common privilege. Super: High privilege. And the default value is Normal. This parameter is valid for MySQL 5.5/5.6 only. MySQL 5.7, SQL Server 2012/2016, PostgreSQL, and PPAS each can have only one initial account. Other accounts are created by the initial account that has logged on to the database.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(AccountProps.__init__)
+            check_type(argname="argument account_name", value=account_name, expected_type=type_hints["account_name"])
+            check_type(argname="argument account_password", value=account_password, expected_type=type_hints["account_password"])
+            check_type(argname="argument db_instance_id", value=db_instance_id, expected_type=type_hints["db_instance_id"])
+            check_type(argname="argument account_description", value=account_description, expected_type=type_hints["account_description"])
+            check_type(argname="argument account_type", value=account_type, expected_type=type_hints["account_type"])
         self._values: typing.Dict[str, typing.Any] = {
             "account_name": account_name,
             "account_password": account_password,
             "db_instance_id": db_instance_id,
         }
         if account_description is not None:
             self._values["account_description"] = account_description
@@ -398,67 +438,73 @@
 ):
     '''A ROS resource type:  ``ALIYUN::RDS::DBInstance``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "DBInstanceProps",
+        props: typing.Union["DBInstanceProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::RDS::DBInstance``.
 
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
     @jsii.member(jsii_name="attrDbInstanceId")
     def attr_db_instance_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute DBInstanceId: The instance id of created database instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDbInstanceId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInnerConnectionString")
     def attr_inner_connection_string(self) -> ros_cdk_core.IResolvable:
         '''Attribute InnerConnectionString: DB instance connection url by Intranet.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInnerConnectionString"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInnerIpAddress")
     def attr_inner_ip_address(self) -> ros_cdk_core.IResolvable:
         '''Attribute InnerIPAddress: IP Address for created DB instance of Intranet.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInnerIpAddress"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInnerPort")
     def attr_inner_port(self) -> ros_cdk_core.IResolvable:
         '''Attribute InnerPort: Intranet port of created DB instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInnerPort"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPublicConnectionString")
     def attr_public_connection_string(self) -> ros_cdk_core.IResolvable:
         '''Attribute PublicConnectionString: DB instance connection url by Internet.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPublicConnectionString"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPublicIpAddress")
     def attr_public_ip_address(self) -> ros_cdk_core.IResolvable:
         '''Attribute PublicIPAddress: IP Address for created DB instance of Internet.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPublicIpAddress"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPublicPort")
     def attr_public_port(self) -> ros_cdk_core.IResolvable:
         '''Attribute PublicPort: Internet port of created DB instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPublicPort"))
 
 
 class DBInstanceClone(
@@ -468,67 +514,73 @@
 ):
     '''A ROS resource type:  ``ALIYUN::RDS::DBInstanceClone``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "DBInstanceCloneProps",
+        props: typing.Union["DBInstanceCloneProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::RDS::DBInstanceClone``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(DBInstanceClone.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDbInstanceId")
     def attr_db_instance_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute DBInstanceId: The instance id of created database instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDbInstanceId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInnerConnectionString")
     def attr_inner_connection_string(self) -> ros_cdk_core.IResolvable:
         '''Attribute InnerConnectionString: DB instance connection url by Intranet.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInnerConnectionString"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInnerIpAddress")
     def attr_inner_ip_address(self) -> ros_cdk_core.IResolvable:
         '''Attribute InnerIPAddress: IP Address for created DB instance of Intranet.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInnerIpAddress"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInnerPort")
     def attr_inner_port(self) -> ros_cdk_core.IResolvable:
         '''Attribute InnerPort: Intranet port of created DB instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInnerPort"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPublicConnectionString")
     def attr_public_connection_string(self) -> ros_cdk_core.IResolvable:
         '''Attribute PublicConnectionString: DB instance connection url by Internet.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPublicConnectionString"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPublicIpAddress")
     def attr_public_ip_address(self) -> ros_cdk_core.IResolvable:
         '''Attribute PublicIPAddress: IP Address for created DB instance of Internet.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPublicIpAddress"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPublicPort")
     def attr_public_port(self) -> ros_cdk_core.IResolvable:
         '''Attribute PublicPort: Internet port of created DB instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPublicPort"))
 
 
 @jsii.data_type(
@@ -590,15 +642,15 @@
         category: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         connection_string_prefix: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         connection_string_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         db_instance_class: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         db_instance_description: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         db_instance_storage: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         db_instance_storage_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        db_mappings: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosDBInstanceClone.DBMappingsProperty"]]]] = None,
+        db_mappings: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosDBInstanceClone.DBMappingsProperty", typing.Dict[str, typing.Any]]]]]] = None,
         db_names: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         dedicated_host_group_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         instance_network_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         maintain_time: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         master_username: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         master_user_password: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         master_user_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
@@ -611,15 +663,15 @@
         restore_table: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         restore_time: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         security_group_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         security_ip_list: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         slave_zone_ids: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]] = None,
         sql_collector_status: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ssl_setting: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        table_meta: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosDBInstanceClone.TableMetaProperty"]]]] = None,
+        table_meta: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosDBInstanceClone.TableMetaProperty", typing.Dict[str, typing.Any]]]]]] = None,
         tags: typing.Optional[typing.Mapping[builtins.str, typing.Any]] = None,
         timeout_in_minutes: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         vpc_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         v_switch_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         zone_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::RDS::DBInstanceClone``.
@@ -661,14 +713,56 @@
         :param table_meta: Property tableMeta: The information about the databases and tables that you want to restore.
         :param tags: Property tags: The tags of an instance. You should input the information of the tag with the format of the Key-Value, such as {"key1":"value1","key2":"value2", ... "key5":"value5"}. At most 5 tags can be specified. Key It can be up to 64 characters in length. Cannot begin with aliyun. Cannot begin with http:// or https://. Cannot be a null string. Value It can be up to 128 characters in length. Cannot begin with aliyun. Cannot begin with http:// or https://. Can be a null string.
         :param timeout_in_minutes: Property timeoutInMinutes: The timeout period for creating the clone instance resource. Unit: Minute. Default: 120.
         :param vpc_id: Property vpcId: The VPC id of created database instance. For VPC network, the property is required.
         :param v_switch_id: Property vSwitchId: The vSwitch id of created instance. For VPC network, the property is required.
         :param zone_id: Property zoneId: selected zone to create database instance. You cannot set the ZoneId parameter if the MultiAZ parameter is set to true.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(DBInstanceCloneProps.__init__)
+            check_type(argname="argument db_instance_id", value=db_instance_id, expected_type=type_hints["db_instance_id"])
+            check_type(argname="argument pay_type", value=pay_type, expected_type=type_hints["pay_type"])
+            check_type(argname="argument allocate_public_connection", value=allocate_public_connection, expected_type=type_hints["allocate_public_connection"])
+            check_type(argname="argument backup_id", value=backup_id, expected_type=type_hints["backup_id"])
+            check_type(argname="argument backup_retention_period", value=backup_retention_period, expected_type=type_hints["backup_retention_period"])
+            check_type(argname="argument backup_type", value=backup_type, expected_type=type_hints["backup_type"])
+            check_type(argname="argument category", value=category, expected_type=type_hints["category"])
+            check_type(argname="argument connection_string_prefix", value=connection_string_prefix, expected_type=type_hints["connection_string_prefix"])
+            check_type(argname="argument connection_string_type", value=connection_string_type, expected_type=type_hints["connection_string_type"])
+            check_type(argname="argument db_instance_class", value=db_instance_class, expected_type=type_hints["db_instance_class"])
+            check_type(argname="argument db_instance_description", value=db_instance_description, expected_type=type_hints["db_instance_description"])
+            check_type(argname="argument db_instance_storage", value=db_instance_storage, expected_type=type_hints["db_instance_storage"])
+            check_type(argname="argument db_instance_storage_type", value=db_instance_storage_type, expected_type=type_hints["db_instance_storage_type"])
+            check_type(argname="argument db_mappings", value=db_mappings, expected_type=type_hints["db_mappings"])
+            check_type(argname="argument db_names", value=db_names, expected_type=type_hints["db_names"])
+            check_type(argname="argument dedicated_host_group_id", value=dedicated_host_group_id, expected_type=type_hints["dedicated_host_group_id"])
+            check_type(argname="argument instance_network_type", value=instance_network_type, expected_type=type_hints["instance_network_type"])
+            check_type(argname="argument maintain_time", value=maintain_time, expected_type=type_hints["maintain_time"])
+            check_type(argname="argument master_username", value=master_username, expected_type=type_hints["master_username"])
+            check_type(argname="argument master_user_password", value=master_user_password, expected_type=type_hints["master_user_password"])
+            check_type(argname="argument master_user_type", value=master_user_type, expected_type=type_hints["master_user_type"])
+            check_type(argname="argument period", value=period, expected_type=type_hints["period"])
+            check_type(argname="argument period_type", value=period_type, expected_type=type_hints["period_type"])
+            check_type(argname="argument port", value=port, expected_type=type_hints["port"])
+            check_type(argname="argument preferred_backup_period", value=preferred_backup_period, expected_type=type_hints["preferred_backup_period"])
+            check_type(argname="argument preferred_backup_time", value=preferred_backup_time, expected_type=type_hints["preferred_backup_time"])
+            check_type(argname="argument private_ip_address", value=private_ip_address, expected_type=type_hints["private_ip_address"])
+            check_type(argname="argument restore_table", value=restore_table, expected_type=type_hints["restore_table"])
+            check_type(argname="argument restore_time", value=restore_time, expected_type=type_hints["restore_time"])
+            check_type(argname="argument security_group_id", value=security_group_id, expected_type=type_hints["security_group_id"])
+            check_type(argname="argument security_ip_list", value=security_ip_list, expected_type=type_hints["security_ip_list"])
+            check_type(argname="argument slave_zone_ids", value=slave_zone_ids, expected_type=type_hints["slave_zone_ids"])
+            check_type(argname="argument sql_collector_status", value=sql_collector_status, expected_type=type_hints["sql_collector_status"])
+            check_type(argname="argument ssl_setting", value=ssl_setting, expected_type=type_hints["ssl_setting"])
+            check_type(argname="argument table_meta", value=table_meta, expected_type=type_hints["table_meta"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
+            check_type(argname="argument timeout_in_minutes", value=timeout_in_minutes, expected_type=type_hints["timeout_in_minutes"])
+            check_type(argname="argument vpc_id", value=vpc_id, expected_type=type_hints["vpc_id"])
+            check_type(argname="argument v_switch_id", value=v_switch_id, expected_type=type_hints["v_switch_id"])
+            check_type(argname="argument zone_id", value=zone_id, expected_type=type_hints["zone_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "db_instance_id": db_instance_id,
             "pay_type": pay_type,
         }
         if allocate_public_connection is not None:
             self._values["allocate_public_connection"] = allocate_public_connection
         if backup_id is not None:
@@ -1199,28 +1293,34 @@
 ):
     '''A ROS resource type:  ``ALIYUN::RDS::DBInstanceParameterGroup``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "DBInstanceParameterGroupProps",
+        props: typing.Union["DBInstanceParameterGroupProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::RDS::DBInstanceParameterGroup``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(DBInstanceParameterGroup.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-rds.DBInstanceParameterGroupProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -1230,23 +1330,28 @@
     },
 )
 class DBInstanceParameterGroupProps:
     def __init__(
         self,
         *,
         db_instance_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
-        parameters: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosDBInstanceParameterGroup.ParametersProperty"]]],
+        parameters: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosDBInstanceParameterGroup.ParametersProperty", typing.Dict[str, typing.Any]]]]],
         forcerestart: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::RDS::DBInstanceParameterGroup``.
 
         :param db_instance_id: Property dbInstanceId: Database InstanceId to update properties.
         :param parameters: Property parameters: Parameters to update for selected database instance.
         :param forcerestart: Property forcerestart: whether restart database instance.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(DBInstanceParameterGroupProps.__init__)
+            check_type(argname="argument db_instance_id", value=db_instance_id, expected_type=type_hints["db_instance_id"])
+            check_type(argname="argument parameters", value=parameters, expected_type=type_hints["parameters"])
+            check_type(argname="argument forcerestart", value=forcerestart, expected_type=type_hints["forcerestart"])
         self._values: typing.Dict[str, typing.Any] = {
             "db_instance_id": db_instance_id,
             "parameters": parameters,
         }
         if forcerestart is not None:
             self._values["forcerestart"] = forcerestart
 
@@ -1374,15 +1479,15 @@
         connection_mode: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         connection_string_prefix: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         connection_string_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         db_instance_description: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         db_instance_net_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         db_instance_storage_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         db_is_ignore_case: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
-        db_mappings: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosDBInstance.DBMappingsProperty"]]]] = None,
+        db_mappings: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosDBInstance.DBMappingsProperty", typing.Dict[str, typing.Any]]]]]] = None,
         db_param_group_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         db_time_zone: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         dedicated_host_group_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         enable_backup_log: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         encryption_key: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         high_space_usage_protection: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         local_log_retention_hours: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
@@ -1418,15 +1523,15 @@
         zone_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::RDS::DBInstance``.
 
         :param db_instance_class: Property dbInstanceClass: Database instance type. Refer the RDS database instance type reference, such as 'rds.mys2.large', 'rds.mss1.large', 'rds.pg.s1.small' etc
         :param db_instance_storage: Property dbInstanceStorage: Database instance storage size. mysql is [5,1000]. sql server 2008r2 is [10,1000], sql server 2012/2012_web/2016-web is [20,1000]. PostgreSQL and PPAS is [5,2000]. Increased every 5 GB, Unit in GB
         :param engine: Property engine: Database instance engine type. Support MySQL/SQLServer/PostgreSQL/PPAS/MariaDB now.
-        :param engine_version: Property engineVersion: Database instance version of the relative engine type.Support MySQL: 5.5/5.6/5.7/8.0; SQLServer: 2008r2/2012/2012_ent_ha/2012_std_ha/2012_web/2016_ent_ha/2016_std_ha/2016_web/2017_std_ha/2017_ent; PostgreSQL: 9.4/10.0/11.0/12.0; PPAS: 9.3/10.0; MariaDB: 10.3.
+        :param engine_version: Property engineVersion: Database instance version of the relative engine type. Support: Valid values when you set the Engine parameter to MySQL: 5.5, 5.6, 5.7, and 8.0 Valid values when you set the Engine parameter to SQL Server: 2008r2, 08r2_ent_ha, 2012, 2012_ent_ha, 2012_std_ha, 2012_web, 2014_std_ha, 2016_ent_ha, 2016_std_ha, 2016_web, 2017_std_ha, 2017_ent, 2019_std_ha, and 2019_ent Valid values when you set the Engine parameter to PostgreSQL: 10.0, 11.0, 12.0, 13.0, and 14.0 Valid values when you set the Engine parameter to MariaDB: 10.3
         :param security_ip_list: Property securityIpList: Security ip to access the database instance, combine with comma, 0.0.0.0/0 means no limitation.
         :param allocate_public_connection: Property allocatePublicConnection: If true, allocate public connection automate.
         :param archive_backup_keep_count: Property archiveBackupKeepCount: The number of archived backups that can be retained. Default value: 1. Valid values: The value of this parameter ranges from 1 to 31 when the ArchiveBackupKeepPolicy parameter is set to ByMonth. The value of this parameter ranges from 1 to 7 when the ArchiveBackupKeepPolicy parameter is set to ByWeek. Note You do not need to specify this parameter when the ArchiveBackupKeepPolicy parameter is set to KeepAll.
         :param archive_backup_keep_policy: Property archiveBackupKeepPolicy: The period for which to retain archived backups. The number of archived backups that can be retained within the specified period is determined by the ArchiveBackupKeepCount parameter. Default value: 0. Valid values: ByMonth ByWeek KeepAll
         :param archive_backup_retention_period: Property archiveBackupRetentionPeriod: The number of days for which to retain archived backups. The default value 0 specifies not to enable the backup archiving function. Valid values: 30 to 1095.
         :param auto_renew: Property autoRenew: Specifies whether to enable auto-renewal. Valid values: true and false. Note :Monthly subscription: The auto-renewal cycle is one month. Annual subscription: The auto-renewal cycle is one year.
         :param back_up_category: Property backUpCategory: Specifies whether to enable the second-level backup function. This function allows a backup to be completed within seconds. Valid values: Flash: specifies to enable the second-level backup function. Standard: specifies to disable the second-level backup function.
@@ -1476,14 +1581,76 @@
         :param target_dedicated_host_id_for_log: Property targetDedicatedHostIdForLog: The ID of the host to which the instance belongs if you create a log instance in a host group.
         :param target_dedicated_host_id_for_master: Property targetDedicatedHostIdForMaster: The ID of the host to which the instance belongs if you create a primary instance in a host group.
         :param target_dedicated_host_id_for_slave: Property targetDedicatedHostIdForSlave: The ID of the host to which the instance belongs if you create a secondary instance in a host group.
         :param vpc_id: Property vpcId: The VPC id of created database instance. For VPC network, the property is required.
         :param v_switch_id: Property vSwitchId: The vSwitch id of created instance. For VPC network, the property is required.
         :param zone_id: Property zoneId: selected zone to create database instance. You cannot set the ZoneId parameter if the MultiAZ parameter is set to true.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(DBInstanceProps.__init__)
+            check_type(argname="argument db_instance_class", value=db_instance_class, expected_type=type_hints["db_instance_class"])
+            check_type(argname="argument db_instance_storage", value=db_instance_storage, expected_type=type_hints["db_instance_storage"])
+            check_type(argname="argument engine", value=engine, expected_type=type_hints["engine"])
+            check_type(argname="argument engine_version", value=engine_version, expected_type=type_hints["engine_version"])
+            check_type(argname="argument security_ip_list", value=security_ip_list, expected_type=type_hints["security_ip_list"])
+            check_type(argname="argument allocate_public_connection", value=allocate_public_connection, expected_type=type_hints["allocate_public_connection"])
+            check_type(argname="argument archive_backup_keep_count", value=archive_backup_keep_count, expected_type=type_hints["archive_backup_keep_count"])
+            check_type(argname="argument archive_backup_keep_policy", value=archive_backup_keep_policy, expected_type=type_hints["archive_backup_keep_policy"])
+            check_type(argname="argument archive_backup_retention_period", value=archive_backup_retention_period, expected_type=type_hints["archive_backup_retention_period"])
+            check_type(argname="argument auto_renew", value=auto_renew, expected_type=type_hints["auto_renew"])
+            check_type(argname="argument back_up_category", value=back_up_category, expected_type=type_hints["back_up_category"])
+            check_type(argname="argument backup_policy_mode", value=backup_policy_mode, expected_type=type_hints["backup_policy_mode"])
+            check_type(argname="argument backup_retention_period", value=backup_retention_period, expected_type=type_hints["backup_retention_period"])
+            check_type(argname="argument category", value=category, expected_type=type_hints["category"])
+            check_type(argname="argument compress_type", value=compress_type, expected_type=type_hints["compress_type"])
+            check_type(argname="argument connection_mode", value=connection_mode, expected_type=type_hints["connection_mode"])
+            check_type(argname="argument connection_string_prefix", value=connection_string_prefix, expected_type=type_hints["connection_string_prefix"])
+            check_type(argname="argument connection_string_type", value=connection_string_type, expected_type=type_hints["connection_string_type"])
+            check_type(argname="argument db_instance_description", value=db_instance_description, expected_type=type_hints["db_instance_description"])
+            check_type(argname="argument db_instance_net_type", value=db_instance_net_type, expected_type=type_hints["db_instance_net_type"])
+            check_type(argname="argument db_instance_storage_type", value=db_instance_storage_type, expected_type=type_hints["db_instance_storage_type"])
+            check_type(argname="argument db_is_ignore_case", value=db_is_ignore_case, expected_type=type_hints["db_is_ignore_case"])
+            check_type(argname="argument db_mappings", value=db_mappings, expected_type=type_hints["db_mappings"])
+            check_type(argname="argument db_param_group_id", value=db_param_group_id, expected_type=type_hints["db_param_group_id"])
+            check_type(argname="argument db_time_zone", value=db_time_zone, expected_type=type_hints["db_time_zone"])
+            check_type(argname="argument dedicated_host_group_id", value=dedicated_host_group_id, expected_type=type_hints["dedicated_host_group_id"])
+            check_type(argname="argument enable_backup_log", value=enable_backup_log, expected_type=type_hints["enable_backup_log"])
+            check_type(argname="argument encryption_key", value=encryption_key, expected_type=type_hints["encryption_key"])
+            check_type(argname="argument high_space_usage_protection", value=high_space_usage_protection, expected_type=type_hints["high_space_usage_protection"])
+            check_type(argname="argument local_log_retention_hours", value=local_log_retention_hours, expected_type=type_hints["local_log_retention_hours"])
+            check_type(argname="argument local_log_retention_space", value=local_log_retention_space, expected_type=type_hints["local_log_retention_space"])
+            check_type(argname="argument log_backup_frequency", value=log_backup_frequency, expected_type=type_hints["log_backup_frequency"])
+            check_type(argname="argument log_backup_local_retention_number", value=log_backup_local_retention_number, expected_type=type_hints["log_backup_local_retention_number"])
+            check_type(argname="argument log_backup_retention_period", value=log_backup_retention_period, expected_type=type_hints["log_backup_retention_period"])
+            check_type(argname="argument maintain_time", value=maintain_time, expected_type=type_hints["maintain_time"])
+            check_type(argname="argument master_username", value=master_username, expected_type=type_hints["master_username"])
+            check_type(argname="argument master_user_password", value=master_user_password, expected_type=type_hints["master_user_password"])
+            check_type(argname="argument master_user_type", value=master_user_type, expected_type=type_hints["master_user_type"])
+            check_type(argname="argument multi_az", value=multi_az, expected_type=type_hints["multi_az"])
+            check_type(argname="argument pay_type", value=pay_type, expected_type=type_hints["pay_type"])
+            check_type(argname="argument period", value=period, expected_type=type_hints["period"])
+            check_type(argname="argument period_type", value=period_type, expected_type=type_hints["period_type"])
+            check_type(argname="argument port", value=port, expected_type=type_hints["port"])
+            check_type(argname="argument preferred_backup_period", value=preferred_backup_period, expected_type=type_hints["preferred_backup_period"])
+            check_type(argname="argument preferred_backup_time", value=preferred_backup_time, expected_type=type_hints["preferred_backup_time"])
+            check_type(argname="argument private_ip_address", value=private_ip_address, expected_type=type_hints["private_ip_address"])
+            check_type(argname="argument released_keep_policy", value=released_keep_policy, expected_type=type_hints["released_keep_policy"])
+            check_type(argname="argument resource_group_id", value=resource_group_id, expected_type=type_hints["resource_group_id"])
+            check_type(argname="argument role_arn", value=role_arn, expected_type=type_hints["role_arn"])
+            check_type(argname="argument security_group_id", value=security_group_id, expected_type=type_hints["security_group_id"])
+            check_type(argname="argument slave_zone_ids", value=slave_zone_ids, expected_type=type_hints["slave_zone_ids"])
+            check_type(argname="argument sql_collector_status", value=sql_collector_status, expected_type=type_hints["sql_collector_status"])
+            check_type(argname="argument ssl_setting", value=ssl_setting, expected_type=type_hints["ssl_setting"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
+            check_type(argname="argument target_dedicated_host_id_for_log", value=target_dedicated_host_id_for_log, expected_type=type_hints["target_dedicated_host_id_for_log"])
+            check_type(argname="argument target_dedicated_host_id_for_master", value=target_dedicated_host_id_for_master, expected_type=type_hints["target_dedicated_host_id_for_master"])
+            check_type(argname="argument target_dedicated_host_id_for_slave", value=target_dedicated_host_id_for_slave, expected_type=type_hints["target_dedicated_host_id_for_slave"])
+            check_type(argname="argument vpc_id", value=vpc_id, expected_type=type_hints["vpc_id"])
+            check_type(argname="argument v_switch_id", value=v_switch_id, expected_type=type_hints["v_switch_id"])
+            check_type(argname="argument zone_id", value=zone_id, expected_type=type_hints["zone_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "db_instance_class": db_instance_class,
             "db_instance_storage": db_instance_storage,
             "engine": engine,
             "engine_version": engine_version,
             "security_ip_list": security_ip_list,
         }
@@ -1628,15 +1795,22 @@
         '''
         result = self._values.get("engine")
         assert result is not None, "Required property 'engine' is missing"
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], result)
 
     @builtins.property
     def engine_version(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
-        '''Property engineVersion: Database instance version of the relative engine type.Support MySQL: 5.5/5.6/5.7/8.0; SQLServer: 2008r2/2012/2012_ent_ha/2012_std_ha/2012_web/2016_ent_ha/2016_std_ha/2016_web/2017_std_ha/2017_ent; PostgreSQL: 9.4/10.0/11.0/12.0; PPAS: 9.3/10.0; MariaDB: 10.3.'''
+        '''Property engineVersion: Database instance version of the relative engine type.
+
+        Support:
+        Valid values when you set the Engine parameter to MySQL: 5.5, 5.6, 5.7, and 8.0
+        Valid values when you set the Engine parameter to SQL Server: 2008r2, 08r2_ent_ha, 2012, 2012_ent_ha, 2012_std_ha, 2012_web, 2014_std_ha, 2016_ent_ha, 2016_std_ha, 2016_web, 2017_std_ha, 2017_ent, 2019_std_ha, and 2019_ent
+        Valid values when you set the Engine parameter to PostgreSQL: 10.0, 11.0, 12.0, 13.0, and 14.0
+        Valid values when you set the Engine parameter to MariaDB: 10.3
+        '''
         result = self._values.get("engine_version")
         assert result is not None, "Required property 'engine_version' is missing"
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], result)
 
     @builtins.property
     def security_ip_list(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''Property securityIpList: Security ip to access the database instance, combine with comma, 0.0.0.0/0 means no limitation.'''
@@ -2285,31 +2459,37 @@
 ):
     '''A ROS resource type:  ``ALIYUN::RDS::DBInstanceSecurityIps``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "DBInstanceSecurityIpsProps",
+        props: typing.Union["DBInstanceSecurityIpsProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::RDS::DBInstanceSecurityIps``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(DBInstanceSecurityIps.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrSecurityIps")
     def attr_security_ips(self) -> ros_cdk_core.IResolvable:
         '''Attribute SecurityIps: The security ips of selected database instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrSecurityIps"))
 
 
 @jsii.data_type(
@@ -2331,14 +2511,19 @@
     ) -> None:
         '''Properties for defining a ``ALIYUN::RDS::DBInstanceSecurityIps``.
 
         :param db_instance_id: Property dbInstanceId: Database instance id to update security ips.
         :param db_instance_ip_array_attribute: Property dbInstanceIpArrayAttribute: Security ips to add or remove.
         :param db_instance_ip_array_name: Property dbInstanceIpArrayName: Group name of the security ips, only support lower characters and '_'. Advice use a new group name avoid effect your database system. If the properties is not specified, it will set to default group, please be careful.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(DBInstanceSecurityIpsProps.__init__)
+            check_type(argname="argument db_instance_id", value=db_instance_id, expected_type=type_hints["db_instance_id"])
+            check_type(argname="argument db_instance_ip_array_attribute", value=db_instance_ip_array_attribute, expected_type=type_hints["db_instance_ip_array_attribute"])
+            check_type(argname="argument db_instance_ip_array_name", value=db_instance_ip_array_name, expected_type=type_hints["db_instance_ip_array_name"])
         self._values: typing.Dict[str, typing.Any] = {
             "db_instance_id": db_instance_id,
             "db_instance_ip_array_attribute": db_instance_ip_array_attribute,
         }
         if db_instance_ip_array_name is not None:
             self._values["db_instance_ip_array_name"] = db_instance_ip_array_name
 
@@ -2388,37 +2573,43 @@
 ):
     '''A ROS resource type:  ``ALIYUN::RDS::Database``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "DatabaseProps",
+        props: typing.Union["DatabaseProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::RDS::Database``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(Database.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDbInstanceId")
     def attr_db_instance_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute DBInstanceId: The ID of the instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDbInstanceId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDbName")
     def attr_db_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute DBName: The name of the database.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDbName"))
 
 
 @jsii.data_type(
@@ -2443,14 +2634,20 @@
         '''Properties for defining a ``ALIYUN::RDS::Database``.
 
         :param character_set_name: Property characterSetName: The character set you want to use for the database. Valid values: MySQL and MariaDB: utf8 | gbk | latin1 | utf8mb4. SQL Server: Chinese_PRC_CI_AS | Chinese_PRC_CS_AS | SQL_Latin1_General_CP1_CI_AS | SQL_Latin1_General_CP1_CS_AS | Chinese_PRC_BIN. PostgreSQL: KOI8U | UTF8 | WIN866 | WIN874 | WIN1250 | WIN1251 | WIN1252 | WIN1253 | WIN1254 | WIN1255 | WIN1256 | WIN1257 | WIN1258 | EUC_CN | EUC_KR | EUC_TW | EUC_JP | EUC_JIS_2004 | KOI8R | MULE_INTERNAL | LATIN1 | LATIN2 | LATIN3 | LATIN4 | LATIN5 | LATIN6 | LATIN7 | LATIN8 | LATIN9 | LATIN10 | ISO_8859_5 | ISO_8859_6 | ISO_8859_7 | ISO_8859_8 | SQL_ASCII.
         :param db_instance_id: Property dbInstanceId: The ID of the instance.
         :param db_name: Property dbName: The name of the database you want to create. Note The name must be 2 to 64 characters in length. The name must start with a lowercase letter and end with a lowercase letter or digit. The name can contain lowercase letters, digits, underscores (_), and hyphens (-). The name must be unique in the instance. For more information about invalid characters, see Forbidden keywords table.
         :param db_description: Property dbDescription: The description of the database. The description must be 2 to 256 characters in length. The description must start with a letter and can contain letters, digits, underscores (_), and hyphens (-). Note The description cannot start with http:// or https://.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(DatabaseProps.__init__)
+            check_type(argname="argument character_set_name", value=character_set_name, expected_type=type_hints["character_set_name"])
+            check_type(argname="argument db_instance_id", value=db_instance_id, expected_type=type_hints["db_instance_id"])
+            check_type(argname="argument db_name", value=db_name, expected_type=type_hints["db_name"])
+            check_type(argname="argument db_description", value=db_description, expected_type=type_hints["db_description"])
         self._values: typing.Dict[str, typing.Any] = {
             "character_set_name": character_set_name,
             "db_instance_id": db_instance_id,
             "db_name": db_name,
         }
         if db_description is not None:
             self._values["db_description"] = db_description
@@ -2519,84 +2716,282 @@
 
     def __repr__(self) -> str:
         return "DatabaseProps(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
+class MigrateTask(
+    ros_cdk_core.Resource,
+    metaclass=jsii.JSIIMeta,
+    jsii_type="@alicloud/ros-cdk-rds.MigrateTask",
+):
+    '''A ROS resource type:  ``ALIYUN::RDS::MigrateTask``.'''
+
+    def __init__(
+        self,
+        scope: ros_cdk_core.Construct,
+        id: builtins.str,
+        props: typing.Union["MigrateTaskProps", typing.Dict[str, typing.Any]],
+        enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
+    ) -> None:
+        '''Create a new ``ALIYUN::RDS::MigrateTask``.
+
+        Param scope - scope in which this resource is defined
+        Param id    - scoped id of the resource
+        Param props - resource properties
+
+        :param scope: -
+        :param id: -
+        :param props: -
+        :param enable_resource_property_constraint: -
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(MigrateTask.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
+        jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
+
+    @builtins.property
+    @jsii.member(jsii_name="attrMigrateTaskId")
+    def attr_migrate_task_id(self) -> ros_cdk_core.IResolvable:
+        '''Attribute MigrateTaskId: The ID of the migrate task.'''
+        return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrMigrateTaskId"))
+
+
+@jsii.data_type(
+    jsii_type="@alicloud/ros-cdk-rds.MigrateTaskProps",
+    jsii_struct_bases=[],
+    name_mapping={
+        "backup_mode": "backupMode",
+        "db_instance_id": "dbInstanceId",
+        "db_name": "dbName",
+        "is_online_db": "isOnlineDb",
+        "check_db_mode": "checkDbMode",
+        "oss_object_positions": "ossObjectPositions",
+        "oss_urls": "ossUrls",
+    },
+)
+class MigrateTaskProps:
+    def __init__(
+        self,
+        *,
+        backup_mode: typing.Union[builtins.str, ros_cdk_core.IResolvable],
+        db_instance_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
+        db_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
+        is_online_db: typing.Union[builtins.bool, ros_cdk_core.IResolvable],
+        check_db_mode: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
+        oss_object_positions: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
+        oss_urls: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
+    ) -> None:
+        '''Properties for defining a ``ALIYUN::RDS::MigrateTask``.
+
+        :param backup_mode: Property backupMode: The type of the migration task. Valid values: FULL: specifies that full backup files are used to restore data. UPDF: specifies that incremental backup files or log files are used to restore incremental data.
+        :param db_instance_id: Property dbInstanceId: The ID of the instance.
+        :param db_name: Property dbName: The name of the database that you want to restore.
+        :param is_online_db: Property isOnlineDb: Specifies whether to bring the restored database online for user access. Note The value for SQL Server 2008 R2 is fixed to True.
+        :param check_db_mode: Property checkDbMode: The consistency check method of the database. Valid values: SyncExecuteDBCheck: synchronous database check AsyncExecuteDBCheck: asynchronous database check Default value: AsyncExecuteDBCheck (compatible with SQL Server 2008 R2). Note When IsOnlineDB is set to True, this value is valid.
+        :param oss_object_positions: Property ossObjectPositions: The information of the backup file in the OSS bucket. The values consist of three parts that are separated by colons (:): The endpoint of the OSS bucket: oss-ap-southeast-1.aliyuncs.com. The name of the OSS bucket: rdsmssqlsingapore. The key of the backup file in the OSS bucket: autotest_2008R2_TestMigration_FULL.bak. Note This parameter is optional for instances that run SQL Server 2008 R2. This parameter is required for instances that run a database engine later than SQL Server 2008 R2.
+        :param oss_urls: Property ossUrls: The shared URL of the backup file in the OSS bucket. The URL must be encoded. If you specify multiple URLs, separate them with vertical bars (|) and then encode them. Note This parameter must be entered for instances that run SQL Server 2008 R2.
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(MigrateTaskProps.__init__)
+            check_type(argname="argument backup_mode", value=backup_mode, expected_type=type_hints["backup_mode"])
+            check_type(argname="argument db_instance_id", value=db_instance_id, expected_type=type_hints["db_instance_id"])
+            check_type(argname="argument db_name", value=db_name, expected_type=type_hints["db_name"])
+            check_type(argname="argument is_online_db", value=is_online_db, expected_type=type_hints["is_online_db"])
+            check_type(argname="argument check_db_mode", value=check_db_mode, expected_type=type_hints["check_db_mode"])
+            check_type(argname="argument oss_object_positions", value=oss_object_positions, expected_type=type_hints["oss_object_positions"])
+            check_type(argname="argument oss_urls", value=oss_urls, expected_type=type_hints["oss_urls"])
+        self._values: typing.Dict[str, typing.Any] = {
+            "backup_mode": backup_mode,
+            "db_instance_id": db_instance_id,
+            "db_name": db_name,
+            "is_online_db": is_online_db,
+        }
+        if check_db_mode is not None:
+            self._values["check_db_mode"] = check_db_mode
+        if oss_object_positions is not None:
+            self._values["oss_object_positions"] = oss_object_positions
+        if oss_urls is not None:
+            self._values["oss_urls"] = oss_urls
+
+    @builtins.property
+    def backup_mode(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
+        '''Property backupMode: The type of the migration task.
+
+        Valid values:
+        FULL: specifies that full backup files are used to restore data.
+        UPDF: specifies that incremental backup files or log files are used to restore incremental data.
+        '''
+        result = self._values.get("backup_mode")
+        assert result is not None, "Required property 'backup_mode' is missing"
+        return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], result)
+
+    @builtins.property
+    def db_instance_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
+        '''Property dbInstanceId: The ID of the instance.'''
+        result = self._values.get("db_instance_id")
+        assert result is not None, "Required property 'db_instance_id' is missing"
+        return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], result)
+
+    @builtins.property
+    def db_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
+        '''Property dbName: The name of the database that you want to restore.'''
+        result = self._values.get("db_name")
+        assert result is not None, "Required property 'db_name' is missing"
+        return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], result)
+
+    @builtins.property
+    def is_online_db(self) -> typing.Union[builtins.bool, ros_cdk_core.IResolvable]:
+        '''Property isOnlineDb: Specifies whether to bring the restored database online for user access.
+
+        Note The value for SQL Server 2008 R2 is fixed to True.
+        '''
+        result = self._values.get("is_online_db")
+        assert result is not None, "Required property 'is_online_db' is missing"
+        return typing.cast(typing.Union[builtins.bool, ros_cdk_core.IResolvable], result)
+
+    @builtins.property
+    def check_db_mode(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
+        '''Property checkDbMode: The consistency check method of the database.
+
+        Valid values:
+        SyncExecuteDBCheck: synchronous database check
+        AsyncExecuteDBCheck: asynchronous database check
+        Default value: AsyncExecuteDBCheck (compatible with SQL Server 2008 R2).
+        Note When IsOnlineDB is set to True, this value is valid.
+        '''
+        result = self._values.get("check_db_mode")
+        return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], result)
+
+    @builtins.property
+    def oss_object_positions(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
+        '''Property ossObjectPositions: The information of the backup file in the OSS bucket.
+
+        The values consist of three parts that are separated by colons (:):
+        The endpoint of the OSS bucket: oss-ap-southeast-1.aliyuncs.com.
+        The name of the OSS bucket: rdsmssqlsingapore.
+        The key of the backup file in the OSS bucket: autotest_2008R2_TestMigration_FULL.bak.
+        Note
+        This parameter is optional for instances that run SQL Server 2008 R2.
+        This parameter is required for instances that run a database engine later than SQL
+        Server 2008 R2.
+        '''
+        result = self._values.get("oss_object_positions")
+        return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], result)
+
+    @builtins.property
+    def oss_urls(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
+        '''Property ossUrls: The shared URL of the backup file in the OSS bucket.
+
+        The URL must be encoded.
+        If you specify multiple URLs, separate them with vertical bars (|) and then encode
+        them.
+        Note This parameter must be entered for instances that run SQL Server 2008 R2.
+        '''
+        result = self._values.get("oss_urls")
+        return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], result)
+
+    def __eq__(self, rhs: typing.Any) -> builtins.bool:
+        return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+    def __ne__(self, rhs: typing.Any) -> builtins.bool:
+        return not (rhs == self)
+
+    def __repr__(self) -> str:
+        return "MigrateTaskProps(%s)" % ", ".join(
+            k + "=" + repr(v) for k, v in self._values.items()
+        )
+
+
 class PrepayDBInstance(
     ros_cdk_core.Resource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@alicloud/ros-cdk-rds.PrepayDBInstance",
 ):
     '''A ROS resource type:  ``ALIYUN::RDS::PrepayDBInstance``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "PrepayDBInstanceProps",
+        props: typing.Union["PrepayDBInstanceProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::RDS::PrepayDBInstance``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(PrepayDBInstance.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDbInstanceId")
     def attr_db_instance_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute DBInstanceId: The instance id of created database instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDbInstanceId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInnerConnectionString")
     def attr_inner_connection_string(self) -> ros_cdk_core.IResolvable:
         '''Attribute InnerConnectionString: DB instance connection url by Intranet.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInnerConnectionString"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInnerIpAddress")
     def attr_inner_ip_address(self) -> ros_cdk_core.IResolvable:
         '''Attribute InnerIPAddress: IP Address for created DB instance of Intranet.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInnerIpAddress"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInnerPort")
     def attr_inner_port(self) -> ros_cdk_core.IResolvable:
         '''Attribute InnerPort: Intranet port of created DB instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInnerPort"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrOrderId")
     def attr_order_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute OrderId: The order id list of created instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrOrderId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPublicConnectionString")
     def attr_public_connection_string(self) -> ros_cdk_core.IResolvable:
         '''Attribute PublicConnectionString: DB instance connection url by Internet.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPublicConnectionString"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPublicIpAddress")
     def attr_public_ip_address(self) -> ros_cdk_core.IResolvable:
         '''Attribute PublicIPAddress: IP Address for created DB instance of Internet.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPublicIpAddress"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPublicPort")
     def attr_public_port(self) -> ros_cdk_core.IResolvable:
         '''Attribute PublicPort: Internet port of created DB instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPublicPort"))
 
 
 @jsii.data_type(
@@ -2693,15 +3088,15 @@
         connection_string_prefix: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         connection_string_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         coupon_code: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         db_instance_description: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         db_instance_net_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         db_instance_storage_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         db_is_ignore_case: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
-        db_mappings: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosPrepayDBInstance.DBMappingsProperty"]]]] = None,
+        db_mappings: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosPrepayDBInstance.DBMappingsProperty", typing.Dict[str, typing.Any]]]]]] = None,
         db_param_group_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         db_time_zone: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         dedicated_host_group_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         enable_backup_log: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         encryption_key: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         high_space_usage_protection: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         local_log_retention_hours: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
@@ -2736,15 +3131,15 @@
     ) -> None:
         '''Properties for defining a ``ALIYUN::RDS::PrepayDBInstance``.
 
         :param commodity_code: Property commodityCode: The CommodityCode of the order.
         :param db_instance_class: Property dbInstanceClass: Database instance type. Refer the RDS database instance type reference, such as 'rds.mys2.large', 'rds.mss1.large', 'rds.pg.s1.small' etc
         :param db_instance_storage: Property dbInstanceStorage: Database instance storage size. mysql is [5,1000]. sql server 2008r2 is [10,1000], sql server 2012/2012_web/2016-web is [20,1000]. PostgreSQL and PPAS is [5,2000]. Increased every 5 GB, Unit in GB
         :param engine: Property engine: Database instance engine type. Support MySQL/SQLServer/PostgreSQL/PPAS/MariaDB now.
-        :param engine_version: Property engineVersion: Database instance version of the relative engine type.Support MySQL: 5.5/5.6/5.7/8.0; SQLServer: 2008r2/2012/2012_ent_ha/2012_std_ha/2012_web/2016_ent_ha/2016_std_ha/2016_web/2017_std_ha/2017_ent; PostgreSQL: 9.4/10.0/11.0/12.0; PPAS: 9.3/10.0; MariaDB: 10.3.
+        :param engine_version: Property engineVersion: Database instance version of the relative engine type. Support: Valid values when you set the Engine parameter to MySQL: 5.5, 5.6, 5.7, and 8.0 Valid values when you set the Engine parameter to SQL Server: 2008r2, 08r2_ent_ha, 2012, 2012_ent_ha, 2012_std_ha, 2012_web, 2014_std_ha, 2016_ent_ha, 2016_std_ha, 2016_web, 2017_std_ha, 2017_ent, 2019_std_ha, and 2019_ent Valid values when you set the Engine parameter to PostgreSQL: 10.0, 11.0, 12.0, 13.0, and 14.0 Valid values when you set the Engine parameter to MariaDB: 10.3
         :param period: Property period: Prepaid time period. While choose by pay by month, it could be from 1 to 9. While choose pay by year, it could be from 1 to 3.
         :param period_type: Property periodType: Charge period for created instances.
         :param allocate_public_connection: Property allocatePublicConnection: If true, allocate public connection automate.
         :param archive_backup_keep_count: Property archiveBackupKeepCount: The number of archived backups that can be retained. Default value: 1. Valid values: The value of this parameter ranges from 1 to 31 when the ArchiveBackupKeepPolicy parameter is set to ByMonth. The value of this parameter ranges from 1 to 7 when the ArchiveBackupKeepPolicy parameter is set to ByWeek. Note You do not need to specify this parameter when the ArchiveBackupKeepPolicy parameter is set to KeepAll.
         :param archive_backup_keep_policy: Property archiveBackupKeepPolicy: The period for which to retain archived backups. The number of archived backups that can be retained within the specified period is determined by the ArchiveBackupKeepCount parameter. Default value: 0. Valid values: ByMonth ByWeek KeepAll
         :param archive_backup_retention_period: Property archiveBackupRetentionPeriod: The number of days for which to retain archived backups. The default value 0 specifies not to enable the backup archiving function. Valid values: 30 to 1095.
         :param auto_pay: Property autoPay: Automatic Payment. Default is false.
@@ -2795,14 +3190,78 @@
         :param target_dedicated_host_id_for_log: Property targetDedicatedHostIdForLog: The ID of the host to which the instance belongs if you create a log instance in a host group.
         :param target_dedicated_host_id_for_master: Property targetDedicatedHostIdForMaster: The ID of the host to which the instance belongs if you create a primary instance in a host group.
         :param target_dedicated_host_id_for_slave: Property targetDedicatedHostIdForSlave: The ID of the host to which the instance belongs if you create a secondary instance in a host group.
         :param vpc_id: Property vpcId: The VPC id of created database instance. For VPC network, the property is required.
         :param v_switch_id: Property vSwitchId: The vSwitch id of created instance. For VPC network, the property is required.
         :param zone_id: Property zoneId: selected zone to create database instance. You cannot set the ZoneId parameter if the MultiAZ parameter is set to true.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(PrepayDBInstanceProps.__init__)
+            check_type(argname="argument commodity_code", value=commodity_code, expected_type=type_hints["commodity_code"])
+            check_type(argname="argument db_instance_class", value=db_instance_class, expected_type=type_hints["db_instance_class"])
+            check_type(argname="argument db_instance_storage", value=db_instance_storage, expected_type=type_hints["db_instance_storage"])
+            check_type(argname="argument engine", value=engine, expected_type=type_hints["engine"])
+            check_type(argname="argument engine_version", value=engine_version, expected_type=type_hints["engine_version"])
+            check_type(argname="argument period", value=period, expected_type=type_hints["period"])
+            check_type(argname="argument period_type", value=period_type, expected_type=type_hints["period_type"])
+            check_type(argname="argument allocate_public_connection", value=allocate_public_connection, expected_type=type_hints["allocate_public_connection"])
+            check_type(argname="argument archive_backup_keep_count", value=archive_backup_keep_count, expected_type=type_hints["archive_backup_keep_count"])
+            check_type(argname="argument archive_backup_keep_policy", value=archive_backup_keep_policy, expected_type=type_hints["archive_backup_keep_policy"])
+            check_type(argname="argument archive_backup_retention_period", value=archive_backup_retention_period, expected_type=type_hints["archive_backup_retention_period"])
+            check_type(argname="argument auto_pay", value=auto_pay, expected_type=type_hints["auto_pay"])
+            check_type(argname="argument auto_renew", value=auto_renew, expected_type=type_hints["auto_renew"])
+            check_type(argname="argument back_up_category", value=back_up_category, expected_type=type_hints["back_up_category"])
+            check_type(argname="argument backup_policy_mode", value=backup_policy_mode, expected_type=type_hints["backup_policy_mode"])
+            check_type(argname="argument backup_retention_period", value=backup_retention_period, expected_type=type_hints["backup_retention_period"])
+            check_type(argname="argument category", value=category, expected_type=type_hints["category"])
+            check_type(argname="argument compress_type", value=compress_type, expected_type=type_hints["compress_type"])
+            check_type(argname="argument connection_mode", value=connection_mode, expected_type=type_hints["connection_mode"])
+            check_type(argname="argument connection_string_prefix", value=connection_string_prefix, expected_type=type_hints["connection_string_prefix"])
+            check_type(argname="argument connection_string_type", value=connection_string_type, expected_type=type_hints["connection_string_type"])
+            check_type(argname="argument coupon_code", value=coupon_code, expected_type=type_hints["coupon_code"])
+            check_type(argname="argument db_instance_description", value=db_instance_description, expected_type=type_hints["db_instance_description"])
+            check_type(argname="argument db_instance_net_type", value=db_instance_net_type, expected_type=type_hints["db_instance_net_type"])
+            check_type(argname="argument db_instance_storage_type", value=db_instance_storage_type, expected_type=type_hints["db_instance_storage_type"])
+            check_type(argname="argument db_is_ignore_case", value=db_is_ignore_case, expected_type=type_hints["db_is_ignore_case"])
+            check_type(argname="argument db_mappings", value=db_mappings, expected_type=type_hints["db_mappings"])
+            check_type(argname="argument db_param_group_id", value=db_param_group_id, expected_type=type_hints["db_param_group_id"])
+            check_type(argname="argument db_time_zone", value=db_time_zone, expected_type=type_hints["db_time_zone"])
+            check_type(argname="argument dedicated_host_group_id", value=dedicated_host_group_id, expected_type=type_hints["dedicated_host_group_id"])
+            check_type(argname="argument enable_backup_log", value=enable_backup_log, expected_type=type_hints["enable_backup_log"])
+            check_type(argname="argument encryption_key", value=encryption_key, expected_type=type_hints["encryption_key"])
+            check_type(argname="argument high_space_usage_protection", value=high_space_usage_protection, expected_type=type_hints["high_space_usage_protection"])
+            check_type(argname="argument local_log_retention_hours", value=local_log_retention_hours, expected_type=type_hints["local_log_retention_hours"])
+            check_type(argname="argument local_log_retention_space", value=local_log_retention_space, expected_type=type_hints["local_log_retention_space"])
+            check_type(argname="argument log_backup_frequency", value=log_backup_frequency, expected_type=type_hints["log_backup_frequency"])
+            check_type(argname="argument log_backup_local_retention_number", value=log_backup_local_retention_number, expected_type=type_hints["log_backup_local_retention_number"])
+            check_type(argname="argument log_backup_retention_period", value=log_backup_retention_period, expected_type=type_hints["log_backup_retention_period"])
+            check_type(argname="argument maintain_time", value=maintain_time, expected_type=type_hints["maintain_time"])
+            check_type(argname="argument master_username", value=master_username, expected_type=type_hints["master_username"])
+            check_type(argname="argument master_user_password", value=master_user_password, expected_type=type_hints["master_user_password"])
+            check_type(argname="argument master_user_type", value=master_user_type, expected_type=type_hints["master_user_type"])
+            check_type(argname="argument multi_az", value=multi_az, expected_type=type_hints["multi_az"])
+            check_type(argname="argument port", value=port, expected_type=type_hints["port"])
+            check_type(argname="argument preferred_backup_period", value=preferred_backup_period, expected_type=type_hints["preferred_backup_period"])
+            check_type(argname="argument preferred_backup_time", value=preferred_backup_time, expected_type=type_hints["preferred_backup_time"])
+            check_type(argname="argument private_ip_address", value=private_ip_address, expected_type=type_hints["private_ip_address"])
+            check_type(argname="argument quantity", value=quantity, expected_type=type_hints["quantity"])
+            check_type(argname="argument released_keep_policy", value=released_keep_policy, expected_type=type_hints["released_keep_policy"])
+            check_type(argname="argument resource_group_id", value=resource_group_id, expected_type=type_hints["resource_group_id"])
+            check_type(argname="argument role_arn", value=role_arn, expected_type=type_hints["role_arn"])
+            check_type(argname="argument security_group_id", value=security_group_id, expected_type=type_hints["security_group_id"])
+            check_type(argname="argument slave_zone_ids", value=slave_zone_ids, expected_type=type_hints["slave_zone_ids"])
+            check_type(argname="argument sql_collector_status", value=sql_collector_status, expected_type=type_hints["sql_collector_status"])
+            check_type(argname="argument ssl_setting", value=ssl_setting, expected_type=type_hints["ssl_setting"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
+            check_type(argname="argument target_dedicated_host_id_for_log", value=target_dedicated_host_id_for_log, expected_type=type_hints["target_dedicated_host_id_for_log"])
+            check_type(argname="argument target_dedicated_host_id_for_master", value=target_dedicated_host_id_for_master, expected_type=type_hints["target_dedicated_host_id_for_master"])
+            check_type(argname="argument target_dedicated_host_id_for_slave", value=target_dedicated_host_id_for_slave, expected_type=type_hints["target_dedicated_host_id_for_slave"])
+            check_type(argname="argument vpc_id", value=vpc_id, expected_type=type_hints["vpc_id"])
+            check_type(argname="argument v_switch_id", value=v_switch_id, expected_type=type_hints["v_switch_id"])
+            check_type(argname="argument zone_id", value=zone_id, expected_type=type_hints["zone_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "commodity_code": commodity_code,
             "db_instance_class": db_instance_class,
             "db_instance_storage": db_instance_storage,
             "engine": engine,
             "engine_version": engine_version,
             "period": period,
@@ -2956,15 +3415,22 @@
         '''
         result = self._values.get("engine")
         assert result is not None, "Required property 'engine' is missing"
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], result)
 
     @builtins.property
     def engine_version(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
-        '''Property engineVersion: Database instance version of the relative engine type.Support MySQL: 5.5/5.6/5.7/8.0; SQLServer: 2008r2/2012/2012_ent_ha/2012_std_ha/2012_web/2016_ent_ha/2016_std_ha/2016_web/2017_std_ha/2017_ent; PostgreSQL: 9.4/10.0/11.0/12.0; PPAS: 9.3/10.0; MariaDB: 10.3.'''
+        '''Property engineVersion: Database instance version of the relative engine type.
+
+        Support:
+        Valid values when you set the Engine parameter to MySQL: 5.5, 5.6, 5.7, and 8.0
+        Valid values when you set the Engine parameter to SQL Server: 2008r2, 08r2_ent_ha, 2012, 2012_ent_ha, 2012_std_ha, 2012_web, 2014_std_ha, 2016_ent_ha, 2016_std_ha, 2016_web, 2017_std_ha, 2017_ent, 2019_std_ha, and 2019_ent
+        Valid values when you set the Engine parameter to PostgreSQL: 10.0, 11.0, 12.0, 13.0, and 14.0
+        Valid values when you set the Engine parameter to MariaDB: 10.3
+        '''
         result = self._values.get("engine_version")
         assert result is not None, "Required property 'engine_version' is missing"
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], result)
 
     @builtins.property
     def period(self) -> typing.Union[jsii.Number, ros_cdk_core.IResolvable]:
         '''Property period: Prepaid time period.
@@ -3619,43 +4085,49 @@
 ):
     '''A ROS resource type:  ``ALIYUN::RDS::ReadOnlyDBInstance``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "ReadOnlyDBInstanceProps",
+        props: typing.Union["ReadOnlyDBInstanceProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::RDS::ReadOnlyDBInstance``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(ReadOnlyDBInstance.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrConnectionString")
     def attr_connection_string(self) -> ros_cdk_core.IResolvable:
         '''Attribute ConnectionString: DB instance connection url by Intranet.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrConnectionString"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDbInstanceId")
     def attr_db_instance_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute DBInstanceId: The instance id of created database instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDbInstanceId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPort")
     def attr_port(self) -> ros_cdk_core.IResolvable:
         '''Attribute Port: Intranet port of created DB instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPort"))
 
 
 @jsii.data_type(
@@ -3719,14 +4191,33 @@
         :param period_type: Property periodType: Charge period for created instances.
         :param private_ip_address: Property privateIpAddress: The private IP address of the read-only instance. It must be within the IP address range provided by the switch. The system automatically assigns an IP address based on the VPCId and VSwitchId by default.
         :param resource_group_id: Property resourceGroupId: Resource group id.
         :param tags: Property tags: The tags of an instance. You should input the information of the tag with the format of the Key-Value, such as {"key1":"value1","key2":"value2", ... "key5":"value5"}. At most 5 tags can be specified. Key It can be up to 64 characters in length. Cannot begin with aliyun. Cannot begin with http:// or https://. Cannot be a null string. Value It can be up to 128 characters in length. Cannot begin with aliyun. Cannot begin with http:// or https://. Can be a null string.
         :param vpc_id: Property vpcId: The ID of the VPC.
         :param v_switch_id: Property vSwitchId: The ID of the VSwitch.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(ReadOnlyDBInstanceProps.__init__)
+            check_type(argname="argument db_instance_class", value=db_instance_class, expected_type=type_hints["db_instance_class"])
+            check_type(argname="argument db_instance_id", value=db_instance_id, expected_type=type_hints["db_instance_id"])
+            check_type(argname="argument db_instance_storage", value=db_instance_storage, expected_type=type_hints["db_instance_storage"])
+            check_type(argname="argument engine_version", value=engine_version, expected_type=type_hints["engine_version"])
+            check_type(argname="argument zone_id", value=zone_id, expected_type=type_hints["zone_id"])
+            check_type(argname="argument auto_renew", value=auto_renew, expected_type=type_hints["auto_renew"])
+            check_type(argname="argument category", value=category, expected_type=type_hints["category"])
+            check_type(argname="argument db_instance_description", value=db_instance_description, expected_type=type_hints["db_instance_description"])
+            check_type(argname="argument db_instance_storage_type", value=db_instance_storage_type, expected_type=type_hints["db_instance_storage_type"])
+            check_type(argname="argument pay_type", value=pay_type, expected_type=type_hints["pay_type"])
+            check_type(argname="argument period", value=period, expected_type=type_hints["period"])
+            check_type(argname="argument period_type", value=period_type, expected_type=type_hints["period_type"])
+            check_type(argname="argument private_ip_address", value=private_ip_address, expected_type=type_hints["private_ip_address"])
+            check_type(argname="argument resource_group_id", value=resource_group_id, expected_type=type_hints["resource_group_id"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
+            check_type(argname="argument vpc_id", value=vpc_id, expected_type=type_hints["vpc_id"])
+            check_type(argname="argument v_switch_id", value=v_switch_id, expected_type=type_hints["v_switch_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "db_instance_class": db_instance_class,
             "db_instance_id": db_instance_id,
             "db_instance_storage": db_instance_storage,
             "engine_version": engine_version,
             "zone_id": zone_id,
         }
@@ -3959,147 +4450,174 @@
 ):
     '''A ROS template type:  ``ALIYUN::RDS::ADInfo``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosADInfoProps",
+        props: typing.Union["RosADInfoProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::RDS::ADInfo``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosADInfo.__init__)
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
+            type_hints = typing.get_type_hints(RosADInfo._render_properties)
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
     @jsii.member(jsii_name="attrAddns")
     def attr_addns(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ADDNS: Active directory domain name.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAddns"))
 
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
     @jsii.member(jsii_name="adAccountName")
     def ad_account_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: adAccountName: Domain account name.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "adAccountName"))
 
     @ad_account_name.setter
     def ad_account_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosADInfo, "ad_account_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "adAccountName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="addns")
     def addns(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: addns: Active directory domain name.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "addns"))
 
     @addns.setter
     def addns(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosADInfo, "addns").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "addns", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="adPassword")
     def ad_password(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: adPassword: Domain password.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "adPassword"))
 
     @ad_password.setter
     def ad_password(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosADInfo, "ad_password").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "adPassword", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="adServerIpAddress")
     def ad_server_ip_address(
         self,
     ) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: adServerIpAddress: The IP address of the AD server, it must be in the same VPC as the RDS.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "adServerIpAddress"))
 
     @ad_server_ip_address.setter
     def ad_server_ip_address(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosADInfo, "ad_server_ip_address").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "adServerIpAddress", value)
 
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
+            type_hints = typing.get_type_hints(getattr(RosADInfo, "db_instance_id").fset)
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
+            type_hints = typing.get_type_hints(getattr(RosADInfo, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-rds.RosADInfoProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -4124,14 +4642,21 @@
 
         :param ad_account_name: 
         :param addns: 
         :param ad_password: 
         :param ad_server_ip_address: 
         :param db_instance_id: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosADInfoProps.__init__)
+            check_type(argname="argument ad_account_name", value=ad_account_name, expected_type=type_hints["ad_account_name"])
+            check_type(argname="argument addns", value=addns, expected_type=type_hints["addns"])
+            check_type(argname="argument ad_password", value=ad_password, expected_type=type_hints["ad_password"])
+            check_type(argname="argument ad_server_ip_address", value=ad_server_ip_address, expected_type=type_hints["ad_server_ip_address"])
+            check_type(argname="argument db_instance_id", value=db_instance_id, expected_type=type_hints["db_instance_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "ad_account_name": ad_account_name,
             "addns": addns,
             "ad_password": ad_password,
             "ad_server_ip_address": ad_server_ip_address,
             "db_instance_id": db_instance_id,
         }
@@ -4202,56 +4727,65 @@
 ):
     '''A ROS template type:  ``ALIYUN::RDS::Account``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosAccountProps",
+        props: typing.Union["RosAccountProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::RDS::Account``.
 
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
         :Attribute: AccountName: Account name
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAccountName"))
 
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
 
         accountName: Account name, which must be unique and meet the following requirements:
         Start with a letter;
@@ -4262,56 +4796,68 @@
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
         :Property: accountPassword: The account password for the database instance. It may consist of letters, digits, or underlines, with a length of 8 to 32 characters.
         '''
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
         :Property: dbInstanceId: RDS instance ID.
         '''
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
         :Property:
 
@@ -4324,17 +4870,20 @@
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
     @jsii.member(jsii_name="accountType")
     def account_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -4347,129 +4896,156 @@
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
 
 
 class RosAccountPrivilege(
     ros_cdk_core.RosResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@alicloud/ros-cdk-rds.RosAccountPrivilege",
 ):
     '''A ROS template type:  ``ALIYUN::RDS::AccountPrivilege``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosAccountPrivilegeProps",
+        props: typing.Union["RosAccountPrivilegeProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::RDS::AccountPrivilege``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosAccountPrivilege.__init__)
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
+            type_hints = typing.get_type_hints(RosAccountPrivilege._render_properties)
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
     @jsii.member(jsii_name="accountName")
     def account_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: accountName: RDS account name.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "accountName"))
 
     @account_name.setter
     def account_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAccountPrivilege, "account_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "accountName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="accountPrivilege")
     def account_privilege(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: accountPrivilege: RDS account privilege
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "accountPrivilege"))
 
     @account_privilege.setter
     def account_privilege(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAccountPrivilege, "account_privilege").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "accountPrivilege", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dbInstanceId")
     def db_instance_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: dbInstanceId: RDS instance ID.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "dbInstanceId"))
 
     @db_instance_id.setter
     def db_instance_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAccountPrivilege, "db_instance_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dbInstanceId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dbName")
     def db_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: dbName: RDS database name
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "dbName"))
 
     @db_name.setter
     def db_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAccountPrivilege, "db_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dbName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         '''A factory method that creates a new instance of this class from an object containing the properties of this ROS resource.'''
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAccountPrivilege, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-rds.RosAccountPrivilegeProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -4491,14 +5067,20 @@
         '''Properties for defining a ``ALIYUN::RDS::AccountPrivilege``.
 
         :param account_name: 
         :param account_privilege: 
         :param db_instance_id: 
         :param db_name: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosAccountPrivilegeProps.__init__)
+            check_type(argname="argument account_name", value=account_name, expected_type=type_hints["account_name"])
+            check_type(argname="argument account_privilege", value=account_privilege, expected_type=type_hints["account_privilege"])
+            check_type(argname="argument db_instance_id", value=db_instance_id, expected_type=type_hints["db_instance_id"])
+            check_type(argname="argument db_name", value=db_name, expected_type=type_hints["db_name"])
         self._values: typing.Dict[str, typing.Any] = {
             "account_name": account_name,
             "account_privilege": account_privilege,
             "db_instance_id": db_instance_id,
             "db_name": db_name,
         }
 
@@ -4575,14 +5157,21 @@
 
         :param account_name: 
         :param account_password: 
         :param db_instance_id: 
         :param account_description: 
         :param account_type: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosAccountProps.__init__)
+            check_type(argname="argument account_name", value=account_name, expected_type=type_hints["account_name"])
+            check_type(argname="argument account_password", value=account_password, expected_type=type_hints["account_password"])
+            check_type(argname="argument db_instance_id", value=db_instance_id, expected_type=type_hints["db_instance_id"])
+            check_type(argname="argument account_description", value=account_description, expected_type=type_hints["account_description"])
+            check_type(argname="argument account_type", value=account_type, expected_type=type_hints["account_type"])
         self._values: typing.Dict[str, typing.Any] = {
             "account_name": account_name,
             "account_password": account_password,
             "db_instance_id": db_instance_id,
         }
         if account_description is not None:
             self._values["account_description"] = account_description
@@ -4673,213 +5262,243 @@
 ):
     '''A ROS template type:  ``ALIYUN::RDS::DBInstance``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosDBInstanceProps",
+        props: typing.Union["RosDBInstanceProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::RDS::DBInstance``.
 
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
     @jsii.member(jsii_name="attrDbInstanceId")
     def attr_db_instance_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: DBInstanceId: The instance id of created database instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDbInstanceId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInnerConnectionString")
     def attr_inner_connection_string(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: InnerConnectionString: DB instance connection url by Intranet.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInnerConnectionString"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInnerIpAddress")
     def attr_inner_ip_address(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: InnerIPAddress: IP Address for created DB instance of Intranet.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInnerIpAddress"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInnerPort")
     def attr_inner_port(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: InnerPort: Intranet port of created DB instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInnerPort"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPublicConnectionString")
     def attr_public_connection_string(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: PublicConnectionString: DB instance connection url by Internet.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPublicConnectionString"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPublicIpAddress")
     def attr_public_ip_address(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: PublicIPAddress: IP Address for created DB instance of Internet.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPublicIpAddress"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPublicPort")
     def attr_public_port(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: PublicPort: Internet port of created DB instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPublicPort"))
 
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
         :Property: dbInstanceClass: Database instance type. Refer the RDS database instance type reference, such as 'rds.mys2.large', 'rds.mss1.large', 'rds.pg.s1.small' etc
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
     @jsii.member(jsii_name="dbInstanceStorage")
     def db_instance_storage(
         self,
     ) -> typing.Union[jsii.Number, ros_cdk_core.IResolvable]:
         '''
         :Property: dbInstanceStorage: Database instance storage size. mysql is [5,1000]. sql server 2008r2 is [10,1000], sql server 2012/2012_web/2016-web is [20,1000]. PostgreSQL and PPAS is [5,2000]. Increased every 5 GB, Unit in GB
         '''
         return typing.cast(typing.Union[jsii.Number, ros_cdk_core.IResolvable], jsii.get(self, "dbInstanceStorage"))
 
     @db_instance_storage.setter
     def db_instance_storage(
         self,
         value: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstance, "db_instance_storage").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dbInstanceStorage", value)
 
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
     @jsii.member(jsii_name="engine")
     def engine(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: engine: Database instance engine type. Support MySQL/SQLServer/PostgreSQL/PPAS/MariaDB now.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "engine"))
 
     @engine.setter
     def engine(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstance, "engine").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "engine", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="engineVersion")
     def engine_version(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
-        engineVersion: Database instance version of the relative engine type.Support MySQL: 5.5/5.6/5.7/8.0;
-        SQLServer: 2008r2/2012/2012_ent_ha/2012_std_ha/2012_web/2016_ent_ha/2016_std_ha/2016_web/2017_std_ha/2017_ent;
-        PostgreSQL: 9.4/10.0/11.0/12.0;
-        PPAS: 9.3/10.0;
-        MariaDB: 10.3.
+        engineVersion: Database instance version of the relative engine type. Support:
+        Valid values when you set the Engine parameter to MySQL: 5.5, 5.6, 5.7, and 8.0
+        Valid values when you set the Engine parameter to SQL Server: 2008r2, 08r2_ent_ha, 2012, 2012_ent_ha, 2012_std_ha, 2012_web, 2014_std_ha, 2016_ent_ha, 2016_std_ha, 2016_web, 2017_std_ha, 2017_ent, 2019_std_ha, and 2019_ent
+        Valid values when you set the Engine parameter to PostgreSQL: 10.0, 11.0, 12.0, 13.0, and 14.0
+        Valid values when you set the Engine parameter to MariaDB: 10.3
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
     @jsii.member(jsii_name="securityIpList")
     def security_ip_list(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: securityIpList: Security ip to access the database instance, combine with comma, 0.0.0.0/0 means no limitation.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "securityIpList"))
 
     @security_ip_list.setter
     def security_ip_list(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstance, "security_ip_list").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "securityIpList", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="allocatePublicConnection")
     def allocate_public_connection(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property: allocatePublicConnection: If true, allocate public connection automate.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "allocatePublicConnection"))
 
     @allocate_public_connection.setter
     def allocate_public_connection(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstance, "allocate_public_connection").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "allocatePublicConnection", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="archiveBackupKeepCount")
     def archive_backup_keep_count(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -4894,17 +5513,20 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "archiveBackupKeepCount"))
 
     @archive_backup_keep_count.setter
     def archive_backup_keep_count(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstance, "archive_backup_keep_count").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "archiveBackupKeepCount", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="archiveBackupKeepPolicy")
     def archive_backup_keep_policy(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -4918,17 +5540,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "archiveBackupKeepPolicy"))
 
     @archive_backup_keep_policy.setter
     def archive_backup_keep_policy(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstance, "archive_backup_keep_policy").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "archiveBackupKeepPolicy", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="archiveBackupRetentionPeriod")
     def archive_backup_retention_period(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -4938,17 +5563,20 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "archiveBackupRetentionPeriod"))
 
     @archive_backup_retention_period.setter
     def archive_backup_retention_period(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstance, "archive_backup_retention_period").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "archiveBackupRetentionPeriod", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="autoRenew")
     def auto_renew(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -4959,17 +5587,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "autoRenew"))
 
     @auto_renew.setter
     def auto_renew(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstance, "auto_renew").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "autoRenew", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="backUpCategory")
     def back_up_category(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -4981,17 +5612,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "backUpCategory"))
 
     @back_up_category.setter
     def back_up_category(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstance, "back_up_category").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "backUpCategory", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="backupPolicyMode")
     def backup_policy_mode(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -5002,34 +5636,40 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "backupPolicyMode"))
 
     @backup_policy_mode.setter
     def backup_policy_mode(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstance, "backup_policy_mode").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "backupPolicyMode", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="backupRetentionPeriod")
     def backup_retention_period(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: backupRetentionPeriod: The retention period of the data backup. Value range: 7 to 730. The default value is the original value. Note When the BackupPolicyMode parameter is set to LogBackupPolicy, this parameter is required.
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "backupRetentionPeriod"))
 
     @backup_retention_period.setter
     def backup_retention_period(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstance, "backup_retention_period").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "backupRetentionPeriod", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="category")
     def category(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -5042,17 +5682,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "category"))
 
     @category.setter
     def category(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstance, "category").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "category", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="compressType")
     def compress_type(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -5068,34 +5711,40 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "compressType"))
 
     @compress_type.setter
     def compress_type(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstance, "compress_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "compressType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="connectionMode")
     def connection_mode(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: connectionMode: Connection Mode for database instance,support 'Standard' and 'Safe' mode. Default is RDS system assigns.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "connectionMode"))
 
     @connection_mode.setter
     def connection_mode(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstance, "connection_mode").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "connectionMode", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="connectionStringPrefix")
     def connection_string_prefix(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -5106,68 +5755,80 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "connectionStringPrefix"))
 
     @connection_string_prefix.setter
     def connection_string_prefix(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstance, "connection_string_prefix").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "connectionStringPrefix", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="connectionStringType")
     def connection_string_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: connectionStringType: The endpoint type of the instance, allow values: Inner, Public
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "connectionStringType"))
 
     @connection_string_type.setter
     def connection_string_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstance, "connection_string_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "connectionStringType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dbInstanceDescription")
     def db_instance_description(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: dbInstanceDescription: Description of created database instance.
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
     @jsii.member(jsii_name="dbInstanceNetType")
     def db_instance_net_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: dbInstanceNetType: Database instance net type, default is Intranet.Internet for public access, Intranet for private access.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "dbInstanceNetType"))
 
     @db_instance_net_type.setter
     def db_instance_net_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstance, "db_instance_net_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dbInstanceNetType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dbInstanceStorageType")
     def db_instance_storage_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -5181,17 +5842,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "dbInstanceStorageType"))
 
     @db_instance_storage_type.setter
     def db_instance_storage_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstance, "db_instance_storage_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dbInstanceStorageType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dbIsIgnoreCase")
     def db_is_ignore_case(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -5202,85 +5866,100 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "dbIsIgnoreCase"))
 
     @db_is_ignore_case.setter
     def db_is_ignore_case(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstance, "db_is_ignore_case").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dbIsIgnoreCase", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dbMappings")
     def db_mappings(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosDBInstance.DBMappingsProperty"]]]]:
         '''
         :Property: dbMappings: Database mappings to attach to db instance.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosDBInstance.DBMappingsProperty"]]]], jsii.get(self, "dbMappings"))
 
     @db_mappings.setter
     def db_mappings(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosDBInstance.DBMappingsProperty"]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstance, "db_mappings").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dbMappings", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dbParamGroupId")
     def db_param_group_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: dbParamGroupId: The ID of the parameter template used by the instance.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "dbParamGroupId"))
 
     @db_param_group_id.setter
     def db_param_group_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstance, "db_param_group_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dbParamGroupId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dbTimeZone")
     def db_time_zone(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: dbTimeZone: The UTC time zone of the instance. Valid values: -12:00 to +12:00. The time zone must be an integer value such as +08:00. Values such as +08:30 are not allowed.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "dbTimeZone"))
 
     @db_time_zone.setter
     def db_time_zone(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstance, "db_time_zone").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dbTimeZone", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dedicatedHostGroupId")
     def dedicated_host_group_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: dedicatedHostGroupId: The ID of the host group to which the instance belongs if you create an instance in a host group.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "dedicatedHostGroupId"))
 
     @dedicated_host_group_id.setter
     def dedicated_host_group_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstance, "dedicated_host_group_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dedicatedHostGroupId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableBackupLog")
     def enable_backup_log(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -5292,34 +5971,40 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "enableBackupLog"))
 
     @enable_backup_log.setter
     def enable_backup_log(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstance, "enable_backup_log").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableBackupLog", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="encryptionKey")
     def encryption_key(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: encryptionKey: The ID of the encryption key that is used to encrypt data on SSDs in the region. You can view the encryption key ID in the Key Management Service (KMS) console. You can also create an encryption key.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "encryptionKey"))
 
     @encryption_key.setter
     def encryption_key(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstance, "encryption_key").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "encryptionKey", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="highSpaceUsageProtection")
     def high_space_usage_protection(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -5331,17 +6016,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "highSpaceUsageProtection"))
 
     @high_space_usage_protection.setter
     def high_space_usage_protection(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstance, "high_space_usage_protection").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "highSpaceUsageProtection", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="localLogRetentionHours")
     def local_log_retention_hours(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -5353,17 +6041,20 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "localLogRetentionHours"))
 
     @local_log_retention_hours.setter
     def local_log_retention_hours(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstance, "local_log_retention_hours").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "localLogRetentionHours", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="localLogRetentionSpace")
     def local_log_retention_space(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -5376,17 +6067,20 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "localLogRetentionSpace"))
 
     @local_log_retention_space.setter
     def local_log_retention_space(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstance, "local_log_retention_space").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "localLogRetentionSpace", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="logBackupFrequency")
     def log_backup_frequency(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -5398,17 +6092,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "logBackupFrequency"))
 
     @log_backup_frequency.setter
     def log_backup_frequency(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstance, "log_backup_frequency").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "logBackupFrequency", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="logBackupLocalRetentionNumber")
     def log_backup_local_retention_number(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -5418,17 +6115,20 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "logBackupLocalRetentionNumber"))
 
     @log_backup_local_retention_number.setter
     def log_backup_local_retention_number(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstance, "log_backup_local_retention_number").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "logBackupLocalRetentionNumber", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="logBackupRetentionPeriod")
     def log_backup_retention_period(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -5440,68 +6140,80 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "logBackupRetentionPeriod"))
 
     @log_backup_retention_period.setter
     def log_backup_retention_period(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstance, "log_backup_retention_period").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "logBackupRetentionPeriod", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="maintainTime")
     def maintain_time(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: maintainTime: The period during which the maintenance performs. The format is HH:mmZ-HH:mmZ.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "maintainTime"))
 
     @maintain_time.setter
     def maintain_time(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstance, "maintain_time").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "maintainTime", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="masterUsername")
     def master_username(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: masterUsername: The master user name for the database instance.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "masterUsername"))
 
     @master_username.setter
     def master_username(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstance, "master_username").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "masterUsername", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="masterUserPassword")
     def master_user_password(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: masterUserPassword: The master password for the database instance.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "masterUserPassword"))
 
     @master_user_password.setter
     def master_user_password(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstance, "master_user_password").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "masterUserPassword", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="masterUserType")
     def master_user_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -5514,51 +6226,60 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "masterUserType"))
 
     @master_user_type.setter
     def master_user_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstance, "master_user_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "masterUserType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="multiAz")
     def multi_az(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property: multiAz: Specifies if the database instance is a multiple Availability Zone deployment.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "multiAz"))
 
     @multi_az.setter
     def multi_az(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstance, "multi_az").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "multiAz", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="payType")
     def pay_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: payType: The charge type of created instance.
         '''
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
         :Property:
 
@@ -5569,102 +6290,120 @@
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
     @jsii.member(jsii_name="periodType")
     def period_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: periodType: Charge period for created instances.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "periodType"))
 
     @period_type.setter
     def period_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstance, "period_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "periodType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="port")
     def port(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: port: The port of the database service.
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "port"))
 
     @port.setter
     def port(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstance, "port").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "port", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="preferredBackupPeriod")
     def preferred_backup_period(
         self,
     ) -> typing.Optional[typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]]:
         '''
         :Property: preferredBackupPeriod: The backup period. Separate multiple values with commas (,). The default value is the original value. Valid values:Monday Tuesday Wednesday Thursday Friday Saturday Sunday Note When the BackupPolicyMode parameter is set to DataBackupPolicy, this parameter is required.
         '''
         return typing.cast(typing.Optional[typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]], jsii.get(self, "preferredBackupPeriod"))
 
     @preferred_backup_period.setter
     def preferred_backup_period(
         self,
         value: typing.Optional[typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstance, "preferred_backup_period").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "preferredBackupPeriod", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="preferredBackupTime")
     def preferred_backup_time(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: preferredBackupTime: The time when the backup task is performed. Format: yyyy-MM-ddZ-HH:mm:ssZ.Note When the BackupPolicyMode parameter is set to DataBackupPolicy, this parameter is required.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "preferredBackupTime"))
 
     @preferred_backup_time.setter
     def preferred_backup_time(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstance, "preferred_backup_time").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "preferredBackupTime", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="privateIpAddress")
     def private_ip_address(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: privateIpAddress: The private ip for created instance.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "privateIpAddress"))
 
     @private_ip_address.setter
     def private_ip_address(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstance, "private_ip_address").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "privateIpAddress", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="releasedKeepPolicy")
     def released_keep_policy(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -5676,51 +6415,60 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "releasedKeepPolicy"))
 
     @released_keep_policy.setter
     def released_keep_policy(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstance, "released_keep_policy").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "releasedKeepPolicy", value)
 
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
+            type_hints = typing.get_type_hints(getattr(RosDBInstance, "resource_group_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "resourceGroupId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="roleArn")
     def role_arn(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: roleArn: The Alibaba Cloud Resource Name (ARN) provided to the service account of the instance by your Alibaba Cloud account to connect to KMS. You can copy the ARN from the RAM console.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "roleArn"))
 
     @role_arn.setter
     def role_arn(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstance, "role_arn").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "roleArn", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="securityGroupId")
     def security_group_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -5732,34 +6480,40 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "securityGroupId"))
 
     @security_group_id.setter
     def security_group_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstance, "security_group_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "securityGroupId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="slaveZoneIds")
     def slave_zone_ids(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]]:
         '''
         :Property: slaveZoneIds: List of slave zone ids can specify slave zone ids when creating the high-availability or enterprise edition instance. Meanwhile, VSwitchId needs to pass in the corresponding vswitch id to the slave zone by order. For example, ZoneId = "zone-a" and SlaveZoneIds = ["zone-c", "zone-b"], then the VSwitchId must be "vsw-zone-a,vsw-zone-c,vsw-zone-b".
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]], jsii.get(self, "slaveZoneIds"))
 
     @slave_zone_ids.setter
     def slave_zone_ids(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstance, "slave_zone_ids").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "slaveZoneIds", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="sqlCollectorStatus")
     def sql_collector_status(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -5769,17 +6523,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "sqlCollectorStatus"))
 
     @sql_collector_status.setter
     def sql_collector_status(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstance, "sql_collector_status").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "sqlCollectorStatus", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="sslSetting")
     def ssl_setting(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -5792,17 +6549,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "sslSetting"))
 
     @ssl_setting.setter
     def ssl_setting(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstance, "ssl_setting").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "sslSetting", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="tags")
     def tags(self) -> typing.Optional[typing.Mapping[builtins.str, typing.Any]]:
         '''
         :Property:
 
         tags: The tags of an instance.
         You should input the information of the tag with the format of the Key-Value, such as {"key1":"value1","key2":"value2", ... "key5":"value5"}.
@@ -5821,116 +6581,137 @@
         return typing.cast(typing.Optional[typing.Mapping[builtins.str, typing.Any]], jsii.get(self, "tags"))
 
     @tags.setter
     def tags(
         self,
         value: typing.Optional[typing.Mapping[builtins.str, typing.Any]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstance, "tags").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "tags", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="targetDedicatedHostIdForLog")
     def target_dedicated_host_id_for_log(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: targetDedicatedHostIdForLog: The ID of the host to which the instance belongs if you create a log instance in a host group.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "targetDedicatedHostIdForLog"))
 
     @target_dedicated_host_id_for_log.setter
     def target_dedicated_host_id_for_log(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstance, "target_dedicated_host_id_for_log").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "targetDedicatedHostIdForLog", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="targetDedicatedHostIdForMaster")
     def target_dedicated_host_id_for_master(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: targetDedicatedHostIdForMaster: The ID of the host to which the instance belongs if you create a primary instance in a host group.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "targetDedicatedHostIdForMaster"))
 
     @target_dedicated_host_id_for_master.setter
     def target_dedicated_host_id_for_master(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstance, "target_dedicated_host_id_for_master").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "targetDedicatedHostIdForMaster", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="targetDedicatedHostIdForSlave")
     def target_dedicated_host_id_for_slave(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: targetDedicatedHostIdForSlave: The ID of the host to which the instance belongs if you create a secondary instance in a host group.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "targetDedicatedHostIdForSlave"))
 
     @target_dedicated_host_id_for_slave.setter
     def target_dedicated_host_id_for_slave(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstance, "target_dedicated_host_id_for_slave").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "targetDedicatedHostIdForSlave", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vpcId")
     def vpc_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: vpcId: The VPC id of created database instance. For VPC network, the property is required.
         '''
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
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vSwitchId")
     def v_switch_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: vSwitchId: The vSwitch id of created instance. For VPC network, the property is required.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "vSwitchId"))
 
     @v_switch_id.setter
     def v_switch_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstance, "v_switch_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "vSwitchId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="zoneId")
     def zone_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: zoneId: selected zone to create database instance. You cannot set the ZoneId parameter if the MultiAZ parameter is set to true.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "zoneId"))
 
     @zone_id.setter
     def zone_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstance, "zone_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "zoneId", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-rds.RosDBInstance.DBMappingsProperty",
         jsii_struct_bases=[],
         name_mapping={
             "character_set_name": "characterSetName",
@@ -5947,14 +6728,19 @@
             db_description: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param character_set_name: 
             :param db_name: 
             :param db_description: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosDBInstance.DBMappingsProperty.__init__)
+                check_type(argname="argument character_set_name", value=character_set_name, expected_type=type_hints["character_set_name"])
+                check_type(argname="argument db_name", value=db_name, expected_type=type_hints["db_name"])
+                check_type(argname="argument db_description", value=db_description, expected_type=type_hints["db_description"])
             self._values: typing.Dict[str, typing.Any] = {
                 "character_set_name": character_set_name,
                 "db_name": db_name,
             }
             if db_description is not None:
                 self._values["db_description"] = db_description
 
@@ -6007,160 +6793,181 @@
 ):
     '''A ROS template type:  ``ALIYUN::RDS::DBInstanceClone``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosDBInstanceCloneProps",
+        props: typing.Union["RosDBInstanceCloneProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::RDS::DBInstanceClone``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosDBInstanceClone.__init__)
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
+            type_hints = typing.get_type_hints(RosDBInstanceClone._render_properties)
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
     @jsii.member(jsii_name="attrDbInstanceId")
     def attr_db_instance_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: DBInstanceId: The instance id of created database instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDbInstanceId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInnerConnectionString")
     def attr_inner_connection_string(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: InnerConnectionString: DB instance connection url by Intranet.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInnerConnectionString"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInnerIpAddress")
     def attr_inner_ip_address(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: InnerIPAddress: IP Address for created DB instance of Intranet.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInnerIpAddress"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInnerPort")
     def attr_inner_port(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: InnerPort: Intranet port of created DB instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInnerPort"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPublicConnectionString")
     def attr_public_connection_string(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: PublicConnectionString: DB instance connection url by Internet.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPublicConnectionString"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPublicIpAddress")
     def attr_public_ip_address(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: PublicIPAddress: IP Address for created DB instance of Internet.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPublicIpAddress"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPublicPort")
     def attr_public_port(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: PublicPort: Internet port of created DB instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPublicPort"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dbInstanceId")
     def db_instance_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: dbInstanceId: Instance id
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "dbInstanceId"))
 
     @db_instance_id.setter
     def db_instance_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstanceClone, "db_instance_id").fset)
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
+            type_hints = typing.get_type_hints(getattr(RosDBInstanceClone, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="payType")
     def pay_type(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: payType: The charge type of created instance.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "payType"))
 
     @pay_type.setter
     def pay_type(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstanceClone, "pay_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "payType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="allocatePublicConnection")
     def allocate_public_connection(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property: allocatePublicConnection: If true, allocate public connection automate.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "allocatePublicConnection"))
 
     @allocate_public_connection.setter
     def allocate_public_connection(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstanceClone, "allocate_public_connection").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "allocatePublicConnection", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="backupId")
     def backup_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -6171,34 +6978,40 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "backupId"))
 
     @backup_id.setter
     def backup_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstanceClone, "backup_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "backupId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="backupRetentionPeriod")
     def backup_retention_period(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: backupRetentionPeriod: The retention period of the data backup. Value range: 7 to 730. The default value is the original value. Note When the BackupPolicyMode parameter is set to LogBackupPolicy, this parameter is required.
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "backupRetentionPeriod"))
 
     @backup_retention_period.setter
     def backup_retention_period(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstanceClone, "backup_retention_period").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "backupRetentionPeriod", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="backupType")
     def backup_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -6210,17 +7023,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "backupType"))
 
     @backup_type.setter
     def backup_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstanceClone, "backup_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "backupType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="category")
     def category(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -6233,17 +7049,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "category"))
 
     @category.setter
     def category(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstanceClone, "category").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "category", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="connectionStringPrefix")
     def connection_string_prefix(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -6254,85 +7073,100 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "connectionStringPrefix"))
 
     @connection_string_prefix.setter
     def connection_string_prefix(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstanceClone, "connection_string_prefix").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "connectionStringPrefix", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="connectionStringType")
     def connection_string_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: connectionStringType: The endpoint type of the instance, allow values: Inner, Public
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "connectionStringType"))
 
     @connection_string_type.setter
     def connection_string_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstanceClone, "connection_string_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "connectionStringType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dbInstanceClass")
     def db_instance_class(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: dbInstanceClass: Database instance type. Refer the RDS database instance type reference, such as 'rds.mys2.large', 'rds.mss1.large', 'rds.pg.s1.small' etc
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "dbInstanceClass"))
 
     @db_instance_class.setter
     def db_instance_class(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstanceClone, "db_instance_class").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dbInstanceClass", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dbInstanceDescription")
     def db_instance_description(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: dbInstanceDescription: Description of created database instance.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "dbInstanceDescription"))
 
     @db_instance_description.setter
     def db_instance_description(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstanceClone, "db_instance_description").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dbInstanceDescription", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dbInstanceStorage")
     def db_instance_storage(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: dbInstanceStorage: Database instance storage size. mysql is [5,1000]. sql server 2008r2 is [10,1000], sql server 2012/2012_web/2016-web is [20,1000]. PostgreSQL and PPAS is [5,2000]. Increased every 5 GB, Unit in GB
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "dbInstanceStorage"))
 
     @db_instance_storage.setter
     def db_instance_storage(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstanceClone, "db_instance_storage").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dbInstanceStorage", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dbInstanceStorageType")
     def db_instance_storage_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -6346,68 +7180,80 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "dbInstanceStorageType"))
 
     @db_instance_storage_type.setter
     def db_instance_storage_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstanceClone, "db_instance_storage_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dbInstanceStorageType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dbMappings")
     def db_mappings(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosDBInstanceClone.DBMappingsProperty"]]]]:
         '''
         :Property: dbMappings: Database mappings to attach to db instance.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosDBInstanceClone.DBMappingsProperty"]]]], jsii.get(self, "dbMappings"))
 
     @db_mappings.setter
     def db_mappings(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosDBInstanceClone.DBMappingsProperty"]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstanceClone, "db_mappings").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dbMappings", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dbNames")
     def db_names(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: dbNames: The names of the databases that you want to create on the new instance.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "dbNames"))
 
     @db_names.setter
     def db_names(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstanceClone, "db_names").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dbNames", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dedicatedHostGroupId")
     def dedicated_host_group_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: dedicatedHostGroupId: The ID of the host group to which the instance belongs if you create an instance in a host group.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "dedicatedHostGroupId"))
 
     @dedicated_host_group_id.setter
     def dedicated_host_group_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstanceClone, "dedicated_host_group_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dedicatedHostGroupId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="instanceNetworkType")
     def instance_network_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -6420,68 +7266,80 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "instanceNetworkType"))
 
     @instance_network_type.setter
     def instance_network_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstanceClone, "instance_network_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "instanceNetworkType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="maintainTime")
     def maintain_time(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: maintainTime: The period during which the maintenance performs. The format is HH:mmZ-HH:mmZ.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "maintainTime"))
 
     @maintain_time.setter
     def maintain_time(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstanceClone, "maintain_time").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "maintainTime", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="masterUsername")
     def master_username(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: masterUsername: The master user name for the database instance.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "masterUsername"))
 
     @master_username.setter
     def master_username(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstanceClone, "master_username").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "masterUsername", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="masterUserPassword")
     def master_user_password(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: masterUserPassword: The master password for the database instance.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "masterUserPassword"))
 
     @master_user_password.setter
     def master_user_password(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstanceClone, "master_user_password").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "masterUserPassword", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="masterUserType")
     def master_user_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -6494,17 +7352,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "masterUserType"))
 
     @master_user_type.setter
     def master_user_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstanceClone, "master_user_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "masterUserType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="period")
     def period(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -6515,102 +7376,120 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "period"))
 
     @period.setter
     def period(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstanceClone, "period").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "period", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="periodType")
     def period_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: periodType: Charge period for created instances.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "periodType"))
 
     @period_type.setter
     def period_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstanceClone, "period_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "periodType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="port")
     def port(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: port: The port of the database service.
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "port"))
 
     @port.setter
     def port(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstanceClone, "port").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "port", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="preferredBackupPeriod")
     def preferred_backup_period(
         self,
     ) -> typing.Optional[typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]]:
         '''
         :Property: preferredBackupPeriod: The backup period. Separate multiple values with commas (,). The default value is the original value. Valid values:Monday Tuesday Wednesday Thursday Friday Saturday Sunday Note When the BackupPolicyMode parameter is set to DataBackupPolicy, this parameter is required.
         '''
         return typing.cast(typing.Optional[typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]], jsii.get(self, "preferredBackupPeriod"))
 
     @preferred_backup_period.setter
     def preferred_backup_period(
         self,
         value: typing.Optional[typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstanceClone, "preferred_backup_period").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "preferredBackupPeriod", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="preferredBackupTime")
     def preferred_backup_time(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: preferredBackupTime: The time when the backup task is performed. Format: yyyy-MM-ddZ-HH:mm:ssZ.Note When the BackupPolicyMode parameter is set to DataBackupPolicy, this parameter is required.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "preferredBackupTime"))
 
     @preferred_backup_time.setter
     def preferred_backup_time(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstanceClone, "preferred_backup_time").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "preferredBackupTime", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="privateIpAddress")
     def private_ip_address(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: privateIpAddress: The private ip for created instance.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "privateIpAddress"))
 
     @private_ip_address.setter
     def private_ip_address(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstanceClone, "private_ip_address").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "privateIpAddress", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="restoreTable")
     def restore_table(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -6621,17 +7500,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "restoreTable"))
 
     @restore_table.setter
     def restore_table(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstanceClone, "restore_table").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "restoreTable", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="restoreTime")
     def restore_time(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -6643,17 +7525,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "restoreTime"))
 
     @restore_time.setter
     def restore_time(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstanceClone, "restore_time").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "restoreTime", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="securityGroupId")
     def security_group_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -6665,51 +7550,60 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "securityGroupId"))
 
     @security_group_id.setter
     def security_group_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstanceClone, "security_group_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "securityGroupId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="securityIpList")
     def security_ip_list(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: securityIpList: Security ip to access the database instance, combine with comma, 0.0.0.0/0 means no limitation.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "securityIpList"))
 
     @security_ip_list.setter
     def security_ip_list(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstanceClone, "security_ip_list").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "securityIpList", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="slaveZoneIds")
     def slave_zone_ids(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]]:
         '''
         :Property: slaveZoneIds: List of slave zone ids can specify slave zone ids when creating the high-availability or enterprise edition instance. Meanwhile, VSwitchId needs to pass in the corresponding vswitch id to the slave zone by order. For example, ZoneId = "zone-a" and SlaveZoneIds = ["zone-c", "zone-b"], then the VSwitchId must be "vsw-zone-a,vsw-zone-c,vsw-zone-b".
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]], jsii.get(self, "slaveZoneIds"))
 
     @slave_zone_ids.setter
     def slave_zone_ids(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstanceClone, "slave_zone_ids").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "slaveZoneIds", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="sqlCollectorStatus")
     def sql_collector_status(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -6719,17 +7613,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "sqlCollectorStatus"))
 
     @sql_collector_status.setter
     def sql_collector_status(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstanceClone, "sql_collector_status").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "sqlCollectorStatus", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="sslSetting")
     def ssl_setting(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -6742,34 +7639,40 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "sslSetting"))
 
     @ssl_setting.setter
     def ssl_setting(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstanceClone, "ssl_setting").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "sslSetting", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="tableMeta")
     def table_meta(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosDBInstanceClone.TableMetaProperty"]]]]:
         '''
         :Property: tableMeta: The information about the databases and tables that you want to restore.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosDBInstanceClone.TableMetaProperty"]]]], jsii.get(self, "tableMeta"))
 
     @table_meta.setter
     def table_meta(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosDBInstanceClone.TableMetaProperty"]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstanceClone, "table_meta").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "tableMeta", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="tags")
     def tags(self) -> typing.Optional[typing.Mapping[builtins.str, typing.Any]]:
         '''
         :Property:
 
         tags: The tags of an instance.
         You should input the information of the tag with the format of the Key-Value, such as {"key1":"value1","key2":"value2", ... "key5":"value5"}.
@@ -6788,82 +7691,97 @@
         return typing.cast(typing.Optional[typing.Mapping[builtins.str, typing.Any]], jsii.get(self, "tags"))
 
     @tags.setter
     def tags(
         self,
         value: typing.Optional[typing.Mapping[builtins.str, typing.Any]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstanceClone, "tags").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "tags", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="timeoutInMinutes")
     def timeout_in_minutes(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: timeoutInMinutes: The timeout period for creating the clone instance resource. Unit: Minute. Default: 120.
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "timeoutInMinutes"))
 
     @timeout_in_minutes.setter
     def timeout_in_minutes(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstanceClone, "timeout_in_minutes").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "timeoutInMinutes", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vpcId")
     def vpc_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: vpcId: The VPC id of created database instance. For VPC network, the property is required.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "vpcId"))
 
     @vpc_id.setter
     def vpc_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstanceClone, "vpc_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "vpcId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vSwitchId")
     def v_switch_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: vSwitchId: The vSwitch id of created instance. For VPC network, the property is required.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "vSwitchId"))
 
     @v_switch_id.setter
     def v_switch_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstanceClone, "v_switch_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "vSwitchId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="zoneId")
     def zone_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: zoneId: selected zone to create database instance. You cannot set the ZoneId parameter if the MultiAZ parameter is set to true.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "zoneId"))
 
     @zone_id.setter
     def zone_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstanceClone, "zone_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "zoneId", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-rds.RosDBInstanceClone.DBMappingsProperty",
         jsii_struct_bases=[],
         name_mapping={
             "character_set_name": "characterSetName",
@@ -6880,14 +7798,19 @@
             db_description: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param character_set_name: 
             :param db_name: 
             :param db_description: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosDBInstanceClone.DBMappingsProperty.__init__)
+                check_type(argname="argument character_set_name", value=character_set_name, expected_type=type_hints["character_set_name"])
+                check_type(argname="argument db_name", value=db_name, expected_type=type_hints["db_name"])
+                check_type(argname="argument db_description", value=db_description, expected_type=type_hints["db_description"])
             self._values: typing.Dict[str, typing.Any] = {
                 "character_set_name": character_set_name,
                 "db_name": db_name,
             }
             if db_description is not None:
                 self._values["db_description"] = db_description
 
@@ -6944,23 +7867,29 @@
     )
     class TableMetaProperty:
         def __init__(
             self,
             *,
             name: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
             new_name: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-            tables: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, "RosDBInstanceClone.TablesProperty"]]]] = None,
+            tables: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosDBInstanceClone.TablesProperty", typing.Dict[str, typing.Any]]]]]] = None,
             type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param name: 
             :param new_name: 
             :param tables: 
             :param type: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosDBInstanceClone.TableMetaProperty.__init__)
+                check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+                check_type(argname="argument new_name", value=new_name, expected_type=type_hints["new_name"])
+                check_type(argname="argument tables", value=tables, expected_type=type_hints["tables"])
+                check_type(argname="argument type", value=type, expected_type=type_hints["type"])
             self._values: typing.Dict[str, typing.Any] = {}
             if name is not None:
                 self._values["name"] = name
             if new_name is not None:
                 self._values["new_name"] = new_name
             if tables is not None:
                 self._values["tables"] = tables
@@ -7032,14 +7961,19 @@
             type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param name: 
             :param new_name: 
             :param type: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosDBInstanceClone.TablesProperty.__init__)
+                check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+                check_type(argname="argument new_name", value=new_name, expected_type=type_hints["new_name"])
+                check_type(argname="argument type", value=type, expected_type=type_hints["type"])
             self._values: typing.Dict[str, typing.Any] = {}
             if name is not None:
                 self._values["name"] = name
             if new_name is not None:
                 self._values["new_name"] = new_name
             if type is not None:
                 self._values["type"] = type
@@ -7145,15 +8079,15 @@
         category: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         connection_string_prefix: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         connection_string_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         db_instance_class: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         db_instance_description: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         db_instance_storage: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         db_instance_storage_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        db_mappings: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosDBInstanceClone.DBMappingsProperty]]]] = None,
+        db_mappings: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosDBInstanceClone.DBMappingsProperty, typing.Dict[str, typing.Any]]]]]] = None,
         db_names: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         dedicated_host_group_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         instance_network_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         maintain_time: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         master_username: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         master_user_password: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         master_user_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
@@ -7166,15 +8100,15 @@
         restore_table: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         restore_time: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         security_group_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         security_ip_list: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         slave_zone_ids: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]] = None,
         sql_collector_status: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ssl_setting: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        table_meta: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosDBInstanceClone.TableMetaProperty]]]] = None,
+        table_meta: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosDBInstanceClone.TableMetaProperty, typing.Dict[str, typing.Any]]]]]] = None,
         tags: typing.Optional[typing.Mapping[builtins.str, typing.Any]] = None,
         timeout_in_minutes: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         vpc_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         v_switch_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         zone_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::RDS::DBInstanceClone``.
@@ -7216,14 +8150,56 @@
         :param table_meta: 
         :param tags: 
         :param timeout_in_minutes: 
         :param vpc_id: 
         :param v_switch_id: 
         :param zone_id: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosDBInstanceCloneProps.__init__)
+            check_type(argname="argument db_instance_id", value=db_instance_id, expected_type=type_hints["db_instance_id"])
+            check_type(argname="argument pay_type", value=pay_type, expected_type=type_hints["pay_type"])
+            check_type(argname="argument allocate_public_connection", value=allocate_public_connection, expected_type=type_hints["allocate_public_connection"])
+            check_type(argname="argument backup_id", value=backup_id, expected_type=type_hints["backup_id"])
+            check_type(argname="argument backup_retention_period", value=backup_retention_period, expected_type=type_hints["backup_retention_period"])
+            check_type(argname="argument backup_type", value=backup_type, expected_type=type_hints["backup_type"])
+            check_type(argname="argument category", value=category, expected_type=type_hints["category"])
+            check_type(argname="argument connection_string_prefix", value=connection_string_prefix, expected_type=type_hints["connection_string_prefix"])
+            check_type(argname="argument connection_string_type", value=connection_string_type, expected_type=type_hints["connection_string_type"])
+            check_type(argname="argument db_instance_class", value=db_instance_class, expected_type=type_hints["db_instance_class"])
+            check_type(argname="argument db_instance_description", value=db_instance_description, expected_type=type_hints["db_instance_description"])
+            check_type(argname="argument db_instance_storage", value=db_instance_storage, expected_type=type_hints["db_instance_storage"])
+            check_type(argname="argument db_instance_storage_type", value=db_instance_storage_type, expected_type=type_hints["db_instance_storage_type"])
+            check_type(argname="argument db_mappings", value=db_mappings, expected_type=type_hints["db_mappings"])
+            check_type(argname="argument db_names", value=db_names, expected_type=type_hints["db_names"])
+            check_type(argname="argument dedicated_host_group_id", value=dedicated_host_group_id, expected_type=type_hints["dedicated_host_group_id"])
+            check_type(argname="argument instance_network_type", value=instance_network_type, expected_type=type_hints["instance_network_type"])
+            check_type(argname="argument maintain_time", value=maintain_time, expected_type=type_hints["maintain_time"])
+            check_type(argname="argument master_username", value=master_username, expected_type=type_hints["master_username"])
+            check_type(argname="argument master_user_password", value=master_user_password, expected_type=type_hints["master_user_password"])
+            check_type(argname="argument master_user_type", value=master_user_type, expected_type=type_hints["master_user_type"])
+            check_type(argname="argument period", value=period, expected_type=type_hints["period"])
+            check_type(argname="argument period_type", value=period_type, expected_type=type_hints["period_type"])
+            check_type(argname="argument port", value=port, expected_type=type_hints["port"])
+            check_type(argname="argument preferred_backup_period", value=preferred_backup_period, expected_type=type_hints["preferred_backup_period"])
+            check_type(argname="argument preferred_backup_time", value=preferred_backup_time, expected_type=type_hints["preferred_backup_time"])
+            check_type(argname="argument private_ip_address", value=private_ip_address, expected_type=type_hints["private_ip_address"])
+            check_type(argname="argument restore_table", value=restore_table, expected_type=type_hints["restore_table"])
+            check_type(argname="argument restore_time", value=restore_time, expected_type=type_hints["restore_time"])
+            check_type(argname="argument security_group_id", value=security_group_id, expected_type=type_hints["security_group_id"])
+            check_type(argname="argument security_ip_list", value=security_ip_list, expected_type=type_hints["security_ip_list"])
+            check_type(argname="argument slave_zone_ids", value=slave_zone_ids, expected_type=type_hints["slave_zone_ids"])
+            check_type(argname="argument sql_collector_status", value=sql_collector_status, expected_type=type_hints["sql_collector_status"])
+            check_type(argname="argument ssl_setting", value=ssl_setting, expected_type=type_hints["ssl_setting"])
+            check_type(argname="argument table_meta", value=table_meta, expected_type=type_hints["table_meta"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
+            check_type(argname="argument timeout_in_minutes", value=timeout_in_minutes, expected_type=type_hints["timeout_in_minutes"])
+            check_type(argname="argument vpc_id", value=vpc_id, expected_type=type_hints["vpc_id"])
+            check_type(argname="argument v_switch_id", value=v_switch_id, expected_type=type_hints["v_switch_id"])
+            check_type(argname="argument zone_id", value=zone_id, expected_type=type_hints["zone_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "db_instance_id": db_instance_id,
             "pay_type": pay_type,
         }
         if allocate_public_connection is not None:
             self._values["allocate_public_connection"] = allocate_public_connection
         if backup_id is not None:
@@ -7795,104 +8771,125 @@
 ):
     '''A ROS template type:  ``ALIYUN::RDS::DBInstanceParameterGroup``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosDBInstanceParameterGroupProps",
+        props: typing.Union["RosDBInstanceParameterGroupProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::RDS::DBInstanceParameterGroup``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosDBInstanceParameterGroup.__init__)
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
+            type_hints = typing.get_type_hints(RosDBInstanceParameterGroup._render_properties)
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
     @jsii.member(jsii_name="dbInstanceId")
     def db_instance_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: dbInstanceId: Database InstanceId to update properties.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "dbInstanceId"))
 
     @db_instance_id.setter
     def db_instance_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstanceParameterGroup, "db_instance_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dbInstanceId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         '''A factory method that creates a new instance of this class from an object containing the properties of this ROS resource.'''
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstanceParameterGroup, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="parameters")
     def parameters(
         self,
     ) -> typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosDBInstanceParameterGroup.ParametersProperty"]]]:
         '''
         :Property: parameters: Parameters to update for selected database instance.
         '''
         return typing.cast(typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosDBInstanceParameterGroup.ParametersProperty"]]], jsii.get(self, "parameters"))
 
     @parameters.setter
     def parameters(
         self,
         value: typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosDBInstanceParameterGroup.ParametersProperty"]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstanceParameterGroup, "parameters").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "parameters", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="forcerestart")
     def forcerestart(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: forcerestart: whether restart database instance.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "forcerestart"))
 
     @forcerestart.setter
     def forcerestart(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstanceParameterGroup, "forcerestart").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "forcerestart", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-rds.RosDBInstanceParameterGroup.ParametersProperty",
         jsii_struct_bases=[],
         name_mapping={"key": "key", "value": "value"},
     )
@@ -7903,14 +8900,18 @@
             key: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         ) -> None:
             '''
             :param key: 
             :param value: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosDBInstanceParameterGroup.ParametersProperty.__init__)
+                check_type(argname="argument key", value=key, expected_type=type_hints["key"])
+                check_type(argname="argument value", value=value, expected_type=type_hints["value"])
             self._values: typing.Dict[str, typing.Any] = {
                 "key": key,
                 "value": value,
             }
 
         @builtins.property
         def key(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
@@ -7952,23 +8953,28 @@
     },
 )
 class RosDBInstanceParameterGroupProps:
     def __init__(
         self,
         *,
         db_instance_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
-        parameters: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosDBInstanceParameterGroup.ParametersProperty]]],
+        parameters: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosDBInstanceParameterGroup.ParametersProperty, typing.Dict[str, typing.Any]]]]],
         forcerestart: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::RDS::DBInstanceParameterGroup``.
 
         :param db_instance_id: 
         :param parameters: 
         :param forcerestart: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosDBInstanceParameterGroupProps.__init__)
+            check_type(argname="argument db_instance_id", value=db_instance_id, expected_type=type_hints["db_instance_id"])
+            check_type(argname="argument parameters", value=parameters, expected_type=type_hints["parameters"])
+            check_type(argname="argument forcerestart", value=forcerestart, expected_type=type_hints["forcerestart"])
         self._values: typing.Dict[str, typing.Any] = {
             "db_instance_id": db_instance_id,
             "parameters": parameters,
         }
         if forcerestart is not None:
             self._values["forcerestart"] = forcerestart
 
@@ -8102,15 +9108,15 @@
         connection_mode: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         connection_string_prefix: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         connection_string_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         db_instance_description: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         db_instance_net_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         db_instance_storage_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         db_is_ignore_case: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
-        db_mappings: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosDBInstance.DBMappingsProperty]]]] = None,
+        db_mappings: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosDBInstance.DBMappingsProperty, typing.Dict[str, typing.Any]]]]]] = None,
         db_param_group_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         db_time_zone: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         dedicated_host_group_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         enable_backup_log: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         encryption_key: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         high_space_usage_protection: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         local_log_retention_hours: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
@@ -8204,14 +9210,76 @@
         :param target_dedicated_host_id_for_log: 
         :param target_dedicated_host_id_for_master: 
         :param target_dedicated_host_id_for_slave: 
         :param vpc_id: 
         :param v_switch_id: 
         :param zone_id: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosDBInstanceProps.__init__)
+            check_type(argname="argument db_instance_class", value=db_instance_class, expected_type=type_hints["db_instance_class"])
+            check_type(argname="argument db_instance_storage", value=db_instance_storage, expected_type=type_hints["db_instance_storage"])
+            check_type(argname="argument engine", value=engine, expected_type=type_hints["engine"])
+            check_type(argname="argument engine_version", value=engine_version, expected_type=type_hints["engine_version"])
+            check_type(argname="argument security_ip_list", value=security_ip_list, expected_type=type_hints["security_ip_list"])
+            check_type(argname="argument allocate_public_connection", value=allocate_public_connection, expected_type=type_hints["allocate_public_connection"])
+            check_type(argname="argument archive_backup_keep_count", value=archive_backup_keep_count, expected_type=type_hints["archive_backup_keep_count"])
+            check_type(argname="argument archive_backup_keep_policy", value=archive_backup_keep_policy, expected_type=type_hints["archive_backup_keep_policy"])
+            check_type(argname="argument archive_backup_retention_period", value=archive_backup_retention_period, expected_type=type_hints["archive_backup_retention_period"])
+            check_type(argname="argument auto_renew", value=auto_renew, expected_type=type_hints["auto_renew"])
+            check_type(argname="argument back_up_category", value=back_up_category, expected_type=type_hints["back_up_category"])
+            check_type(argname="argument backup_policy_mode", value=backup_policy_mode, expected_type=type_hints["backup_policy_mode"])
+            check_type(argname="argument backup_retention_period", value=backup_retention_period, expected_type=type_hints["backup_retention_period"])
+            check_type(argname="argument category", value=category, expected_type=type_hints["category"])
+            check_type(argname="argument compress_type", value=compress_type, expected_type=type_hints["compress_type"])
+            check_type(argname="argument connection_mode", value=connection_mode, expected_type=type_hints["connection_mode"])
+            check_type(argname="argument connection_string_prefix", value=connection_string_prefix, expected_type=type_hints["connection_string_prefix"])
+            check_type(argname="argument connection_string_type", value=connection_string_type, expected_type=type_hints["connection_string_type"])
+            check_type(argname="argument db_instance_description", value=db_instance_description, expected_type=type_hints["db_instance_description"])
+            check_type(argname="argument db_instance_net_type", value=db_instance_net_type, expected_type=type_hints["db_instance_net_type"])
+            check_type(argname="argument db_instance_storage_type", value=db_instance_storage_type, expected_type=type_hints["db_instance_storage_type"])
+            check_type(argname="argument db_is_ignore_case", value=db_is_ignore_case, expected_type=type_hints["db_is_ignore_case"])
+            check_type(argname="argument db_mappings", value=db_mappings, expected_type=type_hints["db_mappings"])
+            check_type(argname="argument db_param_group_id", value=db_param_group_id, expected_type=type_hints["db_param_group_id"])
+            check_type(argname="argument db_time_zone", value=db_time_zone, expected_type=type_hints["db_time_zone"])
+            check_type(argname="argument dedicated_host_group_id", value=dedicated_host_group_id, expected_type=type_hints["dedicated_host_group_id"])
+            check_type(argname="argument enable_backup_log", value=enable_backup_log, expected_type=type_hints["enable_backup_log"])
+            check_type(argname="argument encryption_key", value=encryption_key, expected_type=type_hints["encryption_key"])
+            check_type(argname="argument high_space_usage_protection", value=high_space_usage_protection, expected_type=type_hints["high_space_usage_protection"])
+            check_type(argname="argument local_log_retention_hours", value=local_log_retention_hours, expected_type=type_hints["local_log_retention_hours"])
+            check_type(argname="argument local_log_retention_space", value=local_log_retention_space, expected_type=type_hints["local_log_retention_space"])
+            check_type(argname="argument log_backup_frequency", value=log_backup_frequency, expected_type=type_hints["log_backup_frequency"])
+            check_type(argname="argument log_backup_local_retention_number", value=log_backup_local_retention_number, expected_type=type_hints["log_backup_local_retention_number"])
+            check_type(argname="argument log_backup_retention_period", value=log_backup_retention_period, expected_type=type_hints["log_backup_retention_period"])
+            check_type(argname="argument maintain_time", value=maintain_time, expected_type=type_hints["maintain_time"])
+            check_type(argname="argument master_username", value=master_username, expected_type=type_hints["master_username"])
+            check_type(argname="argument master_user_password", value=master_user_password, expected_type=type_hints["master_user_password"])
+            check_type(argname="argument master_user_type", value=master_user_type, expected_type=type_hints["master_user_type"])
+            check_type(argname="argument multi_az", value=multi_az, expected_type=type_hints["multi_az"])
+            check_type(argname="argument pay_type", value=pay_type, expected_type=type_hints["pay_type"])
+            check_type(argname="argument period", value=period, expected_type=type_hints["period"])
+            check_type(argname="argument period_type", value=period_type, expected_type=type_hints["period_type"])
+            check_type(argname="argument port", value=port, expected_type=type_hints["port"])
+            check_type(argname="argument preferred_backup_period", value=preferred_backup_period, expected_type=type_hints["preferred_backup_period"])
+            check_type(argname="argument preferred_backup_time", value=preferred_backup_time, expected_type=type_hints["preferred_backup_time"])
+            check_type(argname="argument private_ip_address", value=private_ip_address, expected_type=type_hints["private_ip_address"])
+            check_type(argname="argument released_keep_policy", value=released_keep_policy, expected_type=type_hints["released_keep_policy"])
+            check_type(argname="argument resource_group_id", value=resource_group_id, expected_type=type_hints["resource_group_id"])
+            check_type(argname="argument role_arn", value=role_arn, expected_type=type_hints["role_arn"])
+            check_type(argname="argument security_group_id", value=security_group_id, expected_type=type_hints["security_group_id"])
+            check_type(argname="argument slave_zone_ids", value=slave_zone_ids, expected_type=type_hints["slave_zone_ids"])
+            check_type(argname="argument sql_collector_status", value=sql_collector_status, expected_type=type_hints["sql_collector_status"])
+            check_type(argname="argument ssl_setting", value=ssl_setting, expected_type=type_hints["ssl_setting"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
+            check_type(argname="argument target_dedicated_host_id_for_log", value=target_dedicated_host_id_for_log, expected_type=type_hints["target_dedicated_host_id_for_log"])
+            check_type(argname="argument target_dedicated_host_id_for_master", value=target_dedicated_host_id_for_master, expected_type=type_hints["target_dedicated_host_id_for_master"])
+            check_type(argname="argument target_dedicated_host_id_for_slave", value=target_dedicated_host_id_for_slave, expected_type=type_hints["target_dedicated_host_id_for_slave"])
+            check_type(argname="argument vpc_id", value=vpc_id, expected_type=type_hints["vpc_id"])
+            check_type(argname="argument v_switch_id", value=v_switch_id, expected_type=type_hints["v_switch_id"])
+            check_type(argname="argument zone_id", value=zone_id, expected_type=type_hints["zone_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "db_instance_class": db_instance_class,
             "db_instance_storage": db_instance_storage,
             "engine": engine,
             "engine_version": engine_version,
             "security_ip_list": security_ip_list,
         }
@@ -8356,19 +9424,19 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], result)
 
     @builtins.property
     def engine_version(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
-        engineVersion: Database instance version of the relative engine type.Support MySQL: 5.5/5.6/5.7/8.0;
-        SQLServer: 2008r2/2012/2012_ent_ha/2012_std_ha/2012_web/2016_ent_ha/2016_std_ha/2016_web/2017_std_ha/2017_ent;
-        PostgreSQL: 9.4/10.0/11.0/12.0;
-        PPAS: 9.3/10.0;
-        MariaDB: 10.3.
+        engineVersion: Database instance version of the relative engine type. Support:
+        Valid values when you set the Engine parameter to MySQL: 5.5, 5.6, 5.7, and 8.0
+        Valid values when you set the Engine parameter to SQL Server: 2008r2, 08r2_ent_ha, 2012, 2012_ent_ha, 2012_std_ha, 2012_web, 2014_std_ha, 2016_ent_ha, 2016_std_ha, 2016_web, 2017_std_ha, 2017_ent, 2019_std_ha, and 2019_ent
+        Valid values when you set the Engine parameter to PostgreSQL: 10.0, 11.0, 12.0, 13.0, and 14.0
+        Valid values when you set the Engine parameter to MariaDB: 10.3
         '''
         result = self._values.get("engine_version")
         assert result is not None, "Required property 'engine_version' is missing"
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], result)
 
     @builtins.property
     def security_ip_list(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
@@ -9084,111 +10152,132 @@
 ):
     '''A ROS template type:  ``ALIYUN::RDS::DBInstanceSecurityIps``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosDBInstanceSecurityIpsProps",
+        props: typing.Union["RosDBInstanceSecurityIpsProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::RDS::DBInstanceSecurityIps``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosDBInstanceSecurityIps.__init__)
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
+            type_hints = typing.get_type_hints(RosDBInstanceSecurityIps._render_properties)
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
     @jsii.member(jsii_name="attrSecurityIps")
     def attr_security_ips(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: SecurityIps: The security ips of selected database instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrSecurityIps"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dbInstanceId")
     def db_instance_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: dbInstanceId: Database instance id to update security ips.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "dbInstanceId"))
 
     @db_instance_id.setter
     def db_instance_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstanceSecurityIps, "db_instance_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dbInstanceId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dbInstanceIpArrayAttribute")
     def db_instance_ip_array_attribute(
         self,
     ) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: dbInstanceIpArrayAttribute: Security ips to add or remove.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "dbInstanceIpArrayAttribute"))
 
     @db_instance_ip_array_attribute.setter
     def db_instance_ip_array_attribute(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstanceSecurityIps, "db_instance_ip_array_attribute").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dbInstanceIpArrayAttribute", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstanceSecurityIps, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dbInstanceIpArrayName")
     def db_instance_ip_array_name(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: dbInstanceIpArrayName: Group name of the security ips, only support lower characters and '_'. Advice use a new group name avoid effect your database system. If the properties is not specified, it will set to default group, please be careful.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "dbInstanceIpArrayName"))
 
     @db_instance_ip_array_name.setter
     def db_instance_ip_array_name(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstanceSecurityIps, "db_instance_ip_array_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dbInstanceIpArrayName", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-rds.RosDBInstanceSecurityIpsProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -9207,14 +10296,19 @@
     ) -> None:
         '''Properties for defining a ``ALIYUN::RDS::DBInstanceSecurityIps``.
 
         :param db_instance_id: 
         :param db_instance_ip_array_attribute: 
         :param db_instance_ip_array_name: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosDBInstanceSecurityIpsProps.__init__)
+            check_type(argname="argument db_instance_id", value=db_instance_id, expected_type=type_hints["db_instance_id"])
+            check_type(argname="argument db_instance_ip_array_attribute", value=db_instance_ip_array_attribute, expected_type=type_hints["db_instance_ip_array_attribute"])
+            check_type(argname="argument db_instance_ip_array_name", value=db_instance_ip_array_name, expected_type=type_hints["db_instance_ip_array_name"])
         self._values: typing.Dict[str, typing.Any] = {
             "db_instance_id": db_instance_id,
             "db_instance_ip_array_attribute": db_instance_ip_array_attribute,
         }
         if db_instance_ip_array_name is not None:
             self._values["db_instance_ip_array_name"] = db_instance_ip_array_name
 
@@ -9267,64 +10361,73 @@
 ):
     '''A ROS template type:  ``ALIYUN::RDS::Database``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosDatabaseProps",
+        props: typing.Union["RosDatabaseProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::RDS::Database``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosDatabase.__init__)
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
+            type_hints = typing.get_type_hints(RosDatabase._render_properties)
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
     @jsii.member(jsii_name="attrDbInstanceId")
     def attr_db_instance_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: DBInstanceId: The ID of the instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDbInstanceId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDbName")
     def attr_db_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: DBName: The name of the database.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDbName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="characterSetName")
     def character_set_name(
         self,
     ) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
@@ -9341,32 +10444,38 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "characterSetName"))
 
     @character_set_name.setter
     def character_set_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDatabase, "character_set_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "characterSetName", value)
 
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
+            type_hints = typing.get_type_hints(getattr(RosDatabase, "db_instance_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dbInstanceId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dbName")
     def db_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         dbName: The name of the database you want to create.
         Note
@@ -9379,26 +10488,32 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "dbName"))
 
     @db_name.setter
     def db_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDatabase, "db_name").fset)
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
+            type_hints = typing.get_type_hints(getattr(RosDatabase, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dbDescription")
     def db_description(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -9410,14 +10525,17 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "dbDescription"))
 
     @db_description.setter
     def db_description(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDatabase, "db_description").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dbDescription", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-rds.RosDatabaseProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -9439,14 +10557,20 @@
         '''Properties for defining a ``ALIYUN::RDS::Database``.
 
         :param character_set_name: 
         :param db_instance_id: 
         :param db_name: 
         :param db_description: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosDatabaseProps.__init__)
+            check_type(argname="argument character_set_name", value=character_set_name, expected_type=type_hints["character_set_name"])
+            check_type(argname="argument db_instance_id", value=db_instance_id, expected_type=type_hints["db_instance_id"])
+            check_type(argname="argument db_name", value=db_name, expected_type=type_hints["db_name"])
+            check_type(argname="argument db_description", value=db_description, expected_type=type_hints["db_description"])
         self._values: typing.Dict[str, typing.Any] = {
             "character_set_name": character_set_name,
             "db_instance_id": db_instance_id,
             "db_name": db_name,
         }
         if db_description is not None:
             self._values["db_description"] = db_description
@@ -9521,262 +10645,689 @@
 
     def __repr__(self) -> str:
         return "RosDatabaseProps(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
+class RosMigrateTask(
+    ros_cdk_core.RosResource,
+    metaclass=jsii.JSIIMeta,
+    jsii_type="@alicloud/ros-cdk-rds.RosMigrateTask",
+):
+    '''A ROS template type:  ``ALIYUN::RDS::MigrateTask``.'''
+
+    def __init__(
+        self,
+        scope: ros_cdk_core.Construct,
+        id: builtins.str,
+        props: typing.Union["RosMigrateTaskProps", typing.Dict[str, typing.Any]],
+        enable_resource_property_constraint: builtins.bool,
+    ) -> None:
+        '''Create a new ``ALIYUN::RDS::MigrateTask``.
+
+        :param scope: - scope in which this resource is defined.
+        :param id: - scoped id of the resource.
+        :param props: - resource properties.
+        :param enable_resource_property_constraint: -
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosMigrateTask.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
+        jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
+
+    @jsii.member(jsii_name="renderProperties")
+    def _render_properties(
+        self,
+        props: typing.Mapping[builtins.str, typing.Any],
+    ) -> typing.Mapping[builtins.str, typing.Any]:
+        '''
+        :param props: -
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosMigrateTask._render_properties)
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+        return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.invoke(self, "renderProperties", [props]))
+
+    @jsii.python.classproperty
+    @jsii.member(jsii_name="ROS_RESOURCE_TYPE_NAME")
+    def ROS_RESOURCE_TYPE_NAME(cls) -> builtins.str:
+        '''The resource type name for this resource class.'''
+        return typing.cast(builtins.str, jsii.sget(cls, "ROS_RESOURCE_TYPE_NAME"))
+
+    @builtins.property
+    @jsii.member(jsii_name="attrMigrateTaskId")
+    def attr_migrate_task_id(self) -> ros_cdk_core.IResolvable:
+        '''
+        :Attribute: MigrateTaskId: The ID of the migrate task.
+        '''
+        return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrMigrateTaskId"))
+
+    @builtins.property
+    @jsii.member(jsii_name="rosProperties")
+    def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
+        return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
+
+    @builtins.property
+    @jsii.member(jsii_name="backupMode")
+    def backup_mode(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
+        '''
+        :Property:
+
+        backupMode: The type of the migration task. Valid values:
+        FULL: specifies that full backup files are used to restore data.
+        UPDF: specifies that incremental backup files or log files are used to restore incremental data.
+        '''
+        return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "backupMode"))
+
+    @backup_mode.setter
+    def backup_mode(
+        self,
+        value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosMigrateTask, "backup_mode").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "backupMode", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="dbInstanceId")
+    def db_instance_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
+        '''
+        :Property: dbInstanceId: The ID of the instance.
+        '''
+        return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "dbInstanceId"))
+
+    @db_instance_id.setter
+    def db_instance_id(
+        self,
+        value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosMigrateTask, "db_instance_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "dbInstanceId", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="dbName")
+    def db_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
+        '''
+        :Property: dbName: The name of the database that you want to restore.
+        '''
+        return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "dbName"))
+
+    @db_name.setter
+    def db_name(
+        self,
+        value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosMigrateTask, "db_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "dbName", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="enableResourcePropertyConstraint")
+    def enable_resource_property_constraint(self) -> builtins.bool:
+        return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
+
+    @enable_resource_property_constraint.setter
+    def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosMigrateTask, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "enableResourcePropertyConstraint", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="isOnlineDb")
+    def is_online_db(self) -> typing.Union[builtins.bool, ros_cdk_core.IResolvable]:
+        '''
+        :Property: isOnlineDb: Specifies whether to bring the restored database online for user access. Note The value for SQL Server 2008 R2 is fixed to True.
+        '''
+        return typing.cast(typing.Union[builtins.bool, ros_cdk_core.IResolvable], jsii.get(self, "isOnlineDb"))
+
+    @is_online_db.setter
+    def is_online_db(
+        self,
+        value: typing.Union[builtins.bool, ros_cdk_core.IResolvable],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosMigrateTask, "is_online_db").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "isOnlineDb", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="checkDbMode")
+    def check_db_mode(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
+        '''
+        :Property:
+
+        checkDbMode: The consistency check method of the database. Valid values:
+        SyncExecuteDBCheck: synchronous database check
+        AsyncExecuteDBCheck: asynchronous database check
+        Default value: AsyncExecuteDBCheck (compatible with SQL Server 2008 R2).
+        Note When IsOnlineDB is set to True, this value is valid.
+        '''
+        return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "checkDbMode"))
+
+    @check_db_mode.setter
+    def check_db_mode(
+        self,
+        value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosMigrateTask, "check_db_mode").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "checkDbMode", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="ossObjectPositions")
+    def oss_object_positions(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
+        '''
+        :Property:
+
+        ossObjectPositions: The information of the backup file in the OSS bucket.
+        The values consist of three parts that are separated by colons (:):
+        The endpoint of the OSS bucket: oss-ap-southeast-1.aliyuncs.com.
+        The name of the OSS bucket: rdsmssqlsingapore.
+        The key of the backup file in the OSS bucket: autotest_2008R2_TestMigration_FULL.bak.
+        Note
+        This parameter is optional for instances that run SQL Server 2008 R2.
+        This parameter is required for instances that run a database engine later than SQL
+        Server 2008 R2.
+        '''
+        return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "ossObjectPositions"))
+
+    @oss_object_positions.setter
+    def oss_object_positions(
+        self,
+        value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosMigrateTask, "oss_object_positions").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "ossObjectPositions", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="ossUrls")
+    def oss_urls(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
+        '''
+        :Property:
+
+        ossUrls: The shared URL of the backup file in the OSS bucket. The URL must be encoded.
+        If you specify multiple URLs, separate them with vertical bars (|) and then encode
+        them.
+        Note This parameter must be entered for instances that run SQL Server 2008 R2.
+        '''
+        return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "ossUrls"))
+
+    @oss_urls.setter
+    def oss_urls(
+        self,
+        value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosMigrateTask, "oss_urls").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "ossUrls", value)
+
+
+@jsii.data_type(
+    jsii_type="@alicloud/ros-cdk-rds.RosMigrateTaskProps",
+    jsii_struct_bases=[],
+    name_mapping={
+        "backup_mode": "backupMode",
+        "db_instance_id": "dbInstanceId",
+        "db_name": "dbName",
+        "is_online_db": "isOnlineDb",
+        "check_db_mode": "checkDbMode",
+        "oss_object_positions": "ossObjectPositions",
+        "oss_urls": "ossUrls",
+    },
+)
+class RosMigrateTaskProps:
+    def __init__(
+        self,
+        *,
+        backup_mode: typing.Union[builtins.str, ros_cdk_core.IResolvable],
+        db_instance_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
+        db_name: typing.Union[builtins.str, ros_cdk_core.IResolvable],
+        is_online_db: typing.Union[builtins.bool, ros_cdk_core.IResolvable],
+        check_db_mode: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
+        oss_object_positions: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
+        oss_urls: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
+    ) -> None:
+        '''Properties for defining a ``ALIYUN::RDS::MigrateTask``.
+
+        :param backup_mode: 
+        :param db_instance_id: 
+        :param db_name: 
+        :param is_online_db: 
+        :param check_db_mode: 
+        :param oss_object_positions: 
+        :param oss_urls: 
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosMigrateTaskProps.__init__)
+            check_type(argname="argument backup_mode", value=backup_mode, expected_type=type_hints["backup_mode"])
+            check_type(argname="argument db_instance_id", value=db_instance_id, expected_type=type_hints["db_instance_id"])
+            check_type(argname="argument db_name", value=db_name, expected_type=type_hints["db_name"])
+            check_type(argname="argument is_online_db", value=is_online_db, expected_type=type_hints["is_online_db"])
+            check_type(argname="argument check_db_mode", value=check_db_mode, expected_type=type_hints["check_db_mode"])
+            check_type(argname="argument oss_object_positions", value=oss_object_positions, expected_type=type_hints["oss_object_positions"])
+            check_type(argname="argument oss_urls", value=oss_urls, expected_type=type_hints["oss_urls"])
+        self._values: typing.Dict[str, typing.Any] = {
+            "backup_mode": backup_mode,
+            "db_instance_id": db_instance_id,
+            "db_name": db_name,
+            "is_online_db": is_online_db,
+        }
+        if check_db_mode is not None:
+            self._values["check_db_mode"] = check_db_mode
+        if oss_object_positions is not None:
+            self._values["oss_object_positions"] = oss_object_positions
+        if oss_urls is not None:
+            self._values["oss_urls"] = oss_urls
+
+    @builtins.property
+    def backup_mode(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
+        '''
+        :Property:
+
+        backupMode: The type of the migration task. Valid values:
+        FULL: specifies that full backup files are used to restore data.
+        UPDF: specifies that incremental backup files or log files are used to restore incremental data.
+        '''
+        result = self._values.get("backup_mode")
+        assert result is not None, "Required property 'backup_mode' is missing"
+        return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], result)
+
+    @builtins.property
+    def db_instance_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
+        '''
+        :Property: dbInstanceId: The ID of the instance.
+        '''
+        result = self._values.get("db_instance_id")
+        assert result is not None, "Required property 'db_instance_id' is missing"
+        return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], result)
+
+    @builtins.property
+    def db_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
+        '''
+        :Property: dbName: The name of the database that you want to restore.
+        '''
+        result = self._values.get("db_name")
+        assert result is not None, "Required property 'db_name' is missing"
+        return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], result)
+
+    @builtins.property
+    def is_online_db(self) -> typing.Union[builtins.bool, ros_cdk_core.IResolvable]:
+        '''
+        :Property: isOnlineDb: Specifies whether to bring the restored database online for user access. Note The value for SQL Server 2008 R2 is fixed to True.
+        '''
+        result = self._values.get("is_online_db")
+        assert result is not None, "Required property 'is_online_db' is missing"
+        return typing.cast(typing.Union[builtins.bool, ros_cdk_core.IResolvable], result)
+
+    @builtins.property
+    def check_db_mode(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
+        '''
+        :Property:
+
+        checkDbMode: The consistency check method of the database. Valid values:
+        SyncExecuteDBCheck: synchronous database check
+        AsyncExecuteDBCheck: asynchronous database check
+        Default value: AsyncExecuteDBCheck (compatible with SQL Server 2008 R2).
+        Note When IsOnlineDB is set to True, this value is valid.
+        '''
+        result = self._values.get("check_db_mode")
+        return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], result)
+
+    @builtins.property
+    def oss_object_positions(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
+        '''
+        :Property:
+
+        ossObjectPositions: The information of the backup file in the OSS bucket.
+        The values consist of three parts that are separated by colons (:):
+        The endpoint of the OSS bucket: oss-ap-southeast-1.aliyuncs.com.
+        The name of the OSS bucket: rdsmssqlsingapore.
+        The key of the backup file in the OSS bucket: autotest_2008R2_TestMigration_FULL.bak.
+        Note
+        This parameter is optional for instances that run SQL Server 2008 R2.
+        This parameter is required for instances that run a database engine later than SQL
+        Server 2008 R2.
+        '''
+        result = self._values.get("oss_object_positions")
+        return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], result)
+
+    @builtins.property
+    def oss_urls(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
+        '''
+        :Property:
+
+        ossUrls: The shared URL of the backup file in the OSS bucket. The URL must be encoded.
+        If you specify multiple URLs, separate them with vertical bars (|) and then encode
+        them.
+        Note This parameter must be entered for instances that run SQL Server 2008 R2.
+        '''
+        result = self._values.get("oss_urls")
+        return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], result)
+
+    def __eq__(self, rhs: typing.Any) -> builtins.bool:
+        return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+    def __ne__(self, rhs: typing.Any) -> builtins.bool:
+        return not (rhs == self)
+
+    def __repr__(self) -> str:
+        return "RosMigrateTaskProps(%s)" % ", ".join(
+            k + "=" + repr(v) for k, v in self._values.items()
+        )
+
+
 class RosPrepayDBInstance(
     ros_cdk_core.RosResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@alicloud/ros-cdk-rds.RosPrepayDBInstance",
 ):
     '''A ROS template type:  ``ALIYUN::RDS::PrepayDBInstance``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosPrepayDBInstanceProps",
+        props: typing.Union["RosPrepayDBInstanceProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::RDS::PrepayDBInstance``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosPrepayDBInstance.__init__)
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
+            type_hints = typing.get_type_hints(RosPrepayDBInstance._render_properties)
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
     @jsii.member(jsii_name="attrDbInstanceId")
     def attr_db_instance_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: DBInstanceId: The instance id of created database instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDbInstanceId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInnerConnectionString")
     def attr_inner_connection_string(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: InnerConnectionString: DB instance connection url by Intranet.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInnerConnectionString"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInnerIpAddress")
     def attr_inner_ip_address(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: InnerIPAddress: IP Address for created DB instance of Intranet.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInnerIpAddress"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInnerPort")
     def attr_inner_port(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: InnerPort: Intranet port of created DB instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInnerPort"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrOrderId")
     def attr_order_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: OrderId: The order id list of created instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrOrderId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPublicConnectionString")
     def attr_public_connection_string(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: PublicConnectionString: DB instance connection url by Internet.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPublicConnectionString"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPublicIpAddress")
     def attr_public_ip_address(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: PublicIPAddress: IP Address for created DB instance of Internet.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPublicIpAddress"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPublicPort")
     def attr_public_port(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: PublicPort: Internet port of created DB instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPublicPort"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="commodityCode")
     def commodity_code(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: commodityCode: The CommodityCode of the order.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "commodityCode"))
 
     @commodity_code.setter
     def commodity_code(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPrepayDBInstance, "commodity_code").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "commodityCode", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dbInstanceClass")
     def db_instance_class(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: dbInstanceClass: Database instance type. Refer the RDS database instance type reference, such as 'rds.mys2.large', 'rds.mss1.large', 'rds.pg.s1.small' etc
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "dbInstanceClass"))
 
     @db_instance_class.setter
     def db_instance_class(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPrepayDBInstance, "db_instance_class").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dbInstanceClass", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dbInstanceStorage")
     def db_instance_storage(
         self,
     ) -> typing.Union[jsii.Number, ros_cdk_core.IResolvable]:
         '''
         :Property: dbInstanceStorage: Database instance storage size. mysql is [5,1000]. sql server 2008r2 is [10,1000], sql server 2012/2012_web/2016-web is [20,1000]. PostgreSQL and PPAS is [5,2000]. Increased every 5 GB, Unit in GB
         '''
         return typing.cast(typing.Union[jsii.Number, ros_cdk_core.IResolvable], jsii.get(self, "dbInstanceStorage"))
 
     @db_instance_storage.setter
     def db_instance_storage(
         self,
         value: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPrepayDBInstance, "db_instance_storage").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dbInstanceStorage", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPrepayDBInstance, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="engine")
     def engine(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: engine: Database instance engine type. Support MySQL/SQLServer/PostgreSQL/PPAS/MariaDB now.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "engine"))
 
     @engine.setter
     def engine(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPrepayDBInstance, "engine").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "engine", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="engineVersion")
     def engine_version(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
-        engineVersion: Database instance version of the relative engine type.Support MySQL: 5.5/5.6/5.7/8.0;
-        SQLServer: 2008r2/2012/2012_ent_ha/2012_std_ha/2012_web/2016_ent_ha/2016_std_ha/2016_web/2017_std_ha/2017_ent;
-        PostgreSQL: 9.4/10.0/11.0/12.0;
-        PPAS: 9.3/10.0;
-        MariaDB: 10.3.
+        engineVersion: Database instance version of the relative engine type. Support:
+        Valid values when you set the Engine parameter to MySQL: 5.5, 5.6, 5.7, and 8.0
+        Valid values when you set the Engine parameter to SQL Server: 2008r2, 08r2_ent_ha, 2012, 2012_ent_ha, 2012_std_ha, 2012_web, 2014_std_ha, 2016_ent_ha, 2016_std_ha, 2016_web, 2017_std_ha, 2017_ent, 2019_std_ha, and 2019_ent
+        Valid values when you set the Engine parameter to PostgreSQL: 10.0, 11.0, 12.0, 13.0, and 14.0
+        Valid values when you set the Engine parameter to MariaDB: 10.3
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "engineVersion"))
 
     @engine_version.setter
     def engine_version(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPrepayDBInstance, "engine_version").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "engineVersion", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="period")
     def period(self) -> typing.Union[jsii.Number, ros_cdk_core.IResolvable]:
         '''
         :Property: period: Prepaid time period. While choose by pay by month, it could be from 1 to 9. While choose pay by year, it could be from 1 to 3.
         '''
         return typing.cast(typing.Union[jsii.Number, ros_cdk_core.IResolvable], jsii.get(self, "period"))
 
     @period.setter
     def period(
         self,
         value: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPrepayDBInstance, "period").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "period", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="periodType")
     def period_type(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: periodType: Charge period for created instances.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "periodType"))
 
     @period_type.setter
     def period_type(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPrepayDBInstance, "period_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "periodType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="allocatePublicConnection")
     def allocate_public_connection(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property: allocatePublicConnection: If true, allocate public connection automate.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "allocatePublicConnection"))
 
     @allocate_public_connection.setter
     def allocate_public_connection(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPrepayDBInstance, "allocate_public_connection").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "allocatePublicConnection", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="archiveBackupKeepCount")
     def archive_backup_keep_count(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -9791,17 +11342,20 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "archiveBackupKeepCount"))
 
     @archive_backup_keep_count.setter
     def archive_backup_keep_count(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPrepayDBInstance, "archive_backup_keep_count").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "archiveBackupKeepCount", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="archiveBackupKeepPolicy")
     def archive_backup_keep_policy(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -9815,17 +11369,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "archiveBackupKeepPolicy"))
 
     @archive_backup_keep_policy.setter
     def archive_backup_keep_policy(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPrepayDBInstance, "archive_backup_keep_policy").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "archiveBackupKeepPolicy", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="archiveBackupRetentionPeriod")
     def archive_backup_retention_period(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -9835,51 +11392,60 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "archiveBackupRetentionPeriod"))
 
     @archive_backup_retention_period.setter
     def archive_backup_retention_period(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPrepayDBInstance, "archive_backup_retention_period").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "archiveBackupRetentionPeriod", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="autoPay")
     def auto_pay(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property: autoPay: Automatic Payment. Default is false.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "autoPay"))
 
     @auto_pay.setter
     def auto_pay(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPrepayDBInstance, "auto_pay").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "autoPay", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="autoRenew")
     def auto_renew(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property: autoRenew: Auto renew the prepay instance. If the period type is by year, it will renew by year, else it will renew by month.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "autoRenew"))
 
     @auto_renew.setter
     def auto_renew(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPrepayDBInstance, "auto_renew").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "autoRenew", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="backUpCategory")
     def back_up_category(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -9891,17 +11457,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "backUpCategory"))
 
     @back_up_category.setter
     def back_up_category(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPrepayDBInstance, "back_up_category").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "backUpCategory", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="backupPolicyMode")
     def backup_policy_mode(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -9912,34 +11481,40 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "backupPolicyMode"))
 
     @backup_policy_mode.setter
     def backup_policy_mode(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPrepayDBInstance, "backup_policy_mode").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "backupPolicyMode", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="backupRetentionPeriod")
     def backup_retention_period(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: backupRetentionPeriod: The retention period of the data backup. Value range: 7 to 730. The default value is the original value. Note When the BackupPolicyMode parameter is set to LogBackupPolicy, this parameter is required.
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "backupRetentionPeriod"))
 
     @backup_retention_period.setter
     def backup_retention_period(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPrepayDBInstance, "backup_retention_period").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "backupRetentionPeriod", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="category")
     def category(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -9952,17 +11527,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "category"))
 
     @category.setter
     def category(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPrepayDBInstance, "category").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "category", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="compressType")
     def compress_type(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -9978,34 +11556,40 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "compressType"))
 
     @compress_type.setter
     def compress_type(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPrepayDBInstance, "compress_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "compressType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="connectionMode")
     def connection_mode(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: connectionMode: Connection Mode for database instance,support 'Standard' and 'Safe' mode. Default is RDS system assigns.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "connectionMode"))
 
     @connection_mode.setter
     def connection_mode(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPrepayDBInstance, "connection_mode").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "connectionMode", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="connectionStringPrefix")
     def connection_string_prefix(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -10016,85 +11600,100 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "connectionStringPrefix"))
 
     @connection_string_prefix.setter
     def connection_string_prefix(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPrepayDBInstance, "connection_string_prefix").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "connectionStringPrefix", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="connectionStringType")
     def connection_string_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: connectionStringType: The endpoint type of the instance, allow values: Inner, Public
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "connectionStringType"))
 
     @connection_string_type.setter
     def connection_string_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPrepayDBInstance, "connection_string_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "connectionStringType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="couponCode")
     def coupon_code(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: couponCode: The coupon code of the order.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "couponCode"))
 
     @coupon_code.setter
     def coupon_code(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPrepayDBInstance, "coupon_code").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "couponCode", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dbInstanceDescription")
     def db_instance_description(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: dbInstanceDescription: Description of created database instance.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "dbInstanceDescription"))
 
     @db_instance_description.setter
     def db_instance_description(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPrepayDBInstance, "db_instance_description").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dbInstanceDescription", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dbInstanceNetType")
     def db_instance_net_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: dbInstanceNetType: Database instance net type, default is Intranet.Internet for public access, Intranet for private access.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "dbInstanceNetType"))
 
     @db_instance_net_type.setter
     def db_instance_net_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPrepayDBInstance, "db_instance_net_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dbInstanceNetType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dbInstanceStorageType")
     def db_instance_storage_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -10108,17 +11707,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "dbInstanceStorageType"))
 
     @db_instance_storage_type.setter
     def db_instance_storage_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPrepayDBInstance, "db_instance_storage_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dbInstanceStorageType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dbIsIgnoreCase")
     def db_is_ignore_case(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -10129,85 +11731,100 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "dbIsIgnoreCase"))
 
     @db_is_ignore_case.setter
     def db_is_ignore_case(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPrepayDBInstance, "db_is_ignore_case").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dbIsIgnoreCase", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dbMappings")
     def db_mappings(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosPrepayDBInstance.DBMappingsProperty"]]]]:
         '''
         :Property: dbMappings: Database mappings to attach to db instance.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosPrepayDBInstance.DBMappingsProperty"]]]], jsii.get(self, "dbMappings"))
 
     @db_mappings.setter
     def db_mappings(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosPrepayDBInstance.DBMappingsProperty"]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPrepayDBInstance, "db_mappings").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dbMappings", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dbParamGroupId")
     def db_param_group_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: dbParamGroupId: The ID of the parameter template used by the instance.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "dbParamGroupId"))
 
     @db_param_group_id.setter
     def db_param_group_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPrepayDBInstance, "db_param_group_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dbParamGroupId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dbTimeZone")
     def db_time_zone(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: dbTimeZone: The UTC time zone of the instance. Valid values: -12:00 to +12:00. The time zone must be an integer value such as +08:00. Values such as +08:30 are not allowed.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "dbTimeZone"))
 
     @db_time_zone.setter
     def db_time_zone(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPrepayDBInstance, "db_time_zone").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dbTimeZone", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dedicatedHostGroupId")
     def dedicated_host_group_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: dedicatedHostGroupId: The ID of the host group to which the instance belongs if you create an instance in a host group.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "dedicatedHostGroupId"))
 
     @dedicated_host_group_id.setter
     def dedicated_host_group_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPrepayDBInstance, "dedicated_host_group_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dedicatedHostGroupId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableBackupLog")
     def enable_backup_log(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -10219,34 +11836,40 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "enableBackupLog"))
 
     @enable_backup_log.setter
     def enable_backup_log(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPrepayDBInstance, "enable_backup_log").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableBackupLog", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="encryptionKey")
     def encryption_key(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: encryptionKey: The ID of the encryption key that is used to encrypt data on SSDs in the region. You can view the encryption key ID in the Key Management Service (KMS) console. You can also create an encryption key.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "encryptionKey"))
 
     @encryption_key.setter
     def encryption_key(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPrepayDBInstance, "encryption_key").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "encryptionKey", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="highSpaceUsageProtection")
     def high_space_usage_protection(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -10258,17 +11881,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "highSpaceUsageProtection"))
 
     @high_space_usage_protection.setter
     def high_space_usage_protection(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPrepayDBInstance, "high_space_usage_protection").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "highSpaceUsageProtection", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="localLogRetentionHours")
     def local_log_retention_hours(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -10280,17 +11906,20 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "localLogRetentionHours"))
 
     @local_log_retention_hours.setter
     def local_log_retention_hours(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPrepayDBInstance, "local_log_retention_hours").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "localLogRetentionHours", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="localLogRetentionSpace")
     def local_log_retention_space(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -10303,17 +11932,20 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "localLogRetentionSpace"))
 
     @local_log_retention_space.setter
     def local_log_retention_space(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPrepayDBInstance, "local_log_retention_space").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "localLogRetentionSpace", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="logBackupFrequency")
     def log_backup_frequency(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -10325,17 +11957,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "logBackupFrequency"))
 
     @log_backup_frequency.setter
     def log_backup_frequency(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPrepayDBInstance, "log_backup_frequency").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "logBackupFrequency", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="logBackupLocalRetentionNumber")
     def log_backup_local_retention_number(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -10345,17 +11980,20 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "logBackupLocalRetentionNumber"))
 
     @log_backup_local_retention_number.setter
     def log_backup_local_retention_number(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPrepayDBInstance, "log_backup_local_retention_number").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "logBackupLocalRetentionNumber", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="logBackupRetentionPeriod")
     def log_backup_retention_period(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -10367,68 +12005,80 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "logBackupRetentionPeriod"))
 
     @log_backup_retention_period.setter
     def log_backup_retention_period(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPrepayDBInstance, "log_backup_retention_period").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "logBackupRetentionPeriod", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="maintainTime")
     def maintain_time(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: maintainTime: The period during which the maintenance performs. The format is HH:mmZ-HH:mmZ.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "maintainTime"))
 
     @maintain_time.setter
     def maintain_time(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPrepayDBInstance, "maintain_time").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "maintainTime", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="masterUsername")
     def master_username(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: masterUsername: The master user name for the database instance.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "masterUsername"))
 
     @master_username.setter
     def master_username(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPrepayDBInstance, "master_username").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "masterUsername", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="masterUserPassword")
     def master_user_password(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: masterUserPassword: The master password for the database instance.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "masterUserPassword"))
 
     @master_user_password.setter
     def master_user_password(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPrepayDBInstance, "master_user_password").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "masterUserPassword", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="masterUserType")
     def master_user_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -10441,119 +12091,140 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "masterUserType"))
 
     @master_user_type.setter
     def master_user_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPrepayDBInstance, "master_user_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "masterUserType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="multiAz")
     def multi_az(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property: multiAz: Specifies if the database instance is a multiple Availability Zone deployment.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "multiAz"))
 
     @multi_az.setter
     def multi_az(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPrepayDBInstance, "multi_az").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "multiAz", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="port")
     def port(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: port: The port of the database service.
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "port"))
 
     @port.setter
     def port(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPrepayDBInstance, "port").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "port", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="preferredBackupPeriod")
     def preferred_backup_period(
         self,
     ) -> typing.Optional[typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]]:
         '''
         :Property: preferredBackupPeriod: The backup period. Separate multiple values with commas (,). The default value is the original value. Valid values:Monday Tuesday Wednesday Thursday Friday Saturday Sunday Note When the BackupPolicyMode parameter is set to DataBackupPolicy, this parameter is required.
         '''
         return typing.cast(typing.Optional[typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]], jsii.get(self, "preferredBackupPeriod"))
 
     @preferred_backup_period.setter
     def preferred_backup_period(
         self,
         value: typing.Optional[typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPrepayDBInstance, "preferred_backup_period").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "preferredBackupPeriod", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="preferredBackupTime")
     def preferred_backup_time(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: preferredBackupTime: The time when the backup task is performed. Format: yyyy-MM-ddZ-HH:mm:ssZ.Note When the BackupPolicyMode parameter is set to DataBackupPolicy, this parameter is required.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "preferredBackupTime"))
 
     @preferred_backup_time.setter
     def preferred_backup_time(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPrepayDBInstance, "preferred_backup_time").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "preferredBackupTime", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="privateIpAddress")
     def private_ip_address(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: privateIpAddress: The private ip for created instance.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "privateIpAddress"))
 
     @private_ip_address.setter
     def private_ip_address(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPrepayDBInstance, "private_ip_address").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "privateIpAddress", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="quantity")
     def quantity(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: quantity: The number of instance to be created, default is 1, max number is 99
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "quantity"))
 
     @quantity.setter
     def quantity(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPrepayDBInstance, "quantity").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "quantity", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="releasedKeepPolicy")
     def released_keep_policy(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -10565,51 +12236,60 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "releasedKeepPolicy"))
 
     @released_keep_policy.setter
     def released_keep_policy(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPrepayDBInstance, "released_keep_policy").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "releasedKeepPolicy", value)
 
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
+            type_hints = typing.get_type_hints(getattr(RosPrepayDBInstance, "resource_group_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "resourceGroupId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="roleArn")
     def role_arn(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: roleArn: The Alibaba Cloud Resource Name (ARN) provided to the service account of the instance by your Alibaba Cloud account to connect to KMS. You can copy the ARN from the RAM console.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "roleArn"))
 
     @role_arn.setter
     def role_arn(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPrepayDBInstance, "role_arn").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "roleArn", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="securityGroupId")
     def security_group_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -10621,34 +12301,40 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "securityGroupId"))
 
     @security_group_id.setter
     def security_group_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPrepayDBInstance, "security_group_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "securityGroupId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="slaveZoneIds")
     def slave_zone_ids(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]]:
         '''
         :Property: slaveZoneIds: List of slave zone ids can specify slave zone ids when creating the high-availability or enterprise edition instance. Meanwhile, VSwitchId needs to pass in the corresponding vswitch id to the slave zone by order. For example, ZoneId = "zone-a" and SlaveZoneIds = ["zone-c", "zone-b"], then the VSwitchId must be "vsw-zone-a,vsw-zone-c,vsw-zone-b".
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]], jsii.get(self, "slaveZoneIds"))
 
     @slave_zone_ids.setter
     def slave_zone_ids(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPrepayDBInstance, "slave_zone_ids").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "slaveZoneIds", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="sqlCollectorStatus")
     def sql_collector_status(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -10658,17 +12344,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "sqlCollectorStatus"))
 
     @sql_collector_status.setter
     def sql_collector_status(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPrepayDBInstance, "sql_collector_status").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "sqlCollectorStatus", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="sslSetting")
     def ssl_setting(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -10681,17 +12370,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "sslSetting"))
 
     @ssl_setting.setter
     def ssl_setting(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPrepayDBInstance, "ssl_setting").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "sslSetting", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="tags")
     def tags(self) -> typing.Optional[typing.Mapping[builtins.str, typing.Any]]:
         '''
         :Property:
 
         tags: The tags of an instance.
         You should input the information of the tag with the format of the Key-Value, such as {"key1":"value1","key2":"value2", ... "key5":"value5"}.
@@ -10710,116 +12402,137 @@
         return typing.cast(typing.Optional[typing.Mapping[builtins.str, typing.Any]], jsii.get(self, "tags"))
 
     @tags.setter
     def tags(
         self,
         value: typing.Optional[typing.Mapping[builtins.str, typing.Any]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPrepayDBInstance, "tags").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "tags", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="targetDedicatedHostIdForLog")
     def target_dedicated_host_id_for_log(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: targetDedicatedHostIdForLog: The ID of the host to which the instance belongs if you create a log instance in a host group.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "targetDedicatedHostIdForLog"))
 
     @target_dedicated_host_id_for_log.setter
     def target_dedicated_host_id_for_log(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPrepayDBInstance, "target_dedicated_host_id_for_log").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "targetDedicatedHostIdForLog", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="targetDedicatedHostIdForMaster")
     def target_dedicated_host_id_for_master(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: targetDedicatedHostIdForMaster: The ID of the host to which the instance belongs if you create a primary instance in a host group.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "targetDedicatedHostIdForMaster"))
 
     @target_dedicated_host_id_for_master.setter
     def target_dedicated_host_id_for_master(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPrepayDBInstance, "target_dedicated_host_id_for_master").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "targetDedicatedHostIdForMaster", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="targetDedicatedHostIdForSlave")
     def target_dedicated_host_id_for_slave(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: targetDedicatedHostIdForSlave: The ID of the host to which the instance belongs if you create a secondary instance in a host group.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "targetDedicatedHostIdForSlave"))
 
     @target_dedicated_host_id_for_slave.setter
     def target_dedicated_host_id_for_slave(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPrepayDBInstance, "target_dedicated_host_id_for_slave").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "targetDedicatedHostIdForSlave", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vpcId")
     def vpc_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: vpcId: The VPC id of created database instance. For VPC network, the property is required.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "vpcId"))
 
     @vpc_id.setter
     def vpc_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPrepayDBInstance, "vpc_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "vpcId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vSwitchId")
     def v_switch_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: vSwitchId: The vSwitch id of created instance. For VPC network, the property is required.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "vSwitchId"))
 
     @v_switch_id.setter
     def v_switch_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPrepayDBInstance, "v_switch_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "vSwitchId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="zoneId")
     def zone_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: zoneId: selected zone to create database instance. You cannot set the ZoneId parameter if the MultiAZ parameter is set to true.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "zoneId"))
 
     @zone_id.setter
     def zone_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosPrepayDBInstance, "zone_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "zoneId", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-rds.RosPrepayDBInstance.DBMappingsProperty",
         jsii_struct_bases=[],
         name_mapping={
             "character_set_name": "characterSetName",
@@ -10836,14 +12549,19 @@
             db_description: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param character_set_name: 
             :param db_name: 
             :param db_description: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosPrepayDBInstance.DBMappingsProperty.__init__)
+                check_type(argname="argument character_set_name", value=character_set_name, expected_type=type_hints["character_set_name"])
+                check_type(argname="argument db_name", value=db_name, expected_type=type_hints["db_name"])
+                check_type(argname="argument db_description", value=db_description, expected_type=type_hints["db_description"])
             self._values: typing.Dict[str, typing.Any] = {
                 "character_set_name": character_set_name,
                 "db_name": db_name,
             }
             if db_description is not None:
                 self._values["db_description"] = db_description
 
@@ -10983,15 +12701,15 @@
         connection_string_prefix: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         connection_string_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         coupon_code: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         db_instance_description: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         db_instance_net_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         db_instance_storage_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         db_is_ignore_case: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
-        db_mappings: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosPrepayDBInstance.DBMappingsProperty]]]] = None,
+        db_mappings: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosPrepayDBInstance.DBMappingsProperty, typing.Dict[str, typing.Any]]]]]] = None,
         db_param_group_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         db_time_zone: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         dedicated_host_group_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         enable_backup_log: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         encryption_key: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         high_space_usage_protection: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         local_log_retention_hours: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
@@ -11085,14 +12803,78 @@
         :param target_dedicated_host_id_for_log: 
         :param target_dedicated_host_id_for_master: 
         :param target_dedicated_host_id_for_slave: 
         :param vpc_id: 
         :param v_switch_id: 
         :param zone_id: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosPrepayDBInstanceProps.__init__)
+            check_type(argname="argument commodity_code", value=commodity_code, expected_type=type_hints["commodity_code"])
+            check_type(argname="argument db_instance_class", value=db_instance_class, expected_type=type_hints["db_instance_class"])
+            check_type(argname="argument db_instance_storage", value=db_instance_storage, expected_type=type_hints["db_instance_storage"])
+            check_type(argname="argument engine", value=engine, expected_type=type_hints["engine"])
+            check_type(argname="argument engine_version", value=engine_version, expected_type=type_hints["engine_version"])
+            check_type(argname="argument period", value=period, expected_type=type_hints["period"])
+            check_type(argname="argument period_type", value=period_type, expected_type=type_hints["period_type"])
+            check_type(argname="argument allocate_public_connection", value=allocate_public_connection, expected_type=type_hints["allocate_public_connection"])
+            check_type(argname="argument archive_backup_keep_count", value=archive_backup_keep_count, expected_type=type_hints["archive_backup_keep_count"])
+            check_type(argname="argument archive_backup_keep_policy", value=archive_backup_keep_policy, expected_type=type_hints["archive_backup_keep_policy"])
+            check_type(argname="argument archive_backup_retention_period", value=archive_backup_retention_period, expected_type=type_hints["archive_backup_retention_period"])
+            check_type(argname="argument auto_pay", value=auto_pay, expected_type=type_hints["auto_pay"])
+            check_type(argname="argument auto_renew", value=auto_renew, expected_type=type_hints["auto_renew"])
+            check_type(argname="argument back_up_category", value=back_up_category, expected_type=type_hints["back_up_category"])
+            check_type(argname="argument backup_policy_mode", value=backup_policy_mode, expected_type=type_hints["backup_policy_mode"])
+            check_type(argname="argument backup_retention_period", value=backup_retention_period, expected_type=type_hints["backup_retention_period"])
+            check_type(argname="argument category", value=category, expected_type=type_hints["category"])
+            check_type(argname="argument compress_type", value=compress_type, expected_type=type_hints["compress_type"])
+            check_type(argname="argument connection_mode", value=connection_mode, expected_type=type_hints["connection_mode"])
+            check_type(argname="argument connection_string_prefix", value=connection_string_prefix, expected_type=type_hints["connection_string_prefix"])
+            check_type(argname="argument connection_string_type", value=connection_string_type, expected_type=type_hints["connection_string_type"])
+            check_type(argname="argument coupon_code", value=coupon_code, expected_type=type_hints["coupon_code"])
+            check_type(argname="argument db_instance_description", value=db_instance_description, expected_type=type_hints["db_instance_description"])
+            check_type(argname="argument db_instance_net_type", value=db_instance_net_type, expected_type=type_hints["db_instance_net_type"])
+            check_type(argname="argument db_instance_storage_type", value=db_instance_storage_type, expected_type=type_hints["db_instance_storage_type"])
+            check_type(argname="argument db_is_ignore_case", value=db_is_ignore_case, expected_type=type_hints["db_is_ignore_case"])
+            check_type(argname="argument db_mappings", value=db_mappings, expected_type=type_hints["db_mappings"])
+            check_type(argname="argument db_param_group_id", value=db_param_group_id, expected_type=type_hints["db_param_group_id"])
+            check_type(argname="argument db_time_zone", value=db_time_zone, expected_type=type_hints["db_time_zone"])
+            check_type(argname="argument dedicated_host_group_id", value=dedicated_host_group_id, expected_type=type_hints["dedicated_host_group_id"])
+            check_type(argname="argument enable_backup_log", value=enable_backup_log, expected_type=type_hints["enable_backup_log"])
+            check_type(argname="argument encryption_key", value=encryption_key, expected_type=type_hints["encryption_key"])
+            check_type(argname="argument high_space_usage_protection", value=high_space_usage_protection, expected_type=type_hints["high_space_usage_protection"])
+            check_type(argname="argument local_log_retention_hours", value=local_log_retention_hours, expected_type=type_hints["local_log_retention_hours"])
+            check_type(argname="argument local_log_retention_space", value=local_log_retention_space, expected_type=type_hints["local_log_retention_space"])
+            check_type(argname="argument log_backup_frequency", value=log_backup_frequency, expected_type=type_hints["log_backup_frequency"])
+            check_type(argname="argument log_backup_local_retention_number", value=log_backup_local_retention_number, expected_type=type_hints["log_backup_local_retention_number"])
+            check_type(argname="argument log_backup_retention_period", value=log_backup_retention_period, expected_type=type_hints["log_backup_retention_period"])
+            check_type(argname="argument maintain_time", value=maintain_time, expected_type=type_hints["maintain_time"])
+            check_type(argname="argument master_username", value=master_username, expected_type=type_hints["master_username"])
+            check_type(argname="argument master_user_password", value=master_user_password, expected_type=type_hints["master_user_password"])
+            check_type(argname="argument master_user_type", value=master_user_type, expected_type=type_hints["master_user_type"])
+            check_type(argname="argument multi_az", value=multi_az, expected_type=type_hints["multi_az"])
+            check_type(argname="argument port", value=port, expected_type=type_hints["port"])
+            check_type(argname="argument preferred_backup_period", value=preferred_backup_period, expected_type=type_hints["preferred_backup_period"])
+            check_type(argname="argument preferred_backup_time", value=preferred_backup_time, expected_type=type_hints["preferred_backup_time"])
+            check_type(argname="argument private_ip_address", value=private_ip_address, expected_type=type_hints["private_ip_address"])
+            check_type(argname="argument quantity", value=quantity, expected_type=type_hints["quantity"])
+            check_type(argname="argument released_keep_policy", value=released_keep_policy, expected_type=type_hints["released_keep_policy"])
+            check_type(argname="argument resource_group_id", value=resource_group_id, expected_type=type_hints["resource_group_id"])
+            check_type(argname="argument role_arn", value=role_arn, expected_type=type_hints["role_arn"])
+            check_type(argname="argument security_group_id", value=security_group_id, expected_type=type_hints["security_group_id"])
+            check_type(argname="argument slave_zone_ids", value=slave_zone_ids, expected_type=type_hints["slave_zone_ids"])
+            check_type(argname="argument sql_collector_status", value=sql_collector_status, expected_type=type_hints["sql_collector_status"])
+            check_type(argname="argument ssl_setting", value=ssl_setting, expected_type=type_hints["ssl_setting"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
+            check_type(argname="argument target_dedicated_host_id_for_log", value=target_dedicated_host_id_for_log, expected_type=type_hints["target_dedicated_host_id_for_log"])
+            check_type(argname="argument target_dedicated_host_id_for_master", value=target_dedicated_host_id_for_master, expected_type=type_hints["target_dedicated_host_id_for_master"])
+            check_type(argname="argument target_dedicated_host_id_for_slave", value=target_dedicated_host_id_for_slave, expected_type=type_hints["target_dedicated_host_id_for_slave"])
+            check_type(argname="argument vpc_id", value=vpc_id, expected_type=type_hints["vpc_id"])
+            check_type(argname="argument v_switch_id", value=v_switch_id, expected_type=type_hints["v_switch_id"])
+            check_type(argname="argument zone_id", value=zone_id, expected_type=type_hints["zone_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "commodity_code": commodity_code,
             "db_instance_class": db_instance_class,
             "db_instance_storage": db_instance_storage,
             "engine": engine,
             "engine_version": engine_version,
             "period": period,
@@ -11248,19 +13030,19 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], result)
 
     @builtins.property
     def engine_version(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
-        engineVersion: Database instance version of the relative engine type.Support MySQL: 5.5/5.6/5.7/8.0;
-        SQLServer: 2008r2/2012/2012_ent_ha/2012_std_ha/2012_web/2016_ent_ha/2016_std_ha/2016_web/2017_std_ha/2017_ent;
-        PostgreSQL: 9.4/10.0/11.0/12.0;
-        PPAS: 9.3/10.0;
-        MariaDB: 10.3.
+        engineVersion: Database instance version of the relative engine type. Support:
+        Valid values when you set the Engine parameter to MySQL: 5.5, 5.6, 5.7, and 8.0
+        Valid values when you set the Engine parameter to SQL Server: 2008r2, 08r2_ent_ha, 2012, 2012_ent_ha, 2012_std_ha, 2012_web, 2014_std_ha, 2016_ent_ha, 2016_std_ha, 2016_web, 2017_std_ha, 2017_ent, 2019_std_ha, and 2019_ent
+        Valid values when you set the Engine parameter to PostgreSQL: 10.0, 11.0, 12.0, 13.0, and 14.0
+        Valid values when you set the Engine parameter to MariaDB: 10.3
         '''
         result = self._values.get("engine_version")
         assert result is not None, "Required property 'engine_version' is missing"
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], result)
 
     @builtins.property
     def period(self) -> typing.Union[jsii.Number, ros_cdk_core.IResolvable]:
@@ -11977,158 +13759,185 @@
 ):
     '''A ROS template type:  ``ALIYUN::RDS::ReadOnlyDBInstance``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosReadOnlyDBInstanceProps",
+        props: typing.Union["RosReadOnlyDBInstanceProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::RDS::ReadOnlyDBInstance``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosReadOnlyDBInstance.__init__)
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
+            type_hints = typing.get_type_hints(RosReadOnlyDBInstance._render_properties)
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
         :Attribute: ConnectionString: DB instance connection url by Intranet.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrConnectionString"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDbInstanceId")
     def attr_db_instance_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: DBInstanceId: The instance id of created database instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDbInstanceId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPort")
     def attr_port(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Port: Intranet port of created DB instance.
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
         :Property: dbInstanceClass: The type of the instance. For more information, see Instance type list. The type of the read-only instance must be no less than that of the master instance. Otherwise, the read-only instance incurs high latency and high load.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "dbInstanceClass"))
 
     @db_instance_class.setter
     def db_instance_class(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosReadOnlyDBInstance, "db_instance_class").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dbInstanceClass", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dbInstanceId")
     def db_instance_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: dbInstanceId: The ID of the master instance.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "dbInstanceId"))
 
     @db_instance_id.setter
     def db_instance_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosReadOnlyDBInstance, "db_instance_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dbInstanceId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dbInstanceStorage")
     def db_instance_storage(
         self,
     ) -> typing.Union[jsii.Number, ros_cdk_core.IResolvable]:
         '''
         :Property: dbInstanceStorage: The storage space of the instance. Value range: 5 to 3000. The value must be a multiple of 5. Unit: GB.
         '''
         return typing.cast(typing.Union[jsii.Number, ros_cdk_core.IResolvable], jsii.get(self, "dbInstanceStorage"))
 
     @db_instance_storage.setter
     def db_instance_storage(
         self,
         value: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosReadOnlyDBInstance, "db_instance_storage").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dbInstanceStorage", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosReadOnlyDBInstance, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="engineVersion")
     def engine_version(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: engineVersion: The version of the database. The database and the master instance must have the same database version. Valid values: 5.6, 5.7, 8.0, 2017_ent, 2019_ent
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "engineVersion"))
 
     @engine_version.setter
     def engine_version(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosReadOnlyDBInstance, "engine_version").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "engineVersion", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="zoneId")
     def zone_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: zoneId: The ID of the zone. You can call the DescribeRegions API operation to view the latest zones.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "zoneId"))
 
     @zone_id.setter
     def zone_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosReadOnlyDBInstance, "zone_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "zoneId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="autoRenew")
     def auto_renew(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -12139,17 +13948,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "autoRenew"))
 
     @auto_renew.setter
     def auto_renew(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosReadOnlyDBInstance, "auto_renew").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "autoRenew", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="category")
     def category(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -12162,34 +13974,40 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "category"))
 
     @category.setter
     def category(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosReadOnlyDBInstance, "category").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "category", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dbInstanceDescription")
     def db_instance_description(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: dbInstanceDescription: Description of created database instance.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "dbInstanceDescription"))
 
     @db_instance_description.setter
     def db_instance_description(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosReadOnlyDBInstance, "db_instance_description").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dbInstanceDescription", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dbInstanceStorageType")
     def db_instance_storage_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -12203,34 +14021,40 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "dbInstanceStorageType"))
 
     @db_instance_storage_type.setter
     def db_instance_storage_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosReadOnlyDBInstance, "db_instance_storage_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dbInstanceStorageType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="payType")
     def pay_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: payType: The billing method.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "payType"))
 
     @pay_type.setter
     def pay_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosReadOnlyDBInstance, "pay_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "payType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="period")
     def period(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -12241,68 +14065,80 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "period"))
 
     @period.setter
     def period(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosReadOnlyDBInstance, "period").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "period", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="periodType")
     def period_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: periodType: Charge period for created instances.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "periodType"))
 
     @period_type.setter
     def period_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosReadOnlyDBInstance, "period_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "periodType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="privateIpAddress")
     def private_ip_address(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: privateIpAddress: The private IP address of the read-only instance. It must be within the IP address range provided by the switch. The system automatically assigns an IP address based on the VPCId and VSwitchId by default.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "privateIpAddress"))
 
     @private_ip_address.setter
     def private_ip_address(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosReadOnlyDBInstance, "private_ip_address").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "privateIpAddress", value)
 
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
+            type_hints = typing.get_type_hints(getattr(RosReadOnlyDBInstance, "resource_group_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "resourceGroupId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="tags")
     def tags(self) -> typing.Optional[typing.Mapping[builtins.str, typing.Any]]:
         '''
         :Property:
 
         tags: The tags of an instance.
         You should input the information of the tag with the format of the Key-Value, such as {"key1":"value1","key2":"value2", ... "key5":"value5"}.
@@ -12321,48 +14157,57 @@
         return typing.cast(typing.Optional[typing.Mapping[builtins.str, typing.Any]], jsii.get(self, "tags"))
 
     @tags.setter
     def tags(
         self,
         value: typing.Optional[typing.Mapping[builtins.str, typing.Any]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosReadOnlyDBInstance, "tags").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "tags", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vpcId")
     def vpc_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: vpcId: The ID of the VPC.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "vpcId"))
 
     @vpc_id.setter
     def vpc_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosReadOnlyDBInstance, "vpc_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "vpcId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vSwitchId")
     def v_switch_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: vSwitchId: The ID of the VSwitch.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "vSwitchId"))
 
     @v_switch_id.setter
     def v_switch_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosReadOnlyDBInstance, "v_switch_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "vSwitchId", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-rds.RosReadOnlyDBInstanceProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -12423,14 +14268,33 @@
         :param period_type: 
         :param private_ip_address: 
         :param resource_group_id: 
         :param tags: 
         :param vpc_id: 
         :param v_switch_id: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosReadOnlyDBInstanceProps.__init__)
+            check_type(argname="argument db_instance_class", value=db_instance_class, expected_type=type_hints["db_instance_class"])
+            check_type(argname="argument db_instance_id", value=db_instance_id, expected_type=type_hints["db_instance_id"])
+            check_type(argname="argument db_instance_storage", value=db_instance_storage, expected_type=type_hints["db_instance_storage"])
+            check_type(argname="argument engine_version", value=engine_version, expected_type=type_hints["engine_version"])
+            check_type(argname="argument zone_id", value=zone_id, expected_type=type_hints["zone_id"])
+            check_type(argname="argument auto_renew", value=auto_renew, expected_type=type_hints["auto_renew"])
+            check_type(argname="argument category", value=category, expected_type=type_hints["category"])
+            check_type(argname="argument db_instance_description", value=db_instance_description, expected_type=type_hints["db_instance_description"])
+            check_type(argname="argument db_instance_storage_type", value=db_instance_storage_type, expected_type=type_hints["db_instance_storage_type"])
+            check_type(argname="argument pay_type", value=pay_type, expected_type=type_hints["pay_type"])
+            check_type(argname="argument period", value=period, expected_type=type_hints["period"])
+            check_type(argname="argument period_type", value=period_type, expected_type=type_hints["period_type"])
+            check_type(argname="argument private_ip_address", value=private_ip_address, expected_type=type_hints["private_ip_address"])
+            check_type(argname="argument resource_group_id", value=resource_group_id, expected_type=type_hints["resource_group_id"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
+            check_type(argname="argument vpc_id", value=vpc_id, expected_type=type_hints["vpc_id"])
+            check_type(argname="argument v_switch_id", value=v_switch_id, expected_type=type_hints["v_switch_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "db_instance_class": db_instance_class,
             "db_instance_id": db_instance_id,
             "db_instance_storage": db_instance_storage,
             "engine_version": engine_version,
             "zone_id": zone_id,
         }
@@ -12684,14 +14548,16 @@
     "DBInstanceParameterGroup",
     "DBInstanceParameterGroupProps",
     "DBInstanceProps",
     "DBInstanceSecurityIps",
     "DBInstanceSecurityIpsProps",
     "Database",
     "DatabaseProps",
+    "MigrateTask",
+    "MigrateTaskProps",
     "PrepayDBInstance",
     "PrepayDBInstanceProps",
     "ReadOnlyDBInstance",
     "ReadOnlyDBInstanceProps",
     "RosADInfo",
     "RosADInfoProps",
     "RosAccount",
@@ -12704,14 +14570,16 @@
     "RosDBInstanceParameterGroup",
     "RosDBInstanceParameterGroupProps",
     "RosDBInstanceProps",
     "RosDBInstanceSecurityIps",
     "RosDBInstanceSecurityIpsProps",
     "RosDatabase",
     "RosDatabaseProps",
+    "RosMigrateTask",
+    "RosMigrateTaskProps",
     "RosPrepayDBInstance",
     "RosPrepayDBInstanceProps",
     "RosReadOnlyDBInstance",
     "RosReadOnlyDBInstanceProps",
 ]
 
 publication.publish()
```

### Comparing `ros-cdk-rds-1.0.8/src/ros_cdk_rds.egg-info/PKG-INFO` & `ros-cdk-rds-1.0.9/src/ros_cdk_rds.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-rds
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS RDS Construct Library
```

