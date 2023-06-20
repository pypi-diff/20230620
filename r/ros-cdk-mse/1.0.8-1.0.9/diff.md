# Comparing `tmp/ros-cdk-mse-1.0.8.tar.gz` & `tmp/ros-cdk-mse-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-mse-1.0.8.tar", last modified: Thu Jul 14 02:35:59 2022, max compression
+gzip compressed data, was "dist/ros-cdk-mse-1.0.9.tar", last modified: Fri Sep 23 11:52:09 2022, max compression
```

## Comparing `ros-cdk-mse-1.0.8.tar` & `ros-cdk-mse-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:35:59.000000 ros-cdk-mse-1.0.8/
--rw-r--r--   0 root         (0) root         (0)    10279 2022-07-14 02:35:59.000000 ros-cdk-mse-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2022-07-14 02:35:59.000000 ros-cdk-mse-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2022-07-14 02:35:59.000000 ros-cdk-mse-1.0.8/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1240 2022-07-14 02:35:59.000000 ros-cdk-mse-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      179 2022-07-14 02:35:59.000000 ros-cdk-mse-1.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)      106 2022-07-14 02:35:59.000000 ros-cdk-mse-1.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-07-14 02:35:59.000000 ros-cdk-mse-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1794 2022-07-14 02:35:59.000000 ros-cdk-mse-1.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:35:59.000000 ros-cdk-mse-1.0.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:35:59.000000 ros-cdk-mse-1.0.8/src/ros_cdk_mse/
--rw-r--r--   0 root         (0) root         (0)    82043 2022-07-14 02:35:59.000000 ros-cdk-mse-1.0.8/src/ros_cdk_mse/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:35:59.000000 ros-cdk-mse-1.0.8/src/ros_cdk_mse/_jsii/
--rw-r--r--   0 root         (0) root         (0)      370 2022-07-14 02:35:59.000000 ros-cdk-mse-1.0.8/src/ros_cdk_mse/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    49350 2022-07-14 02:35:59.000000 ros-cdk-mse-1.0.8/src/ros_cdk_mse/_jsii/ros-cdk-mse@1.0.8.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:35:59.000000 ros-cdk-mse-1.0.8/src/ros_cdk_mse/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:35:59.000000 ros-cdk-mse-1.0.8/src/ros_cdk_mse.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1240 2022-07-14 02:35:59.000000 ros-cdk-mse-1.0.8/src/ros_cdk_mse.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      400 2022-07-14 02:35:59.000000 ros-cdk-mse-1.0.8/src/ros_cdk_mse.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:35:59.000000 ros-cdk-mse-1.0.8/src/ros_cdk_mse.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2022-07-14 02:35:59.000000 ros-cdk-mse-1.0.8/src/ros_cdk_mse.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2022-07-14 02:35:59.000000 ros-cdk-mse-1.0.8/src/ros_cdk_mse.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:52:09.000000 ros-cdk-mse-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)    10279 2022-09-23 11:52:09.000000 ros-cdk-mse-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-09-23 11:52:09.000000 ros-cdk-mse-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2022-09-23 11:52:09.000000 ros-cdk-mse-1.0.9/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1240 2022-09-23 11:52:09.000000 ros-cdk-mse-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      179 2022-09-23 11:52:09.000000 ros-cdk-mse-1.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      236 2022-09-23 11:52:09.000000 ros-cdk-mse-1.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-09-23 11:52:09.000000 ros-cdk-mse-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1823 2022-09-23 11:52:09.000000 ros-cdk-mse-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:52:09.000000 ros-cdk-mse-1.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:52:09.000000 ros-cdk-mse-1.0.9/src/ros_cdk_mse/
+-rw-r--r--   0 root         (0) root         (0)    99972 2022-09-23 11:52:09.000000 ros-cdk-mse-1.0.9/src/ros_cdk_mse/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:52:09.000000 ros-cdk-mse-1.0.9/src/ros_cdk_mse/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      404 2022-09-23 11:52:09.000000 ros-cdk-mse-1.0.9/src/ros_cdk_mse/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    50698 2022-09-23 11:52:09.000000 ros-cdk-mse-1.0.9/src/ros_cdk_mse/_jsii/ros-cdk-mse@1.0.9.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 11:52:09.000000 ros-cdk-mse-1.0.9/src/ros_cdk_mse/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 11:52:09.000000 ros-cdk-mse-1.0.9/src/ros_cdk_mse.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1240 2022-09-23 11:52:09.000000 ros-cdk-mse-1.0.9/src/ros_cdk_mse.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      400 2022-09-23 11:52:09.000000 ros-cdk-mse-1.0.9/src/ros_cdk_mse.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 11:52:09.000000 ros-cdk-mse-1.0.9/src/ros_cdk_mse.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2022-09-23 11:52:09.000000 ros-cdk-mse-1.0.9/src/ros_cdk_mse.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2022-09-23 11:52:09.000000 ros-cdk-mse-1.0.9/src/ros_cdk_mse.egg-info/top_level.txt
```

### Comparing `ros-cdk-mse-1.0.8/LICENSE` & `ros-cdk-mse-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-mse-1.0.8/PKG-INFO` & `ros-cdk-mse-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-mse
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS MSE Construct Library
```

### Comparing `ros-cdk-mse-1.0.8/setup.py` & `ros-cdk-mse-1.0.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-mse",
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
         "ros_cdk_mse",
         "ros_cdk_mse._jsii"
     ],
     "package_data": {
         "ros_cdk_mse._jsii": [
-            "ros-cdk-mse@1.0.8.jsii.tgz"
+            "ros-cdk-mse@1.0.9.jsii.tgz"
         ],
         "ros_cdk_mse": [
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

### Comparing `ros-cdk-mse-1.0.8/src/ros_cdk_mse/__init__.py` & `ros-cdk-mse-1.0.9/src/ros_cdk_mse/__init__.py`

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
 
 
 class Cluster(
     ros_cdk_core.Resource,
@@ -29,203 +31,248 @@
 ):
     '''A ROS resource type:  ``ALIYUN::MSE::Cluster``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "ClusterProps",
+        props: typing.Union["ClusterProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::MSE::Cluster``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(Cluster.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrAclEntryList")
     def attr_acl_entry_list(self) -> ros_cdk_core.IResolvable:
-        '''Attribute AclEntryList: acl entry list.'''
+        '''Attribute AclEntryList: The public network whitelist list is used only when the public network is enabled.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAclEntryList"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrAclId")
     def attr_acl_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute AclId: acl id.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAclId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrAppVersion")
     def attr_app_version(self) -> ros_cdk_core.IResolvable:
         '''Attribute AppVersion: app version.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAppVersion"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrClusterAliasName")
     def attr_cluster_alias_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute ClusterAliasName: cluster alias name.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrClusterAliasName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrClusterId")
     def attr_cluster_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute ClusterId: cluster id.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrClusterId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrClusterName")
     def attr_cluster_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute ClusterName: cluster name.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrClusterName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrClusterSpecification")
     def attr_cluster_specification(self) -> ros_cdk_core.IResolvable:
-        '''Attribute ClusterSpecification: cluster specification, Enum: MSE_SC_1_2_200_c,MSE_SC_2_4_200_c,MSE_SC_4_8_200_c,MSE_SC_8_16_200_c.'''
+        '''Attribute ClusterSpecification: Cluster specifications.
+
+        Note the msversion requirements of the version parameter,
+        Optional parameters:
+        "MSE_ SC *1_2_60_c",
+        "MSE* SC *2_4_60_c",
+        "MSE* SC *4_8_60_c",
+        "MSE* SC *8_16_60_c",
+        "MSE* SC _16_32_60_c"
+        '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrClusterSpecification"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrClusterType")
     def attr_cluster_type(self) -> ros_cdk_core.IResolvable:
         '''Attribute ClusterType: cluster type.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrClusterType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrClusterVersion")
     def attr_cluster_version(self) -> ros_cdk_core.IResolvable:
-        '''Attribute ClusterVersion: cluster version, Enum: ZooKeeper_3_4_14,ZooKeeper_3_5_5,NACOS_ANS_1_2_1,NACOS_2_0_0.'''
+        '''Attribute ClusterVersion: Cluster version, such as ZooKeeper_3_8_0,NACOS_2_0_0.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrClusterVersion"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
+    @jsii.member(jsii_name="attrConfigAuthEnabled")
+    def attr_config_auth_enabled(self) -> ros_cdk_core.IResolvable:
+        '''Attribute ConfigAuthEnabled: Whether the configuration supports it.
+
+        Valid values: true: false: not supported
+        '''
+        return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrConfigAuthEnabled"))
+
+    @builtins.property
+    @jsii.member(jsii_name="attrConfigSecretEnabled")
+    def attr_config_secret_enabled(self) -> ros_cdk_core.IResolvable:
+        '''Attribute ConfigSecretEnabled: Whether the configuration password takes effect.
+
+        The value is as follows: true: valid false: not valid
+        '''
+        return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrConfigSecretEnabled"))
+
+    @builtins.property
     @jsii.member(jsii_name="attrConnectionType")
     def attr_connection_type(self) -> ros_cdk_core.IResolvable:
         '''Attribute ConnectionType: network connect type.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrConnectionType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrCpu")
     def attr_cpu(self) -> ros_cdk_core.IResolvable:
         '''Attribute Cpu: cpu core size.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrCpu"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDiskCapacity")
     def attr_disk_capacity(self) -> ros_cdk_core.IResolvable:
         '''Attribute DiskCapacity: disk capacity, unit: G.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDiskCapacity"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDiskType")
     def attr_disk_type(self) -> ros_cdk_core.IResolvable:
         '''Attribute DiskType: disk type.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDiskType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrHealthStatus")
     def attr_health_status(self) -> ros_cdk_core.IResolvable:
         '''Attribute HealthStatus: health status.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrHealthStatus"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInstanceCount")
     def attr_instance_count(self) -> ros_cdk_core.IResolvable:
         '''Attribute InstanceCount: instance count.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInstanceCount"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInstanceId")
     def attr_instance_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute InstanceId: instance id.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInstanceId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInternetAddress")
     def attr_internet_address(self) -> ros_cdk_core.IResolvable:
         '''Attribute InternetAddress: internet address.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInternetAddress"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInternetDomain")
     def attr_internet_domain(self) -> ros_cdk_core.IResolvable:
         '''Attribute InternetDomain: internet domain.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInternetDomain"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInternetPort")
     def attr_internet_port(self) -> ros_cdk_core.IResolvable:
         '''Attribute InternetPort: internet port.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInternetPort"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrIntranetAddress")
     def attr_intranet_address(self) -> ros_cdk_core.IResolvable:
         '''Attribute IntranetAddress: intranet address.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrIntranetAddress"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrIntranetDomain")
     def attr_intranet_domain(self) -> ros_cdk_core.IResolvable:
         '''Attribute IntranetDomain: intranet domain.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrIntranetDomain"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrIntranetPort")
     def attr_intranet_port(self) -> ros_cdk_core.IResolvable:
         '''Attribute IntranetPort: intranet port.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrIntranetPort"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
+    @jsii.member(jsii_name="attrMcpEnabled")
+    def attr_mcp_enabled(self) -> ros_cdk_core.IResolvable:
+        '''Attribute MCPEnabled: Whether MCP takes effect, the value is as follows: true: valid false: not valid.'''
+        return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrMcpEnabled"))
+
+    @builtins.property
     @jsii.member(jsii_name="attrMemoryCapacity")
     def attr_memory_capacity(self) -> ros_cdk_core.IResolvable:
         '''Attribute MemoryCapacity: memory capacity.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrMemoryCapacity"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrMseVersion")
     def attr_mse_version(self) -> ros_cdk_core.IResolvable:
-        '''Attribute MseVersion: This parameter is required when creating a professional version. The value is as follows:.
+        '''Attribute MseVersion: Required, the value is as follows:.
 
-        -'mse_basic': indicates the basic version (default value).
-        -'mse_pro': means professional version.
+        -'mse_dev': indicates the development version.
+        -'Mse_pro': means professional version. When this version is selected, the specification is 2c4g or above, and the specification is 3 nodes or above.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrMseVersion"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrNetType")
     def attr_net_type(self) -> ros_cdk_core.IResolvable:
-        '''Attribute NetType: network type, Enum: privatenet,pubnet.'''
+        '''Attribute NetType: Network type (whether private network is enabled or not).
+
+        privatenet indicates that private network is enabled.
+        '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrNetType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPayInfo")
     def attr_pay_info(self) -> ros_cdk_core.IResolvable:
         '''Attribute PayInfo: pay info.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPayInfo"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPubNetworkFlow")
     def attr_pub_network_flow(self) -> ros_cdk_core.IResolvable:
-        '''Attribute PubNetworkFlow: pub network flow.'''
+        '''Attribute PubNetworkFlow: Public network bandwidth.
+
+        If the bandwidth is greater than 0, the public network is enabled.
+        '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPubNetworkFlow"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVpcId")
     def attr_vpc_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute VpcId: vpc id.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVpcId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVSwitchId")
     def attr_v_switch_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute VSwitchId: switcher Id.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVSwitchId"))
 
 
 @jsii.data_type(
@@ -271,32 +318,51 @@
         pub_slb_specification: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         request_pars: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         vpc_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         v_switch_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::MSE::Cluster``.
 
-        :param cluster_specification: Property clusterSpecification: cluster specification, Enum: MSE_SC_1_2_200_c,MSE_SC_2_4_200_c,MSE_SC_4_8_200_c,MSE_SC_8_16_200_c.
+        :param cluster_specification: Property clusterSpecification: Cluster specifications. Note the msversion requirements of the version parameter, Optional parameters: "MSE_ SC *1_2_60_c", "MSE* SC *2_4_60_c", "MSE* SC *4_8_60_c", "MSE* SC *8_16_60_c", "MSE* SC _16_32_60_c"
         :param cluster_type: Property clusterType: cluster type.
-        :param cluster_version: Property clusterVersion: cluster version, Enum: ZooKeeper_3_4_14,ZooKeeper_3_5_5,NACOS_ANS_1_2_1,NACOS_2_0_0.
+        :param cluster_version: Property clusterVersion: Cluster version, such as ZooKeeper_3_8_0,NACOS_2_0_0.
         :param instance_count: Property instanceCount: instance count.
-        :param net_type: Property netType: network type, Enum: privatenet,pubnet.
+        :param net_type: Property netType: Network type (whether private network is enabled or not). privatenet indicates that private network is enabled.
         :param accept_language: Property acceptLanguage:.
-        :param acl_entry_list: Property aclEntryList: acl entry list.
+        :param acl_entry_list: Property aclEntryList: The public network whitelist list is used only when the public network is enabled.
         :param cluster_alias_name: Property clusterAliasName: cluster alias name.
         :param connection_type: Property connectionType: network connect type.
         :param disk_type: Property diskType: disk type.
-        :param mse_version: Property mseVersion: This parameter is required when creating a professional version. The value is as follows:. -'mse_basic': indicates the basic version (default value). -'mse_pro': means professional version.
+        :param mse_version: Property mseVersion: Required, the value is as follows:. -'mse_dev': indicates the development version. -'Mse_pro': means professional version. When this version is selected, the specification is 2c4g or above, and the specification is 3 nodes or above.
         :param private_slb_specification: Property privateSlbSpecification:.
-        :param pub_network_flow: Property pubNetworkFlow: pub network flow.
+        :param pub_network_flow: Property pubNetworkFlow: Public network bandwidth. If the bandwidth is greater than 0, the public network is enabled.
         :param pub_slb_specification: Property pubSlbSpecification:.
         :param request_pars: Property requestPars:.
         :param vpc_id: Property vpcId: vpc id.
         :param v_switch_id: Property vSwitchId: switcher Id.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(ClusterProps.__init__)
+            check_type(argname="argument cluster_specification", value=cluster_specification, expected_type=type_hints["cluster_specification"])
+            check_type(argname="argument cluster_type", value=cluster_type, expected_type=type_hints["cluster_type"])
+            check_type(argname="argument cluster_version", value=cluster_version, expected_type=type_hints["cluster_version"])
+            check_type(argname="argument instance_count", value=instance_count, expected_type=type_hints["instance_count"])
+            check_type(argname="argument net_type", value=net_type, expected_type=type_hints["net_type"])
+            check_type(argname="argument accept_language", value=accept_language, expected_type=type_hints["accept_language"])
+            check_type(argname="argument acl_entry_list", value=acl_entry_list, expected_type=type_hints["acl_entry_list"])
+            check_type(argname="argument cluster_alias_name", value=cluster_alias_name, expected_type=type_hints["cluster_alias_name"])
+            check_type(argname="argument connection_type", value=connection_type, expected_type=type_hints["connection_type"])
+            check_type(argname="argument disk_type", value=disk_type, expected_type=type_hints["disk_type"])
+            check_type(argname="argument mse_version", value=mse_version, expected_type=type_hints["mse_version"])
+            check_type(argname="argument private_slb_specification", value=private_slb_specification, expected_type=type_hints["private_slb_specification"])
+            check_type(argname="argument pub_network_flow", value=pub_network_flow, expected_type=type_hints["pub_network_flow"])
+            check_type(argname="argument pub_slb_specification", value=pub_slb_specification, expected_type=type_hints["pub_slb_specification"])
+            check_type(argname="argument request_pars", value=request_pars, expected_type=type_hints["request_pars"])
+            check_type(argname="argument vpc_id", value=vpc_id, expected_type=type_hints["vpc_id"])
+            check_type(argname="argument v_switch_id", value=v_switch_id, expected_type=type_hints["v_switch_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "cluster_specification": cluster_specification,
             "cluster_type": cluster_type,
             "cluster_version": cluster_version,
             "instance_count": instance_count,
             "net_type": net_type,
         }
@@ -325,43 +391,55 @@
         if v_switch_id is not None:
             self._values["v_switch_id"] = v_switch_id
 
     @builtins.property
     def cluster_specification(
         self,
     ) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
-        '''Property clusterSpecification: cluster specification, Enum: MSE_SC_1_2_200_c,MSE_SC_2_4_200_c,MSE_SC_4_8_200_c,MSE_SC_8_16_200_c.'''
+        '''Property clusterSpecification: Cluster specifications.
+
+        Note the msversion requirements of the version parameter,
+        Optional parameters:
+        "MSE_ SC *1_2_60_c",
+        "MSE* SC *2_4_60_c",
+        "MSE* SC *4_8_60_c",
+        "MSE* SC *8_16_60_c",
+        "MSE* SC _16_32_60_c"
+        '''
         result = self._values.get("cluster_specification")
         assert result is not None, "Required property 'cluster_specification' is missing"
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], result)
 
     @builtins.property
     def cluster_type(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''Property clusterType: cluster type.'''
         result = self._values.get("cluster_type")
         assert result is not None, "Required property 'cluster_type' is missing"
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], result)
 
     @builtins.property
     def cluster_version(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
-        '''Property clusterVersion: cluster version, Enum: ZooKeeper_3_4_14,ZooKeeper_3_5_5,NACOS_ANS_1_2_1,NACOS_2_0_0.'''
+        '''Property clusterVersion: Cluster version, such as ZooKeeper_3_8_0,NACOS_2_0_0.'''
         result = self._values.get("cluster_version")
         assert result is not None, "Required property 'cluster_version' is missing"
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], result)
 
     @builtins.property
     def instance_count(self) -> typing.Union[jsii.Number, ros_cdk_core.IResolvable]:
         '''Property instanceCount: instance count.'''
         result = self._values.get("instance_count")
         assert result is not None, "Required property 'instance_count' is missing"
         return typing.cast(typing.Union[jsii.Number, ros_cdk_core.IResolvable], result)
 
     @builtins.property
     def net_type(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
-        '''Property netType: network type, Enum: privatenet,pubnet.'''
+        '''Property netType: Network type (whether private network is enabled or not).
+
+        privatenet indicates that private network is enabled.
+        '''
         result = self._values.get("net_type")
         assert result is not None, "Required property 'net_type' is missing"
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], result)
 
     @builtins.property
     def accept_language(
         self,
@@ -370,15 +448,15 @@
         result = self._values.get("accept_language")
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], result)
 
     @builtins.property
     def acl_entry_list(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]]:
-        '''Property aclEntryList: acl entry list.'''
+        '''Property aclEntryList: The public network whitelist list is used only when the public network is enabled.'''
         result = self._values.get("acl_entry_list")
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]], result)
 
     @builtins.property
     def cluster_alias_name(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
@@ -402,18 +480,18 @@
         result = self._values.get("disk_type")
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], result)
 
     @builtins.property
     def mse_version(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
-        '''Property mseVersion: This parameter is required when creating a professional version. The value is as follows:.
+        '''Property mseVersion: Required, the value is as follows:.
 
-        -'mse_basic': indicates the basic version (default value).
-        -'mse_pro': means professional version.
+        -'mse_dev': indicates the development version.
+        -'Mse_pro': means professional version. When this version is selected, the specification is 2c4g or above, and the specification is 3 nodes or above.
         '''
         result = self._values.get("mse_version")
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], result)
 
     @builtins.property
     def private_slb_specification(
         self,
@@ -422,15 +500,18 @@
         result = self._values.get("private_slb_specification")
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], result)
 
     @builtins.property
     def pub_network_flow(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
-        '''Property pubNetworkFlow: pub network flow.'''
+        '''Property pubNetworkFlow: Public network bandwidth.
+
+        If the bandwidth is greater than 0, the public network is enabled.
+        '''
         result = self._values.get("pub_network_flow")
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], result)
 
     @builtins.property
     def pub_slb_specification(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
@@ -481,67 +562,73 @@
 ):
     '''A ROS resource type:  ``ALIYUN::MSE::Gateway``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "GatewayProps",
+        props: typing.Union["GatewayProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::MSE::Gateway``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(Gateway.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrBackupVSwitchId")
     def attr_backup_v_switch_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute BackupVSwitchId: VSwitchId For Backup.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrBackupVSwitchId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrGatewayUniqueId")
     def attr_gateway_unique_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute GatewayUniqueId: Gateway unique identification.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrGatewayUniqueId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPaymentType")
     def attr_payment_type(self) -> ros_cdk_core.IResolvable:
         '''Attribute PaymentType: The payment type of the resource.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPaymentType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrReplica")
     def attr_replica(self) -> ros_cdk_core.IResolvable:
         '''Attribute Replica: Gateway Node Number.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrReplica"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrSpec")
     def attr_spec(self) -> ros_cdk_core.IResolvable:
         '''Attribute Spec: Gateway Node Specifications.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrSpec"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVpcId")
     def attr_vpc_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute VpcId: VpcId.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVpcId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVSwitchId")
     def attr_v_switch_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute VSwitchId: VSwitchId.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVSwitchId"))
 
 
 @jsii.data_type(
@@ -581,14 +668,25 @@
         :param v_switch_id: Property vSwitchId: VSwitchId.
         :param backup_v_switch_id: Property backupVSwitchId: VSwitchId For Backup.
         :param enterprise_security_group: Property enterpriseSecurityGroup:.
         :param internet_slb_spec: Property internetSlbSpec:.
         :param name: Property name:.
         :param slb_spec: Property slbSpec:.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(GatewayProps.__init__)
+            check_type(argname="argument replica", value=replica, expected_type=type_hints["replica"])
+            check_type(argname="argument spec", value=spec, expected_type=type_hints["spec"])
+            check_type(argname="argument vpc_id", value=vpc_id, expected_type=type_hints["vpc_id"])
+            check_type(argname="argument v_switch_id", value=v_switch_id, expected_type=type_hints["v_switch_id"])
+            check_type(argname="argument backup_v_switch_id", value=backup_v_switch_id, expected_type=type_hints["backup_v_switch_id"])
+            check_type(argname="argument enterprise_security_group", value=enterprise_security_group, expected_type=type_hints["enterprise_security_group"])
+            check_type(argname="argument internet_slb_spec", value=internet_slb_spec, expected_type=type_hints["internet_slb_spec"])
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+            check_type(argname="argument slb_spec", value=slb_spec, expected_type=type_hints["slb_spec"])
         self._values: typing.Dict[str, typing.Any] = {
             "replica": replica,
             "spec": spec,
             "vpc_id": vpc_id,
             "v_switch_id": v_switch_id,
         }
         if backup_v_switch_id is not None:
@@ -689,576 +787,679 @@
 ):
     '''A ROS template type:  ``ALIYUN::MSE::Cluster``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosClusterProps",
+        props: typing.Union["RosClusterProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::MSE::Cluster``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosCluster.__init__)
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
+            type_hints = typing.get_type_hints(RosCluster._render_properties)
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
     @jsii.member(jsii_name="attrAclEntryList")
     def attr_acl_entry_list(self) -> ros_cdk_core.IResolvable:
         '''
-        :Attribute: AclEntryList: acl entry list
+        :Attribute: AclEntryList: The public network whitelist list is used only when the public network is enabled.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAclEntryList"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrAclId")
     def attr_acl_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: AclId: acl id
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAclId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrAppVersion")
     def attr_app_version(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: AppVersion: app version
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAppVersion"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrClusterAliasName")
     def attr_cluster_alias_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ClusterAliasName: cluster alias name
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrClusterAliasName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrClusterId")
     def attr_cluster_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ClusterId: cluster id
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrClusterId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrClusterName")
     def attr_cluster_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ClusterName: cluster name
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrClusterName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrClusterSpecification")
     def attr_cluster_specification(self) -> ros_cdk_core.IResolvable:
         '''
-        :Attribute: ClusterSpecification: cluster specification, Enum: MSE_SC_1_2_200_c,MSE_SC_2_4_200_c,MSE_SC_4_8_200_c,MSE_SC_8_16_200_c
+        :Attribute:
+
+        ClusterSpecification: Cluster specifications. Note the msversion requirements of the version parameter,
+        Optional parameters:
+        "MSE_ SC *1_2_60_c",
+        "MSE* SC *2_4_60_c",
+        "MSE* SC *4_8_60_c",
+        "MSE* SC *8_16_60_c",
+        "MSE* SC _16_32_60_c"
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrClusterSpecification"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrClusterType")
     def attr_cluster_type(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ClusterType: cluster type
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrClusterType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrClusterVersion")
     def attr_cluster_version(self) -> ros_cdk_core.IResolvable:
         '''
-        :Attribute: ClusterVersion: cluster version, Enum: ZooKeeper_3_4_14,ZooKeeper_3_5_5,NACOS_ANS_1_2_1,NACOS_2_0_0
+        :Attribute: ClusterVersion: Cluster version, such as ZooKeeper_3_8_0,NACOS_2_0_0
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrClusterVersion"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
+    @jsii.member(jsii_name="attrConfigAuthEnabled")
+    def attr_config_auth_enabled(self) -> ros_cdk_core.IResolvable:
+        '''
+        :Attribute: ConfigAuthEnabled: Whether the configuration supports it. Valid values: true: false: not supported
+        '''
+        return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrConfigAuthEnabled"))
+
+    @builtins.property
+    @jsii.member(jsii_name="attrConfigSecretEnabled")
+    def attr_config_secret_enabled(self) -> ros_cdk_core.IResolvable:
+        '''
+        :Attribute: ConfigSecretEnabled: Whether the configuration password takes effect. The value is as follows: true: valid false: not valid
+        '''
+        return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrConfigSecretEnabled"))
+
+    @builtins.property
     @jsii.member(jsii_name="attrConnectionType")
     def attr_connection_type(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ConnectionType: network connect type
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrConnectionType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrCpu")
     def attr_cpu(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Cpu: cpu core size
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrCpu"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDiskCapacity")
     def attr_disk_capacity(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: DiskCapacity: disk capacity, unit: G
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDiskCapacity"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDiskType")
     def attr_disk_type(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: DiskType: disk type
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDiskType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrHealthStatus")
     def attr_health_status(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: HealthStatus: health status
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrHealthStatus"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInstanceCount")
     def attr_instance_count(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: InstanceCount: instance count
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInstanceCount"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInstanceId")
     def attr_instance_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: InstanceId: instance id
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInstanceId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInternetAddress")
     def attr_internet_address(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: InternetAddress: internet address
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInternetAddress"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInternetDomain")
     def attr_internet_domain(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: InternetDomain: internet domain
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInternetDomain"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInternetPort")
     def attr_internet_port(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: InternetPort: internet port
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInternetPort"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrIntranetAddress")
     def attr_intranet_address(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: IntranetAddress: intranet address
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrIntranetAddress"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrIntranetDomain")
     def attr_intranet_domain(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: IntranetDomain: intranet domain
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrIntranetDomain"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrIntranetPort")
     def attr_intranet_port(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: IntranetPort: intranet port
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrIntranetPort"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
+    @jsii.member(jsii_name="attrMcpEnabled")
+    def attr_mcp_enabled(self) -> ros_cdk_core.IResolvable:
+        '''
+        :Attribute: MCPEnabled: Whether MCP takes effect, the value is as follows: true: valid false: not valid
+        '''
+        return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrMcpEnabled"))
+
+    @builtins.property
     @jsii.member(jsii_name="attrMemoryCapacity")
     def attr_memory_capacity(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: MemoryCapacity: memory capacity
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrMemoryCapacity"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrMseVersion")
     def attr_mse_version(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute:
 
-        MseVersion: This parameter is required when creating a professional version. The value is as follows:
-        -'mse_basic': indicates the basic version (default value).
-        -'mse_pro': means professional version.
+        MseVersion: Required, the value is as follows:
+        -'mse_dev': indicates the development version.
+        -'Mse_pro': means professional version. When this version is selected, the specification is 2c4g or above, and the specification is 3 nodes or above.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrMseVersion"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrNetType")
     def attr_net_type(self) -> ros_cdk_core.IResolvable:
         '''
-        :Attribute: NetType: network type, Enum: privatenet,pubnet
+        :Attribute: NetType: Network type (whether private network is enabled or not). privatenet indicates that private network is enabled.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrNetType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPayInfo")
     def attr_pay_info(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: PayInfo: pay info
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPayInfo"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPubNetworkFlow")
     def attr_pub_network_flow(self) -> ros_cdk_core.IResolvable:
         '''
-        :Attribute: PubNetworkFlow: pub network flow
+        :Attribute: PubNetworkFlow: Public network bandwidth. If the bandwidth is greater than 0, the public network is enabled.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPubNetworkFlow"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVpcId")
     def attr_vpc_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: VpcId: vpc id
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVpcId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVSwitchId")
     def attr_v_switch_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: VSwitchId: switcher Id
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVSwitchId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="clusterSpecification")
     def cluster_specification(
         self,
     ) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
-        :Property: clusterSpecification: cluster specification, Enum: MSE_SC_1_2_200_c,MSE_SC_2_4_200_c,MSE_SC_4_8_200_c,MSE_SC_8_16_200_c
+        :Property:
+
+        clusterSpecification: Cluster specifications. Note the msversion requirements of the version parameter,
+        Optional parameters:
+        "MSE_ SC *1_2_60_c",
+        "MSE* SC *2_4_60_c",
+        "MSE* SC *4_8_60_c",
+        "MSE* SC *8_16_60_c",
+        "MSE* SC _16_32_60_c"
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "clusterSpecification"))
 
     @cluster_specification.setter
     def cluster_specification(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "cluster_specification").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "clusterSpecification", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="clusterType")
     def cluster_type(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: clusterType: cluster type
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "clusterType"))
 
     @cluster_type.setter
     def cluster_type(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "cluster_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "clusterType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="clusterVersion")
     def cluster_version(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
-        :Property: clusterVersion: cluster version, Enum: ZooKeeper_3_4_14,ZooKeeper_3_5_5,NACOS_ANS_1_2_1,NACOS_2_0_0
+        :Property: clusterVersion: Cluster version, such as ZooKeeper_3_8_0,NACOS_2_0_0
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "clusterVersion"))
 
     @cluster_version.setter
     def cluster_version(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "cluster_version").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "clusterVersion", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="instanceCount")
     def instance_count(self) -> typing.Union[jsii.Number, ros_cdk_core.IResolvable]:
         '''
         :Property: instanceCount: instance count
         '''
         return typing.cast(typing.Union[jsii.Number, ros_cdk_core.IResolvable], jsii.get(self, "instanceCount"))
 
     @instance_count.setter
     def instance_count(
         self,
         value: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "instance_count").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "instanceCount", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="netType")
     def net_type(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
-        :Property: netType: network type, Enum: privatenet,pubnet
+        :Property: netType: Network type (whether private network is enabled or not). privatenet indicates that private network is enabled.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "netType"))
 
     @net_type.setter
     def net_type(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "net_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "netType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="acceptLanguage")
     def accept_language(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: acceptLanguage:
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "acceptLanguage"))
 
     @accept_language.setter
     def accept_language(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "accept_language").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "acceptLanguage", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="aclEntryList")
     def acl_entry_list(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]]:
         '''
-        :Property: aclEntryList: acl entry list
+        :Property: aclEntryList: The public network whitelist list is used only when the public network is enabled.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]], jsii.get(self, "aclEntryList"))
 
     @acl_entry_list.setter
     def acl_entry_list(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "acl_entry_list").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "aclEntryList", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="clusterAliasName")
     def cluster_alias_name(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: clusterAliasName: cluster alias name
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "clusterAliasName"))
 
     @cluster_alias_name.setter
     def cluster_alias_name(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "cluster_alias_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "clusterAliasName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="connectionType")
     def connection_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: connectionType: network connect type
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "connectionType"))
 
     @connection_type.setter
     def connection_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "connection_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "connectionType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="diskType")
     def disk_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: diskType: disk type
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "diskType"))
 
     @disk_type.setter
     def disk_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "disk_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "diskType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="mseVersion")
     def mse_version(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
-        mseVersion: This parameter is required when creating a professional version. The value is as follows:
+        mseVersion: Required, the value is as follows:
 
-        -'mse_basic': indicates the basic version (default value).
-        -'mse_pro': means professional version.
+        -'mse_dev': indicates the development version.
+        -'Mse_pro': means professional version. When this version is selected, the specification is 2c4g or above, and the specification is 3 nodes or above.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "mseVersion"))
 
     @mse_version.setter
     def mse_version(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "mse_version").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "mseVersion", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="privateSlbSpecification")
     def private_slb_specification(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: privateSlbSpecification:
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "privateSlbSpecification"))
 
     @private_slb_specification.setter
     def private_slb_specification(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "private_slb_specification").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "privateSlbSpecification", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="pubNetworkFlow")
     def pub_network_flow(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
-        :Property: pubNetworkFlow: pub network flow
+        :Property: pubNetworkFlow: Public network bandwidth. If the bandwidth is greater than 0, the public network is enabled.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "pubNetworkFlow"))
 
     @pub_network_flow.setter
     def pub_network_flow(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "pub_network_flow").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "pubNetworkFlow", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="pubSlbSpecification")
     def pub_slb_specification(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: pubSlbSpecification:
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "pubSlbSpecification"))
 
     @pub_slb_specification.setter
     def pub_slb_specification(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "pub_slb_specification").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "pubSlbSpecification", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="requestPars")
     def request_pars(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: requestPars:
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "requestPars"))
 
     @request_pars.setter
     def request_pars(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "request_pars").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "requestPars", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vpcId")
     def vpc_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: vpcId: vpc id
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "vpcId"))
 
     @vpc_id.setter
     def vpc_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "vpc_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "vpcId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vSwitchId")
     def v_switch_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: vSwitchId: switcher Id
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "vSwitchId"))
 
     @v_switch_id.setter
     def v_switch_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCluster, "v_switch_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "vSwitchId", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-mse.RosClusterProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -1319,14 +1520,33 @@
         :param private_slb_specification: 
         :param pub_network_flow: 
         :param pub_slb_specification: 
         :param request_pars: 
         :param vpc_id: 
         :param v_switch_id: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosClusterProps.__init__)
+            check_type(argname="argument cluster_specification", value=cluster_specification, expected_type=type_hints["cluster_specification"])
+            check_type(argname="argument cluster_type", value=cluster_type, expected_type=type_hints["cluster_type"])
+            check_type(argname="argument cluster_version", value=cluster_version, expected_type=type_hints["cluster_version"])
+            check_type(argname="argument instance_count", value=instance_count, expected_type=type_hints["instance_count"])
+            check_type(argname="argument net_type", value=net_type, expected_type=type_hints["net_type"])
+            check_type(argname="argument accept_language", value=accept_language, expected_type=type_hints["accept_language"])
+            check_type(argname="argument acl_entry_list", value=acl_entry_list, expected_type=type_hints["acl_entry_list"])
+            check_type(argname="argument cluster_alias_name", value=cluster_alias_name, expected_type=type_hints["cluster_alias_name"])
+            check_type(argname="argument connection_type", value=connection_type, expected_type=type_hints["connection_type"])
+            check_type(argname="argument disk_type", value=disk_type, expected_type=type_hints["disk_type"])
+            check_type(argname="argument mse_version", value=mse_version, expected_type=type_hints["mse_version"])
+            check_type(argname="argument private_slb_specification", value=private_slb_specification, expected_type=type_hints["private_slb_specification"])
+            check_type(argname="argument pub_network_flow", value=pub_network_flow, expected_type=type_hints["pub_network_flow"])
+            check_type(argname="argument pub_slb_specification", value=pub_slb_specification, expected_type=type_hints["pub_slb_specification"])
+            check_type(argname="argument request_pars", value=request_pars, expected_type=type_hints["request_pars"])
+            check_type(argname="argument vpc_id", value=vpc_id, expected_type=type_hints["vpc_id"])
+            check_type(argname="argument v_switch_id", value=v_switch_id, expected_type=type_hints["v_switch_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "cluster_specification": cluster_specification,
             "cluster_type": cluster_type,
             "cluster_version": cluster_version,
             "instance_count": instance_count,
             "net_type": net_type,
         }
@@ -1356,15 +1576,23 @@
             self._values["v_switch_id"] = v_switch_id
 
     @builtins.property
     def cluster_specification(
         self,
     ) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
-        :Property: clusterSpecification: cluster specification, Enum: MSE_SC_1_2_200_c,MSE_SC_2_4_200_c,MSE_SC_4_8_200_c,MSE_SC_8_16_200_c
+        :Property:
+
+        clusterSpecification: Cluster specifications. Note the msversion requirements of the version parameter,
+        Optional parameters:
+        "MSE_ SC *1_2_60_c",
+        "MSE* SC *2_4_60_c",
+        "MSE* SC *4_8_60_c",
+        "MSE* SC *8_16_60_c",
+        "MSE* SC _16_32_60_c"
         '''
         result = self._values.get("cluster_specification")
         assert result is not None, "Required property 'cluster_specification' is missing"
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], result)
 
     @builtins.property
     def cluster_type(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
@@ -1374,15 +1602,15 @@
         result = self._values.get("cluster_type")
         assert result is not None, "Required property 'cluster_type' is missing"
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], result)
 
     @builtins.property
     def cluster_version(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
-        :Property: clusterVersion: cluster version, Enum: ZooKeeper_3_4_14,ZooKeeper_3_5_5,NACOS_ANS_1_2_1,NACOS_2_0_0
+        :Property: clusterVersion: Cluster version, such as ZooKeeper_3_8_0,NACOS_2_0_0
         '''
         result = self._values.get("cluster_version")
         assert result is not None, "Required property 'cluster_version' is missing"
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], result)
 
     @builtins.property
     def instance_count(self) -> typing.Union[jsii.Number, ros_cdk_core.IResolvable]:
@@ -1392,15 +1620,15 @@
         result = self._values.get("instance_count")
         assert result is not None, "Required property 'instance_count' is missing"
         return typing.cast(typing.Union[jsii.Number, ros_cdk_core.IResolvable], result)
 
     @builtins.property
     def net_type(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
-        :Property: netType: network type, Enum: privatenet,pubnet
+        :Property: netType: Network type (whether private network is enabled or not). privatenet indicates that private network is enabled.
         '''
         result = self._values.get("net_type")
         assert result is not None, "Required property 'net_type' is missing"
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], result)
 
     @builtins.property
     def accept_language(
@@ -1413,15 +1641,15 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], result)
 
     @builtins.property
     def acl_entry_list(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]]:
         '''
-        :Property: aclEntryList: acl entry list
+        :Property: aclEntryList: The public network whitelist list is used only when the public network is enabled.
         '''
         result = self._values.get("acl_entry_list")
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]], result)
 
     @builtins.property
     def cluster_alias_name(
         self,
@@ -1455,18 +1683,18 @@
     @builtins.property
     def mse_version(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
-        mseVersion: This parameter is required when creating a professional version. The value is as follows:
+        mseVersion: Required, the value is as follows:
 
-        -'mse_basic': indicates the basic version (default value).
-        -'mse_pro': means professional version.
+        -'mse_dev': indicates the development version.
+        -'Mse_pro': means professional version. When this version is selected, the specification is 2c4g or above, and the specification is 3 nodes or above.
         '''
         result = self._values.get("mse_version")
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], result)
 
     @builtins.property
     def private_slb_specification(
         self,
@@ -1478,15 +1706,15 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], result)
 
     @builtins.property
     def pub_network_flow(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
-        :Property: pubNetworkFlow: pub network flow
+        :Property: pubNetworkFlow: Public network bandwidth. If the bandwidth is greater than 0, the public network is enabled.
         '''
         result = self._values.get("pub_network_flow")
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], result)
 
     @builtins.property
     def pub_slb_specification(
         self,
@@ -1546,252 +1774,291 @@
 ):
     '''A ROS template type:  ``ALIYUN::MSE::Gateway``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosGatewayProps",
+        props: typing.Union["RosGatewayProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::MSE::Gateway``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosGateway.__init__)
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
+            type_hints = typing.get_type_hints(RosGateway._render_properties)
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
     @jsii.member(jsii_name="attrBackupVSwitchId")
     def attr_backup_v_switch_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: BackupVSwitchId: VSwitchId For Backup
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrBackupVSwitchId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrGatewayUniqueId")
     def attr_gateway_unique_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: GatewayUniqueId: Gateway unique identification
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrGatewayUniqueId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPaymentType")
     def attr_payment_type(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: PaymentType: The payment type of the resource
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPaymentType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrReplica")
     def attr_replica(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Replica: Gateway Node Number
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrReplica"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrSpec")
     def attr_spec(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Spec: Gateway Node Specifications
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrSpec"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVpcId")
     def attr_vpc_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: VpcId: VpcId
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVpcId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVSwitchId")
     def attr_v_switch_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: VSwitchId: VSwitchId
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
+            type_hints = typing.get_type_hints(getattr(RosGateway, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="replica")
     def replica(self) -> typing.Union[jsii.Number, ros_cdk_core.IResolvable]:
         '''
         :Property: replica: Gateway Node Number
         '''
         return typing.cast(typing.Union[jsii.Number, ros_cdk_core.IResolvable], jsii.get(self, "replica"))
 
     @replica.setter
     def replica(
         self,
         value: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosGateway, "replica").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "replica", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="spec")
     def spec(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: spec: Gateway Node Specifications
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "spec"))
 
     @spec.setter
     def spec(self, value: typing.Union[builtins.str, ros_cdk_core.IResolvable]) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosGateway, "spec").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "spec", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vpcId")
     def vpc_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: vpcId: VpcId
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "vpcId"))
 
     @vpc_id.setter
     def vpc_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosGateway, "vpc_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "vpcId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vSwitchId")
     def v_switch_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: vSwitchId: VSwitchId
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "vSwitchId"))
 
     @v_switch_id.setter
     def v_switch_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosGateway, "v_switch_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "vSwitchId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="backupVSwitchId")
     def backup_v_switch_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: backupVSwitchId: VSwitchId For Backup
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "backupVSwitchId"))
 
     @backup_v_switch_id.setter
     def backup_v_switch_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosGateway, "backup_v_switch_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "backupVSwitchId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enterpriseSecurityGroup")
     def enterprise_security_group(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: enterpriseSecurityGroup:
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "enterpriseSecurityGroup"))
 
     @enterprise_security_group.setter
     def enterprise_security_group(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosGateway, "enterprise_security_group").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enterpriseSecurityGroup", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="internetSlbSpec")
     def internet_slb_spec(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: internetSlbSpec:
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "internetSlbSpec"))
 
     @internet_slb_spec.setter
     def internet_slb_spec(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosGateway, "internet_slb_spec").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "internetSlbSpec", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="name")
     def name(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: name:
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "name"))
 
     @name.setter
     def name(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosGateway, "name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "name", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="slbSpec")
     def slb_spec(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: slbSpec:
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "slbSpec"))
 
     @slb_spec.setter
     def slb_spec(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosGateway, "slb_spec").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "slbSpec", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-mse.RosGatewayProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -1828,14 +2095,25 @@
         :param v_switch_id: 
         :param backup_v_switch_id: 
         :param enterprise_security_group: 
         :param internet_slb_spec: 
         :param name: 
         :param slb_spec: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosGatewayProps.__init__)
+            check_type(argname="argument replica", value=replica, expected_type=type_hints["replica"])
+            check_type(argname="argument spec", value=spec, expected_type=type_hints["spec"])
+            check_type(argname="argument vpc_id", value=vpc_id, expected_type=type_hints["vpc_id"])
+            check_type(argname="argument v_switch_id", value=v_switch_id, expected_type=type_hints["v_switch_id"])
+            check_type(argname="argument backup_v_switch_id", value=backup_v_switch_id, expected_type=type_hints["backup_v_switch_id"])
+            check_type(argname="argument enterprise_security_group", value=enterprise_security_group, expected_type=type_hints["enterprise_security_group"])
+            check_type(argname="argument internet_slb_spec", value=internet_slb_spec, expected_type=type_hints["internet_slb_spec"])
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+            check_type(argname="argument slb_spec", value=slb_spec, expected_type=type_hints["slb_spec"])
         self._values: typing.Dict[str, typing.Any] = {
             "replica": replica,
             "spec": spec,
             "vpc_id": vpc_id,
             "v_switch_id": v_switch_id,
         }
         if backup_v_switch_id is not None:
```

### Comparing `ros-cdk-mse-1.0.8/src/ros_cdk_mse.egg-info/PKG-INFO` & `ros-cdk-mse-1.0.9/src/ros_cdk_mse.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-mse
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS MSE Construct Library
```

