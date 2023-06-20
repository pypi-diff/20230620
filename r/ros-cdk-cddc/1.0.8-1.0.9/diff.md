# Comparing `tmp/ros-cdk-cddc-1.0.8.tar.gz` & `tmp/ros-cdk-cddc-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-cddc-1.0.8.tar", last modified: Thu Jul 14 02:30:25 2022, max compression
+gzip compressed data, was "dist/ros-cdk-cddc-1.0.9.tar", last modified: Fri Sep 23 10:51:52 2022, max compression
```

## Comparing `ros-cdk-cddc-1.0.8.tar` & `ros-cdk-cddc-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:30:25.000000 ros-cdk-cddc-1.0.8/
--rw-r--r--   0 root         (0) root         (0)    10279 2022-07-14 02:30:24.000000 ros-cdk-cddc-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2022-07-14 02:30:24.000000 ros-cdk-cddc-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2022-07-14 02:30:24.000000 ros-cdk-cddc-1.0.8/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1244 2022-07-14 02:30:25.000000 ros-cdk-cddc-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      182 2022-07-14 02:30:24.000000 ros-cdk-cddc-1.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)      106 2022-07-14 02:30:24.000000 ros-cdk-cddc-1.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-07-14 02:30:25.000000 ros-cdk-cddc-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1800 2022-07-14 02:30:24.000000 ros-cdk-cddc-1.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:30:25.000000 ros-cdk-cddc-1.0.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:30:25.000000 ros-cdk-cddc-1.0.8/src/ros_cdk_cddc/
--rw-r--r--   0 root         (0) root         (0)    81083 2022-07-14 02:30:24.000000 ros-cdk-cddc-1.0.8/src/ros_cdk_cddc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:30:25.000000 ros-cdk-cddc-1.0.8/src/ros_cdk_cddc/_jsii/
--rw-r--r--   0 root         (0) root         (0)      372 2022-07-14 02:30:24.000000 ros-cdk-cddc-1.0.8/src/ros_cdk_cddc/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    45708 2022-07-14 02:30:24.000000 ros-cdk-cddc-1.0.8/src/ros_cdk_cddc/_jsii/ros-cdk-cddc@1.0.8.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:30:24.000000 ros-cdk-cddc-1.0.8/src/ros_cdk_cddc/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:30:25.000000 ros-cdk-cddc-1.0.8/src/ros_cdk_cddc.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1244 2022-07-14 02:30:25.000000 ros-cdk-cddc-1.0.8/src/ros_cdk_cddc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      410 2022-07-14 02:30:25.000000 ros-cdk-cddc-1.0.8/src/ros_cdk_cddc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:30:25.000000 ros-cdk-cddc-1.0.8/src/ros_cdk_cddc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2022-07-14 02:30:25.000000 ros-cdk-cddc-1.0.8/src/ros_cdk_cddc.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2022-07-14 02:30:25.000000 ros-cdk-cddc-1.0.8/src/ros_cdk_cddc.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 10:51:52.000000 ros-cdk-cddc-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)    10279 2022-09-23 10:51:51.000000 ros-cdk-cddc-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-09-23 10:51:51.000000 ros-cdk-cddc-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2022-09-23 10:51:51.000000 ros-cdk-cddc-1.0.9/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1244 2022-09-23 10:51:52.000000 ros-cdk-cddc-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      182 2022-09-23 10:51:51.000000 ros-cdk-cddc-1.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      236 2022-09-23 10:51:51.000000 ros-cdk-cddc-1.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-09-23 10:51:52.000000 ros-cdk-cddc-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1829 2022-09-23 10:51:51.000000 ros-cdk-cddc-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 10:51:52.000000 ros-cdk-cddc-1.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 10:51:52.000000 ros-cdk-cddc-1.0.9/src/ros_cdk_cddc/
+-rw-r--r--   0 root         (0) root         (0)    92353 2022-09-23 10:51:51.000000 ros-cdk-cddc-1.0.9/src/ros_cdk_cddc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 10:51:52.000000 ros-cdk-cddc-1.0.9/src/ros_cdk_cddc/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      406 2022-09-23 10:51:51.000000 ros-cdk-cddc-1.0.9/src/ros_cdk_cddc/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    45783 2022-09-23 10:51:51.000000 ros-cdk-cddc-1.0.9/src/ros_cdk_cddc/_jsii/ros-cdk-cddc@1.0.9.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 10:51:51.000000 ros-cdk-cddc-1.0.9/src/ros_cdk_cddc/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 10:51:52.000000 ros-cdk-cddc-1.0.9/src/ros_cdk_cddc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1244 2022-09-23 10:51:51.000000 ros-cdk-cddc-1.0.9/src/ros_cdk_cddc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      410 2022-09-23 10:51:51.000000 ros-cdk-cddc-1.0.9/src/ros_cdk_cddc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 10:51:51.000000 ros-cdk-cddc-1.0.9/src/ros_cdk_cddc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2022-09-23 10:51:51.000000 ros-cdk-cddc-1.0.9/src/ros_cdk_cddc.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2022-09-23 10:51:51.000000 ros-cdk-cddc-1.0.9/src/ros_cdk_cddc.egg-info/top_level.txt
```

### Comparing `ros-cdk-cddc-1.0.8/LICENSE` & `ros-cdk-cddc-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-cddc-1.0.8/PKG-INFO` & `ros-cdk-cddc-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-cddc
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS CDDC Construct Library
```

### Comparing `ros-cdk-cddc-1.0.8/setup.py` & `ros-cdk-cddc-1.0.9/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-cddc",
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
         "ros_cdk_cddc",
         "ros_cdk_cddc._jsii"
     ],
     "package_data": {
         "ros_cdk_cddc._jsii": [
-            "ros-cdk-cddc@1.0.8.jsii.tgz"
+            "ros-cdk-cddc@1.0.9.jsii.tgz"
         ],
         "ros_cdk_cddc": [
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

### Comparing `ros-cdk-cddc-1.0.8/src/ros_cdk_cddc/__init__.py` & `ros-cdk-cddc-1.0.9/src/ros_cdk_cddc/__init__.py`

 * *Files 24% similar despite different names*

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
 
 
 class DedicatedHost(
     ros_cdk_core.Resource,
@@ -29,163 +31,169 @@
 ):
     '''A ROS resource type:  ``ALIYUN::CDDC::DedicatedHost``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "DedicatedHostProps",
+        props: typing.Union["DedicatedHostProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::CDDC::DedicatedHost``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(DedicatedHost.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrAutoRenew")
     def attr_auto_renew(self) -> ros_cdk_core.IResolvable:
         '''Attribute AutoRenew: Whether Auto Renew.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAutoRenew"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrCpuAllocationRatio")
     def attr_cpu_allocation_ratio(self) -> ros_cdk_core.IResolvable:
         '''Attribute CpuAllocationRatio: CPU Allocation Ratio.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrCpuAllocationRatio"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrCpuUsed")
     def attr_cpu_used(self) -> ros_cdk_core.IResolvable:
         '''Attribute CpuUsed: CPU Used.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrCpuUsed"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDedicatedHostGroupId")
     def attr_dedicated_host_group_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute DedicatedHostGroupId: Dedicated Host Group ID.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDedicatedHostGroupId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDedicatedHostId")
     def attr_dedicated_host_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute DedicatedHostId: The first ID of the resource.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDedicatedHostId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDiskAllocationRatio")
     def attr_disk_allocation_ratio(self) -> ros_cdk_core.IResolvable:
         '''Attribute DiskAllocationRatio: Disk Allocation Ratio.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDiskAllocationRatio"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrEcsClassCode")
     def attr_ecs_class_code(self) -> ros_cdk_core.IResolvable:
         '''Attribute EcsClassCode: ECS Class Code.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrEcsClassCode"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrHostClass")
     def attr_host_class(self) -> ros_cdk_core.IResolvable:
         '''Attribute HostClass: Host Class.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrHostClass"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrHostCpu")
     def attr_host_cpu(self) -> ros_cdk_core.IResolvable:
         '''Attribute HostCpu: Host CPU.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrHostCpu"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrHostMem")
     def attr_host_mem(self) -> ros_cdk_core.IResolvable:
         '''Attribute HostMem: Host Memory.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrHostMem"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrHostName")
     def attr_host_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute HostName: Host Name.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrHostName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrHostStorage")
     def attr_host_storage(self) -> ros_cdk_core.IResolvable:
         '''Attribute HostStorage: Host Storage.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrHostStorage"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrHostType")
     def attr_host_type(self) -> ros_cdk_core.IResolvable:
         '''Attribute HostType: Host Storage Type.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrHostType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrImageCategory")
     def attr_image_category(self) -> ros_cdk_core.IResolvable:
         '''Attribute ImageCategory: Host Image Category.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrImageCategory"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrIpAddress")
     def attr_ip_address(self) -> ros_cdk_core.IResolvable:
         '''Attribute IpAddress: Host IP Address.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrIpAddress"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrMemAllocationRatio")
     def attr_mem_allocation_ratio(self) -> ros_cdk_core.IResolvable:
         '''Attribute MemAllocationRatio: Memory Allocation Ratio.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrMemAllocationRatio"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrMemoryUsed")
     def attr_memory_used(self) -> ros_cdk_core.IResolvable:
         '''Attribute MemoryUsed: Host Memory Used.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrMemoryUsed"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrOpenPermission")
     def attr_open_permission(self) -> ros_cdk_core.IResolvable:
         '''Attribute OpenPermission: Whether Open OS Permission.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrOpenPermission"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPaymentType")
     def attr_payment_type(self) -> ros_cdk_core.IResolvable:
         '''Attribute PaymentType: Payment Type.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPaymentType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrStorageUsed")
     def attr_storage_used(self) -> ros_cdk_core.IResolvable:
         '''Attribute StorageUsed: Storage Used.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrStorageUsed"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVpcId")
     def attr_vpc_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute VpcId: VPC ID.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVpcId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVSwitchId")
     def attr_v_switch_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute VSwitchId: VSwitch ID.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVSwitchId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrZoneId")
     def attr_zone_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute ZoneId: Zone ID.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrZoneId"))
 
 
 class DedicatedHostGroup(
@@ -195,175 +203,181 @@
 ):
     '''A ROS resource type:  ``ALIYUN::CDDC::DedicatedHostGroup``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "DedicatedHostGroupProps",
+        props: typing.Union["DedicatedHostGroupProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::CDDC::DedicatedHostGroup``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(DedicatedHostGroup.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrAllocationPolicy")
     def attr_allocation_policy(self) -> ros_cdk_core.IResolvable:
         '''Attribute AllocationPolicy: Allocation Policy.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAllocationPolicy"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrBastionInstanceId")
     def attr_bastion_instance_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute BastionInstanceId: BastionInstanceId.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrBastionInstanceId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrCpuAllocatedAmount")
     def attr_cpu_allocated_amount(self) -> ros_cdk_core.IResolvable:
         '''Attribute CpuAllocatedAmount: CpuAllocatedAmount.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrCpuAllocatedAmount"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrCpuAllocateRation")
     def attr_cpu_allocate_ration(self) -> ros_cdk_core.IResolvable:
         '''Attribute CpuAllocateRation: CpuAllocateRation.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrCpuAllocateRation"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrCpuAllocationRatio")
     def attr_cpu_allocation_ratio(self) -> ros_cdk_core.IResolvable:
         '''Attribute CpuAllocationRatio: Cpu Allocation Ratio.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrCpuAllocationRatio"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDedicatedHostGroupDesc")
     def attr_dedicated_host_group_desc(self) -> ros_cdk_core.IResolvable:
         '''Attribute DedicatedHostGroupDesc: Dedicated Host Group Description.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDedicatedHostGroupDesc"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDedicatedHostGroupId")
     def attr_dedicated_host_group_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute DedicatedHostGroupId: Dedicated Host Group ID.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDedicatedHostGroupId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDeployType")
     def attr_deploy_type(self) -> ros_cdk_core.IResolvable:
         '''Attribute DeployType: DeployType.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDeployType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDiskAllocatedAmount")
     def attr_disk_allocated_amount(self) -> ros_cdk_core.IResolvable:
         '''Attribute DiskAllocatedAmount: DiskAllocatedAmount.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDiskAllocatedAmount"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDiskAllocateRation")
     def attr_disk_allocate_ration(self) -> ros_cdk_core.IResolvable:
         '''Attribute DiskAllocateRation: DiskAllocateRation.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDiskAllocateRation"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDiskAllocationRatio")
     def attr_disk_allocation_ratio(self) -> ros_cdk_core.IResolvable:
         '''Attribute DiskAllocationRatio: Disk Allocation Ratio.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDiskAllocationRatio"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDiskUsedAmount")
     def attr_disk_used_amount(self) -> ros_cdk_core.IResolvable:
         '''Attribute DiskUsedAmount: DiskUsedAmount.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDiskUsedAmount"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDiskUtility")
     def attr_disk_utility(self) -> ros_cdk_core.IResolvable:
         '''Attribute DiskUtility: DiskUtility.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDiskUtility"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrEngine")
     def attr_engine(self) -> ros_cdk_core.IResolvable:
         '''Attribute Engine: Database Engine Type.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrEngine"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrHostNumber")
     def attr_host_number(self) -> ros_cdk_core.IResolvable:
         '''Attribute HostNumber: Total Host Number.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrHostNumber"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrHostReplacePolicy")
     def attr_host_replace_policy(self) -> ros_cdk_core.IResolvable:
         '''Attribute HostReplacePolicy: Host Replace Policy.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrHostReplacePolicy"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInstanceNumber")
     def attr_instance_number(self) -> ros_cdk_core.IResolvable:
         '''Attribute InstanceNumber: Total Instance Number.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInstanceNumber"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrMemAllocatedAmount")
     def attr_mem_allocated_amount(self) -> ros_cdk_core.IResolvable:
         '''Attribute MemAllocatedAmount: MemAllocatedAmount.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrMemAllocatedAmount"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrMemAllocateRation")
     def attr_mem_allocate_ration(self) -> ros_cdk_core.IResolvable:
         '''Attribute MemAllocateRation: MemAllocateRation.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrMemAllocateRation"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrMemAllocationRatio")
     def attr_mem_allocation_ratio(self) -> ros_cdk_core.IResolvable:
         '''Attribute MemAllocationRatio: Memory Allocation Ratio.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrMemAllocationRatio"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrMemUsedAmount")
     def attr_mem_used_amount(self) -> ros_cdk_core.IResolvable:
         '''Attribute MemUsedAmount: MemUsedAmount.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrMemUsedAmount"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrMemUtility")
     def attr_mem_utility(self) -> ros_cdk_core.IResolvable:
         '''Attribute MemUtility: MemUtility.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrMemUtility"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrOpenPermission")
     def attr_open_permission(self) -> ros_cdk_core.IResolvable:
         '''Attribute OpenPermission: Whether Open OS Permission.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrOpenPermission"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrText")
     def attr_text(self) -> ros_cdk_core.IResolvable:
         '''Attribute Text: Text.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrText"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVpcId")
     def attr_vpc_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute VpcId: VPC ID.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVpcId"))
 
 
 @jsii.data_type(
@@ -403,14 +417,25 @@
         :param cpu_allocation_ratio: Property cpuAllocationRatio: Cpu Allocation Ratio.
         :param dedicated_host_group_desc: Property dedicatedHostGroupDesc: Dedicated Host Group Description.
         :param disk_allocation_ratio: Property diskAllocationRatio: Disk Allocation Ratio.
         :param host_replace_policy: Property hostReplacePolicy: Host Replace Policy.
         :param mem_allocation_ratio: Property memAllocationRatio: Memory Allocation Ratio.
         :param open_permission: Property openPermission: Whether Open OS Permission.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(DedicatedHostGroupProps.__init__)
+            check_type(argname="argument engine", value=engine, expected_type=type_hints["engine"])
+            check_type(argname="argument vpc_id", value=vpc_id, expected_type=type_hints["vpc_id"])
+            check_type(argname="argument allocation_policy", value=allocation_policy, expected_type=type_hints["allocation_policy"])
+            check_type(argname="argument cpu_allocation_ratio", value=cpu_allocation_ratio, expected_type=type_hints["cpu_allocation_ratio"])
+            check_type(argname="argument dedicated_host_group_desc", value=dedicated_host_group_desc, expected_type=type_hints["dedicated_host_group_desc"])
+            check_type(argname="argument disk_allocation_ratio", value=disk_allocation_ratio, expected_type=type_hints["disk_allocation_ratio"])
+            check_type(argname="argument host_replace_policy", value=host_replace_policy, expected_type=type_hints["host_replace_policy"])
+            check_type(argname="argument mem_allocation_ratio", value=mem_allocation_ratio, expected_type=type_hints["mem_allocation_ratio"])
+            check_type(argname="argument open_permission", value=open_permission, expected_type=type_hints["open_permission"])
         self._values: typing.Dict[str, typing.Any] = {
             "engine": engine,
             "vpc_id": vpc_id,
         }
         if allocation_policy is not None:
             self._values["allocation_policy"] = allocation_policy
         if cpu_allocation_ratio is not None:
@@ -536,15 +561,15 @@
         v_switch_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         zone_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         auto_renew: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         host_name: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         image_category: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         os_password: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         period: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        tags: typing.Optional[typing.Sequence["RosDedicatedHost.TagsProperty"]] = None,
+        tags: typing.Optional[typing.Sequence[typing.Union["RosDedicatedHost.TagsProperty", typing.Dict[str, typing.Any]]]] = None,
         used_time: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::CDDC::DedicatedHost``.
 
         :param dedicated_host_group_id: Property dedicatedHostGroupId: Dedicated Host Group ID.
         :param host_class: Property hostClass: Host Class.
         :param payment_type: Property paymentType: Payment Type.
@@ -554,14 +579,28 @@
         :param host_name: Property hostName: Host Name.
         :param image_category: Property imageCategory: Host Image Category.
         :param os_password: Property osPassword:.
         :param period: Property period:.
         :param tags: Property tags: The tag of the resource.
         :param used_time: Property usedTime:.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(DedicatedHostProps.__init__)
+            check_type(argname="argument dedicated_host_group_id", value=dedicated_host_group_id, expected_type=type_hints["dedicated_host_group_id"])
+            check_type(argname="argument host_class", value=host_class, expected_type=type_hints["host_class"])
+            check_type(argname="argument payment_type", value=payment_type, expected_type=type_hints["payment_type"])
+            check_type(argname="argument v_switch_id", value=v_switch_id, expected_type=type_hints["v_switch_id"])
+            check_type(argname="argument zone_id", value=zone_id, expected_type=type_hints["zone_id"])
+            check_type(argname="argument auto_renew", value=auto_renew, expected_type=type_hints["auto_renew"])
+            check_type(argname="argument host_name", value=host_name, expected_type=type_hints["host_name"])
+            check_type(argname="argument image_category", value=image_category, expected_type=type_hints["image_category"])
+            check_type(argname="argument os_password", value=os_password, expected_type=type_hints["os_password"])
+            check_type(argname="argument period", value=period, expected_type=type_hints["period"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
+            check_type(argname="argument used_time", value=used_time, expected_type=type_hints["used_time"])
         self._values: typing.Dict[str, typing.Any] = {
             "dedicated_host_group_id": dedicated_host_group_id,
             "host_class": host_class,
             "payment_type": payment_type,
             "v_switch_id": v_switch_id,
             "zone_id": zone_id,
         }
@@ -690,432 +729,480 @@
 ):
     '''A ROS template type:  ``ALIYUN::CDDC::DedicatedHost``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosDedicatedHostProps",
+        props: typing.Union["RosDedicatedHostProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::CDDC::DedicatedHost``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosDedicatedHost.__init__)
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
+            type_hints = typing.get_type_hints(RosDedicatedHost._render_properties)
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
     @jsii.member(jsii_name="attrAutoRenew")
     def attr_auto_renew(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: AutoRenew: Whether Auto Renew
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAutoRenew"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrCpuAllocationRatio")
     def attr_cpu_allocation_ratio(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: CpuAllocationRatio: CPU Allocation Ratio
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrCpuAllocationRatio"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrCpuUsed")
     def attr_cpu_used(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: CpuUsed: CPU Used
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrCpuUsed"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDedicatedHostGroupId")
     def attr_dedicated_host_group_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: DedicatedHostGroupId: Dedicated Host Group ID
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDedicatedHostGroupId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDedicatedHostId")
     def attr_dedicated_host_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: DedicatedHostId: The first ID of the resource
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDedicatedHostId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDiskAllocationRatio")
     def attr_disk_allocation_ratio(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: DiskAllocationRatio: Disk Allocation Ratio
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDiskAllocationRatio"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrEcsClassCode")
     def attr_ecs_class_code(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: EcsClassCode: ECS Class Code
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrEcsClassCode"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrHostClass")
     def attr_host_class(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: HostClass: Host Class
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrHostClass"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrHostCpu")
     def attr_host_cpu(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: HostCpu: Host CPU
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrHostCpu"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrHostMem")
     def attr_host_mem(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: HostMem: Host Memory
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrHostMem"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrHostName")
     def attr_host_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: HostName: Host Name
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrHostName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrHostStorage")
     def attr_host_storage(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: HostStorage: Host Storage
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrHostStorage"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrHostType")
     def attr_host_type(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: HostType: Host Storage Type
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrHostType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrImageCategory")
     def attr_image_category(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ImageCategory: Host Image Category
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrImageCategory"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrIpAddress")
     def attr_ip_address(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: IpAddress: Host IP Address
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrIpAddress"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrMemAllocationRatio")
     def attr_mem_allocation_ratio(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: MemAllocationRatio: Memory Allocation Ratio
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrMemAllocationRatio"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrMemoryUsed")
     def attr_memory_used(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: MemoryUsed: Host Memory Used
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrMemoryUsed"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrOpenPermission")
     def attr_open_permission(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: OpenPermission: Whether Open OS Permission
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrOpenPermission"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPaymentType")
     def attr_payment_type(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: PaymentType: Payment Type
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPaymentType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrStorageUsed")
     def attr_storage_used(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: StorageUsed: Storage Used
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrStorageUsed"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVpcId")
     def attr_vpc_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: VpcId: VPC ID
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVpcId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVSwitchId")
     def attr_v_switch_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: VSwitchId: VSwitch ID
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVSwitchId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrZoneId")
     def attr_zone_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ZoneId: Zone ID
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrZoneId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dedicatedHostGroupId")
     def dedicated_host_group_id(
         self,
     ) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: dedicatedHostGroupId: Dedicated Host Group ID
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "dedicatedHostGroupId"))
 
     @dedicated_host_group_id.setter
     def dedicated_host_group_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDedicatedHost, "dedicated_host_group_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dedicatedHostGroupId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDedicatedHost, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="hostClass")
     def host_class(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: hostClass: Host Class
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "hostClass"))
 
     @host_class.setter
     def host_class(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDedicatedHost, "host_class").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "hostClass", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="paymentType")
     def payment_type(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: paymentType: Payment Type
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "paymentType"))
 
     @payment_type.setter
     def payment_type(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDedicatedHost, "payment_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "paymentType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vSwitchId")
     def v_switch_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: vSwitchId: VSwitch ID
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "vSwitchId"))
 
     @v_switch_id.setter
     def v_switch_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDedicatedHost, "v_switch_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "vSwitchId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="zoneId")
     def zone_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: zoneId: Zone ID
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "zoneId"))
 
     @zone_id.setter
     def zone_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDedicatedHost, "zone_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "zoneId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="autoRenew")
     def auto_renew(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: autoRenew: Whether Auto Renew
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "autoRenew"))
 
     @auto_renew.setter
     def auto_renew(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDedicatedHost, "auto_renew").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "autoRenew", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="hostName")
     def host_name(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: hostName: Host Name
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "hostName"))
 
     @host_name.setter
     def host_name(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDedicatedHost, "host_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "hostName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="imageCategory")
     def image_category(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: imageCategory: Host Image Category
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "imageCategory"))
 
     @image_category.setter
     def image_category(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDedicatedHost, "image_category").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "imageCategory", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="osPassword")
     def os_password(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: osPassword:
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "osPassword"))
 
     @os_password.setter
     def os_password(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDedicatedHost, "os_password").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "osPassword", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="period")
     def period(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: period:
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "period"))
 
     @period.setter
     def period(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDedicatedHost, "period").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "period", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="tags")
     def tags(self) -> typing.Optional[typing.List["RosDedicatedHost.TagsProperty"]]:
         '''
         :Property: tags: The tag of the resource
         '''
         return typing.cast(typing.Optional[typing.List["RosDedicatedHost.TagsProperty"]], jsii.get(self, "tags"))
 
     @tags.setter
     def tags(
         self,
         value: typing.Optional[typing.List["RosDedicatedHost.TagsProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDedicatedHost, "tags").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "tags", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="usedTime")
     def used_time(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: usedTime:
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "usedTime"))
 
     @used_time.setter
     def used_time(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDedicatedHost, "used_time").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "usedTime", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-cddc.RosDedicatedHost.TagsProperty",
         jsii_struct_bases=[],
         name_mapping={"tag_key": "tagKey", "tag_value": "tagValue"},
     )
@@ -1126,14 +1213,18 @@
             tag_key: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
             tag_value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param tag_key: 
             :param tag_value: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosDedicatedHost.TagsProperty.__init__)
+                check_type(argname="argument tag_key", value=tag_key, expected_type=type_hints["tag_key"])
+                check_type(argname="argument tag_value", value=tag_value, expected_type=type_hints["tag_value"])
             self._values: typing.Dict[str, typing.Any] = {}
             if tag_key is not None:
                 self._values["tag_key"] = tag_key
             if tag_value is not None:
                 self._values["tag_value"] = tag_value
 
         @builtins.property
@@ -1175,403 +1266,442 @@
 ):
     '''A ROS template type:  ``ALIYUN::CDDC::DedicatedHostGroup``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosDedicatedHostGroupProps",
+        props: typing.Union["RosDedicatedHostGroupProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::CDDC::DedicatedHostGroup``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosDedicatedHostGroup.__init__)
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
+            type_hints = typing.get_type_hints(RosDedicatedHostGroup._render_properties)
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
     @jsii.member(jsii_name="attrAllocationPolicy")
     def attr_allocation_policy(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: AllocationPolicy: Allocation Policy
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAllocationPolicy"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrBastionInstanceId")
     def attr_bastion_instance_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: BastionInstanceId: BastionInstanceId
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrBastionInstanceId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrCpuAllocatedAmount")
     def attr_cpu_allocated_amount(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: CpuAllocatedAmount: CpuAllocatedAmount
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrCpuAllocatedAmount"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrCpuAllocateRation")
     def attr_cpu_allocate_ration(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: CpuAllocateRation: CpuAllocateRation
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrCpuAllocateRation"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrCpuAllocationRatio")
     def attr_cpu_allocation_ratio(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: CpuAllocationRatio: Cpu Allocation Ratio
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrCpuAllocationRatio"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDedicatedHostGroupDesc")
     def attr_dedicated_host_group_desc(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: DedicatedHostGroupDesc: Dedicated Host Group Description
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDedicatedHostGroupDesc"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDedicatedHostGroupId")
     def attr_dedicated_host_group_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: DedicatedHostGroupId: Dedicated Host Group ID
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDedicatedHostGroupId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDeployType")
     def attr_deploy_type(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: DeployType: DeployType
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDeployType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDiskAllocatedAmount")
     def attr_disk_allocated_amount(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: DiskAllocatedAmount: DiskAllocatedAmount
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDiskAllocatedAmount"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDiskAllocateRation")
     def attr_disk_allocate_ration(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: DiskAllocateRation: DiskAllocateRation
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDiskAllocateRation"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDiskAllocationRatio")
     def attr_disk_allocation_ratio(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: DiskAllocationRatio: Disk Allocation Ratio
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDiskAllocationRatio"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDiskUsedAmount")
     def attr_disk_used_amount(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: DiskUsedAmount: DiskUsedAmount
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDiskUsedAmount"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrDiskUtility")
     def attr_disk_utility(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: DiskUtility: DiskUtility
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDiskUtility"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrEngine")
     def attr_engine(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Engine: Database Engine Type
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrEngine"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrHostNumber")
     def attr_host_number(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: HostNumber: Total Host Number
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrHostNumber"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrHostReplacePolicy")
     def attr_host_replace_policy(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: HostReplacePolicy: Host Replace Policy
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrHostReplacePolicy"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrInstanceNumber")
     def attr_instance_number(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: InstanceNumber: Total Instance Number
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrInstanceNumber"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrMemAllocatedAmount")
     def attr_mem_allocated_amount(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: MemAllocatedAmount: MemAllocatedAmount
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrMemAllocatedAmount"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrMemAllocateRation")
     def attr_mem_allocate_ration(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: MemAllocateRation: MemAllocateRation
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrMemAllocateRation"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrMemAllocationRatio")
     def attr_mem_allocation_ratio(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: MemAllocationRatio: Memory Allocation Ratio
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrMemAllocationRatio"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrMemUsedAmount")
     def attr_mem_used_amount(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: MemUsedAmount: MemUsedAmount
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrMemUsedAmount"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrMemUtility")
     def attr_mem_utility(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: MemUtility: MemUtility
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrMemUtility"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrOpenPermission")
     def attr_open_permission(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: OpenPermission: Whether Open OS Permission
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrOpenPermission"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrText")
     def attr_text(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Text: Text
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrText"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVpcId")
     def attr_vpc_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: VpcId: VPC ID
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVpcId"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosDedicatedHostGroup, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="engine")
     def engine(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: engine: Database Engine Type
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "engine"))
 
     @engine.setter
     def engine(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDedicatedHostGroup, "engine").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "engine", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vpcId")
     def vpc_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: vpcId: VPC ID
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "vpcId"))
 
     @vpc_id.setter
     def vpc_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDedicatedHostGroup, "vpc_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "vpcId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="allocationPolicy")
     def allocation_policy(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: allocationPolicy: Allocation Policy
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "allocationPolicy"))
 
     @allocation_policy.setter
     def allocation_policy(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDedicatedHostGroup, "allocation_policy").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "allocationPolicy", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="cpuAllocationRatio")
     def cpu_allocation_ratio(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: cpuAllocationRatio: Cpu Allocation Ratio
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "cpuAllocationRatio"))
 
     @cpu_allocation_ratio.setter
     def cpu_allocation_ratio(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDedicatedHostGroup, "cpu_allocation_ratio").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "cpuAllocationRatio", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="dedicatedHostGroupDesc")
     def dedicated_host_group_desc(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: dedicatedHostGroupDesc: Dedicated Host Group Description
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "dedicatedHostGroupDesc"))
 
     @dedicated_host_group_desc.setter
     def dedicated_host_group_desc(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDedicatedHostGroup, "dedicated_host_group_desc").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "dedicatedHostGroupDesc", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="diskAllocationRatio")
     def disk_allocation_ratio(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: diskAllocationRatio: Disk Allocation Ratio
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "diskAllocationRatio"))
 
     @disk_allocation_ratio.setter
     def disk_allocation_ratio(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDedicatedHostGroup, "disk_allocation_ratio").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "diskAllocationRatio", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="hostReplacePolicy")
     def host_replace_policy(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: hostReplacePolicy: Host Replace Policy
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "hostReplacePolicy"))
 
     @host_replace_policy.setter
     def host_replace_policy(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDedicatedHostGroup, "host_replace_policy").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "hostReplacePolicy", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="memAllocationRatio")
     def mem_allocation_ratio(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: memAllocationRatio: Memory Allocation Ratio
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "memAllocationRatio"))
 
     @mem_allocation_ratio.setter
     def mem_allocation_ratio(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDedicatedHostGroup, "mem_allocation_ratio").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "memAllocationRatio", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="openPermission")
     def open_permission(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: openPermission: Whether Open OS Permission
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "openPermission"))
 
     @open_permission.setter
     def open_permission(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosDedicatedHostGroup, "open_permission").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "openPermission", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-cddc.RosDedicatedHostGroupProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -1608,14 +1738,25 @@
         :param cpu_allocation_ratio: 
         :param dedicated_host_group_desc: 
         :param disk_allocation_ratio: 
         :param host_replace_policy: 
         :param mem_allocation_ratio: 
         :param open_permission: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosDedicatedHostGroupProps.__init__)
+            check_type(argname="argument engine", value=engine, expected_type=type_hints["engine"])
+            check_type(argname="argument vpc_id", value=vpc_id, expected_type=type_hints["vpc_id"])
+            check_type(argname="argument allocation_policy", value=allocation_policy, expected_type=type_hints["allocation_policy"])
+            check_type(argname="argument cpu_allocation_ratio", value=cpu_allocation_ratio, expected_type=type_hints["cpu_allocation_ratio"])
+            check_type(argname="argument dedicated_host_group_desc", value=dedicated_host_group_desc, expected_type=type_hints["dedicated_host_group_desc"])
+            check_type(argname="argument disk_allocation_ratio", value=disk_allocation_ratio, expected_type=type_hints["disk_allocation_ratio"])
+            check_type(argname="argument host_replace_policy", value=host_replace_policy, expected_type=type_hints["host_replace_policy"])
+            check_type(argname="argument mem_allocation_ratio", value=mem_allocation_ratio, expected_type=type_hints["mem_allocation_ratio"])
+            check_type(argname="argument open_permission", value=open_permission, expected_type=type_hints["open_permission"])
         self._values: typing.Dict[str, typing.Any] = {
             "engine": engine,
             "vpc_id": vpc_id,
         }
         if allocation_policy is not None:
             self._values["allocation_policy"] = allocation_policy
         if cpu_allocation_ratio is not None:
@@ -1759,15 +1900,15 @@
         v_switch_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         zone_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         auto_renew: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         host_name: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         image_category: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         os_password: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         period: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        tags: typing.Optional[typing.Sequence[RosDedicatedHost.TagsProperty]] = None,
+        tags: typing.Optional[typing.Sequence[typing.Union[RosDedicatedHost.TagsProperty, typing.Dict[str, typing.Any]]]] = None,
         used_time: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::CDDC::DedicatedHost``.
 
         :param dedicated_host_group_id: 
         :param host_class: 
         :param payment_type: 
@@ -1777,14 +1918,28 @@
         :param host_name: 
         :param image_category: 
         :param os_password: 
         :param period: 
         :param tags: 
         :param used_time: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosDedicatedHostProps.__init__)
+            check_type(argname="argument dedicated_host_group_id", value=dedicated_host_group_id, expected_type=type_hints["dedicated_host_group_id"])
+            check_type(argname="argument host_class", value=host_class, expected_type=type_hints["host_class"])
+            check_type(argname="argument payment_type", value=payment_type, expected_type=type_hints["payment_type"])
+            check_type(argname="argument v_switch_id", value=v_switch_id, expected_type=type_hints["v_switch_id"])
+            check_type(argname="argument zone_id", value=zone_id, expected_type=type_hints["zone_id"])
+            check_type(argname="argument auto_renew", value=auto_renew, expected_type=type_hints["auto_renew"])
+            check_type(argname="argument host_name", value=host_name, expected_type=type_hints["host_name"])
+            check_type(argname="argument image_category", value=image_category, expected_type=type_hints["image_category"])
+            check_type(argname="argument os_password", value=os_password, expected_type=type_hints["os_password"])
+            check_type(argname="argument period", value=period, expected_type=type_hints["period"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
+            check_type(argname="argument used_time", value=used_time, expected_type=type_hints["used_time"])
         self._values: typing.Dict[str, typing.Any] = {
             "dedicated_host_group_id": dedicated_host_group_id,
             "host_class": host_class,
             "payment_type": payment_type,
             "v_switch_id": v_switch_id,
             "zone_id": zone_id,
         }
```

### Comparing `ros-cdk-cddc-1.0.8/src/ros_cdk_cddc.egg-info/PKG-INFO` & `ros-cdk-cddc-1.0.9/src/ros_cdk_cddc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-cddc
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS CDDC Construct Library
```

