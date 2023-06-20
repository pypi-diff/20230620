# Comparing `tmp/ros-cdk-polardb-1.0.8.tar.gz` & `tmp/ros-cdk-polardb-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-polardb-1.0.8.tar", last modified: Thu Jul 14 02:24:58 2022, max compression
+gzip compressed data, was "dist/ros-cdk-polardb-1.0.9.tar", last modified: Fri Sep 23 12:06:11 2022, max compression
```

## Comparing `ros-cdk-polardb-1.0.8.tar` & `ros-cdk-polardb-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:24:58.000000 ros-cdk-polardb-1.0.8/
--rw-r--r--   0 root         (0) root         (0)    10279 2022-07-14 02:24:58.000000 ros-cdk-polardb-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2022-07-14 02:24:58.000000 ros-cdk-polardb-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2022-07-14 02:24:58.000000 ros-cdk-polardb-1.0.8/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1256 2022-07-14 02:24:58.000000 ros-cdk-polardb-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      191 2022-07-14 02:24:58.000000 ros-cdk-polardb-1.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)      106 2022-07-14 02:24:58.000000 ros-cdk-polardb-1.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-07-14 02:24:58.000000 ros-cdk-polardb-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1818 2022-07-14 02:24:58.000000 ros-cdk-polardb-1.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:24:58.000000 ros-cdk-polardb-1.0.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:24:58.000000 ros-cdk-polardb-1.0.8/src/ros_cdk_polardb/
--rw-r--r--   0 root         (0) root         (0)   216476 2022-07-14 02:24:58.000000 ros-cdk-polardb-1.0.8/src/ros_cdk_polardb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:24:58.000000 ros-cdk-polardb-1.0.8/src/ros_cdk_polardb/_jsii/
--rw-r--r--   0 root         (0) root         (0)      391 2022-07-14 02:24:58.000000 ros-cdk-polardb-1.0.8/src/ros_cdk_polardb/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)   102078 2022-07-14 02:24:58.000000 ros-cdk-polardb-1.0.8/src/ros_cdk_polardb/_jsii/ros-cdk-polardb@1.0.8.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:24:58.000000 ros-cdk-polardb-1.0.8/src/ros_cdk_polardb/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:24:58.000000 ros-cdk-polardb-1.0.8/src/ros_cdk_polardb.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1256 2022-07-14 02:24:58.000000 ros-cdk-polardb-1.0.8/src/ros_cdk_polardb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      440 2022-07-14 02:24:58.000000 ros-cdk-polardb-1.0.8/src/ros_cdk_polardb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:24:58.000000 ros-cdk-polardb-1.0.8/src/ros_cdk_polardb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2022-07-14 02:24:58.000000 ros-cdk-polardb-1.0.8/src/ros_cdk_polardb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2022-07-14 02:24:58.000000 ros-cdk-polardb-1.0.8/src/ros_cdk_polardb.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:06:11.000000 ros-cdk-polardb-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)    10279 2022-09-23 12:06:10.000000 ros-cdk-polardb-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-09-23 12:06:10.000000 ros-cdk-polardb-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2022-09-23 12:06:10.000000 ros-cdk-polardb-1.0.9/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1256 2022-09-23 12:06:11.000000 ros-cdk-polardb-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      191 2022-09-23 12:06:10.000000 ros-cdk-polardb-1.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      236 2022-09-23 12:06:10.000000 ros-cdk-polardb-1.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-09-23 12:06:11.000000 ros-cdk-polardb-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1847 2022-09-23 12:06:10.000000 ros-cdk-polardb-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:06:11.000000 ros-cdk-polardb-1.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:06:11.000000 ros-cdk-polardb-1.0.9/src/ros_cdk_polardb/
+-rw-r--r--   0 root         (0) root         (0)   260824 2022-09-23 12:06:10.000000 ros-cdk-polardb-1.0.9/src/ros_cdk_polardb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:06:11.000000 ros-cdk-polardb-1.0.9/src/ros_cdk_polardb/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      425 2022-09-23 12:06:10.000000 ros-cdk-polardb-1.0.9/src/ros_cdk_polardb/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   101412 2022-09-23 12:06:10.000000 ros-cdk-polardb-1.0.9/src/ros_cdk_polardb/_jsii/ros-cdk-polardb@1.0.9.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 12:06:10.000000 ros-cdk-polardb-1.0.9/src/ros_cdk_polardb/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 12:06:11.000000 ros-cdk-polardb-1.0.9/src/ros_cdk_polardb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1256 2022-09-23 12:06:11.000000 ros-cdk-polardb-1.0.9/src/ros_cdk_polardb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      440 2022-09-23 12:06:11.000000 ros-cdk-polardb-1.0.9/src/ros_cdk_polardb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 12:06:11.000000 ros-cdk-polardb-1.0.9/src/ros_cdk_polardb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2022-09-23 12:06:11.000000 ros-cdk-polardb-1.0.9/src/ros_cdk_polardb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2022-09-23 12:06:11.000000 ros-cdk-polardb-1.0.9/src/ros_cdk_polardb.egg-info/top_level.txt
```

### Comparing `ros-cdk-polardb-1.0.8/LICENSE` & `ros-cdk-polardb-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-polardb-1.0.8/PKG-INFO` & `ros-cdk-polardb-1.0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-polardb
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS POLARDB Construct Library
```

### Comparing `ros-cdk-polardb-1.0.8/setup.py` & `ros-cdk-polardb-1.0.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-polardb",
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
         "ros_cdk_polardb",
         "ros_cdk_polardb._jsii"
     ],
     "package_data": {
         "ros_cdk_polardb._jsii": [
-            "ros-cdk-polardb@1.0.8.jsii.tgz"
+            "ros-cdk-polardb@1.0.9.jsii.tgz"
         ],
         "ros_cdk_polardb": [
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

### Comparing `ros-cdk-polardb-1.0.8/src/ros_cdk_polardb/__init__.py` & `ros-cdk-polardb-1.0.9/src/ros_cdk_polardb/__init__.py`

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
 
 
 class Account(
     ros_cdk_core.Resource,
@@ -29,56 +31,68 @@
 ):
     '''A ROS resource type:  ``ALIYUN::POLARDB::Account``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "AccountProps",
+        props: typing.Union["AccountProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::POLARDB::Account``.
 
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
 
 
 class AccountPrivilege(
     ros_cdk_core.Resource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@alicloud/ros-cdk-polardb.AccountPrivilege",
 ):
     '''A ROS resource type:  ``ALIYUN::POLARDB::AccountPrivilege``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "AccountPrivilegeProps",
+        props: typing.Union["AccountPrivilegeProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::POLARDB::AccountPrivilege``.
 
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
     jsii_type="@alicloud/ros-cdk-polardb.AccountPrivilegeProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -100,14 +114,20 @@
         '''Properties for defining a ``ALIYUN::POLARDB::AccountPrivilege``.
 
         :param account_name: Property accountName: The name of the database account to be granted access permissions.
         :param account_privilege: Property accountPrivilege: The permissions of the database account on the database. Valid values: - ReadWrite: has read and write permissions on the database. - ReadOnly: has the read-only permission on the database. - DMLOnly: runs only data manipulation language (DML) statements. - DDLOnly: runs only data definition language (DDL) statements. The number of account permissions specified by the AccountPrivilege parameter must be the same as that of database names specified by the DBName parameter. Each account permission must correspond to a database name in sequence. Separate multiple permissions with a comma (,).
         :param db_cluster_id: Property dbClusterId: The ID of the ApsaraDB for POLARDB cluster to which a database account belongs.
         :param db_name: Property dbName: The name of the database whose access permissions are to be granted to the database account. You can grant access permissions on one or more databases to the database account. Separate multiple databases with a comma (,).
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(AccountPrivilegeProps.__init__)
+            check_type(argname="argument account_name", value=account_name, expected_type=type_hints["account_name"])
+            check_type(argname="argument account_privilege", value=account_privilege, expected_type=type_hints["account_privilege"])
+            check_type(argname="argument db_cluster_id", value=db_cluster_id, expected_type=type_hints["db_cluster_id"])
+            check_type(argname="argument db_name", value=db_name, expected_type=type_hints["db_name"])
         self._values: typing.Dict[str, typing.Any] = {
             "account_name": account_name,
             "account_privilege": account_privilege,
             "db_cluster_id": db_cluster_id,
             "db_name": db_name,
         }
 
@@ -196,14 +216,23 @@
         :param account_password: Property accountPassword: The password of the database account. The password must comply with the following rules: - It must consist of uppercase letters, lowercase letters, digits, and special characters. - Special characters include exclamation points (!), number signs (#), dollar signs ($), percent signs (%), carets (^), ampersands (&), asterisks (*), parentheses (()), underscores (_), plus signs (+), hyphens (-), and equal signs (=). - It must be 8 to 32 characters in length.
         :param db_cluster_id: Property dbClusterId: The ID of the ApsaraDB for POLARDB cluster for which a database account is to be created.
         :param account_description: Property accountDescription: The description of the database account. The description must comply with the following rules: - It cannot start with http:// or https://. - It must be 2 to 256 characters in length.
         :param account_privilege: Property accountPrivilege: The permissions of the database account on the database. Valid values: ReadWrite: has read and write permissions on the database. ReadOnly: has the read-only permission on the database. DMLOnly: runs only data manipulation language (DML) statements. DDLOnly: runs only data definition language (DDL) statements. Default value: ReadWrite. Separate multiple permissions with a comma (,).
         :param account_type: Property accountType: The type of the database account. Valid values: - Normal: standard account - Super: privileged account Default value: Super. Currently, POLARDB for PostgreSQL and POLARDB compatible with Oracle do not support standard accounts. You can create only one privileged account for an ApsaraDB for POLARDB cluster.
         :param db_name: Property dbName: The name of the database whose access permissions are to be granted to the database account. Separate multiple databases with a comma (,).
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(AccountProps.__init__)
+            check_type(argname="argument account_name", value=account_name, expected_type=type_hints["account_name"])
+            check_type(argname="argument account_password", value=account_password, expected_type=type_hints["account_password"])
+            check_type(argname="argument db_cluster_id", value=db_cluster_id, expected_type=type_hints["db_cluster_id"])
+            check_type(argname="argument account_description", value=account_description, expected_type=type_hints["account_description"])
+            check_type(argname="argument account_privilege", value=account_privilege, expected_type=type_hints["account_privilege"])
+            check_type(argname="argument account_type", value=account_type, expected_type=type_hints["account_type"])
+            check_type(argname="argument db_name", value=db_name, expected_type=type_hints["db_name"])
         self._values: typing.Dict[str, typing.Any] = {
             "account_name": account_name,
             "account_password": account_password,
             "db_cluster_id": db_cluster_id,
         }
         if account_description is not None:
             self._values["account_description"] = account_description
@@ -326,79 +355,85 @@
 ):
     '''A ROS resource type:  ``ALIYUN::POLARDB::DBCluster``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "DBClusterProps",
+        props: typing.Union["DBClusterProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::POLARDB::DBCluster``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(DBCluster.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrClusterConnectionString")
     def attr_cluster_connection_string(self) -> ros_cdk_core.IResolvable:
         '''Attribute ClusterConnectionString: The cluster connection string of the db cluster.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrClusterConnectionString"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrClusterEndpointId")
     def attr_cluster_endpoint_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute ClusterEndpointId: The cluster endpoint ID of the db cluster.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrClusterEndpointId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrCustomConnectionStrings")
     def attr_custom_connection_strings(self) -> ros_cdk_core.IResolvable:
         '''Attribute CustomConnectionStrings: The custom connection strings of the db cluster.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrCustomConnectionStrings"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrCustomEndpointIds")
     def attr_custom_endpoint_ids(self) -> ros_cdk_core.IResolvable:
         '''Attribute CustomEndpointIds: The custom endpoint IDs of the db cluster.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrCustomEndpointIds"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDbClusterId")
     def attr_db_cluster_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute DBClusterId: The ID of the ApsaraDB for POLARDB cluster.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDbClusterId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDbNodeIds")
     def attr_db_node_ids(self) -> ros_cdk_core.IResolvable:
         '''Attribute DBNodeIds: The ID list of cluster nodes.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDbNodeIds"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrOrderId")
     def attr_order_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute OrderId: The Order ID.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrOrderId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPrimaryConnectionString")
     def attr_primary_connection_string(self) -> ros_cdk_core.IResolvable:
         '''Attribute PrimaryConnectionString: The primary connection string of the db cluster.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPrimaryConnectionString"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPrimaryEndpointId")
     def attr_primary_endpoint_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute PrimaryEndpointId: The primary endpoint ID of the db cluster.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPrimaryEndpointId"))
 
 
 class DBClusterAccessWhiteList(
@@ -408,31 +443,37 @@
 ):
     '''A ROS resource type:  ``ALIYUN::POLARDB::DBClusterAccessWhiteList``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "DBClusterAccessWhiteListProps",
+        props: typing.Union["DBClusterAccessWhiteListProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::POLARDB::DBClusterAccessWhiteList``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(DBClusterAccessWhiteList.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDbClusterId")
     def attr_db_cluster_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute DBClusterId: The ID of the ApsaraDB for POLARDB cluster whose IP address whitelist is to be modified.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDbClusterId"))
 
 
 @jsii.data_type(
@@ -454,14 +495,19 @@
     ) -> None:
         '''Properties for defining a ``ALIYUN::POLARDB::DBClusterAccessWhiteList``.
 
         :param db_cluster_id: Property dbClusterId: The ID of the ApsaraDB for POLARDB cluster whose IP address whitelist is to be modified.
         :param security_ips: Property securityIps: The IP addresses to be added to the IP address whitelist group to be modified. Each whitelist group can contain a maximum of 1,000 IP addresses. Separate multiple IP addresses with a comma (,). The following two formats are supported: IP address: for example, 10.23.12.24. Classless inter-domain routing (CIDR) block: for example, 10.23.12.24/24, where the suffix /24 indicates the number of bits for the prefix of the IP address. The suffix ranges from 1 to 32.
         :param db_cluster_ip_array_name: Property dbClusterIpArrayName: The name of the IP address whitelist group. If you do not specify this parameter, the Default whitelist group is modified by default. Note You can create up to 50 whitelist groups for an ApsaraDB for POLARDB cluster.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(DBClusterAccessWhiteListProps.__init__)
+            check_type(argname="argument db_cluster_id", value=db_cluster_id, expected_type=type_hints["db_cluster_id"])
+            check_type(argname="argument security_ips", value=security_ips, expected_type=type_hints["security_ips"])
+            check_type(argname="argument db_cluster_ip_array_name", value=db_cluster_ip_array_name, expected_type=type_hints["db_cluster_ip_array_name"])
         self._values: typing.Dict[str, typing.Any] = {
             "db_cluster_id": db_cluster_id,
             "security_ips": security_ips,
         }
         if db_cluster_ip_array_name is not None:
             self._values["db_cluster_ip_array_name"] = db_cluster_ip_array_name
 
@@ -520,43 +566,49 @@
 ):
     '''A ROS resource type:  ``ALIYUN::POLARDB::DBClusterEndpoint``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "DBClusterEndpointProps",
+        props: typing.Union["DBClusterEndpointProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::POLARDB::DBClusterEndpoint``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(DBClusterEndpoint.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrAddresses")
     def attr_addresses(self) -> ros_cdk_core.IResolvable:
         '''Attribute Addresses: The address items of the db cluster endpoint.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAddresses"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrConnectionString")
     def attr_connection_string(self) -> ros_cdk_core.IResolvable:
         '''Attribute ConnectionString: The first connection string of the db cluster endpoint.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrConnectionString"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDbEndpointId")
     def attr_db_endpoint_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute DBEndpointId: DB cluster endpoint ID.
 
         E.g. pe-xxxxxxxx.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDbEndpointId"))
@@ -569,37 +621,43 @@
 ):
     '''A ROS resource type:  ``ALIYUN::POLARDB::DBClusterEndpointAddress``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "DBClusterEndpointAddressProps",
+        props: typing.Union["DBClusterEndpointAddressProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::POLARDB::DBClusterEndpointAddress``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(DBClusterEndpointAddress.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrAddress")
     def attr_address(self) -> ros_cdk_core.IResolvable:
         '''Attribute Address: The details of the endpoint address.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAddress"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrConnectionString")
     def attr_connection_string(self) -> ros_cdk_core.IResolvable:
         '''Attribute ConnectionString: The connection string of the endpoint address.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrConnectionString"))
 
 
 @jsii.data_type(
@@ -624,14 +682,20 @@
         '''Properties for defining a ``ALIYUN::POLARDB::DBClusterEndpointAddress``.
 
         :param db_cluster_id: Property dbClusterId: The ID of the ApsaraDB for POLARDB cluster for which a public connection point is to be created.
         :param db_endpoint_id: Property dbEndpointId: The ID of the cluster connection point.
         :param connection_string_prefix: Property connectionStringPrefix: The prefix of the connection string. The prefix must comply with the following rules: It must start with a letter and consist of lowercase letters, digits, and hyphens(-), cannot end with a dash. The length is 6~30 characters.
         :param net_type: Property netType: The network type of the connection string. If set to Public, ROS will create, modify and delete Public address for you. If set to Private, ROS will only modify Private address for you. Default to Public.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(DBClusterEndpointAddressProps.__init__)
+            check_type(argname="argument db_cluster_id", value=db_cluster_id, expected_type=type_hints["db_cluster_id"])
+            check_type(argname="argument db_endpoint_id", value=db_endpoint_id, expected_type=type_hints["db_endpoint_id"])
+            check_type(argname="argument connection_string_prefix", value=connection_string_prefix, expected_type=type_hints["connection_string_prefix"])
+            check_type(argname="argument net_type", value=net_type, expected_type=type_hints["net_type"])
         self._values: typing.Dict[str, typing.Any] = {
             "db_cluster_id": db_cluster_id,
             "db_endpoint_id": db_endpoint_id,
         }
         if connection_string_prefix is not None:
             self._values["connection_string_prefix"] = connection_string_prefix
         if net_type is not None:
@@ -703,28 +767,36 @@
 )
 class DBClusterEndpointProps:
     def __init__(
         self,
         *,
         db_cluster_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         auto_add_new_nodes: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        endpoint_config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosDBClusterEndpoint.EndpointConfigProperty"]] = None,
+        endpoint_config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosDBClusterEndpoint.EndpointConfigProperty", typing.Dict[str, typing.Any]]]] = None,
         endpoint_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         nodes: typing.Optional[typing.Union[typing.Sequence[typing.Any], ros_cdk_core.IResolvable]] = None,
         read_write_mode: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::POLARDB::DBClusterEndpoint``.
 
         :param db_cluster_id: Property dbClusterId: The ID of the ApsaraDB for POLARDB cluster for which a custom connection point is to be created.
         :param auto_add_new_nodes: Property autoAddNewNodes: Specifies whether a newly added node is automatically added to this connection point. Valid values: Enable, Disable. Default value: Disable.
         :param endpoint_config: Property endpointConfig:.
         :param endpoint_type: Property endpointType: The type of the cluster connection point. Set this parameter to Custom.
         :param nodes: Property nodes: The nodes to be added to this connection point to process read requests from this connection point. Add at least two nodes. If you do not specify this parameter, all nodes of the cluster are added to this connection point by default.
         :param read_write_mode: Property readWriteMode: The read/write mode of the cluster connection point. Valid values: ReadWrite: receives and forwards read and write requests (automatic read-write splitting). ReadOnly: receives and forwards only read requests. Default value: ReadOnly.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(DBClusterEndpointProps.__init__)
+            check_type(argname="argument db_cluster_id", value=db_cluster_id, expected_type=type_hints["db_cluster_id"])
+            check_type(argname="argument auto_add_new_nodes", value=auto_add_new_nodes, expected_type=type_hints["auto_add_new_nodes"])
+            check_type(argname="argument endpoint_config", value=endpoint_config, expected_type=type_hints["endpoint_config"])
+            check_type(argname="argument endpoint_type", value=endpoint_type, expected_type=type_hints["endpoint_type"])
+            check_type(argname="argument nodes", value=nodes, expected_type=type_hints["nodes"])
+            check_type(argname="argument read_write_mode", value=read_write_mode, expected_type=type_hints["read_write_mode"])
         self._values: typing.Dict[str, typing.Any] = {
             "db_cluster_id": db_cluster_id,
         }
         if auto_add_new_nodes is not None:
             self._values["auto_add_new_nodes"] = auto_add_new_nodes
         if endpoint_config is not None:
             self._values["endpoint_config"] = endpoint_config
@@ -828,14 +900,15 @@
         "db_cluster_description": "dbClusterDescription",
         "db_cluster_parameters": "dbClusterParameters",
         "default_time_zone": "defaultTimeZone",
         "gdn_id": "gdnId",
         "lower_case_table_names": "lowerCaseTableNames",
         "maintain_time": "maintainTime",
         "period": "period",
+        "period_unit": "periodUnit",
         "renewal_status": "renewalStatus",
         "resource_group_id": "resourceGroupId",
         "security_group_ids": "securityGroupIds",
         "security_ip_list": "securityIpList",
         "source_resource_id": "sourceResourceId",
         "tags": "tags",
         "tde_status": "tdeStatus",
@@ -855,26 +928,27 @@
         auto_renew_period: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         backup_retention_policy_on_cluster_deletion: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         clone_data_point: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         cluster_network_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         creation_category: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         creation_option: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         db_cluster_description: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        db_cluster_parameters: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosDBCluster.DBClusterParametersProperty"]] = None,
+        db_cluster_parameters: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union["RosDBCluster.DBClusterParametersProperty", typing.Dict[str, typing.Any]]]] = None,
         default_time_zone: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         gdn_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         lower_case_table_names: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         maintain_time: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         period: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
+        period_unit: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         renewal_status: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         resource_group_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         security_group_ids: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]] = None,
         security_ip_list: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         source_resource_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        tags: typing.Optional[typing.Sequence["RosDBCluster.TagsProperty"]] = None,
+        tags: typing.Optional[typing.Sequence[typing.Union["RosDBCluster.TagsProperty", typing.Dict[str, typing.Any]]]] = None,
         tde_status: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         vpc_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         v_switch_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         zone_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::POLARDB::DBCluster``.
 
@@ -890,26 +964,57 @@
         :param creation_option: Property creationOption: The method for creating an ApsaraDB for POLARDB cluster. Valid values: Normal: creates an ApsaraDB for POLARDB cluster. CloneFromPolarDB: clones data from an existing ApsaraDB for POLARDB cluster to a new ApsaraDB for POLARDB cluster. CloneFromRDS: clones data from an existing ApsaraDB for RDS instance to a new ApsaraDB for POLARDB cluster. MigrationFromRDS: migrates data from an existing ApsaraDB for RDS instance to a new ApsaraDB for POLARDB cluster. The created ApsaraDB for POLARDB cluster is in read-only mode and has binary logs enabled by default. CreateGdnStandby: Create a secondary cluster. Default value: Normal. Note: When DBType is MySQL and DBVersion is 5.6, this parameter can be specified as CloneFromRDS or MigrationFromRDS. When DBType is MySQL and DBVersion is 8.0, this parameter can be specified as CreateGdnStandby.
         :param db_cluster_description: Property dbClusterDescription: The description of the cluster. The description must comply with the following rules: It must start with a Chinese character or an English letter. It can contain Chinese and English characters, digits, underscores (_), and hyphens (-). It cannot start with http:// or https://. It must be 2 to 256 characters in length.
         :param db_cluster_parameters: Property dbClusterParameters: Modifies the parameters of a the PolarDB cluster.
         :param default_time_zone: Property defaultTimeZone: Set up a time zone (UTC), the value range is as follows: System: The default time zone is the same as the time zone where the region is located. This is default value. Other pickable value range is from -12:00 to +13:00, for example, 00:00. Note: This parameter takes effect only when DBType is MySQL.
         :param gdn_id: Property gdnId: The ID of the Global Database Network (GDN). Note: This parameter is required when the CreationOption is CreateGdnStandby.
         :param lower_case_table_names: Property lowerCaseTableNames: Whether the table name is case sensitive, the value range is as follows: 1: Not case sensitive0: case sensitive The default value is 1. Note: This parameter takes effect only when the value of DBType is MySQL.
         :param maintain_time: Property maintainTime: The maintainable time of the cluster: Format: HH: mmZ- HH: mmZ. Example: 16:00Z-17:00Z, which means 0 to 1 (UTC+08:00) for routine maintenance.
-        :param period: Property period: The subscription period of the cluster in month. Valid values: 1, 2, 3, 4, 5, 6, 7, 8, 9, 12, 24, 36.
+        :param period: Property period: The subscription period of the clusterIf PeriodUnit is month, the valid range is 1, 2, 3, 4, 5, 6, 7, 8, 9, 12, 24, 36 If periodUnit is year, the valid range is 1, 2, 3.
+        :param period_unit: Property periodUnit: The unit of the subscription duration. Valid values: Month Year Default value: Month.
         :param renewal_status: Property renewalStatus: The auto renewal status of the cluster Valid values: AutoRenewal: automatically renews the cluster. Normal: manually renews the cluster. NotRenewal: does not renew the cluster. Default value: Normal. Note If this parameter is set to NotRenewal, the system does not send a reminder for expiration, but only sends an SMS message three days before the cluster expires to remind you that the cluster is not renewed.
         :param resource_group_id: Property resourceGroupId: The ID of the resource group.
         :param security_group_ids: Property securityGroupIds: The ID of the security group. You can add up to three security groups to a cluster.
         :param security_ip_list: Property securityIpList: The whitelist of the Apsara PolarDB cluster.
         :param source_resource_id: Property sourceResourceId: The ID of the source RDS instance or source POLARDB cluster. Note This parameter takes effect only when the DBType parameter is set to MySQL and the DBVersion parameter is set to 5.6. This parameter is required if the CreationOption parameter is not set to Normal.
         :param tags: Property tags: Tags to attach to instance. Max support 20 tags to add during create instance. Each tag with two properties Key and Value, and Key is required.
         :param tde_status: Property tdeStatus: Specifies whether to enable Transparent Data Encryption (TDE). Valid values: true: enable TDE false: disable TDE (default) Note: The parameter takes effect only when DBType is PostgreSQL or Oracle. You cannot disable TDE after it is enabled.
         :param vpc_id: Property vpcId: The ID of the VPC to connect to.
         :param v_switch_id: Property vSwitchId: The ID of the VSwitch to connect to.
         :param zone_id: Property zoneId: The zone ID of the cluster. You can call the DescribeRegions operation to query available zones.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(DBClusterProps.__init__)
+            check_type(argname="argument db_node_class", value=db_node_class, expected_type=type_hints["db_node_class"])
+            check_type(argname="argument db_type", value=db_type, expected_type=type_hints["db_type"])
+            check_type(argname="argument db_version", value=db_version, expected_type=type_hints["db_version"])
+            check_type(argname="argument pay_type", value=pay_type, expected_type=type_hints["pay_type"])
+            check_type(argname="argument auto_renew_period", value=auto_renew_period, expected_type=type_hints["auto_renew_period"])
+            check_type(argname="argument backup_retention_policy_on_cluster_deletion", value=backup_retention_policy_on_cluster_deletion, expected_type=type_hints["backup_retention_policy_on_cluster_deletion"])
+            check_type(argname="argument clone_data_point", value=clone_data_point, expected_type=type_hints["clone_data_point"])
+            check_type(argname="argument cluster_network_type", value=cluster_network_type, expected_type=type_hints["cluster_network_type"])
+            check_type(argname="argument creation_category", value=creation_category, expected_type=type_hints["creation_category"])
+            check_type(argname="argument creation_option", value=creation_option, expected_type=type_hints["creation_option"])
+            check_type(argname="argument db_cluster_description", value=db_cluster_description, expected_type=type_hints["db_cluster_description"])
+            check_type(argname="argument db_cluster_parameters", value=db_cluster_parameters, expected_type=type_hints["db_cluster_parameters"])
+            check_type(argname="argument default_time_zone", value=default_time_zone, expected_type=type_hints["default_time_zone"])
+            check_type(argname="argument gdn_id", value=gdn_id, expected_type=type_hints["gdn_id"])
+            check_type(argname="argument lower_case_table_names", value=lower_case_table_names, expected_type=type_hints["lower_case_table_names"])
+            check_type(argname="argument maintain_time", value=maintain_time, expected_type=type_hints["maintain_time"])
+            check_type(argname="argument period", value=period, expected_type=type_hints["period"])
+            check_type(argname="argument period_unit", value=period_unit, expected_type=type_hints["period_unit"])
+            check_type(argname="argument renewal_status", value=renewal_status, expected_type=type_hints["renewal_status"])
+            check_type(argname="argument resource_group_id", value=resource_group_id, expected_type=type_hints["resource_group_id"])
+            check_type(argname="argument security_group_ids", value=security_group_ids, expected_type=type_hints["security_group_ids"])
+            check_type(argname="argument security_ip_list", value=security_ip_list, expected_type=type_hints["security_ip_list"])
+            check_type(argname="argument source_resource_id", value=source_resource_id, expected_type=type_hints["source_resource_id"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
+            check_type(argname="argument tde_status", value=tde_status, expected_type=type_hints["tde_status"])
+            check_type(argname="argument vpc_id", value=vpc_id, expected_type=type_hints["vpc_id"])
+            check_type(argname="argument v_switch_id", value=v_switch_id, expected_type=type_hints["v_switch_id"])
+            check_type(argname="argument zone_id", value=zone_id, expected_type=type_hints["zone_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "db_node_class": db_node_class,
             "db_type": db_type,
             "db_version": db_version,
             "pay_type": pay_type,
         }
         if auto_renew_period is not None:
@@ -934,14 +1039,16 @@
             self._values["gdn_id"] = gdn_id
         if lower_case_table_names is not None:
             self._values["lower_case_table_names"] = lower_case_table_names
         if maintain_time is not None:
             self._values["maintain_time"] = maintain_time
         if period is not None:
             self._values["period"] = period
+        if period_unit is not None:
+            self._values["period_unit"] = period_unit
         if renewal_status is not None:
             self._values["renewal_status"] = renewal_status
         if resource_group_id is not None:
             self._values["resource_group_id"] = resource_group_id
         if security_group_ids is not None:
             self._values["security_group_ids"] = security_group_ids
         if security_ip_list is not None:
@@ -1157,22 +1264,33 @@
         result = self._values.get("maintain_time")
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], result)
 
     @builtins.property
     def period(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
-        '''Property period: The subscription period of the cluster in month.
-
-        Valid values: 1, 2, 3, 4, 5, 6, 7, 8, 9, 12, 24, 36.
-        '''
+        '''Property period: The subscription period of the clusterIf PeriodUnit is month, the valid range is 1, 2, 3, 4, 5, 6, 7, 8, 9, 12, 24, 36 If periodUnit is year, the valid range is 1, 2, 3.'''
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
     def renewal_status(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''Property renewalStatus: The auto renewal status of the cluster Valid values: AutoRenewal: automatically renews the cluster.
 
         Normal: manually renews the cluster.
         NotRenewal: does not renew the cluster.
@@ -1293,28 +1411,34 @@
 ):
     '''A ROS resource type:  ``ALIYUN::POLARDB::DBInstance``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "DBInstanceProps",
+        props: typing.Union["DBInstanceProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::POLARDB::DBInstance``.
 
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
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-polardb.DBInstanceProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -1342,14 +1466,22 @@
         :param character_set_name: Property characterSetName: The character set of the database. For more information, see Character sets.
         :param db_cluster_id: Property dbClusterId: The ID of the ApsaraDB for POLARDB cluster for which a database is to be created.
         :param db_name: Property dbName: The name of the database to be created. The name must comply with the following rules: It must start with a lowercase letter and consist of lowercase letters, digits, hyphens (-), and underscores (_). It must end with a letter or a digit. It can be up to 64 characters in length.
         :param account_name: Property accountName: The name of the database account to be used.
         :param account_privilege: Property accountPrivilege: The permissions of the database account on the database. Valid values: ReadWrite: has read and write permissions on the database. ReadOnly: has the read-only permission on the database. DMLOnly: runs only data manipulation language (DML) statements. DDLOnly: runs only data definition language (DDL) statements. Default value: ReadWrite.
         :param db_description: Property dbDescription: The description of the database. Valid values: It cannot start with http:// or https://. It must be 2 to 256 characters in length.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(DBInstanceProps.__init__)
+            check_type(argname="argument character_set_name", value=character_set_name, expected_type=type_hints["character_set_name"])
+            check_type(argname="argument db_cluster_id", value=db_cluster_id, expected_type=type_hints["db_cluster_id"])
+            check_type(argname="argument db_name", value=db_name, expected_type=type_hints["db_name"])
+            check_type(argname="argument account_name", value=account_name, expected_type=type_hints["account_name"])
+            check_type(argname="argument account_privilege", value=account_privilege, expected_type=type_hints["account_privilege"])
+            check_type(argname="argument db_description", value=db_description, expected_type=type_hints["db_description"])
         self._values: typing.Dict[str, typing.Any] = {
             "character_set_name": character_set_name,
             "db_cluster_id": db_cluster_id,
             "db_name": db_name,
         }
         if account_name is not None:
             self._values["account_name"] = account_name
@@ -1446,37 +1578,43 @@
 ):
     '''A ROS resource type:  ``ALIYUN::POLARDB::DBNodes``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "DBNodesProps",
+        props: typing.Union["DBNodesProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::POLARDB::DBNodes``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(DBNodes.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDbNodeIds")
     def attr_db_node_ids(self) -> ros_cdk_core.IResolvable:
         '''Attribute DBNodeIds: The ID list of added cluster nodes.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDbNodeIds"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrOrderIds")
     def attr_order_ids(self) -> ros_cdk_core.IResolvable:
         '''Attribute OrderIds: The order ID list of added cluster nodes.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrOrderIds"))
 
 
 @jsii.data_type(
@@ -1498,14 +1636,19 @@
     ) -> None:
         '''Properties for defining a ``ALIYUN::POLARDB::DBNodes``.
 
         :param amount: Property amount: Number of nodes to be added to cluster.
         :param db_cluster_id: Property dbClusterId: The ID of the ApsaraDB for POLARDB cluster to be added nodes to.
         :param imci_switch: Property imciSwitch: Specifies whether to enable the In-Memory Column Index (IMCI) feature.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(DBNodesProps.__init__)
+            check_type(argname="argument amount", value=amount, expected_type=type_hints["amount"])
+            check_type(argname="argument db_cluster_id", value=db_cluster_id, expected_type=type_hints["db_cluster_id"])
+            check_type(argname="argument imci_switch", value=imci_switch, expected_type=type_hints["imci_switch"])
         self._values: typing.Dict[str, typing.Any] = {
             "amount": amount,
             "db_cluster_id": db_cluster_id,
         }
         if imci_switch is not None:
             self._values["imci_switch"] = imci_switch
 
@@ -1550,48 +1693,57 @@
 ):
     '''A ROS template type:  ``ALIYUN::POLARDB::Account``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosAccountProps",
+        props: typing.Union["RosAccountProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::POLARDB::Account``.
 
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
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="accountName")
     def account_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         accountName: The name of the database account. The name must comply with the following rules:
 
@@ -1601,17 +1753,20 @@
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
         :Property:
 
         accountPassword: The password of the database account. The password must comply with the following rules:
 
@@ -1622,42 +1777,51 @@
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
     @jsii.member(jsii_name="dbClusterId")
     def db_cluster_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: dbClusterId: The ID of the ApsaraDB for POLARDB cluster for which a database account is to be created.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "dbClusterId"))
 
     @db_cluster_id.setter
     def db_cluster_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAccount, "db_cluster_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dbClusterId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         '''A factory method that creates a new instance of this class from an object containing the properties of this ROS resource.'''
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
 
@@ -1669,17 +1833,20 @@
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
 
@@ -1694,17 +1861,20 @@
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
         :Property:
 
@@ -1719,94 +1889,112 @@
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
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dbName")
     def db_name(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: dbName: The name of the database whose access permissions are to be granted to the database account. Separate multiple databases with a comma (,).
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "dbName"))
 
     @db_name.setter
     def db_name(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAccount, "db_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dbName", value)
 
 
 class RosAccountPrivilege(
     ros_cdk_core.RosResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@alicloud/ros-cdk-polardb.RosAccountPrivilege",
 ):
     '''A ROS template type:  ``ALIYUN::POLARDB::AccountPrivilege``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosAccountPrivilegeProps",
+        props: typing.Union["RosAccountPrivilegeProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::POLARDB::AccountPrivilege``.
 
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
         :Property: accountName: The name of the database account to be granted access permissions.
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
         :Property:
 
         accountPrivilege: The permissions of the database account on the database. Valid values:
 
@@ -1820,32 +2008,38 @@
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
     @jsii.member(jsii_name="dbClusterId")
     def db_cluster_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: dbClusterId: The ID of the ApsaraDB for POLARDB cluster to which a database account belongs.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "dbClusterId"))
 
     @db_cluster_id.setter
     def db_cluster_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosAccountPrivilege, "db_cluster_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dbClusterId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dbName")
     def db_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         dbName: The name of the database whose access permissions are to be granted to the database account.
         You can grant access permissions on one or more databases to the database account.
@@ -1854,24 +2048,30 @@
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
     jsii_type="@alicloud/ros-cdk-polardb.RosAccountPrivilegeProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -1893,14 +2093,20 @@
         '''Properties for defining a ``ALIYUN::POLARDB::AccountPrivilege``.
 
         :param account_name: 
         :param account_privilege: 
         :param db_cluster_id: 
         :param db_name: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosAccountPrivilegeProps.__init__)
+            check_type(argname="argument account_name", value=account_name, expected_type=type_hints["account_name"])
+            check_type(argname="argument account_privilege", value=account_privilege, expected_type=type_hints["account_privilege"])
+            check_type(argname="argument db_cluster_id", value=db_cluster_id, expected_type=type_hints["db_cluster_id"])
+            check_type(argname="argument db_name", value=db_name, expected_type=type_hints["db_name"])
         self._values: typing.Dict[str, typing.Any] = {
             "account_name": account_name,
             "account_privilege": account_privilege,
             "db_cluster_id": db_cluster_id,
             "db_name": db_name,
         }
 
@@ -1996,14 +2202,23 @@
         :param account_password: 
         :param db_cluster_id: 
         :param account_description: 
         :param account_privilege: 
         :param account_type: 
         :param db_name: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosAccountProps.__init__)
+            check_type(argname="argument account_name", value=account_name, expected_type=type_hints["account_name"])
+            check_type(argname="argument account_password", value=account_password, expected_type=type_hints["account_password"])
+            check_type(argname="argument db_cluster_id", value=db_cluster_id, expected_type=type_hints["db_cluster_id"])
+            check_type(argname="argument account_description", value=account_description, expected_type=type_hints["account_description"])
+            check_type(argname="argument account_privilege", value=account_privilege, expected_type=type_hints["account_privilege"])
+            check_type(argname="argument account_type", value=account_type, expected_type=type_hints["account_type"])
+            check_type(argname="argument db_name", value=db_name, expected_type=type_hints["db_name"])
         self._values: typing.Dict[str, typing.Any] = {
             "account_name": account_name,
             "account_password": account_password,
             "db_cluster_id": db_cluster_id,
         }
         if account_description is not None:
             self._values["account_description"] = account_description
@@ -2132,135 +2347,147 @@
 ):
     '''A ROS template type:  ``ALIYUN::POLARDB::DBCluster``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosDBClusterProps",
+        props: typing.Union["RosDBClusterProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::POLARDB::DBCluster``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosDBCluster.__init__)
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
+            type_hints = typing.get_type_hints(RosDBCluster._render_properties)
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
     @jsii.member(jsii_name="attrClusterConnectionString")
     def attr_cluster_connection_string(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ClusterConnectionString: The cluster connection string of the db cluster.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrClusterConnectionString"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrClusterEndpointId")
     def attr_cluster_endpoint_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ClusterEndpointId: The cluster endpoint ID of the db cluster.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrClusterEndpointId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrCustomConnectionStrings")
     def attr_custom_connection_strings(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: CustomConnectionStrings: The custom connection strings of the db cluster.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrCustomConnectionStrings"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrCustomEndpointIds")
     def attr_custom_endpoint_ids(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: CustomEndpointIds: The custom endpoint IDs of the db cluster.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrCustomEndpointIds"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDbClusterId")
     def attr_db_cluster_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: DBClusterId: The ID of the ApsaraDB for POLARDB cluster.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDbClusterId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDbNodeIds")
     def attr_db_node_ids(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: DBNodeIds: The ID list of cluster nodes.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDbNodeIds"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrOrderId")
     def attr_order_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: OrderId: The Order ID.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrOrderId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPrimaryConnectionString")
     def attr_primary_connection_string(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: PrimaryConnectionString: The primary connection string of the db cluster.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPrimaryConnectionString"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPrimaryEndpointId")
     def attr_primary_endpoint_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: PrimaryEndpointId: The primary endpoint ID of the db cluster.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPrimaryEndpointId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dbNodeClass")
     def db_node_class(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: dbNodeClass: The node specifications of the cluster. For more information, see Specifications and pricing.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "dbNodeClass"))
 
     @db_node_class.setter
     def db_node_class(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBCluster, "db_node_class").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dbNodeClass", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dbType")
     def db_type(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         dbType: Database type, value:
         MySQL
@@ -2270,17 +2497,20 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "dbType"))
 
     @db_type.setter
     def db_type(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBCluster, "db_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dbType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dbVersion")
     def db_version(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         dbVersion: The version of the database. Valid values:
         MySQL: 5.6, 5.7 or 8.0
@@ -2290,26 +2520,32 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "dbVersion"))
 
     @db_version.setter
     def db_version(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBCluster, "db_version").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dbVersion", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBCluster, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="payType")
     def pay_type(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         payType: The billing method of the cluster. Valid values:
         Postpaid: pay-as-you-go
@@ -2318,34 +2554,40 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "payType"))
 
     @pay_type.setter
     def pay_type(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBCluster, "pay_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "payType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="autoRenewPeriod")
     def auto_renew_period(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: autoRenewPeriod: Set the cluster auto renewal time. Valid values: 1, 2, 3, 6, 12, 24, 36. Default to 1.
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "autoRenewPeriod"))
 
     @auto_renew_period.setter
     def auto_renew_period(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBCluster, "auto_renew_period").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "autoRenewPeriod", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="backupRetentionPolicyOnClusterDeletion")
     def backup_retention_policy_on_cluster_deletion(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -2359,17 +2601,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "backupRetentionPolicyOnClusterDeletion"))
 
     @backup_retention_policy_on_cluster_deletion.setter
     def backup_retention_policy_on_cluster_deletion(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBCluster, "backup_retention_policy_on_cluster_deletion").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "backupRetentionPolicyOnClusterDeletion", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="cloneDataPoint")
     def clone_data_point(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -2386,51 +2631,60 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "cloneDataPoint"))
 
     @clone_data_point.setter
     def clone_data_point(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBCluster, "clone_data_point").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "cloneDataPoint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="clusterNetworkType")
     def cluster_network_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: clusterNetworkType: The network type of the cluster. Currently, only VPC is supported. Default value: VPC.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "clusterNetworkType"))
 
     @cluster_network_type.setter
     def cluster_network_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBCluster, "cluster_network_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "clusterNetworkType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="creationCategory")
     def creation_category(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: creationCategory: Cluster series. The value could be Normal (standard version).
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "creationCategory"))
 
     @creation_category.setter
     def creation_category(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBCluster, "creation_category").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "creationCategory", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="creationOption")
     def creation_option(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -2449,17 +2703,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "creationOption"))
 
     @creation_option.setter
     def creation_option(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBCluster, "creation_option").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "creationOption", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dbClusterDescription")
     def db_cluster_description(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -2472,34 +2729,40 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "dbClusterDescription"))
 
     @db_cluster_description.setter
     def db_cluster_description(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBCluster, "db_cluster_description").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dbClusterDescription", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dbClusterParameters")
     def db_cluster_parameters(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosDBCluster.DBClusterParametersProperty"]]:
         '''
         :Property: dbClusterParameters: Modifies the parameters of a the PolarDB cluster.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosDBCluster.DBClusterParametersProperty"]], jsii.get(self, "dbClusterParameters"))
 
     @db_cluster_parameters.setter
     def db_cluster_parameters(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosDBCluster.DBClusterParametersProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBCluster, "db_cluster_parameters").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dbClusterParameters", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="defaultTimeZone")
     def default_time_zone(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -2511,17 +2774,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "defaultTimeZone"))
 
     @default_time_zone.setter
     def default_time_zone(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBCluster, "default_time_zone").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "defaultTimeZone", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="gdnId")
     def gdn_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -2531,17 +2797,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "gdnId"))
 
     @gdn_id.setter
     def gdn_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBCluster, "gdn_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "gdnId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="lowerCaseTableNames")
     def lower_case_table_names(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -2553,17 +2822,20 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "lowerCaseTableNames"))
 
     @lower_case_table_names.setter
     def lower_case_table_names(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBCluster, "lower_case_table_names").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "lowerCaseTableNames", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="maintainTime")
     def maintain_time(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -2574,34 +2846,68 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "maintainTime"))
 
     @maintain_time.setter
     def maintain_time(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBCluster, "maintain_time").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "maintainTime", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="period")
     def period(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
-        :Property: period: The subscription period of the cluster in month. Valid values: 1, 2, 3, 4, 5, 6, 7, 8, 9, 12, 24, 36.
+        :Property:
+
+        period: The subscription period of the clusterIf PeriodUnit is month, the valid range is 1, 2, 3, 4, 5, 6, 7, 8, 9, 12, 24, 36
+        If periodUnit is year, the valid range is 1, 2, 3
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "period"))
 
     @period.setter
     def period(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBCluster, "period").fset)
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
+            type_hints = typing.get_type_hints(getattr(RosDBCluster, "period_unit").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "periodUnit", value)
+
+    @builtins.property
     @jsii.member(jsii_name="renewalStatus")
     def renewal_status(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -2617,34 +2923,40 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "renewalStatus"))
 
     @renewal_status.setter
     def renewal_status(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBCluster, "renewal_status").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "renewalStatus", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="resourceGroupId")
     def resource_group_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: resourceGroupId: The ID of the resource group.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "resourceGroupId"))
 
     @resource_group_id.setter
     def resource_group_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBCluster, "resource_group_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "resourceGroupId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="securityGroupIds")
     def security_group_ids(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]]:
         '''
         :Property:
 
@@ -2654,34 +2966,40 @@
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]], jsii.get(self, "securityGroupIds"))
 
     @security_group_ids.setter
     def security_group_ids(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBCluster, "security_group_ids").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "securityGroupIds", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="securityIpList")
     def security_ip_list(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: securityIpList: The whitelist of the Apsara PolarDB cluster.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "securityIpList"))
 
     @security_ip_list.setter
     def security_ip_list(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBCluster, "security_ip_list").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "securityIpList", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="sourceResourceId")
     def source_resource_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -2693,32 +3011,38 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "sourceResourceId"))
 
     @source_resource_id.setter
     def source_resource_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBCluster, "source_resource_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "sourceResourceId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="tags")
     def tags(self) -> typing.Optional[typing.List["RosDBCluster.TagsProperty"]]:
         '''
         :Property: tags: Tags to attach to instance. Max support 20 tags to add during create instance. Each tag with two properties Key and Value, and Key is required.
         '''
         return typing.cast(typing.Optional[typing.List["RosDBCluster.TagsProperty"]], jsii.get(self, "tags"))
 
     @tags.setter
     def tags(
         self,
         value: typing.Optional[typing.List["RosDBCluster.TagsProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBCluster, "tags").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "tags", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="tdeStatus")
     def tde_status(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -2730,65 +3054,77 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "tdeStatus"))
 
     @tde_status.setter
     def tde_status(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBCluster, "tde_status").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "tdeStatus", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vpcId")
     def vpc_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: vpcId: The ID of the VPC to connect to.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "vpcId"))
 
     @vpc_id.setter
     def vpc_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBCluster, "vpc_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "vpcId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vSwitchId")
     def v_switch_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: vSwitchId: The ID of the VSwitch to connect to.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "vSwitchId"))
 
     @v_switch_id.setter
     def v_switch_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBCluster, "v_switch_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "vSwitchId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="zoneId")
     def zone_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: zoneId: The zone ID of the cluster. You can call the DescribeRegions operation to query available zones.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "zoneId"))
 
     @zone_id.setter
     def zone_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBCluster, "zone_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "zoneId", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-polardb.RosDBCluster.DBClusterParametersProperty",
         jsii_struct_bases=[],
         name_mapping={"effective_time": "effectiveTime", "parameters": "parameters"},
     )
@@ -2799,14 +3135,18 @@
             effective_time: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
             parameters: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param effective_time: 
             :param parameters: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosDBCluster.DBClusterParametersProperty.__init__)
+                check_type(argname="argument effective_time", value=effective_time, expected_type=type_hints["effective_time"])
+                check_type(argname="argument parameters", value=parameters, expected_type=type_hints["parameters"])
             self._values: typing.Dict[str, typing.Any] = {}
             if effective_time is not None:
                 self._values["effective_time"] = effective_time
             if parameters is not None:
                 self._values["parameters"] = parameters
 
         @builtins.property
@@ -2873,14 +3213,18 @@
             key: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param key: 
             :param value: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosDBCluster.TagsProperty.__init__)
+                check_type(argname="argument key", value=key, expected_type=type_hints["key"])
+                check_type(argname="argument value", value=value, expected_type=type_hints["value"])
             self._values: typing.Dict[str, typing.Any] = {
                 "key": key,
             }
             if value is not None:
                 self._values["value"] = value
 
         @builtins.property
@@ -2921,80 +3265,95 @@
 ):
     '''A ROS template type:  ``ALIYUN::POLARDB::DBClusterAccessWhiteList``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosDBClusterAccessWhiteListProps",
+        props: typing.Union["RosDBClusterAccessWhiteListProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::POLARDB::DBClusterAccessWhiteList``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosDBClusterAccessWhiteList.__init__)
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
+            type_hints = typing.get_type_hints(RosDBClusterAccessWhiteList._render_properties)
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
     @jsii.member(jsii_name="attrDbClusterId")
     def attr_db_cluster_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: DBClusterId: The ID of the ApsaraDB for POLARDB cluster whose IP address whitelist is to be modified.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDbClusterId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dbClusterId")
     def db_cluster_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: dbClusterId: The ID of the ApsaraDB for POLARDB cluster whose IP address whitelist is to be modified.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "dbClusterId"))
 
     @db_cluster_id.setter
     def db_cluster_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBClusterAccessWhiteList, "db_cluster_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dbClusterId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBClusterAccessWhiteList, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="securityIps")
     def security_ips(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         securityIps: The IP addresses to be added to the IP address whitelist group to be modified. Each
         whitelist group can contain a maximum of 1,000 IP addresses. Separate multiple IP
@@ -3007,17 +3366,20 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "securityIps"))
 
     @security_ips.setter
     def security_ips(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBClusterAccessWhiteList, "security_ips").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "securityIps", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dbClusterIpArrayName")
     def db_cluster_ip_array_name(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -3028,14 +3390,17 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "dbClusterIpArrayName"))
 
     @db_cluster_ip_array_name.setter
     def db_cluster_ip_array_name(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBClusterAccessWhiteList, "db_cluster_ip_array_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dbClusterIpArrayName", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-polardb.RosDBClusterAccessWhiteListProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -3054,14 +3419,19 @@
     ) -> None:
         '''Properties for defining a ``ALIYUN::POLARDB::DBClusterAccessWhiteList``.
 
         :param db_cluster_id: 
         :param security_ips: 
         :param db_cluster_ip_array_name: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosDBClusterAccessWhiteListProps.__init__)
+            check_type(argname="argument db_cluster_id", value=db_cluster_id, expected_type=type_hints["db_cluster_id"])
+            check_type(argname="argument security_ips", value=security_ips, expected_type=type_hints["security_ips"])
+            check_type(argname="argument db_cluster_ip_array_name", value=db_cluster_ip_array_name, expected_type=type_hints["db_cluster_ip_array_name"])
         self._values: typing.Dict[str, typing.Any] = {
             "db_cluster_id": db_cluster_id,
             "security_ips": security_ips,
         }
         if db_cluster_ip_array_name is not None:
             self._values["db_cluster_ip_array_name"] = db_cluster_ip_array_name
 
@@ -3124,96 +3494,111 @@
 ):
     '''A ROS template type:  ``ALIYUN::POLARDB::DBClusterEndpoint``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosDBClusterEndpointProps",
+        props: typing.Union["RosDBClusterEndpointProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::POLARDB::DBClusterEndpoint``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosDBClusterEndpoint.__init__)
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
+            type_hints = typing.get_type_hints(RosDBClusterEndpoint._render_properties)
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
     @jsii.member(jsii_name="attrAddresses")
     def attr_addresses(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Addresses: The address items of the db cluster endpoint.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAddresses"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrConnectionString")
     def attr_connection_string(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ConnectionString: The first connection string of the db cluster endpoint.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrConnectionString"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDbEndpointId")
     def attr_db_endpoint_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: DBEndpointId: DB cluster endpoint ID. E.g. pe-xxxxxxxx.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDbEndpointId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dbClusterId")
     def db_cluster_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: dbClusterId: The ID of the ApsaraDB for POLARDB cluster for which a custom connection point is to be created.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "dbClusterId"))
 
     @db_cluster_id.setter
     def db_cluster_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBClusterEndpoint, "db_cluster_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dbClusterId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBClusterEndpoint, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="autoAddNewNodes")
     def auto_add_new_nodes(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -3224,51 +3609,60 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "autoAddNewNodes"))
 
     @auto_add_new_nodes.setter
     def auto_add_new_nodes(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBClusterEndpoint, "auto_add_new_nodes").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "autoAddNewNodes", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="endpointConfig")
     def endpoint_config(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosDBClusterEndpoint.EndpointConfigProperty"]]:
         '''
         :Property: endpointConfig:
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosDBClusterEndpoint.EndpointConfigProperty"]], jsii.get(self, "endpointConfig"))
 
     @endpoint_config.setter
     def endpoint_config(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, "RosDBClusterEndpoint.EndpointConfigProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBClusterEndpoint, "endpoint_config").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "endpointConfig", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="endpointType")
     def endpoint_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: endpointType: The type of the cluster connection point. Set this parameter to Custom.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "endpointType"))
 
     @endpoint_type.setter
     def endpoint_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBClusterEndpoint, "endpoint_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "endpointType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="nodes")
     def nodes(
         self,
     ) -> typing.Optional[typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -3278,17 +3672,20 @@
         return typing.cast(typing.Optional[typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]], jsii.get(self, "nodes"))
 
     @nodes.setter
     def nodes(
         self,
         value: typing.Optional[typing.Union[typing.List[typing.Any], ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBClusterEndpoint, "nodes").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "nodes", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="readWriteMode")
     def read_write_mode(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -3300,14 +3697,17 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "readWriteMode"))
 
     @read_write_mode.setter
     def read_write_mode(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBClusterEndpoint, "read_write_mode").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "readWriteMode", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-polardb.RosDBClusterEndpoint.EndpointConfigProperty",
         jsii_struct_bases=[],
         name_mapping={"consist_level": "consistLevel"},
     )
@@ -3316,14 +3716,17 @@
             self,
             *,
             consist_level: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param consist_level: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosDBClusterEndpoint.EndpointConfigProperty.__init__)
+                check_type(argname="argument consist_level", value=consist_level, expected_type=type_hints["consist_level"])
             self._values: typing.Dict[str, typing.Any] = {}
             if consist_level is not None:
                 self._values["consist_level"] = consist_level
 
         @builtins.property
         def consist_level(
             self,
@@ -3359,103 +3762,121 @@
 ):
     '''A ROS template type:  ``ALIYUN::POLARDB::DBClusterEndpointAddress``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosDBClusterEndpointAddressProps",
+        props: typing.Union["RosDBClusterEndpointAddressProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::POLARDB::DBClusterEndpointAddress``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosDBClusterEndpointAddress.__init__)
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
+            type_hints = typing.get_type_hints(RosDBClusterEndpointAddress._render_properties)
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
     @jsii.member(jsii_name="attrAddress")
     def attr_address(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Address: The details of the endpoint address.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAddress"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrConnectionString")
     def attr_connection_string(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ConnectionString: The connection string of the endpoint address.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrConnectionString"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dbClusterId")
     def db_cluster_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: dbClusterId: The ID of the ApsaraDB for POLARDB cluster for which a public connection point is to be created.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "dbClusterId"))
 
     @db_cluster_id.setter
     def db_cluster_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBClusterEndpointAddress, "db_cluster_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dbClusterId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dbEndpointId")
     def db_endpoint_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: dbEndpointId: The ID of the cluster connection point.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "dbEndpointId"))
 
     @db_endpoint_id.setter
     def db_endpoint_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBClusterEndpointAddress, "db_endpoint_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dbEndpointId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBClusterEndpointAddress, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="connectionStringPrefix")
     def connection_string_prefix(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -3466,17 +3887,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "connectionStringPrefix"))
 
     @connection_string_prefix.setter
     def connection_string_prefix(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBClusterEndpointAddress, "connection_string_prefix").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "connectionStringPrefix", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="netType")
     def net_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -3488,14 +3912,17 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "netType"))
 
     @net_type.setter
     def net_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBClusterEndpointAddress, "net_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "netType", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-polardb.RosDBClusterEndpointAddressProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -3517,14 +3944,20 @@
         '''Properties for defining a ``ALIYUN::POLARDB::DBClusterEndpointAddress``.
 
         :param db_cluster_id: 
         :param db_endpoint_id: 
         :param connection_string_prefix: 
         :param net_type: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosDBClusterEndpointAddressProps.__init__)
+            check_type(argname="argument db_cluster_id", value=db_cluster_id, expected_type=type_hints["db_cluster_id"])
+            check_type(argname="argument db_endpoint_id", value=db_endpoint_id, expected_type=type_hints["db_endpoint_id"])
+            check_type(argname="argument connection_string_prefix", value=connection_string_prefix, expected_type=type_hints["connection_string_prefix"])
+            check_type(argname="argument net_type", value=net_type, expected_type=type_hints["net_type"])
         self._values: typing.Dict[str, typing.Any] = {
             "db_cluster_id": db_cluster_id,
             "db_endpoint_id": db_endpoint_id,
         }
         if connection_string_prefix is not None:
             self._values["connection_string_prefix"] = connection_string_prefix
         if net_type is not None:
@@ -3603,28 +4036,36 @@
 )
 class RosDBClusterEndpointProps:
     def __init__(
         self,
         *,
         db_cluster_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         auto_add_new_nodes: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        endpoint_config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, RosDBClusterEndpoint.EndpointConfigProperty]] = None,
+        endpoint_config: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosDBClusterEndpoint.EndpointConfigProperty, typing.Dict[str, typing.Any]]]] = None,
         endpoint_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         nodes: typing.Optional[typing.Union[typing.Sequence[typing.Any], ros_cdk_core.IResolvable]] = None,
         read_write_mode: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::POLARDB::DBClusterEndpoint``.
 
         :param db_cluster_id: 
         :param auto_add_new_nodes: 
         :param endpoint_config: 
         :param endpoint_type: 
         :param nodes: 
         :param read_write_mode: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosDBClusterEndpointProps.__init__)
+            check_type(argname="argument db_cluster_id", value=db_cluster_id, expected_type=type_hints["db_cluster_id"])
+            check_type(argname="argument auto_add_new_nodes", value=auto_add_new_nodes, expected_type=type_hints["auto_add_new_nodes"])
+            check_type(argname="argument endpoint_config", value=endpoint_config, expected_type=type_hints["endpoint_config"])
+            check_type(argname="argument endpoint_type", value=endpoint_type, expected_type=type_hints["endpoint_type"])
+            check_type(argname="argument nodes", value=nodes, expected_type=type_hints["nodes"])
+            check_type(argname="argument read_write_mode", value=read_write_mode, expected_type=type_hints["read_write_mode"])
         self._values: typing.Dict[str, typing.Any] = {
             "db_cluster_id": db_cluster_id,
         }
         if auto_add_new_nodes is not None:
             self._values["auto_add_new_nodes"] = auto_add_new_nodes
         if endpoint_config is not None:
             self._values["endpoint_config"] = endpoint_config
@@ -3735,14 +4176,15 @@
         "db_cluster_description": "dbClusterDescription",
         "db_cluster_parameters": "dbClusterParameters",
         "default_time_zone": "defaultTimeZone",
         "gdn_id": "gdnId",
         "lower_case_table_names": "lowerCaseTableNames",
         "maintain_time": "maintainTime",
         "period": "period",
+        "period_unit": "periodUnit",
         "renewal_status": "renewalStatus",
         "resource_group_id": "resourceGroupId",
         "security_group_ids": "securityGroupIds",
         "security_ip_list": "securityIpList",
         "source_resource_id": "sourceResourceId",
         "tags": "tags",
         "tde_status": "tdeStatus",
@@ -3762,26 +4204,27 @@
         auto_renew_period: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         backup_retention_policy_on_cluster_deletion: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         clone_data_point: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         cluster_network_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         creation_category: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         creation_option: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         db_cluster_description: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        db_cluster_parameters: typing.Optional[typing.Union[ros_cdk_core.IResolvable, RosDBCluster.DBClusterParametersProperty]] = None,
+        db_cluster_parameters: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosDBCluster.DBClusterParametersProperty, typing.Dict[str, typing.Any]]]] = None,
         default_time_zone: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         gdn_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         lower_case_table_names: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
         maintain_time: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         period: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]] = None,
+        period_unit: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         renewal_status: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         resource_group_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         security_group_ids: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]] = None,
         security_ip_list: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         source_resource_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        tags: typing.Optional[typing.Sequence[RosDBCluster.TagsProperty]] = None,
+        tags: typing.Optional[typing.Sequence[typing.Union[RosDBCluster.TagsProperty, typing.Dict[str, typing.Any]]]] = None,
         tde_status: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         vpc_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         v_switch_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         zone_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::POLARDB::DBCluster``.
 
@@ -3798,25 +4241,56 @@
         :param db_cluster_description: 
         :param db_cluster_parameters: 
         :param default_time_zone: 
         :param gdn_id: 
         :param lower_case_table_names: 
         :param maintain_time: 
         :param period: 
+        :param period_unit: 
         :param renewal_status: 
         :param resource_group_id: 
         :param security_group_ids: 
         :param security_ip_list: 
         :param source_resource_id: 
         :param tags: 
         :param tde_status: 
         :param vpc_id: 
         :param v_switch_id: 
         :param zone_id: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosDBClusterProps.__init__)
+            check_type(argname="argument db_node_class", value=db_node_class, expected_type=type_hints["db_node_class"])
+            check_type(argname="argument db_type", value=db_type, expected_type=type_hints["db_type"])
+            check_type(argname="argument db_version", value=db_version, expected_type=type_hints["db_version"])
+            check_type(argname="argument pay_type", value=pay_type, expected_type=type_hints["pay_type"])
+            check_type(argname="argument auto_renew_period", value=auto_renew_period, expected_type=type_hints["auto_renew_period"])
+            check_type(argname="argument backup_retention_policy_on_cluster_deletion", value=backup_retention_policy_on_cluster_deletion, expected_type=type_hints["backup_retention_policy_on_cluster_deletion"])
+            check_type(argname="argument clone_data_point", value=clone_data_point, expected_type=type_hints["clone_data_point"])
+            check_type(argname="argument cluster_network_type", value=cluster_network_type, expected_type=type_hints["cluster_network_type"])
+            check_type(argname="argument creation_category", value=creation_category, expected_type=type_hints["creation_category"])
+            check_type(argname="argument creation_option", value=creation_option, expected_type=type_hints["creation_option"])
+            check_type(argname="argument db_cluster_description", value=db_cluster_description, expected_type=type_hints["db_cluster_description"])
+            check_type(argname="argument db_cluster_parameters", value=db_cluster_parameters, expected_type=type_hints["db_cluster_parameters"])
+            check_type(argname="argument default_time_zone", value=default_time_zone, expected_type=type_hints["default_time_zone"])
+            check_type(argname="argument gdn_id", value=gdn_id, expected_type=type_hints["gdn_id"])
+            check_type(argname="argument lower_case_table_names", value=lower_case_table_names, expected_type=type_hints["lower_case_table_names"])
+            check_type(argname="argument maintain_time", value=maintain_time, expected_type=type_hints["maintain_time"])
+            check_type(argname="argument period", value=period, expected_type=type_hints["period"])
+            check_type(argname="argument period_unit", value=period_unit, expected_type=type_hints["period_unit"])
+            check_type(argname="argument renewal_status", value=renewal_status, expected_type=type_hints["renewal_status"])
+            check_type(argname="argument resource_group_id", value=resource_group_id, expected_type=type_hints["resource_group_id"])
+            check_type(argname="argument security_group_ids", value=security_group_ids, expected_type=type_hints["security_group_ids"])
+            check_type(argname="argument security_ip_list", value=security_ip_list, expected_type=type_hints["security_ip_list"])
+            check_type(argname="argument source_resource_id", value=source_resource_id, expected_type=type_hints["source_resource_id"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
+            check_type(argname="argument tde_status", value=tde_status, expected_type=type_hints["tde_status"])
+            check_type(argname="argument vpc_id", value=vpc_id, expected_type=type_hints["vpc_id"])
+            check_type(argname="argument v_switch_id", value=v_switch_id, expected_type=type_hints["v_switch_id"])
+            check_type(argname="argument zone_id", value=zone_id, expected_type=type_hints["zone_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "db_node_class": db_node_class,
             "db_type": db_type,
             "db_version": db_version,
             "pay_type": pay_type,
         }
         if auto_renew_period is not None:
@@ -3841,14 +4315,16 @@
             self._values["gdn_id"] = gdn_id
         if lower_case_table_names is not None:
             self._values["lower_case_table_names"] = lower_case_table_names
         if maintain_time is not None:
             self._values["maintain_time"] = maintain_time
         if period is not None:
             self._values["period"] = period
+        if period_unit is not None:
+            self._values["period_unit"] = period_unit
         if renewal_status is not None:
             self._values["renewal_status"] = renewal_status
         if resource_group_id is not None:
             self._values["resource_group_id"] = resource_group_id
         if security_group_ids is not None:
             self._values["security_group_ids"] = security_group_ids
         if security_ip_list is not None:
@@ -4089,20 +4565,38 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], result)
 
     @builtins.property
     def period(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
-        :Property: period: The subscription period of the cluster in month. Valid values: 1, 2, 3, 4, 5, 6, 7, 8, 9, 12, 24, 36.
+        :Property:
+
+        period: The subscription period of the clusterIf PeriodUnit is month, the valid range is 1, 2, 3, 4, 5, 6, 7, 8, 9, 12, 24, 36
+        If periodUnit is year, the valid range is 1, 2, 3
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
     def renewal_status(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
         renewalStatus: The auto renewal status of the cluster Valid values:
@@ -4237,80 +4731,95 @@
 ):
     '''A ROS template type:  ``ALIYUN::POLARDB::DBInstance``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosDBInstanceProps",
+        props: typing.Union["RosDBInstanceProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::POLARDB::DBInstance``.
 
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
         :Property: characterSetName: The character set of the database. For more information, see Character sets.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "characterSetName"))
 
     @character_set_name.setter
     def character_set_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstance, "character_set_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "characterSetName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dbClusterId")
     def db_cluster_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: dbClusterId: The ID of the ApsaraDB for POLARDB cluster for which a database is to be created.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "dbClusterId"))
 
     @db_cluster_id.setter
     def db_cluster_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstance, "db_cluster_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dbClusterId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dbName")
     def db_name(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         dbName: The name of the database to be created. The name must comply with the following rules:
         It must start with a lowercase letter and consist of lowercase letters, digits, hyphens
@@ -4320,44 +4829,53 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "dbName"))
 
     @db_name.setter
     def db_name(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstance, "db_name").fset)
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
+            type_hints = typing.get_type_hints(getattr(RosDBInstance, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="accountName")
     def account_name(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: accountName: The name of the database account to be used.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "accountName"))
 
     @account_name.setter
     def account_name(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstance, "account_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "accountName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="accountPrivilege")
     def account_privilege(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -4371,17 +4889,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "accountPrivilege"))
 
     @account_privilege.setter
     def account_privilege(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstance, "account_privilege").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "accountPrivilege", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dbDescription")
     def db_description(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -4392,14 +4913,17 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "dbDescription"))
 
     @db_description.setter
     def db_description(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBInstance, "db_description").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dbDescription", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-polardb.RosDBInstanceProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -4427,14 +4951,22 @@
         :param character_set_name: 
         :param db_cluster_id: 
         :param db_name: 
         :param account_name: 
         :param account_privilege: 
         :param db_description: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosDBInstanceProps.__init__)
+            check_type(argname="argument character_set_name", value=character_set_name, expected_type=type_hints["character_set_name"])
+            check_type(argname="argument db_cluster_id", value=db_cluster_id, expected_type=type_hints["db_cluster_id"])
+            check_type(argname="argument db_name", value=db_name, expected_type=type_hints["db_name"])
+            check_type(argname="argument account_name", value=account_name, expected_type=type_hints["account_name"])
+            check_type(argname="argument account_privilege", value=account_privilege, expected_type=type_hints["account_privilege"])
+            check_type(argname="argument db_description", value=db_description, expected_type=type_hints["db_description"])
         self._values: typing.Dict[str, typing.Any] = {
             "character_set_name": character_set_name,
             "db_cluster_id": db_cluster_id,
             "db_name": db_name,
         }
         if account_name is not None:
             self._values["account_name"] = account_name
@@ -4537,117 +5069,138 @@
 ):
     '''A ROS template type:  ``ALIYUN::POLARDB::DBNodes``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosDBNodesProps",
+        props: typing.Union["RosDBNodesProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::POLARDB::DBNodes``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosDBNodes.__init__)
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
+            type_hints = typing.get_type_hints(RosDBNodes._render_properties)
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
     @jsii.member(jsii_name="attrDbNodeIds")
     def attr_db_node_ids(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: DBNodeIds: The ID list of added cluster nodes.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDbNodeIds"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrOrderIds")
     def attr_order_ids(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: OrderIds: The order ID list of added cluster nodes.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrOrderIds"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="amount")
     def amount(self) -> typing.Union[jsii.Number, ros_cdk_core.IResolvable]:
         '''
         :Property: amount: Number of nodes to be added to cluster.
         '''
         return typing.cast(typing.Union[jsii.Number, ros_cdk_core.IResolvable], jsii.get(self, "amount"))
 
     @amount.setter
     def amount(
         self,
         value: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBNodes, "amount").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "amount", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dbClusterId")
     def db_cluster_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: dbClusterId: The ID of the ApsaraDB for POLARDB cluster to be added nodes to.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "dbClusterId"))
 
     @db_cluster_id.setter
     def db_cluster_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBNodes, "db_cluster_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dbClusterId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBNodes, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="imciSwitch")
     def imci_switch(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: imciSwitch: Specifies whether to enable the In-Memory Column Index (IMCI) feature.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "imciSwitch"))
 
     @imci_switch.setter
     def imci_switch(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDBNodes, "imci_switch").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "imciSwitch", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-polardb.RosDBNodesProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -4666,14 +5219,19 @@
     ) -> None:
         '''Properties for defining a ``ALIYUN::POLARDB::DBNodes``.
 
         :param amount: 
         :param db_cluster_id: 
         :param imci_switch: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosDBNodesProps.__init__)
+            check_type(argname="argument amount", value=amount, expected_type=type_hints["amount"])
+            check_type(argname="argument db_cluster_id", value=db_cluster_id, expected_type=type_hints["db_cluster_id"])
+            check_type(argname="argument imci_switch", value=imci_switch, expected_type=type_hints["imci_switch"])
         self._values: typing.Dict[str, typing.Any] = {
             "amount": amount,
             "db_cluster_id": db_cluster_id,
         }
         if imci_switch is not None:
             self._values["imci_switch"] = imci_switch
```

### Comparing `ros-cdk-polardb-1.0.8/src/ros_cdk_polardb.egg-info/PKG-INFO` & `ros-cdk-polardb-1.0.9/src/ros_cdk_polardb.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-polardb
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS POLARDB Construct Library
```

