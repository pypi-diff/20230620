# Comparing `tmp/ros-cdk-cen-1.0.8.tar.gz` & `tmp/ros-cdk-cen-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ros-cdk-cen-1.0.8.tar", last modified: Thu Jul 14 02:32:00 2022, max compression
+gzip compressed data, was "dist/ros-cdk-cen-1.0.9.tar", last modified: Fri Sep 23 10:50:07 2022, max compression
```

## Comparing `ros-cdk-cen-1.0.8.tar` & `ros-cdk-cen-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:32:00.000000 ros-cdk-cen-1.0.8/
--rw-r--r--   0 root         (0) root         (0)    10279 2022-07-14 02:31:59.000000 ros-cdk-cen-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2022-07-14 02:31:59.000000 ros-cdk-cen-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      121 2022-07-14 02:31:59.000000 ros-cdk-cen-1.0.8/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1240 2022-07-14 02:32:00.000000 ros-cdk-cen-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      179 2022-07-14 02:31:59.000000 ros-cdk-cen-1.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)      106 2022-07-14 02:31:59.000000 ros-cdk-cen-1.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-07-14 02:32:00.000000 ros-cdk-cen-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1794 2022-07-14 02:31:59.000000 ros-cdk-cen-1.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:32:00.000000 ros-cdk-cen-1.0.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:32:00.000000 ros-cdk-cen-1.0.8/src/ros_cdk_cen/
--rw-r--r--   0 root         (0) root         (0)   438539 2022-07-14 02:31:59.000000 ros-cdk-cen-1.0.8/src/ros_cdk_cen/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:32:00.000000 ros-cdk-cen-1.0.8/src/ros_cdk_cen/_jsii/
--rw-r--r--   0 root         (0) root         (0)      370 2022-07-14 02:31:59.000000 ros-cdk-cen-1.0.8/src/ros_cdk_cen/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)   132482 2022-07-14 02:31:59.000000 ros-cdk-cen-1.0.8/src/ros_cdk_cen/_jsii/ros-cdk-cen@1.0.8.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:31:59.000000 ros-cdk-cen-1.0.8/src/ros_cdk_cen/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-14 02:32:00.000000 ros-cdk-cen-1.0.8/src/ros_cdk_cen.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1240 2022-07-14 02:32:00.000000 ros-cdk-cen-1.0.8/src/ros_cdk_cen.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      400 2022-07-14 02:32:00.000000 ros-cdk-cen-1.0.8/src/ros_cdk_cen.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-14 02:32:00.000000 ros-cdk-cen-1.0.8/src/ros_cdk_cen.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2022-07-14 02:32:00.000000 ros-cdk-cen-1.0.8/src/ros_cdk_cen.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2022-07-14 02:32:00.000000 ros-cdk-cen-1.0.8/src/ros_cdk_cen.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 10:50:07.000000 ros-cdk-cen-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)    10279 2022-09-23 10:50:07.000000 ros-cdk-cen-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2022-09-23 10:50:07.000000 ros-cdk-cen-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      121 2022-09-23 10:50:07.000000 ros-cdk-cen-1.0.9/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1240 2022-09-23 10:50:07.000000 ros-cdk-cen-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      179 2022-09-23 10:50:07.000000 ros-cdk-cen-1.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      236 2022-09-23 10:50:07.000000 ros-cdk-cen-1.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-09-23 10:50:07.000000 ros-cdk-cen-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1823 2022-09-23 10:50:07.000000 ros-cdk-cen-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 10:50:07.000000 ros-cdk-cen-1.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 10:50:07.000000 ros-cdk-cen-1.0.9/src/ros_cdk_cen/
+-rw-r--r--   0 root         (0) root         (0)   545313 2022-09-23 10:50:07.000000 ros-cdk-cen-1.0.9/src/ros_cdk_cen/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 10:50:07.000000 ros-cdk-cen-1.0.9/src/ros_cdk_cen/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      404 2022-09-23 10:50:07.000000 ros-cdk-cen-1.0.9/src/ros_cdk_cen/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   135316 2022-09-23 10:50:07.000000 ros-cdk-cen-1.0.9/src/ros_cdk_cen/_jsii/ros-cdk-cen@1.0.9.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 10:50:07.000000 ros-cdk-cen-1.0.9/src/ros_cdk_cen/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-23 10:50:07.000000 ros-cdk-cen-1.0.9/src/ros_cdk_cen.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1240 2022-09-23 10:50:07.000000 ros-cdk-cen-1.0.9/src/ros_cdk_cen.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      400 2022-09-23 10:50:07.000000 ros-cdk-cen-1.0.9/src/ros_cdk_cen.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-23 10:50:07.000000 ros-cdk-cen-1.0.9/src/ros_cdk_cen.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2022-09-23 10:50:07.000000 ros-cdk-cen-1.0.9/src/ros_cdk_cen.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2022-09-23 10:50:07.000000 ros-cdk-cen-1.0.9/src/ros_cdk_cen.egg-info/top_level.txt
```

### Comparing `ros-cdk-cen-1.0.8/LICENSE` & `ros-cdk-cen-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ros-cdk-cen-1.0.8/PKG-INFO` & `ros-cdk-cen-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-cen
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS CEN Construct Library
```

### Comparing `ros-cdk-cen-1.0.8/setup.py` & `ros-cdk-cen-1.0.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "ros-cdk-cen",
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
         "ros_cdk_cen",
         "ros_cdk_cen._jsii"
     ],
     "package_data": {
         "ros_cdk_cen._jsii": [
-            "ros-cdk-cen@1.0.8.jsii.tgz"
+            "ros-cdk-cen@1.0.9.jsii.tgz"
         ],
         "ros_cdk_cen": [
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

### Comparing `ros-cdk-cen-1.0.8/src/ros_cdk_cen/__init__.py` & `ros-cdk-cen-1.0.9/src/ros_cdk_cen/__init__.py`

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
 
 
 class CenBandwidthLimit(
     ros_cdk_core.Resource,
@@ -29,28 +31,34 @@
 ):
     '''A ROS resource type:  ``ALIYUN::CEN::CenBandwidthLimit``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "CenBandwidthLimitProps",
+        props: typing.Union["CenBandwidthLimitProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::CEN::CenBandwidthLimit``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(CenBandwidthLimit.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-cen.CenBandwidthLimitProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -72,14 +80,20 @@
         '''Properties for defining a ``ALIYUN::CEN::CenBandwidthLimit``.
 
         :param bandwidth_limit: Property bandwidthLimit: The bandwidth configured for the interconnected regions communication. Minimal value: 1
         :param cen_id: Property cenId: The ID of the CEN instance.
         :param local_region_id: Property localRegionId: The ID of the local region.
         :param opposite_region_id: Property oppositeRegionId: The ID of the other interconnected region.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(CenBandwidthLimitProps.__init__)
+            check_type(argname="argument bandwidth_limit", value=bandwidth_limit, expected_type=type_hints["bandwidth_limit"])
+            check_type(argname="argument cen_id", value=cen_id, expected_type=type_hints["cen_id"])
+            check_type(argname="argument local_region_id", value=local_region_id, expected_type=type_hints["local_region_id"])
+            check_type(argname="argument opposite_region_id", value=opposite_region_id, expected_type=type_hints["opposite_region_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "bandwidth_limit": bandwidth_limit,
             "cen_id": cen_id,
             "local_region_id": local_region_id,
             "opposite_region_id": opposite_region_id,
         }
 
@@ -135,31 +149,37 @@
 ):
     '''A ROS resource type:  ``ALIYUN::CEN::CenBandwidthPackage``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "CenBandwidthPackageProps",
+        props: typing.Union["CenBandwidthPackageProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::CEN::CenBandwidthPackage``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(CenBandwidthPackage.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrCenBandwidthPackageId")
     def attr_cen_bandwidth_package_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute CenBandwidthPackageId: The ID of the bandwidth package.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrCenBandwidthPackageId"))
 
 
 class CenBandwidthPackageAssociation(
@@ -169,28 +189,34 @@
 ):
     '''A ROS resource type:  ``ALIYUN::CEN::CenBandwidthPackageAssociation``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "CenBandwidthPackageAssociationProps",
+        props: typing.Union["CenBandwidthPackageAssociationProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::CEN::CenBandwidthPackageAssociation``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(CenBandwidthPackageAssociation.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-cen.CenBandwidthPackageAssociationProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -206,14 +232,18 @@
         cen_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
         '''Properties for defining a ``ALIYUN::CEN::CenBandwidthPackageAssociation``.
 
         :param cen_bandwidth_package_id: Property cenBandwidthPackageId: The ID of the bandwidth package.
         :param cen_id: Property cenId: The ID of the CEN instance.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(CenBandwidthPackageAssociationProps.__init__)
+            check_type(argname="argument cen_bandwidth_package_id", value=cen_bandwidth_package_id, expected_type=type_hints["cen_bandwidth_package_id"])
+            check_type(argname="argument cen_id", value=cen_id, expected_type=type_hints["cen_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "cen_bandwidth_package_id": cen_bandwidth_package_id,
             "cen_id": cen_id,
         }
 
     @builtins.property
     def cen_bandwidth_package_id(
@@ -289,14 +319,28 @@
         :param bandwidth_package_charge_type: Property bandwidthPackageChargeType: The billing method. Valid value: PREPAY, POSTPAY (Default)
         :param description: Property description: The description of the bandwidth package. The description can contain [2,256] characters, numbers, underscores, and hyphens, and the name must start with English letters, but cannot start with http:// or https://.
         :param name: Property name: The name of the bandwidth package. The name can contain 2-128 characters including a-z, A-Z, 0-9, periods, underlines, and hyphens. It must start with English letters, but cannot start with http:// or https://.
         :param period: Property period: The purchase period. The default value is 1.
         :param pricing_cycle: Property pricingCycle: The pricing cycle.
         :param resource_group_id: Property resourceGroupId: Resource group id.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(CenBandwidthPackageProps.__init__)
+            check_type(argname="argument bandwidth", value=bandwidth, expected_type=type_hints["bandwidth"])
+            check_type(argname="argument geographic_region_a_id", value=geographic_region_a_id, expected_type=type_hints["geographic_region_a_id"])
+            check_type(argname="argument geographic_region_b_id", value=geographic_region_b_id, expected_type=type_hints["geographic_region_b_id"])
+            check_type(argname="argument auto_pay", value=auto_pay, expected_type=type_hints["auto_pay"])
+            check_type(argname="argument auto_renew", value=auto_renew, expected_type=type_hints["auto_renew"])
+            check_type(argname="argument auto_renew_duration", value=auto_renew_duration, expected_type=type_hints["auto_renew_duration"])
+            check_type(argname="argument bandwidth_package_charge_type", value=bandwidth_package_charge_type, expected_type=type_hints["bandwidth_package_charge_type"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+            check_type(argname="argument period", value=period, expected_type=type_hints["period"])
+            check_type(argname="argument pricing_cycle", value=pricing_cycle, expected_type=type_hints["pricing_cycle"])
+            check_type(argname="argument resource_group_id", value=resource_group_id, expected_type=type_hints["resource_group_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "bandwidth": bandwidth,
             "geographic_region_a_id": geographic_region_a_id,
             "geographic_region_b_id": geographic_region_b_id,
         }
         if auto_pay is not None:
             self._values["auto_pay"] = auto_pay
@@ -465,31 +509,37 @@
 ):
     '''A ROS resource type:  ``ALIYUN::CEN::CenInstance``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: typing.Optional["CenInstanceProps"] = None,
+        props: typing.Optional[typing.Union["CenInstanceProps", typing.Dict[str, typing.Any]]] = None,
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::CEN::CenInstance``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(CenInstance.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrCenId")
     def attr_cen_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute CenId: The ID of the request.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrCenId"))
 
 
 class CenInstanceAttachment(
@@ -499,28 +549,34 @@
 ):
     '''A ROS resource type:  ``ALIYUN::CEN::CenInstanceAttachment``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "CenInstanceAttachmentProps",
+        props: typing.Union["CenInstanceAttachmentProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::CEN::CenInstanceAttachment``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(CenInstanceAttachment.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-cen.CenInstanceAttachmentProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -545,14 +601,21 @@
 
         :param cen_id: Property cenId: The ID of the CEN instance.
         :param child_instance_id: Property childInstanceId: The ID of the network to attach.
         :param child_instance_region_id: Property childInstanceRegionId: The ID of the region where the network is located. The ID of the region where the network is located.
         :param child_instance_type: Property childInstanceType: The type of the network to attach. Support VPC, VBR or CCN.
         :param child_instance_owner_id: Property childInstanceOwnerId: The account ID to which the network belongs.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(CenInstanceAttachmentProps.__init__)
+            check_type(argname="argument cen_id", value=cen_id, expected_type=type_hints["cen_id"])
+            check_type(argname="argument child_instance_id", value=child_instance_id, expected_type=type_hints["child_instance_id"])
+            check_type(argname="argument child_instance_region_id", value=child_instance_region_id, expected_type=type_hints["child_instance_region_id"])
+            check_type(argname="argument child_instance_type", value=child_instance_type, expected_type=type_hints["child_instance_type"])
+            check_type(argname="argument child_instance_owner_id", value=child_instance_owner_id, expected_type=type_hints["child_instance_owner_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "cen_id": cen_id,
             "child_instance_id": child_instance_id,
             "child_instance_region_id": child_instance_region_id,
             "child_instance_type": child_instance_type,
         }
         if child_instance_owner_id is not None:
@@ -631,24 +694,31 @@
     def __init__(
         self,
         *,
         description: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         name: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         protection_level: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         resource_group_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        tags: typing.Optional[typing.Sequence["RosCenInstance.TagsProperty"]] = None,
+        tags: typing.Optional[typing.Sequence[typing.Union["RosCenInstance.TagsProperty", typing.Dict[str, typing.Any]]]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::CEN::CenInstance``.
 
         :param description: Property description: The description of the instance. The name can be 2-256 characters in length. It can start with an uppercase letter, lowercase letter, or Chinese character. It can contain numbers, underscores (_), and hyphens (-), but cannot start with http:// or https://.
         :param name: Property name: The name of the instance. The name can be 2-128 characters in length. It can start with an uppercase letter, lowercase letter, or Chinese character. It can contain numbers, underscores (_), and hyphens (-), but cannot start with http:// or https://.
         :param protection_level: Property protectionLevel: The level of CIDR block overlapping. Set the value to REDUCED. REDUCED indicates that the CIDR blocks can overlap with each other but must not be the same.
         :param resource_group_id: Property resourceGroupId: Resource group id.
         :param tags: Property tags: Tags to attach to instance. Max support 20 tags to add during create instance. Each tag with two properties Key and Value, and Key is required.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(CenInstanceProps.__init__)
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+            check_type(argname="argument protection_level", value=protection_level, expected_type=type_hints["protection_level"])
+            check_type(argname="argument resource_group_id", value=resource_group_id, expected_type=type_hints["resource_group_id"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
         self._values: typing.Dict[str, typing.Any] = {}
         if description is not None:
             self._values["description"] = description
         if name is not None:
             self._values["name"] = name
         if protection_level is not None:
             self._values["protection_level"] = protection_level
@@ -727,31 +797,37 @@
 ):
     '''A ROS resource type:  ``ALIYUN::CEN::CenRouteMap``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "CenRouteMapProps",
+        props: typing.Union["CenRouteMapProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::CEN::CenRouteMap``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(CenRouteMap.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrRouteMapId")
     def attr_route_map_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute RouteMapId: The ID of the route map.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrRouteMapId"))
 
 
 @jsii.data_type(
@@ -845,14 +921,43 @@
         :param route_types: Property routeTypes: Match statements are used to match the route types. Valid values: System: system routes that are generated by the system. Custom: custom routes that are created by users. BGP: Border Gateway Protocol (BGP) routes that are advertised to BGP. You can enter multiple types.
         :param source_child_instance_types: Property sourceChildInstanceTypes: Match statements are used to match source instance types of the routes. Valid values: VPC: VPCs. VBR: VBRs. CCN: CCN instances in mainland China.
         :param source_instance_ids: Property sourceInstanceIds: Match statements are used to match source instance IDs of the routes. You can enter instance IDs of the following types: virtual private cloud (VPC), virtual border router (VBR), Cloud Connect Network (CCN) in mainland China, Smart Access Gateway (SAG). You can enter at most 32 instance IDs.
         :param source_instance_ids_reverse_match: Property sourceInstanceIdsReverseMatch: The IDs of source instances to be advertised do not support match statements. Valid values: false (default value): If the source instance ID is in the SourceInstanceIds field, the match is successful. true: If the source instance ID is not in the SourceInstanceIds field, the match is successful.
         :param source_region_ids: Property sourceRegionIds: Match statements are used to match source region IDs of the routes. You can enter at most 32 region IDs.
         :param source_route_table_ids: Property sourceRouteTableIds: Match statements are used to match source route table IDs of the routes. You can enter at most 32 route table IDs.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(CenRouteMapProps.__init__)
+            check_type(argname="argument cen_id", value=cen_id, expected_type=type_hints["cen_id"])
+            check_type(argname="argument cen_region_id", value=cen_region_id, expected_type=type_hints["cen_region_id"])
+            check_type(argname="argument map_result", value=map_result, expected_type=type_hints["map_result"])
+            check_type(argname="argument priority", value=priority, expected_type=type_hints["priority"])
+            check_type(argname="argument transmit_direction", value=transmit_direction, expected_type=type_hints["transmit_direction"])
+            check_type(argname="argument as_path_match_mode", value=as_path_match_mode, expected_type=type_hints["as_path_match_mode"])
+            check_type(argname="argument cidr_match_mode", value=cidr_match_mode, expected_type=type_hints["cidr_match_mode"])
+            check_type(argname="argument community_match_mode", value=community_match_mode, expected_type=type_hints["community_match_mode"])
+            check_type(argname="argument community_operate_mode", value=community_operate_mode, expected_type=type_hints["community_operate_mode"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument destination_child_instance_types", value=destination_child_instance_types, expected_type=type_hints["destination_child_instance_types"])
+            check_type(argname="argument destination_cidr_blocks", value=destination_cidr_blocks, expected_type=type_hints["destination_cidr_blocks"])
+            check_type(argname="argument destination_instance_ids", value=destination_instance_ids, expected_type=type_hints["destination_instance_ids"])
+            check_type(argname="argument destination_instance_ids_reverse_match", value=destination_instance_ids_reverse_match, expected_type=type_hints["destination_instance_ids_reverse_match"])
+            check_type(argname="argument destination_route_table_ids", value=destination_route_table_ids, expected_type=type_hints["destination_route_table_ids"])
+            check_type(argname="argument match_asns", value=match_asns, expected_type=type_hints["match_asns"])
+            check_type(argname="argument match_community_set", value=match_community_set, expected_type=type_hints["match_community_set"])
+            check_type(argname="argument next_priority", value=next_priority, expected_type=type_hints["next_priority"])
+            check_type(argname="argument operate_community_set", value=operate_community_set, expected_type=type_hints["operate_community_set"])
+            check_type(argname="argument preference", value=preference, expected_type=type_hints["preference"])
+            check_type(argname="argument prepend_as_path", value=prepend_as_path, expected_type=type_hints["prepend_as_path"])
+            check_type(argname="argument route_types", value=route_types, expected_type=type_hints["route_types"])
+            check_type(argname="argument source_child_instance_types", value=source_child_instance_types, expected_type=type_hints["source_child_instance_types"])
+            check_type(argname="argument source_instance_ids", value=source_instance_ids, expected_type=type_hints["source_instance_ids"])
+            check_type(argname="argument source_instance_ids_reverse_match", value=source_instance_ids_reverse_match, expected_type=type_hints["source_instance_ids_reverse_match"])
+            check_type(argname="argument source_region_ids", value=source_region_ids, expected_type=type_hints["source_region_ids"])
+            check_type(argname="argument source_route_table_ids", value=source_route_table_ids, expected_type=type_hints["source_route_table_ids"])
         self._values: typing.Dict[str, typing.Any] = {
             "cen_id": cen_id,
             "cen_region_id": cen_region_id,
             "map_result": map_result,
             "priority": priority,
             "transmit_direction": transmit_direction,
         }
@@ -1251,31 +1356,37 @@
 ):
     '''A ROS resource type:  ``ALIYUN::CEN::CenRouteService``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "CenRouteServiceProps",
+        props: typing.Union["CenRouteServiceProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::CEN::CenRouteService``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(CenRouteService.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrId")
     def attr_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute Id: The ID of the cloud service.
 
         It is formatted to {CenId}/{HostRegionId}/{Host}/{AccessRegionId}
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrId"))
@@ -1312,14 +1423,23 @@
         :param cen_id: Property cenId: The ID of the Cloud Enterprise Network (CEN) instance.
         :param host: Property host: The domain or IP address of the cloud service.
         :param host_region_id: Property hostRegionId: The region where the cloud service is deployed. You can call the DescribeRegions operation to query region IDs. Note The HostRegionId and AccessRegionIds.N must be set to the same value.
         :param host_vpc_id: Property hostVpcId: The virtual private cloud (VPC) that is associated with the cloud service.
         :param conflict_ignore: Property conflictIgnore: Whether to ignore conflict when creating. If true, when the CloudRoute.Conflict error code is encountered during creation, it will be ignored as the creation is successful, and the deletion phase will be skipped. Default false.
         :param description: Property description: The description of the cloud service.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(CenRouteServiceProps.__init__)
+            check_type(argname="argument access_region_id", value=access_region_id, expected_type=type_hints["access_region_id"])
+            check_type(argname="argument cen_id", value=cen_id, expected_type=type_hints["cen_id"])
+            check_type(argname="argument host", value=host, expected_type=type_hints["host"])
+            check_type(argname="argument host_region_id", value=host_region_id, expected_type=type_hints["host_region_id"])
+            check_type(argname="argument host_vpc_id", value=host_vpc_id, expected_type=type_hints["host_vpc_id"])
+            check_type(argname="argument conflict_ignore", value=conflict_ignore, expected_type=type_hints["conflict_ignore"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
         self._values: typing.Dict[str, typing.Any] = {
             "access_region_id": access_region_id,
             "cen_id": cen_id,
             "host": host,
             "host_region_id": host_region_id,
             "host_vpc_id": host_vpc_id,
         }
@@ -1406,85 +1526,91 @@
 ):
     '''A ROS resource type:  ``ALIYUN::CEN::CenVbrHealthCheck``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "CenVbrHealthCheckProps",
+        props: typing.Union["CenVbrHealthCheckProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::CEN::CenVbrHealthCheck``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(CenVbrHealthCheck.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrCenId")
     def attr_cen_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute CenId: The ID of the CEN instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrCenId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrHealthCheckInterval")
     def attr_health_check_interval(self) -> ros_cdk_core.IResolvable:
         '''Attribute HealthCheckInterval: Specifies the time interval at which probe packets are sent during the health check.
 
         Default value: 2. Valid values: 2 to 3.  Unit: second.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrHealthCheckInterval"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrHealthCheckSourceIp")
     def attr_health_check_source_ip(self) -> ros_cdk_core.IResolvable:
         '''Attribute HealthCheckSourceIp: You can use either of the following methods to specify the source IP address of the health check.
 
         Automatic IP Address: The system automatically assigns an IP address within the CIDR block 100.96.0.0/16 (recommended).  Custom IP Address: You can specify a source IP address that is available within the CIDR block 10.0.0.0/8, 192.168.0.0/16, or 172.16.0.0/12. The specified source IP address must not overlap with the IP addresses of the Alibaba Cloud-facing and client-facing interfaces on the VBR instance, or the IP addresses of the instances with which the VBR instance needs to communicate in the CEN.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrHealthCheckSourceIp"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrHealthCheckTargetIp")
     def attr_health_check_target_ip(self) -> ros_cdk_core.IResolvable:
         '''Attribute HealthCheckTargetIp: Specifies the destination IP address of the health check.
 
         The destination IP address is the IP address of the client-facing interface on the VBR instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrHealthCheckTargetIp"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrHealthyThreshold")
     def attr_healthy_threshold(self) -> ros_cdk_core.IResolvable:
         '''Attribute HealthyThreshold: Specifies the number of probe packets to be sent during the health check.
 
         Default value: 8. Valid values: 3 to 8.  Unit: packet.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrHealthyThreshold"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVbrInstanceId")
     def attr_vbr_instance_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute VbrInstanceId: The ID of the VBR instance.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVbrInstanceId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVbrInstanceOwnerId")
     def attr_vbr_instance_owner_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute VbrInstanceOwnerId: The User ID (UID) of the account to which the VBR instance belongs.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVbrInstanceOwnerId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVbrInstanceRegionId")
     def attr_vbr_instance_region_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute VbrInstanceRegionId: The ID of the region where the VBR instance is deployed.
 
         You can call the DescribeRegionsoperation to query region IDs.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVbrInstanceRegionId"))
@@ -1524,14 +1650,24 @@
         :param vbr_instance_id: Property vbrInstanceId: The ID of the VBR instance.
         :param vbr_instance_region_id: Property vbrInstanceRegionId: The ID of the region where the VBR instance is deployed. You can call the DescribeRegionsoperation to query region IDs.
         :param health_check_interval: Property healthCheckInterval: Specifies the time interval at which probe packets are sent during the health check. Default value: 2. Valid values: 2 to 3. Unit: second.
         :param health_check_source_ip: Property healthCheckSourceIp: You can use either of the following methods to specify the source IP address of the health check. Automatic IP Address: The system automatically assigns an IP address within the CIDR block 100.96.0.0/16 (recommended). Custom IP Address: You can specify a source IP address that is available within the CIDR block 10.0.0.0/8, 192.168.0.0/16, or 172.16.0.0/12. The specified source IP address must not overlap with the IP addresses of the Alibaba Cloud-facing and client-facing interfaces on the VBR instance, or the IP addresses of the instances with which the VBR instance needs to communicate in the CEN.
         :param healthy_threshold: Property healthyThreshold: Specifies the number of probe packets to be sent during the health check. Default value: 8. Valid values: 3 to 8. Unit: packet.
         :param vbr_instance_owner_id: Property vbrInstanceOwnerId: The User ID (UID) of the account to which the VBR instance belongs.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(CenVbrHealthCheckProps.__init__)
+            check_type(argname="argument cen_id", value=cen_id, expected_type=type_hints["cen_id"])
+            check_type(argname="argument health_check_target_ip", value=health_check_target_ip, expected_type=type_hints["health_check_target_ip"])
+            check_type(argname="argument vbr_instance_id", value=vbr_instance_id, expected_type=type_hints["vbr_instance_id"])
+            check_type(argname="argument vbr_instance_region_id", value=vbr_instance_region_id, expected_type=type_hints["vbr_instance_region_id"])
+            check_type(argname="argument health_check_interval", value=health_check_interval, expected_type=type_hints["health_check_interval"])
+            check_type(argname="argument health_check_source_ip", value=health_check_source_ip, expected_type=type_hints["health_check_source_ip"])
+            check_type(argname="argument healthy_threshold", value=healthy_threshold, expected_type=type_hints["healthy_threshold"])
+            check_type(argname="argument vbr_instance_owner_id", value=vbr_instance_owner_id, expected_type=type_hints["vbr_instance_owner_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "cen_id": cen_id,
             "health_check_target_ip": health_check_target_ip,
             "vbr_instance_id": vbr_instance_id,
             "vbr_instance_region_id": vbr_instance_region_id,
         }
         if health_check_interval is not None:
@@ -1630,128 +1766,293 @@
 
     def __repr__(self) -> str:
         return "CenVbrHealthCheckProps(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
+class ChildInstanceRouteEntryToAttachment(
+    ros_cdk_core.Resource,
+    metaclass=jsii.JSIIMeta,
+    jsii_type="@alicloud/ros-cdk-cen.ChildInstanceRouteEntryToAttachment",
+):
+    '''A ROS resource type:  ``ALIYUN::CEN::ChildInstanceRouteEntryToAttachment``.'''
+
+    def __init__(
+        self,
+        scope: ros_cdk_core.Construct,
+        id: builtins.str,
+        props: typing.Union["ChildInstanceRouteEntryToAttachmentProps", typing.Dict[str, typing.Any]],
+        enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
+    ) -> None:
+        '''Create a new ``ALIYUN::CEN::ChildInstanceRouteEntryToAttachment``.
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
+            type_hints = typing.get_type_hints(ChildInstanceRouteEntryToAttachment.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
+        jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
+
+    @builtins.property
+    @jsii.member(jsii_name="attrCenId")
+    def attr_cen_id(self) -> ros_cdk_core.IResolvable:
+        '''Attribute CenId: The ID of the CEN instance.'''
+        return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrCenId"))
+
+    @builtins.property
+    @jsii.member(jsii_name="attrDestinationCidrBlock")
+    def attr_destination_cidr_block(self) -> ros_cdk_core.IResolvable:
+        '''Attribute DestinationCidrBlock: The destination CIDR block of the route.'''
+        return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDestinationCidrBlock"))
+
+    @builtins.property
+    @jsii.member(jsii_name="attrRouteTableId")
+    def attr_route_table_id(self) -> ros_cdk_core.IResolvable:
+        '''Attribute RouteTableId: The ID of the route table configured on the network instance.'''
+        return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrRouteTableId"))
+
+    @builtins.property
+    @jsii.member(jsii_name="attrTransitRouterAttachmentId")
+    def attr_transit_router_attachment_id(self) -> ros_cdk_core.IResolvable:
+        '''Attribute TransitRouterAttachmentId: The ID of the network instance connection.'''
+        return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTransitRouterAttachmentId"))
+
+
+@jsii.data_type(
+    jsii_type="@alicloud/ros-cdk-cen.ChildInstanceRouteEntryToAttachmentProps",
+    jsii_struct_bases=[],
+    name_mapping={
+        "cen_id": "cenId",
+        "destination_cidr_block": "destinationCidrBlock",
+        "route_table_id": "routeTableId",
+        "transit_router_attachment_id": "transitRouterAttachmentId",
+    },
+)
+class ChildInstanceRouteEntryToAttachmentProps:
+    def __init__(
+        self,
+        *,
+        cen_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
+        destination_cidr_block: typing.Union[builtins.str, ros_cdk_core.IResolvable],
+        route_table_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
+        transit_router_attachment_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
+    ) -> None:
+        '''Properties for defining a ``ALIYUN::CEN::ChildInstanceRouteEntryToAttachment``.
+
+        :param cen_id: Property cenId: The ID of the CEN instance.
+        :param destination_cidr_block: Property destinationCidrBlock: The destination CIDR block of the route.
+        :param route_table_id: Property routeTableId: The ID of the route table configured on the network instance.
+        :param transit_router_attachment_id: Property transitRouterAttachmentId: The ID of the network instance connection.
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(ChildInstanceRouteEntryToAttachmentProps.__init__)
+            check_type(argname="argument cen_id", value=cen_id, expected_type=type_hints["cen_id"])
+            check_type(argname="argument destination_cidr_block", value=destination_cidr_block, expected_type=type_hints["destination_cidr_block"])
+            check_type(argname="argument route_table_id", value=route_table_id, expected_type=type_hints["route_table_id"])
+            check_type(argname="argument transit_router_attachment_id", value=transit_router_attachment_id, expected_type=type_hints["transit_router_attachment_id"])
+        self._values: typing.Dict[str, typing.Any] = {
+            "cen_id": cen_id,
+            "destination_cidr_block": destination_cidr_block,
+            "route_table_id": route_table_id,
+            "transit_router_attachment_id": transit_router_attachment_id,
+        }
+
+    @builtins.property
+    def cen_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
+        '''Property cenId: The ID of the CEN instance.'''
+        result = self._values.get("cen_id")
+        assert result is not None, "Required property 'cen_id' is missing"
+        return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], result)
+
+    @builtins.property
+    def destination_cidr_block(
+        self,
+    ) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
+        '''Property destinationCidrBlock: The destination CIDR block of the route.'''
+        result = self._values.get("destination_cidr_block")
+        assert result is not None, "Required property 'destination_cidr_block' is missing"
+        return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], result)
+
+    @builtins.property
+    def route_table_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
+        '''Property routeTableId: The ID of the route table configured on the network instance.'''
+        result = self._values.get("route_table_id")
+        assert result is not None, "Required property 'route_table_id' is missing"
+        return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], result)
+
+    @builtins.property
+    def transit_router_attachment_id(
+        self,
+    ) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
+        '''Property transitRouterAttachmentId: The ID of the network instance connection.'''
+        result = self._values.get("transit_router_attachment_id")
+        assert result is not None, "Required property 'transit_router_attachment_id' is missing"
+        return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], result)
+
+    def __eq__(self, rhs: typing.Any) -> builtins.bool:
+        return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+    def __ne__(self, rhs: typing.Any) -> builtins.bool:
+        return not (rhs == self)
+
+    def __repr__(self) -> str:
+        return "ChildInstanceRouteEntryToAttachmentProps(%s)" % ", ".join(
+            k + "=" + repr(v) for k, v in self._values.items()
+        )
+
+
 class RosCenBandwidthLimit(
     ros_cdk_core.RosResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@alicloud/ros-cdk-cen.RosCenBandwidthLimit",
 ):
     '''A ROS template type:  ``ALIYUN::CEN::CenBandwidthLimit``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosCenBandwidthLimitProps",
+        props: typing.Union["RosCenBandwidthLimitProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::CEN::CenBandwidthLimit``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosCenBandwidthLimit.__init__)
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
+            type_hints = typing.get_type_hints(RosCenBandwidthLimit._render_properties)
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
     @jsii.member(jsii_name="bandwidthLimit")
     def bandwidth_limit(self) -> typing.Union[jsii.Number, ros_cdk_core.IResolvable]:
         '''
         :Property: bandwidthLimit: The bandwidth configured for the interconnected regions communication. Minimal value: 1
         '''
         return typing.cast(typing.Union[jsii.Number, ros_cdk_core.IResolvable], jsii.get(self, "bandwidthLimit"))
 
     @bandwidth_limit.setter
     def bandwidth_limit(
         self,
         value: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCenBandwidthLimit, "bandwidth_limit").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "bandwidthLimit", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="cenId")
     def cen_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: cenId: The ID of the CEN instance.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "cenId"))
 
     @cen_id.setter
     def cen_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCenBandwidthLimit, "cen_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "cenId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         '''A factory method that creates a new instance of this class from an object containing the properties of this ROS resource.'''
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCenBandwidthLimit, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="localRegionId")
     def local_region_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: localRegionId: The ID of the local region.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "localRegionId"))
 
     @local_region_id.setter
     def local_region_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCenBandwidthLimit, "local_region_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "localRegionId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="oppositeRegionId")
     def opposite_region_id(
         self,
     ) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: oppositeRegionId: The ID of the other interconnected region.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "oppositeRegionId"))
 
     @opposite_region_id.setter
     def opposite_region_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCenBandwidthLimit, "opposite_region_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "oppositeRegionId", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-cen.RosCenBandwidthLimitProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -1773,14 +2074,20 @@
         '''Properties for defining a ``ALIYUN::CEN::CenBandwidthLimit``.
 
         :param bandwidth_limit: 
         :param cen_id: 
         :param local_region_id: 
         :param opposite_region_id: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosCenBandwidthLimitProps.__init__)
+            check_type(argname="argument bandwidth_limit", value=bandwidth_limit, expected_type=type_hints["bandwidth_limit"])
+            check_type(argname="argument cen_id", value=cen_id, expected_type=type_hints["cen_id"])
+            check_type(argname="argument local_region_id", value=local_region_id, expected_type=type_hints["local_region_id"])
+            check_type(argname="argument opposite_region_id", value=opposite_region_id, expected_type=type_hints["opposite_region_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "bandwidth_limit": bandwidth_limit,
             "cen_id": cen_id,
             "local_region_id": local_region_id,
             "opposite_region_id": opposite_region_id,
         }
 
@@ -1841,80 +2148,95 @@
 ):
     '''A ROS template type:  ``ALIYUN::CEN::CenBandwidthPackage``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosCenBandwidthPackageProps",
+        props: typing.Union["RosCenBandwidthPackageProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::CEN::CenBandwidthPackage``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosCenBandwidthPackage.__init__)
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
+            type_hints = typing.get_type_hints(RosCenBandwidthPackage._render_properties)
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
     @jsii.member(jsii_name="attrCenBandwidthPackageId")
     def attr_cen_bandwidth_package_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: CenBandwidthPackageId: The ID of the bandwidth package.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrCenBandwidthPackageId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="bandwidth")
     def bandwidth(self) -> typing.Union[jsii.Number, ros_cdk_core.IResolvable]:
         '''
         :Property: bandwidth: The bandwidth in Mbps of the bandwidth package. The bandwidth cannot be less than 2 Mbps.
         '''
         return typing.cast(typing.Union[jsii.Number, ros_cdk_core.IResolvable], jsii.get(self, "bandwidth"))
 
     @bandwidth.setter
     def bandwidth(
         self,
         value: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCenBandwidthPackage, "bandwidth").fset)
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
+            type_hints = typing.get_type_hints(getattr(RosCenBandwidthPackage, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="geographicRegionAId")
     def geographic_region_a_id(
         self,
     ) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
@@ -1924,17 +2246,20 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "geographicRegionAId"))
 
     @geographic_region_a_id.setter
     def geographic_region_a_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCenBandwidthPackage, "geographic_region_a_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "geographicRegionAId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="geographicRegionBId")
     def geographic_region_b_id(
         self,
     ) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
@@ -1944,17 +2269,20 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "geographicRegionBId"))
 
     @geographic_region_b_id.setter
     def geographic_region_b_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCenBandwidthPackage, "geographic_region_b_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "geographicRegionBId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="autoPay")
     def auto_pay(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -1965,68 +2293,80 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "autoPay"))
 
     @auto_pay.setter
     def auto_pay(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCenBandwidthPackage, "auto_pay").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "autoPay", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="autoRenew")
     def auto_renew(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property: autoRenew: Indicates whether automatic renewal is enabled. Valid values:true: Automatic renewal is enabled.false: Automatic renewal is not enabled. You must renew the instance manually.Default value: false.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "autoRenew"))
 
     @auto_renew.setter
     def auto_renew(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCenBandwidthPackage, "auto_renew").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "autoRenew", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="autoRenewDuration")
     def auto_renew_duration(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: autoRenewDuration: Duration of each automatic renewals. It takes effect when AutoRenew is true.
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "autoRenewDuration"))
 
     @auto_renew_duration.setter
     def auto_renew_duration(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCenBandwidthPackage, "auto_renew_duration").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "autoRenewDuration", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="bandwidthPackageChargeType")
     def bandwidth_package_charge_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: bandwidthPackageChargeType: The billing method. Valid value: PREPAY, POSTPAY (Default)
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "bandwidthPackageChargeType"))
 
     @bandwidth_package_charge_type.setter
     def bandwidth_package_charge_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCenBandwidthPackage, "bandwidth_package_charge_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "bandwidthPackageChargeType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="description")
     def description(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -2036,17 +2376,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "description"))
 
     @description.setter
     def description(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCenBandwidthPackage, "description").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "description", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="name")
     def name(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -2056,152 +2399,182 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "name"))
 
     @name.setter
     def name(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCenBandwidthPackage, "name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "name", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="period")
     def period(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: period: The purchase period. The default value is 1.
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "period"))
 
     @period.setter
     def period(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCenBandwidthPackage, "period").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "period", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="pricingCycle")
     def pricing_cycle(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: pricingCycle: The pricing cycle.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "pricingCycle"))
 
     @pricing_cycle.setter
     def pricing_cycle(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCenBandwidthPackage, "pricing_cycle").fset)
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
+            type_hints = typing.get_type_hints(getattr(RosCenBandwidthPackage, "resource_group_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "resourceGroupId", value)
 
 
 class RosCenBandwidthPackageAssociation(
     ros_cdk_core.RosResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@alicloud/ros-cdk-cen.RosCenBandwidthPackageAssociation",
 ):
     '''A ROS template type:  ``ALIYUN::CEN::CenBandwidthPackageAssociation``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosCenBandwidthPackageAssociationProps",
+        props: typing.Union["RosCenBandwidthPackageAssociationProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::CEN::CenBandwidthPackageAssociation``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosCenBandwidthPackageAssociation.__init__)
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
+            type_hints = typing.get_type_hints(RosCenBandwidthPackageAssociation._render_properties)
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
     @jsii.member(jsii_name="cenBandwidthPackageId")
     def cen_bandwidth_package_id(
         self,
     ) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: cenBandwidthPackageId: The ID of the bandwidth package.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "cenBandwidthPackageId"))
 
     @cen_bandwidth_package_id.setter
     def cen_bandwidth_package_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCenBandwidthPackageAssociation, "cen_bandwidth_package_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "cenBandwidthPackageId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="cenId")
     def cen_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: cenId: The ID of the CEN instance.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "cenId"))
 
     @cen_id.setter
     def cen_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCenBandwidthPackageAssociation, "cen_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "cenId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         '''A factory method that creates a new instance of this class from an object containing the properties of this ROS resource.'''
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCenBandwidthPackageAssociation, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-cen.RosCenBandwidthPackageAssociationProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -2217,14 +2590,18 @@
         cen_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
         '''Properties for defining a ``ALIYUN::CEN::CenBandwidthPackageAssociation``.
 
         :param cen_bandwidth_package_id: 
         :param cen_id: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosCenBandwidthPackageAssociationProps.__init__)
+            check_type(argname="argument cen_bandwidth_package_id", value=cen_bandwidth_package_id, expected_type=type_hints["cen_bandwidth_package_id"])
+            check_type(argname="argument cen_id", value=cen_id, expected_type=type_hints["cen_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "cen_bandwidth_package_id": cen_bandwidth_package_id,
             "cen_id": cen_id,
         }
 
     @builtins.property
     def cen_bandwidth_package_id(
@@ -2304,14 +2681,28 @@
         :param bandwidth_package_charge_type: 
         :param description: 
         :param name: 
         :param period: 
         :param pricing_cycle: 
         :param resource_group_id: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosCenBandwidthPackageProps.__init__)
+            check_type(argname="argument bandwidth", value=bandwidth, expected_type=type_hints["bandwidth"])
+            check_type(argname="argument geographic_region_a_id", value=geographic_region_a_id, expected_type=type_hints["geographic_region_a_id"])
+            check_type(argname="argument geographic_region_b_id", value=geographic_region_b_id, expected_type=type_hints["geographic_region_b_id"])
+            check_type(argname="argument auto_pay", value=auto_pay, expected_type=type_hints["auto_pay"])
+            check_type(argname="argument auto_renew", value=auto_renew, expected_type=type_hints["auto_renew"])
+            check_type(argname="argument auto_renew_duration", value=auto_renew_duration, expected_type=type_hints["auto_renew_duration"])
+            check_type(argname="argument bandwidth_package_charge_type", value=bandwidth_package_charge_type, expected_type=type_hints["bandwidth_package_charge_type"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+            check_type(argname="argument period", value=period, expected_type=type_hints["period"])
+            check_type(argname="argument pricing_cycle", value=pricing_cycle, expected_type=type_hints["pricing_cycle"])
+            check_type(argname="argument resource_group_id", value=resource_group_id, expected_type=type_hints["resource_group_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "bandwidth": bandwidth,
             "geographic_region_a_id": geographic_region_a_id,
             "geographic_region_b_id": geographic_region_b_id,
         }
         if auto_pay is not None:
             self._values["auto_pay"] = auto_pay
@@ -2488,65 +2879,77 @@
 ):
     '''A ROS template type:  ``ALIYUN::CEN::CenInstance``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosCenInstanceProps",
+        props: typing.Union["RosCenInstanceProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::CEN::CenInstance``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosCenInstance.__init__)
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
+            type_hints = typing.get_type_hints(RosCenInstance._render_properties)
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
     @jsii.member(jsii_name="attrCenId")
     def attr_cen_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: CenId: The ID of the request.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrCenId"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosCenInstance, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="description")
     def description(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -2556,17 +2959,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "description"))
 
     @description.setter
     def description(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCenInstance, "description").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "description", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="name")
     def name(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -2576,17 +2982,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "name"))
 
     @name.setter
     def name(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCenInstance, "name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "name", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="protectionLevel")
     def protection_level(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -2597,46 +3006,55 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "protectionLevel"))
 
     @protection_level.setter
     def protection_level(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCenInstance, "protection_level").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "protectionLevel", value)
 
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
+            type_hints = typing.get_type_hints(getattr(RosCenInstance, "resource_group_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "resourceGroupId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="tags")
     def tags(self) -> typing.Optional[typing.List["RosCenInstance.TagsProperty"]]:
         '''
         :Property: tags: Tags to attach to instance. Max support 20 tags to add during create instance. Each tag with two properties Key and Value, and Key is required.
         '''
         return typing.cast(typing.Optional[typing.List["RosCenInstance.TagsProperty"]], jsii.get(self, "tags"))
 
     @tags.setter
     def tags(
         self,
         value: typing.Optional[typing.List["RosCenInstance.TagsProperty"]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCenInstance, "tags").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "tags", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-cen.RosCenInstance.TagsProperty",
         jsii_struct_bases=[],
         name_mapping={"key": "key", "value": "value"},
     )
@@ -2647,14 +3065,18 @@
             key: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         ) -> None:
             '''
             :param key: 
             :param value: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosCenInstance.TagsProperty.__init__)
+                check_type(argname="argument key", value=key, expected_type=type_hints["key"])
+                check_type(argname="argument value", value=value, expected_type=type_hints["value"])
             self._values: typing.Dict[str, typing.Any] = {
                 "key": key,
             }
             if value is not None:
                 self._values["value"] = value
 
         @builtins.property
@@ -2695,136 +3117,163 @@
 ):
     '''A ROS template type:  ``ALIYUN::CEN::CenInstanceAttachment``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosCenInstanceAttachmentProps",
+        props: typing.Union["RosCenInstanceAttachmentProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::CEN::CenInstanceAttachment``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosCenInstanceAttachment.__init__)
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
+            type_hints = typing.get_type_hints(RosCenInstanceAttachment._render_properties)
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
     @jsii.member(jsii_name="cenId")
     def cen_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: cenId: The ID of the CEN instance.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "cenId"))
 
     @cen_id.setter
     def cen_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCenInstanceAttachment, "cen_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "cenId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="childInstanceId")
     def child_instance_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: childInstanceId: The ID of the network to attach.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "childInstanceId"))
 
     @child_instance_id.setter
     def child_instance_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCenInstanceAttachment, "child_instance_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "childInstanceId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="childInstanceRegionId")
     def child_instance_region_id(
         self,
     ) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: childInstanceRegionId: The ID of the region where the network is located. The ID of the region where the network is located.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "childInstanceRegionId"))
 
     @child_instance_region_id.setter
     def child_instance_region_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCenInstanceAttachment, "child_instance_region_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "childInstanceRegionId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="childInstanceType")
     def child_instance_type(
         self,
     ) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: childInstanceType: The type of the network to attach. Support VPC, VBR or CCN.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "childInstanceType"))
 
     @child_instance_type.setter
     def child_instance_type(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCenInstanceAttachment, "child_instance_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "childInstanceType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         '''A factory method that creates a new instance of this class from an object containing the properties of this ROS resource.'''
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCenInstanceAttachment, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="childInstanceOwnerId")
     def child_instance_owner_id(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: childInstanceOwnerId: The account ID to which the network belongs.
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "childInstanceOwnerId"))
 
     @child_instance_owner_id.setter
     def child_instance_owner_id(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCenInstanceAttachment, "child_instance_owner_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "childInstanceOwnerId", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-cen.RosCenInstanceAttachmentProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -2849,14 +3298,21 @@
 
         :param cen_id: 
         :param child_instance_id: 
         :param child_instance_region_id: 
         :param child_instance_type: 
         :param child_instance_owner_id: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosCenInstanceAttachmentProps.__init__)
+            check_type(argname="argument cen_id", value=cen_id, expected_type=type_hints["cen_id"])
+            check_type(argname="argument child_instance_id", value=child_instance_id, expected_type=type_hints["child_instance_id"])
+            check_type(argname="argument child_instance_region_id", value=child_instance_region_id, expected_type=type_hints["child_instance_region_id"])
+            check_type(argname="argument child_instance_type", value=child_instance_type, expected_type=type_hints["child_instance_type"])
+            check_type(argname="argument child_instance_owner_id", value=child_instance_owner_id, expected_type=type_hints["child_instance_owner_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "cen_id": cen_id,
             "child_instance_id": child_instance_id,
             "child_instance_region_id": child_instance_region_id,
             "child_instance_type": child_instance_type,
         }
         if child_instance_owner_id is not None:
@@ -2939,24 +3395,31 @@
     def __init__(
         self,
         *,
         description: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         name: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         protection_level: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         resource_group_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
-        tags: typing.Optional[typing.Sequence[RosCenInstance.TagsProperty]] = None,
+        tags: typing.Optional[typing.Sequence[typing.Union[RosCenInstance.TagsProperty, typing.Dict[str, typing.Any]]]] = None,
     ) -> None:
         '''Properties for defining a ``ALIYUN::CEN::CenInstance``.
 
         :param description: 
         :param name: 
         :param protection_level: 
         :param resource_group_id: 
         :param tags: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosCenInstanceProps.__init__)
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+            check_type(argname="argument protection_level", value=protection_level, expected_type=type_hints["protection_level"])
+            check_type(argname="argument resource_group_id", value=resource_group_id, expected_type=type_hints["resource_group_id"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
         self._values: typing.Dict[str, typing.Any] = {}
         if description is not None:
             self._values["description"] = description
         if name is not None:
             self._values["name"] = name
         if protection_level is not None:
             self._values["protection_level"] = protection_level
@@ -3042,95 +3505,113 @@
 ):
     '''A ROS template type:  ``ALIYUN::CEN::CenRouteMap``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosCenRouteMapProps",
+        props: typing.Union["RosCenRouteMapProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::CEN::CenRouteMap``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosCenRouteMap.__init__)
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
+            type_hints = typing.get_type_hints(RosCenRouteMap._render_properties)
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
     @jsii.member(jsii_name="attrRouteMapId")
     def attr_route_map_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: RouteMapId: The ID of the route map.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrRouteMapId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="cenId")
     def cen_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: cenId: The ID of the Cloud Enterprise Network (CEN) instance.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "cenId"))
 
     @cen_id.setter
     def cen_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCenRouteMap, "cen_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "cenId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="cenRegionId")
     def cen_region_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: cenRegionId: The region where the CEN instance is deployed. You can call the DescribeRegions operation to query region IDs.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "cenRegionId"))
 
     @cen_region_id.setter
     def cen_region_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCenRouteMap, "cen_region_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "cenRegionId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCenRouteMap, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="mapResult")
     def map_result(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         mapResult: The route map behavior after all conditions are matched. Valid values:
         Permit: allows the routes that are matched.
@@ -3139,17 +3620,20 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "mapResult"))
 
     @map_result.setter
     def map_result(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCenRouteMap, "map_result").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "mapResult", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="priority")
     def priority(self) -> typing.Union[jsii.Number, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         priority: The priority of the route map. Valid values: 1 to 100 . A lower value indicates a higher priority.
         Note In the same region, for route maps that are applied in the same direction, the priority is unique. When a route map is implemented, the system matches conditions with a route map whose priority number is the smallest. Therefore, make sure that you set priorities for route maps to meet your requirements.
@@ -3157,17 +3641,20 @@
         return typing.cast(typing.Union[jsii.Number, ros_cdk_core.IResolvable], jsii.get(self, "priority"))
 
     @priority.setter
     def priority(
         self,
         value: typing.Union[jsii.Number, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCenRouteMap, "priority").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "priority", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="transmitDirection")
     def transmit_direction(
         self,
     ) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
@@ -3180,17 +3667,20 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "transmitDirection"))
 
     @transmit_direction.setter
     def transmit_direction(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCenRouteMap, "transmit_direction").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "transmitDirection", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="asPathMatchMode")
     def as_path_match_mode(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -3201,17 +3691,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "asPathMatchMode"))
 
     @as_path_match_mode.setter
     def as_path_match_mode(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCenRouteMap, "as_path_match_mode").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "asPathMatchMode", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="cidrMatchMode")
     def cidr_match_mode(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -3224,17 +3717,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "cidrMatchMode"))
 
     @cidr_match_mode.setter
     def cidr_match_mode(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCenRouteMap, "cidr_match_mode").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "cidrMatchMode", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="communityMatchMode")
     def community_match_mode(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -3245,17 +3741,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "communityMatchMode"))
 
     @community_match_mode.setter
     def community_match_mode(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCenRouteMap, "community_match_mode").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "communityMatchMode", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="communityOperateMode")
     def community_operate_mode(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -3266,34 +3765,40 @@
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "communityOperateMode"))
 
     @community_operate_mode.setter
     def community_operate_mode(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCenRouteMap, "community_operate_mode").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "communityOperateMode", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="description")
     def description(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: description: The description of the route map.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "description"))
 
     @description.setter
     def description(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCenRouteMap, "description").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "description", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="destinationChildInstanceTypes")
     def destination_child_instance_types(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]]:
         '''
         :Property:
 
@@ -3306,34 +3811,40 @@
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]], jsii.get(self, "destinationChildInstanceTypes"))
 
     @destination_child_instance_types.setter
     def destination_child_instance_types(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCenRouteMap, "destination_child_instance_types").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "destinationChildInstanceTypes", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="destinationCidrBlocks")
     def destination_cidr_blocks(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]]:
         '''
         :Property: destinationCidrBlocks: Match statements are used to match the routing prefixes. The CIDR format is used. You can enter at most 32 CIDR blocks.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]], jsii.get(self, "destinationCidrBlocks"))
 
     @destination_cidr_blocks.setter
     def destination_cidr_blocks(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCenRouteMap, "destination_cidr_blocks").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "destinationCidrBlocks", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="destinationInstanceIds")
     def destination_instance_ids(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]]:
         '''
         :Property:
 
@@ -3344,17 +3855,20 @@
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]], jsii.get(self, "destinationInstanceIds"))
 
     @destination_instance_ids.setter
     def destination_instance_ids(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCenRouteMap, "destination_instance_ids").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "destinationInstanceIds", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="destinationInstanceIdsReverseMatch")
     def destination_instance_ids_reverse_match(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -3365,17 +3879,20 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "destinationInstanceIdsReverseMatch"))
 
     @destination_instance_ids_reverse_match.setter
     def destination_instance_ids_reverse_match(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCenRouteMap, "destination_instance_ids_reverse_match").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "destinationInstanceIdsReverseMatch", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="destinationRouteTableIds")
     def destination_route_table_ids(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]]:
         '''
         :Property:
 
@@ -3385,17 +3902,20 @@
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]], jsii.get(self, "destinationRouteTableIds"))
 
     @destination_route_table_ids.setter
     def destination_route_table_ids(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCenRouteMap, "destination_route_table_ids").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "destinationRouteTableIds", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="matchAsns")
     def match_asns(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]]:
         '''
         :Property:
 
@@ -3405,17 +3925,20 @@
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]], jsii.get(self, "matchAsns"))
 
     @match_asns.setter
     def match_asns(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCenRouteMap, "match_asns").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "matchAsns", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="matchCommunitySet")
     def match_community_set(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]]:
         '''
         :Property:
 
@@ -3425,17 +3948,20 @@
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]], jsii.get(self, "matchCommunitySet"))
 
     @match_community_set.setter
     def match_community_set(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCenRouteMap, "match_community_set").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "matchCommunitySet", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="nextPriority")
     def next_priority(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -3448,17 +3974,20 @@
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "nextPriority"))
 
     @next_priority.setter
     def next_priority(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCenRouteMap, "next_priority").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "nextPriority", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="operateCommunitySet")
     def operate_community_set(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]]:
         '''
         :Property:
 
@@ -3468,34 +3997,40 @@
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]], jsii.get(self, "operateCommunitySet"))
 
     @operate_community_set.setter
     def operate_community_set(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCenRouteMap, "operate_community_set").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "operateCommunitySet", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="preference")
     def preference(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: preference: Action statements are used to modify route priorities. Valid values: 1 to 100. Default value: 50. A smaller number indicates a higher priority.
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "preference"))
 
     @preference.setter
     def preference(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCenRouteMap, "preference").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "preference", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="prependAsPath")
     def prepend_as_path(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]]:
         '''
         :Property:
 
@@ -3507,17 +4042,20 @@
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]], jsii.get(self, "prependAsPath"))
 
     @prepend_as_path.setter
     def prepend_as_path(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCenRouteMap, "prepend_as_path").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "prependAsPath", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="routeTypes")
     def route_types(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]]:
         '''
         :Property:
 
@@ -3530,17 +4068,20 @@
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]], jsii.get(self, "routeTypes"))
 
     @route_types.setter
     def route_types(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCenRouteMap, "route_types").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "routeTypes", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="sourceChildInstanceTypes")
     def source_child_instance_types(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]]:
         '''
         :Property:
 
@@ -3552,17 +4093,20 @@
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]], jsii.get(self, "sourceChildInstanceTypes"))
 
     @source_child_instance_types.setter
     def source_child_instance_types(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCenRouteMap, "source_child_instance_types").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "sourceChildInstanceTypes", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="sourceInstanceIds")
     def source_instance_ids(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]]:
         '''
         :Property:
 
@@ -3572,17 +4116,20 @@
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]], jsii.get(self, "sourceInstanceIds"))
 
     @source_instance_ids.setter
     def source_instance_ids(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCenRouteMap, "source_instance_ids").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "sourceInstanceIds", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="sourceInstanceIdsReverseMatch")
     def source_instance_ids_reverse_match(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -3593,48 +4140,57 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "sourceInstanceIdsReverseMatch"))
 
     @source_instance_ids_reverse_match.setter
     def source_instance_ids_reverse_match(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCenRouteMap, "source_instance_ids_reverse_match").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "sourceInstanceIdsReverseMatch", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="sourceRegionIds")
     def source_region_ids(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]]:
         '''
         :Property: sourceRegionIds: Match statements are used to match source region IDs of the routes. You can enter at most 32 region IDs.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]], jsii.get(self, "sourceRegionIds"))
 
     @source_region_ids.setter
     def source_region_ids(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCenRouteMap, "source_region_ids").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "sourceRegionIds", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="sourceRouteTableIds")
     def source_route_table_ids(
         self,
     ) -> typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]]:
         '''
         :Property: sourceRouteTableIds: Match statements are used to match source route table IDs of the routes. You can enter at most 32 route table IDs.
         '''
         return typing.cast(typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]], jsii.get(self, "sourceRouteTableIds"))
 
     @source_route_table_ids.setter
     def source_route_table_ids(
         self,
         value: typing.Optional[typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[builtins.str, ros_cdk_core.IResolvable]]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCenRouteMap, "source_route_table_ids").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "sourceRouteTableIds", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-cen.RosCenRouteMapProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -3725,14 +4281,43 @@
         :param route_types: 
         :param source_child_instance_types: 
         :param source_instance_ids: 
         :param source_instance_ids_reverse_match: 
         :param source_region_ids: 
         :param source_route_table_ids: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosCenRouteMapProps.__init__)
+            check_type(argname="argument cen_id", value=cen_id, expected_type=type_hints["cen_id"])
+            check_type(argname="argument cen_region_id", value=cen_region_id, expected_type=type_hints["cen_region_id"])
+            check_type(argname="argument map_result", value=map_result, expected_type=type_hints["map_result"])
+            check_type(argname="argument priority", value=priority, expected_type=type_hints["priority"])
+            check_type(argname="argument transmit_direction", value=transmit_direction, expected_type=type_hints["transmit_direction"])
+            check_type(argname="argument as_path_match_mode", value=as_path_match_mode, expected_type=type_hints["as_path_match_mode"])
+            check_type(argname="argument cidr_match_mode", value=cidr_match_mode, expected_type=type_hints["cidr_match_mode"])
+            check_type(argname="argument community_match_mode", value=community_match_mode, expected_type=type_hints["community_match_mode"])
+            check_type(argname="argument community_operate_mode", value=community_operate_mode, expected_type=type_hints["community_operate_mode"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument destination_child_instance_types", value=destination_child_instance_types, expected_type=type_hints["destination_child_instance_types"])
+            check_type(argname="argument destination_cidr_blocks", value=destination_cidr_blocks, expected_type=type_hints["destination_cidr_blocks"])
+            check_type(argname="argument destination_instance_ids", value=destination_instance_ids, expected_type=type_hints["destination_instance_ids"])
+            check_type(argname="argument destination_instance_ids_reverse_match", value=destination_instance_ids_reverse_match, expected_type=type_hints["destination_instance_ids_reverse_match"])
+            check_type(argname="argument destination_route_table_ids", value=destination_route_table_ids, expected_type=type_hints["destination_route_table_ids"])
+            check_type(argname="argument match_asns", value=match_asns, expected_type=type_hints["match_asns"])
+            check_type(argname="argument match_community_set", value=match_community_set, expected_type=type_hints["match_community_set"])
+            check_type(argname="argument next_priority", value=next_priority, expected_type=type_hints["next_priority"])
+            check_type(argname="argument operate_community_set", value=operate_community_set, expected_type=type_hints["operate_community_set"])
+            check_type(argname="argument preference", value=preference, expected_type=type_hints["preference"])
+            check_type(argname="argument prepend_as_path", value=prepend_as_path, expected_type=type_hints["prepend_as_path"])
+            check_type(argname="argument route_types", value=route_types, expected_type=type_hints["route_types"])
+            check_type(argname="argument source_child_instance_types", value=source_child_instance_types, expected_type=type_hints["source_child_instance_types"])
+            check_type(argname="argument source_instance_ids", value=source_instance_ids, expected_type=type_hints["source_instance_ids"])
+            check_type(argname="argument source_instance_ids_reverse_match", value=source_instance_ids_reverse_match, expected_type=type_hints["source_instance_ids_reverse_match"])
+            check_type(argname="argument source_region_ids", value=source_region_ids, expected_type=type_hints["source_region_ids"])
+            check_type(argname="argument source_route_table_ids", value=source_route_table_ids, expected_type=type_hints["source_route_table_ids"])
         self._values: typing.Dict[str, typing.Any] = {
             "cen_id": cen_id,
             "cen_region_id": cen_region_id,
             "map_result": map_result,
             "priority": priority,
             "transmit_direction": transmit_direction,
         }
@@ -4153,107 +4738,128 @@
 ):
     '''A ROS template type:  ``ALIYUN::CEN::CenRouteService``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosCenRouteServiceProps",
+        props: typing.Union["RosCenRouteServiceProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::CEN::CenRouteService``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosCenRouteService.__init__)
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
+            type_hints = typing.get_type_hints(RosCenRouteService._render_properties)
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
     @jsii.member(jsii_name="attrId")
     def attr_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Id: The ID of the cloud service. It is formatted to {CenId}/{HostRegionId}/{Host}/{AccessRegionId}
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="accessRegionId")
     def access_region_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: accessRegionId: The region where the cloud service is deployed.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "accessRegionId"))
 
     @access_region_id.setter
     def access_region_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCenRouteService, "access_region_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "accessRegionId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="cenId")
     def cen_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: cenId: The ID of the Cloud Enterprise Network (CEN) instance.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "cenId"))
 
     @cen_id.setter
     def cen_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCenRouteService, "cen_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "cenId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCenRouteService, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="host")
     def host(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: host: The domain or IP address of the cloud service.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "host"))
 
     @host.setter
     def host(self, value: typing.Union[builtins.str, ros_cdk_core.IResolvable]) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCenRouteService, "host").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "host", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="hostRegionId")
     def host_region_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property:
 
         hostRegionId: The region where the cloud service is deployed.
         You can call the DescribeRegions operation to query region IDs.
@@ -4262,32 +4868,38 @@
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "hostRegionId"))
 
     @host_region_id.setter
     def host_region_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCenRouteService, "host_region_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "hostRegionId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="hostVpcId")
     def host_vpc_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: hostVpcId: The virtual private cloud (VPC) that is associated with the cloud service.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "hostVpcId"))
 
     @host_vpc_id.setter
     def host_vpc_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCenRouteService, "host_vpc_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "hostVpcId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="conflictIgnore")
     def conflict_ignore(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property:
 
@@ -4297,31 +4909,37 @@
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "conflictIgnore"))
 
     @conflict_ignore.setter
     def conflict_ignore(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCenRouteService, "conflict_ignore").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "conflictIgnore", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="description")
     def description(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: description: The description of the cloud service.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "description"))
 
     @description.setter
     def description(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCenRouteService, "description").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "description", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-cen.RosCenRouteServiceProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -4352,14 +4970,23 @@
         :param cen_id: 
         :param host: 
         :param host_region_id: 
         :param host_vpc_id: 
         :param conflict_ignore: 
         :param description: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosCenRouteServiceProps.__init__)
+            check_type(argname="argument access_region_id", value=access_region_id, expected_type=type_hints["access_region_id"])
+            check_type(argname="argument cen_id", value=cen_id, expected_type=type_hints["cen_id"])
+            check_type(argname="argument host", value=host, expected_type=type_hints["host"])
+            check_type(argname="argument host_region_id", value=host_region_id, expected_type=type_hints["host_region_id"])
+            check_type(argname="argument host_vpc_id", value=host_vpc_id, expected_type=type_hints["host_vpc_id"])
+            check_type(argname="argument conflict_ignore", value=conflict_ignore, expected_type=type_hints["conflict_ignore"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
         self._values: typing.Dict[str, typing.Any] = {
             "access_region_id": access_region_id,
             "cen_id": cen_id,
             "host": host,
             "host_region_id": host_region_id,
             "host_vpc_id": host_vpc_id,
         }
@@ -4459,250 +5086,286 @@
 ):
     '''A ROS template type:  ``ALIYUN::CEN::CenVbrHealthCheck``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosCenVbrHealthCheckProps",
+        props: typing.Union["RosCenVbrHealthCheckProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::CEN::CenVbrHealthCheck``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosCenVbrHealthCheck.__init__)
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
+            type_hints = typing.get_type_hints(RosCenVbrHealthCheck._render_properties)
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
     @jsii.member(jsii_name="attrCenId")
     def attr_cen_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: CenId: The ID of the CEN instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrCenId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrHealthCheckInterval")
     def attr_health_check_interval(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: HealthCheckInterval: Specifies the time interval at which probe packets are sent during the health check.  Default value: 2. Valid values: 2 to 3.  Unit: second.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrHealthCheckInterval"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrHealthCheckSourceIp")
     def attr_health_check_source_ip(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: HealthCheckSourceIp: You can use either of the following methods to specify the source IP address of the health check.  Automatic IP Address: The system automatically assigns an IP address within the CIDR block 100.96.0.0/16 (recommended).  Custom IP Address: You can specify a source IP address that is available within the CIDR block 10.0.0.0/8, 192.168.0.0/16, or 172.16.0.0/12. The specified source IP address must not overlap with the IP addresses of the Alibaba Cloud-facing and client-facing interfaces on the VBR instance, or the IP addresses of the instances with which the VBR instance needs to communicate in the CEN.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrHealthCheckSourceIp"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrHealthCheckTargetIp")
     def attr_health_check_target_ip(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: HealthCheckTargetIp: Specifies the destination IP address of the health check. The destination IP address is the IP address of the client-facing interface on the VBR instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrHealthCheckTargetIp"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrHealthyThreshold")
     def attr_healthy_threshold(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: HealthyThreshold: Specifies the number of probe packets to be sent during the health check.  Default value: 8. Valid values: 3 to 8.  Unit: packet.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrHealthyThreshold"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVbrInstanceId")
     def attr_vbr_instance_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: VbrInstanceId: The ID of the VBR instance.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVbrInstanceId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVbrInstanceOwnerId")
     def attr_vbr_instance_owner_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: VbrInstanceOwnerId: The User ID (UID) of the account to which the VBR instance belongs.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVbrInstanceOwnerId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVbrInstanceRegionId")
     def attr_vbr_instance_region_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: VbrInstanceRegionId: The ID of the region where the VBR instance is deployed. You can call the DescribeRegionsoperation to query region IDs.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVbrInstanceRegionId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="cenId")
     def cen_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: cenId: The ID of the CEN instance.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "cenId"))
 
     @cen_id.setter
     def cen_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCenVbrHealthCheck, "cen_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "cenId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCenVbrHealthCheck, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="healthCheckTargetIp")
     def health_check_target_ip(
         self,
     ) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: healthCheckTargetIp: Specifies the destination IP address of the health check. The destination IP address is the IP address of the client-facing interface on the VBR instance.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "healthCheckTargetIp"))
 
     @health_check_target_ip.setter
     def health_check_target_ip(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCenVbrHealthCheck, "health_check_target_ip").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "healthCheckTargetIp", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vbrInstanceId")
     def vbr_instance_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: vbrInstanceId: The ID of the VBR instance.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "vbrInstanceId"))
 
     @vbr_instance_id.setter
     def vbr_instance_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCenVbrHealthCheck, "vbr_instance_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "vbrInstanceId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vbrInstanceRegionId")
     def vbr_instance_region_id(
         self,
     ) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: vbrInstanceRegionId: The ID of the region where the VBR instance is deployed. You can call the DescribeRegionsoperation to query region IDs.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "vbrInstanceRegionId"))
 
     @vbr_instance_region_id.setter
     def vbr_instance_region_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCenVbrHealthCheck, "vbr_instance_region_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "vbrInstanceRegionId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="healthCheckInterval")
     def health_check_interval(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: healthCheckInterval: Specifies the time interval at which probe packets are sent during the health check.  Default value: 2. Valid values: 2 to 3.  Unit: second.
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "healthCheckInterval"))
 
     @health_check_interval.setter
     def health_check_interval(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCenVbrHealthCheck, "health_check_interval").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "healthCheckInterval", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="healthCheckSourceIp")
     def health_check_source_ip(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: healthCheckSourceIp: You can use either of the following methods to specify the source IP address of the health check.  Automatic IP Address: The system automatically assigns an IP address within the CIDR block 100.96.0.0/16 (recommended).  Custom IP Address: You can specify a source IP address that is available within the CIDR block 10.0.0.0/8, 192.168.0.0/16, or 172.16.0.0/12. The specified source IP address must not overlap with the IP addresses of the Alibaba Cloud-facing and client-facing interfaces on the VBR instance, or the IP addresses of the instances with which the VBR instance needs to communicate in the CEN.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "healthCheckSourceIp"))
 
     @health_check_source_ip.setter
     def health_check_source_ip(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCenVbrHealthCheck, "health_check_source_ip").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "healthCheckSourceIp", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="healthyThreshold")
     def healthy_threshold(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: healthyThreshold: Specifies the number of probe packets to be sent during the health check.  Default value: 8. Valid values: 3 to 8.  Unit: packet.
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "healthyThreshold"))
 
     @healthy_threshold.setter
     def healthy_threshold(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCenVbrHealthCheck, "healthy_threshold").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "healthyThreshold", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vbrInstanceOwnerId")
     def vbr_instance_owner_id(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: vbrInstanceOwnerId: The User ID (UID) of the account to which the VBR instance belongs.
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "vbrInstanceOwnerId"))
 
     @vbr_instance_owner_id.setter
     def vbr_instance_owner_id(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosCenVbrHealthCheck, "vbr_instance_owner_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "vbrInstanceOwnerId", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-cen.RosCenVbrHealthCheckProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -4736,14 +5399,24 @@
         :param vbr_instance_id: 
         :param vbr_instance_region_id: 
         :param health_check_interval: 
         :param health_check_source_ip: 
         :param healthy_threshold: 
         :param vbr_instance_owner_id: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosCenVbrHealthCheckProps.__init__)
+            check_type(argname="argument cen_id", value=cen_id, expected_type=type_hints["cen_id"])
+            check_type(argname="argument health_check_target_ip", value=health_check_target_ip, expected_type=type_hints["health_check_target_ip"])
+            check_type(argname="argument vbr_instance_id", value=vbr_instance_id, expected_type=type_hints["vbr_instance_id"])
+            check_type(argname="argument vbr_instance_region_id", value=vbr_instance_region_id, expected_type=type_hints["vbr_instance_region_id"])
+            check_type(argname="argument health_check_interval", value=health_check_interval, expected_type=type_hints["health_check_interval"])
+            check_type(argname="argument health_check_source_ip", value=health_check_source_ip, expected_type=type_hints["health_check_source_ip"])
+            check_type(argname="argument healthy_threshold", value=healthy_threshold, expected_type=type_hints["healthy_threshold"])
+            check_type(argname="argument vbr_instance_owner_id", value=vbr_instance_owner_id, expected_type=type_hints["vbr_instance_owner_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "cen_id": cen_id,
             "health_check_target_ip": health_check_target_ip,
             "vbr_instance_id": vbr_instance_id,
             "vbr_instance_region_id": vbr_instance_region_id,
         }
         if health_check_interval is not None:
@@ -4843,164 +5516,459 @@
 
     def __repr__(self) -> str:
         return "RosCenVbrHealthCheckProps(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
+class RosChildInstanceRouteEntryToAttachment(
+    ros_cdk_core.RosResource,
+    metaclass=jsii.JSIIMeta,
+    jsii_type="@alicloud/ros-cdk-cen.RosChildInstanceRouteEntryToAttachment",
+):
+    '''A ROS template type:  ``ALIYUN::CEN::ChildInstanceRouteEntryToAttachment``.'''
+
+    def __init__(
+        self,
+        scope: ros_cdk_core.Construct,
+        id: builtins.str,
+        props: typing.Union["RosChildInstanceRouteEntryToAttachmentProps", typing.Dict[str, typing.Any]],
+        enable_resource_property_constraint: builtins.bool,
+    ) -> None:
+        '''Create a new ``ALIYUN::CEN::ChildInstanceRouteEntryToAttachment``.
+
+        :param scope: - scope in which this resource is defined.
+        :param id: - scoped id of the resource.
+        :param props: - resource properties.
+        :param enable_resource_property_constraint: -
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosChildInstanceRouteEntryToAttachment.__init__)
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
+            type_hints = typing.get_type_hints(RosChildInstanceRouteEntryToAttachment._render_properties)
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
+    @jsii.member(jsii_name="attrCenId")
+    def attr_cen_id(self) -> ros_cdk_core.IResolvable:
+        '''
+        :Attribute: CenId: The ID of the CEN instance.
+        '''
+        return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrCenId"))
+
+    @builtins.property
+    @jsii.member(jsii_name="attrDestinationCidrBlock")
+    def attr_destination_cidr_block(self) -> ros_cdk_core.IResolvable:
+        '''
+        :Attribute: DestinationCidrBlock: The destination CIDR block of the route.
+        '''
+        return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrDestinationCidrBlock"))
+
+    @builtins.property
+    @jsii.member(jsii_name="attrRouteTableId")
+    def attr_route_table_id(self) -> ros_cdk_core.IResolvable:
+        '''
+        :Attribute: RouteTableId: The ID of the route table configured on the network instance.
+        '''
+        return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrRouteTableId"))
+
+    @builtins.property
+    @jsii.member(jsii_name="attrTransitRouterAttachmentId")
+    def attr_transit_router_attachment_id(self) -> ros_cdk_core.IResolvable:
+        '''
+        :Attribute: TransitRouterAttachmentId: The ID of the network instance connection.
+        '''
+        return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTransitRouterAttachmentId"))
+
+    @builtins.property
+    @jsii.member(jsii_name="rosProperties")
+    def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
+        return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
+
+    @builtins.property
+    @jsii.member(jsii_name="cenId")
+    def cen_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
+        '''
+        :Property: cenId: The ID of the CEN instance.
+        '''
+        return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "cenId"))
+
+    @cen_id.setter
+    def cen_id(
+        self,
+        value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosChildInstanceRouteEntryToAttachment, "cen_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "cenId", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="destinationCidrBlock")
+    def destination_cidr_block(
+        self,
+    ) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
+        '''
+        :Property: destinationCidrBlock: The destination CIDR block of the route.
+        '''
+        return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "destinationCidrBlock"))
+
+    @destination_cidr_block.setter
+    def destination_cidr_block(
+        self,
+        value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosChildInstanceRouteEntryToAttachment, "destination_cidr_block").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "destinationCidrBlock", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="enableResourcePropertyConstraint")
+    def enable_resource_property_constraint(self) -> builtins.bool:
+        return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
+
+    @enable_resource_property_constraint.setter
+    def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosChildInstanceRouteEntryToAttachment, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "enableResourcePropertyConstraint", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="routeTableId")
+    def route_table_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
+        '''
+        :Property: routeTableId: The ID of the route table configured on the network instance.
+        '''
+        return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "routeTableId"))
+
+    @route_table_id.setter
+    def route_table_id(
+        self,
+        value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosChildInstanceRouteEntryToAttachment, "route_table_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "routeTableId", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="transitRouterAttachmentId")
+    def transit_router_attachment_id(
+        self,
+    ) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
+        '''
+        :Property: transitRouterAttachmentId: The ID of the network instance connection.
+        '''
+        return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "transitRouterAttachmentId"))
+
+    @transit_router_attachment_id.setter
+    def transit_router_attachment_id(
+        self,
+        value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosChildInstanceRouteEntryToAttachment, "transit_router_attachment_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "transitRouterAttachmentId", value)
+
+
+@jsii.data_type(
+    jsii_type="@alicloud/ros-cdk-cen.RosChildInstanceRouteEntryToAttachmentProps",
+    jsii_struct_bases=[],
+    name_mapping={
+        "cen_id": "cenId",
+        "destination_cidr_block": "destinationCidrBlock",
+        "route_table_id": "routeTableId",
+        "transit_router_attachment_id": "transitRouterAttachmentId",
+    },
+)
+class RosChildInstanceRouteEntryToAttachmentProps:
+    def __init__(
+        self,
+        *,
+        cen_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
+        destination_cidr_block: typing.Union[builtins.str, ros_cdk_core.IResolvable],
+        route_table_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
+        transit_router_attachment_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
+    ) -> None:
+        '''Properties for defining a ``ALIYUN::CEN::ChildInstanceRouteEntryToAttachment``.
+
+        :param cen_id: 
+        :param destination_cidr_block: 
+        :param route_table_id: 
+        :param transit_router_attachment_id: 
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosChildInstanceRouteEntryToAttachmentProps.__init__)
+            check_type(argname="argument cen_id", value=cen_id, expected_type=type_hints["cen_id"])
+            check_type(argname="argument destination_cidr_block", value=destination_cidr_block, expected_type=type_hints["destination_cidr_block"])
+            check_type(argname="argument route_table_id", value=route_table_id, expected_type=type_hints["route_table_id"])
+            check_type(argname="argument transit_router_attachment_id", value=transit_router_attachment_id, expected_type=type_hints["transit_router_attachment_id"])
+        self._values: typing.Dict[str, typing.Any] = {
+            "cen_id": cen_id,
+            "destination_cidr_block": destination_cidr_block,
+            "route_table_id": route_table_id,
+            "transit_router_attachment_id": transit_router_attachment_id,
+        }
+
+    @builtins.property
+    def cen_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
+        '''
+        :Property: cenId: The ID of the CEN instance.
+        '''
+        result = self._values.get("cen_id")
+        assert result is not None, "Required property 'cen_id' is missing"
+        return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], result)
+
+    @builtins.property
+    def destination_cidr_block(
+        self,
+    ) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
+        '''
+        :Property: destinationCidrBlock: The destination CIDR block of the route.
+        '''
+        result = self._values.get("destination_cidr_block")
+        assert result is not None, "Required property 'destination_cidr_block' is missing"
+        return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], result)
+
+    @builtins.property
+    def route_table_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
+        '''
+        :Property: routeTableId: The ID of the route table configured on the network instance.
+        '''
+        result = self._values.get("route_table_id")
+        assert result is not None, "Required property 'route_table_id' is missing"
+        return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], result)
+
+    @builtins.property
+    def transit_router_attachment_id(
+        self,
+    ) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
+        '''
+        :Property: transitRouterAttachmentId: The ID of the network instance connection.
+        '''
+        result = self._values.get("transit_router_attachment_id")
+        assert result is not None, "Required property 'transit_router_attachment_id' is missing"
+        return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], result)
+
+    def __eq__(self, rhs: typing.Any) -> builtins.bool:
+        return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+    def __ne__(self, rhs: typing.Any) -> builtins.bool:
+        return not (rhs == self)
+
+    def __repr__(self) -> str:
+        return "RosChildInstanceRouteEntryToAttachmentProps(%s)" % ", ".join(
+            k + "=" + repr(v) for k, v in self._values.items()
+        )
+
+
 class RosRouteEntry(
     ros_cdk_core.RosResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@alicloud/ros-cdk-cen.RosRouteEntry",
 ):
     '''A ROS template type:  ``ALIYUN::CEN::RouteEntry``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosRouteEntryProps",
+        props: typing.Union["RosRouteEntryProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::CEN::RouteEntry``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosRouteEntry.__init__)
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
+            type_hints = typing.get_type_hints(RosRouteEntry._render_properties)
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
     @jsii.member(jsii_name="cenId")
     def cen_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: cenId: The ID of the CEN instance where the route entry is published.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "cenId"))
 
     @cen_id.setter
     def cen_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosRouteEntry, "cen_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "cenId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="childInstanceId")
     def child_instance_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: childInstanceId: The ID of the attached network (VPC or VBR).
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "childInstanceId"))
 
     @child_instance_id.setter
     def child_instance_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosRouteEntry, "child_instance_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "childInstanceId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="childInstanceRegionId")
     def child_instance_region_id(
         self,
     ) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: childInstanceRegionId: The ID of the region where the attached VBR or VPC is located.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "childInstanceRegionId"))
 
     @child_instance_region_id.setter
     def child_instance_region_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosRouteEntry, "child_instance_region_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "childInstanceRegionId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="childInstanceRouteTableId")
     def child_instance_route_table_id(
         self,
     ) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: childInstanceRouteTableId: The route table of the attached VBR or VPC.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "childInstanceRouteTableId"))
 
     @child_instance_route_table_id.setter
     def child_instance_route_table_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosRouteEntry, "child_instance_route_table_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "childInstanceRouteTableId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="childInstanceType")
     def child_instance_type(
         self,
     ) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: childInstanceType: The type of the network, value: VPC VBR
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "childInstanceType"))
 
     @child_instance_type.setter
     def child_instance_type(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosRouteEntry, "child_instance_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "childInstanceType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="destinationCidrBlock")
     def destination_cidr_block(
         self,
     ) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: destinationCidrBlock: The destination CIDR block of the route entry to publish.
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "destinationCidrBlock"))
 
     @destination_cidr_block.setter
     def destination_cidr_block(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosRouteEntry, "destination_cidr_block").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "destinationCidrBlock", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         '''A factory method that creates a new instance of this class from an object containing the properties of this ROS resource.'''
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosRouteEntry, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-cen.RosRouteEntryProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -5028,14 +5996,22 @@
         :param cen_id: 
         :param child_instance_id: 
         :param child_instance_region_id: 
         :param child_instance_route_table_id: 
         :param child_instance_type: 
         :param destination_cidr_block: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosRouteEntryProps.__init__)
+            check_type(argname="argument cen_id", value=cen_id, expected_type=type_hints["cen_id"])
+            check_type(argname="argument child_instance_id", value=child_instance_id, expected_type=type_hints["child_instance_id"])
+            check_type(argname="argument child_instance_region_id", value=child_instance_region_id, expected_type=type_hints["child_instance_region_id"])
+            check_type(argname="argument child_instance_route_table_id", value=child_instance_route_table_id, expected_type=type_hints["child_instance_route_table_id"])
+            check_type(argname="argument child_instance_type", value=child_instance_type, expected_type=type_hints["child_instance_type"])
+            check_type(argname="argument destination_cidr_block", value=destination_cidr_block, expected_type=type_hints["destination_cidr_block"])
         self._values: typing.Dict[str, typing.Any] = {
             "cen_id": cen_id,
             "child_instance_id": child_instance_id,
             "child_instance_region_id": child_instance_region_id,
             "child_instance_route_table_id": child_instance_route_table_id,
             "child_instance_type": child_instance_type,
             "destination_cidr_block": destination_cidr_block,
@@ -5122,478 +6098,538 @@
 ):
     '''A ROS template type:  ``ALIYUN::CEN::TransitRouter``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosTransitRouterProps",
+        props: typing.Union["RosTransitRouterProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::CEN::TransitRouter``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosTransitRouter.__init__)
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
+            type_hints = typing.get_type_hints(RosTransitRouter._render_properties)
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
     @jsii.member(jsii_name="attrAliUid")
     def attr_ali_uid(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: AliUid: AliUid
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAliUid"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrCenId")
     def attr_cen_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: CenId: CenId
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrCenId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrSystemTransitRouterRouteTableId")
     def attr_system_transit_router_route_table_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: SystemTransitRouterRouteTableId: The system route table ID of transit router.
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrSystemTransitRouterRouteTableId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTransitRouterDescription")
     def attr_transit_router_description(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: TransitRouterDescription: TransitRouterDescription
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTransitRouterDescription"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTransitRouterId")
     def attr_transit_router_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: TransitRouterId: TransitRouterId
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTransitRouterId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTransitRouterName")
     def attr_transit_router_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: TransitRouterName: TransitRouterName
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTransitRouterName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrType")
     def attr_type(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Type: Type
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="rosProperties")
     def _ros_properties(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "rosProperties"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="cenId")
     def cen_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: cenId: CenId
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "cenId"))
 
     @cen_id.setter
     def cen_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTransitRouter, "cen_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "cenId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="enableResourcePropertyConstraint")
     def enable_resource_property_constraint(self) -> builtins.bool:
         return typing.cast(builtins.bool, jsii.get(self, "enableResourcePropertyConstraint"))
 
     @enable_resource_property_constraint.setter
     def enable_resource_property_constraint(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTransitRouter, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="transitRouterDescription")
     def transit_router_description(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: transitRouterDescription: TransitRouterDescription
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "transitRouterDescription"))
 
     @transit_router_description.setter
     def transit_router_description(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTransitRouter, "transit_router_description").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "transitRouterDescription", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="transitRouterName")
     def transit_router_name(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: transitRouterName: TransitRouterName
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "transitRouterName"))
 
     @transit_router_name.setter
     def transit_router_name(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTransitRouter, "transit_router_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "transitRouterName", value)
 
 
 class RosTransitRouterPeerAttachment(
     ros_cdk_core.RosResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@alicloud/ros-cdk-cen.RosTransitRouterPeerAttachment",
 ):
     '''A ROS template type:  ``ALIYUN::CEN::TransitRouterPeerAttachment``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosTransitRouterPeerAttachmentProps",
+        props: typing.Union["RosTransitRouterPeerAttachmentProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::CEN::TransitRouterPeerAttachment``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosTransitRouterPeerAttachment.__init__)
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
+            type_hints = typing.get_type_hints(RosTransitRouterPeerAttachment._render_properties)
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
     @jsii.member(jsii_name="attrAutoPublishRouteEnabled")
     def attr_auto_publish_route_enabled(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: AutoPublishRouteEnabled: AutoPublishRouteEnabled
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAutoPublishRouteEnabled"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrBandwidth")
     def attr_bandwidth(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: Bandwidth: Bandwidth
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrBandwidth"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrCenBandwidthPackageId")
     def attr_cen_bandwidth_package_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: CenBandwidthPackageId: BandwidthPackageId
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrCenBandwidthPackageId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrCenId")
     def attr_cen_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: CenId: CenId
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrCenId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrClientToken")
     def attr_client_token(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ClientToken: ClientToken
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrClientToken"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrGeographicSpanId")
     def attr_geographic_span_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: GeographicSpanId: GeographicSpanId
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrGeographicSpanId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPeerTransitRouterId")
     def attr_peer_transit_router_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: PeerTransitRouterId: PeerTransitRouterId
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPeerTransitRouterId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPeerTransitRouterOwnerId")
     def attr_peer_transit_router_owner_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: PeerTransitRouterOwnerId: PeerTransitRouterOwnerId
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPeerTransitRouterOwnerId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPeerTransitRouterRegionId")
     def attr_peer_transit_router_region_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: PeerTransitRouterRegionId: PeerTransitRouterRegionId
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPeerTransitRouterRegionId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrResourceType")
     def attr_resource_type(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ResourceType: ResourceType
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrResourceType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTransitRouterAttachmentDescription")
     def attr_transit_router_attachment_description(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: TransitRouterAttachmentDescription: TransitRouterAttachmentDescription
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTransitRouterAttachmentDescription"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTransitRouterAttachmentId")
     def attr_transit_router_attachment_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: TransitRouterAttachmentId: The first ID of the resource
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTransitRouterAttachmentId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTransitRouterAttachmentName")
     def attr_transit_router_attachment_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: TransitRouterAttachmentName: TransitRouterAttachmentName
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTransitRouterAttachmentName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTransitRouterId")
     def attr_transit_router_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: TransitRouterId: TransitRouterId
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTransitRouterId"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosTransitRouterPeerAttachment, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="peerTransitRouterId")
     def peer_transit_router_id(
         self,
     ) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: peerTransitRouterId: PeerTransitRouterId
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "peerTransitRouterId"))
 
     @peer_transit_router_id.setter
     def peer_transit_router_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTransitRouterPeerAttachment, "peer_transit_router_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "peerTransitRouterId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="autoPublishRouteEnabled")
     def auto_publish_route_enabled(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property: autoPublishRouteEnabled: AutoPublishRouteEnabled
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "autoPublishRouteEnabled"))
 
     @auto_publish_route_enabled.setter
     def auto_publish_route_enabled(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTransitRouterPeerAttachment, "auto_publish_route_enabled").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "autoPublishRouteEnabled", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="bandwidth")
     def bandwidth(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: bandwidth: Bandwidth
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "bandwidth"))
 
     @bandwidth.setter
     def bandwidth(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTransitRouterPeerAttachment, "bandwidth").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "bandwidth", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="cenBandwidthPackageId")
     def cen_bandwidth_package_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: cenBandwidthPackageId: BandwidthPackageId
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "cenBandwidthPackageId"))
 
     @cen_bandwidth_package_id.setter
     def cen_bandwidth_package_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTransitRouterPeerAttachment, "cen_bandwidth_package_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "cenBandwidthPackageId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="cenId")
     def cen_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: cenId: CenId
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "cenId"))
 
     @cen_id.setter
     def cen_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTransitRouterPeerAttachment, "cen_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "cenId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="peerTransitRouterRegionId")
     def peer_transit_router_region_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: peerTransitRouterRegionId: PeerTransitRouterRegionId
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "peerTransitRouterRegionId"))
 
     @peer_transit_router_region_id.setter
     def peer_transit_router_region_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTransitRouterPeerAttachment, "peer_transit_router_region_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "peerTransitRouterRegionId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="transitRouterAttachmentDescription")
     def transit_router_attachment_description(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: transitRouterAttachmentDescription: TransitRouterAttachmentDescription
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "transitRouterAttachmentDescription"))
 
     @transit_router_attachment_description.setter
     def transit_router_attachment_description(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTransitRouterPeerAttachment, "transit_router_attachment_description").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "transitRouterAttachmentDescription", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="transitRouterAttachmentName")
     def transit_router_attachment_name(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: transitRouterAttachmentName: TransitRouterAttachmentName
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "transitRouterAttachmentName"))
 
     @transit_router_attachment_name.setter
     def transit_router_attachment_name(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTransitRouterPeerAttachment, "transit_router_attachment_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "transitRouterAttachmentName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="transitRouterId")
     def transit_router_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: transitRouterId: TransitRouterId
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "transitRouterId"))
 
     @transit_router_id.setter
     def transit_router_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTransitRouterPeerAttachment, "transit_router_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "transitRouterId", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-cen.RosTransitRouterPeerAttachmentProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -5630,14 +6666,25 @@
         :param cen_bandwidth_package_id: 
         :param cen_id: 
         :param peer_transit_router_region_id: 
         :param transit_router_attachment_description: 
         :param transit_router_attachment_name: 
         :param transit_router_id: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosTransitRouterPeerAttachmentProps.__init__)
+            check_type(argname="argument peer_transit_router_id", value=peer_transit_router_id, expected_type=type_hints["peer_transit_router_id"])
+            check_type(argname="argument auto_publish_route_enabled", value=auto_publish_route_enabled, expected_type=type_hints["auto_publish_route_enabled"])
+            check_type(argname="argument bandwidth", value=bandwidth, expected_type=type_hints["bandwidth"])
+            check_type(argname="argument cen_bandwidth_package_id", value=cen_bandwidth_package_id, expected_type=type_hints["cen_bandwidth_package_id"])
+            check_type(argname="argument cen_id", value=cen_id, expected_type=type_hints["cen_id"])
+            check_type(argname="argument peer_transit_router_region_id", value=peer_transit_router_region_id, expected_type=type_hints["peer_transit_router_region_id"])
+            check_type(argname="argument transit_router_attachment_description", value=transit_router_attachment_description, expected_type=type_hints["transit_router_attachment_description"])
+            check_type(argname="argument transit_router_attachment_name", value=transit_router_attachment_name, expected_type=type_hints["transit_router_attachment_name"])
+            check_type(argname="argument transit_router_id", value=transit_router_id, expected_type=type_hints["transit_router_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "peer_transit_router_id": peer_transit_router_id,
         }
         if auto_publish_route_enabled is not None:
             self._values["auto_publish_route_enabled"] = auto_publish_route_enabled
         if bandwidth is not None:
             self._values["bandwidth"] = bandwidth
@@ -5776,14 +6823,19 @@
     ) -> None:
         '''Properties for defining a ``ALIYUN::CEN::TransitRouter``.
 
         :param cen_id: 
         :param transit_router_description: 
         :param transit_router_name: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosTransitRouterProps.__init__)
+            check_type(argname="argument cen_id", value=cen_id, expected_type=type_hints["cen_id"])
+            check_type(argname="argument transit_router_description", value=transit_router_description, expected_type=type_hints["transit_router_description"])
+            check_type(argname="argument transit_router_name", value=transit_router_name, expected_type=type_hints["transit_router_name"])
         self._values: typing.Dict[str, typing.Any] = {
             "cen_id": cen_id,
         }
         if transit_router_description is not None:
             self._values["transit_router_description"] = transit_router_description
         if transit_router_name is not None:
             self._values["transit_router_name"] = transit_router_name
@@ -5836,222 +6888,252 @@
 ):
     '''A ROS template type:  ``ALIYUN::CEN::TransitRouterRouteEntry``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosTransitRouterRouteEntryProps",
+        props: typing.Union["RosTransitRouterRouteEntryProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::CEN::TransitRouterRouteEntry``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosTransitRouterRouteEntry.__init__)
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
+            type_hints = typing.get_type_hints(RosTransitRouterRouteEntry._render_properties)
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
     @jsii.member(jsii_name="attrTransitRouterRouteEntryDescription")
     def attr_transit_router_route_entry_description(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: TransitRouterRouteEntryDescription: TransitRouterRouteEntryDescription
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTransitRouterRouteEntryDescription"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTransitRouterRouteEntryDestinationCidrBlock")
     def attr_transit_router_route_entry_destination_cidr_block(
         self,
     ) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: TransitRouterRouteEntryDestinationCidrBlock: TransitRouterRouteEntryDestinationCidrBlock
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTransitRouterRouteEntryDestinationCidrBlock"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTransitRouterRouteEntryId")
     def attr_transit_router_route_entry_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: TransitRouterRouteEntryId: The first ID of the resource
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTransitRouterRouteEntryId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTransitRouterRouteEntryName")
     def attr_transit_router_route_entry_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: TransitRouterRouteEntryName: TransitRouterRouteEntryName
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTransitRouterRouteEntryName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTransitRouterRouteEntryNextHopId")
     def attr_transit_router_route_entry_next_hop_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: TransitRouterRouteEntryNextHopId: TransitRouterRouteEntryNextHopId
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTransitRouterRouteEntryNextHopId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTransitRouterRouteEntryNextHopType")
     def attr_transit_router_route_entry_next_hop_type(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: TransitRouterRouteEntryNextHopType: TransitRouterRouteEntryNextHopType
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTransitRouterRouteEntryNextHopType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTransitRouterRouteEntryType")
     def attr_transit_router_route_entry_type(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: TransitRouterRouteEntryType: TransitRouterRouteEntryType
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTransitRouterRouteEntryType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTransitRouterRouteTableId")
     def attr_transit_router_route_table_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: TransitRouterRouteTableId: TransitRouterRouteTableId
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTransitRouterRouteTableId"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosTransitRouterRouteEntry, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="transitRouterRouteEntryDestinationCidrBlock")
     def transit_router_route_entry_destination_cidr_block(
         self,
     ) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: transitRouterRouteEntryDestinationCidrBlock: TransitRouterRouteEntryDestinationCidrBlock
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "transitRouterRouteEntryDestinationCidrBlock"))
 
     @transit_router_route_entry_destination_cidr_block.setter
     def transit_router_route_entry_destination_cidr_block(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTransitRouterRouteEntry, "transit_router_route_entry_destination_cidr_block").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "transitRouterRouteEntryDestinationCidrBlock", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="transitRouterRouteEntryNextHopType")
     def transit_router_route_entry_next_hop_type(
         self,
     ) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: transitRouterRouteEntryNextHopType: TransitRouterRouteEntryNextHopType
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "transitRouterRouteEntryNextHopType"))
 
     @transit_router_route_entry_next_hop_type.setter
     def transit_router_route_entry_next_hop_type(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTransitRouterRouteEntry, "transit_router_route_entry_next_hop_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "transitRouterRouteEntryNextHopType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="transitRouterRouteTableId")
     def transit_router_route_table_id(
         self,
     ) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: transitRouterRouteTableId: TransitRouterRouteTableId
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "transitRouterRouteTableId"))
 
     @transit_router_route_table_id.setter
     def transit_router_route_table_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTransitRouterRouteEntry, "transit_router_route_table_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "transitRouterRouteTableId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="transitRouterRouteEntryDescription")
     def transit_router_route_entry_description(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: transitRouterRouteEntryDescription: TransitRouterRouteEntryDescription
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "transitRouterRouteEntryDescription"))
 
     @transit_router_route_entry_description.setter
     def transit_router_route_entry_description(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTransitRouterRouteEntry, "transit_router_route_entry_description").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "transitRouterRouteEntryDescription", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="transitRouterRouteEntryName")
     def transit_router_route_entry_name(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: transitRouterRouteEntryName: TransitRouterRouteEntryName
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "transitRouterRouteEntryName"))
 
     @transit_router_route_entry_name.setter
     def transit_router_route_entry_name(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTransitRouterRouteEntry, "transit_router_route_entry_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "transitRouterRouteEntryName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="transitRouterRouteEntryNextHopId")
     def transit_router_route_entry_next_hop_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: transitRouterRouteEntryNextHopId: TransitRouterRouteEntryNextHopId
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "transitRouterRouteEntryNextHopId"))
 
     @transit_router_route_entry_next_hop_id.setter
     def transit_router_route_entry_next_hop_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTransitRouterRouteEntry, "transit_router_route_entry_next_hop_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "transitRouterRouteEntryNextHopId", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-cen.RosTransitRouterRouteEntryProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -6079,14 +7161,22 @@
         :param transit_router_route_entry_destination_cidr_block: 
         :param transit_router_route_entry_next_hop_type: 
         :param transit_router_route_table_id: 
         :param transit_router_route_entry_description: 
         :param transit_router_route_entry_name: 
         :param transit_router_route_entry_next_hop_id: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosTransitRouterRouteEntryProps.__init__)
+            check_type(argname="argument transit_router_route_entry_destination_cidr_block", value=transit_router_route_entry_destination_cidr_block, expected_type=type_hints["transit_router_route_entry_destination_cidr_block"])
+            check_type(argname="argument transit_router_route_entry_next_hop_type", value=transit_router_route_entry_next_hop_type, expected_type=type_hints["transit_router_route_entry_next_hop_type"])
+            check_type(argname="argument transit_router_route_table_id", value=transit_router_route_table_id, expected_type=type_hints["transit_router_route_table_id"])
+            check_type(argname="argument transit_router_route_entry_description", value=transit_router_route_entry_description, expected_type=type_hints["transit_router_route_entry_description"])
+            check_type(argname="argument transit_router_route_entry_name", value=transit_router_route_entry_name, expected_type=type_hints["transit_router_route_entry_name"])
+            check_type(argname="argument transit_router_route_entry_next_hop_id", value=transit_router_route_entry_next_hop_id, expected_type=type_hints["transit_router_route_entry_next_hop_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "transit_router_route_entry_destination_cidr_block": transit_router_route_entry_destination_cidr_block,
             "transit_router_route_entry_next_hop_type": transit_router_route_entry_next_hop_type,
             "transit_router_route_table_id": transit_router_route_table_id,
         }
         if transit_router_route_entry_description is not None:
             self._values["transit_router_route_entry_description"] = transit_router_route_entry_description
@@ -6177,271 +7267,310 @@
 ):
     '''A ROS template type:  ``ALIYUN::CEN::TransitRouterRouteTable``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosTransitRouterRouteTableProps",
+        props: typing.Union["RosTransitRouterRouteTableProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::CEN::TransitRouterRouteTable``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosTransitRouterRouteTable.__init__)
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
+            type_hints = typing.get_type_hints(RosTransitRouterRouteTable._render_properties)
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
     @jsii.member(jsii_name="attrClientToken")
     def attr_client_token(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ClientToken: ClientToken
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrClientToken"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTransitRouterId")
     def attr_transit_router_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: TransitRouterId: TransitRouterId
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTransitRouterId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTransitRouterRouteTableDescription")
     def attr_transit_router_route_table_description(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: TransitRouterRouteTableDescription: TransitRouterRouteTableDescription
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTransitRouterRouteTableDescription"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTransitRouterRouteTableId")
     def attr_transit_router_route_table_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: TransitRouterRouteTableId: TransitRouterRouteTableId
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTransitRouterRouteTableId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTransitRouterRouteTableName")
     def attr_transit_router_route_table_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: TransitRouterRouteTableName: TransitRouterRouteTableName
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTransitRouterRouteTableName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTransitRouterRouteTableType")
     def attr_transit_router_route_table_type(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: TransitRouterRouteTableType: TransitRouterRouteTableType
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTransitRouterRouteTableType"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosTransitRouterRouteTable, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="transitRouterId")
     def transit_router_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: transitRouterId: TransitRouterId
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "transitRouterId"))
 
     @transit_router_id.setter
     def transit_router_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTransitRouterRouteTable, "transit_router_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "transitRouterId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="transitRouterRouteTableDescription")
     def transit_router_route_table_description(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: transitRouterRouteTableDescription: TransitRouterRouteTableDescription
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "transitRouterRouteTableDescription"))
 
     @transit_router_route_table_description.setter
     def transit_router_route_table_description(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTransitRouterRouteTable, "transit_router_route_table_description").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "transitRouterRouteTableDescription", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="transitRouterRouteTableName")
     def transit_router_route_table_name(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: transitRouterRouteTableName: TransitRouterRouteTableName
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "transitRouterRouteTableName"))
 
     @transit_router_route_table_name.setter
     def transit_router_route_table_name(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTransitRouterRouteTable, "transit_router_route_table_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "transitRouterRouteTableName", value)
 
 
 class RosTransitRouterRouteTableAssociation(
     ros_cdk_core.RosResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@alicloud/ros-cdk-cen.RosTransitRouterRouteTableAssociation",
 ):
     '''A ROS template type:  ``ALIYUN::CEN::TransitRouterRouteTableAssociation``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosTransitRouterRouteTableAssociationProps",
+        props: typing.Union["RosTransitRouterRouteTableAssociationProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::CEN::TransitRouterRouteTableAssociation``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosTransitRouterRouteTableAssociation.__init__)
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
+            type_hints = typing.get_type_hints(RosTransitRouterRouteTableAssociation._render_properties)
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
     @jsii.member(jsii_name="attrResourceId")
     def attr_resource_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ResourceId: ResourceId
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrResourceId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrResourceType")
     def attr_resource_type(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ResourceType: ResourceType
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrResourceType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTransitRouterAttachmentId")
     def attr_transit_router_attachment_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: TransitRouterAttachmentId: TransitRouterAttachmentId
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTransitRouterAttachmentId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTransitRouterRouteTableId")
     def attr_transit_router_route_table_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: TransitRouterRouteTableId: TransitRouterRouteTableId
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTransitRouterRouteTableId"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosTransitRouterRouteTableAssociation, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="transitRouterAttachmentId")
     def transit_router_attachment_id(
         self,
     ) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: transitRouterAttachmentId: TransitRouterAttachmentId
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "transitRouterAttachmentId"))
 
     @transit_router_attachment_id.setter
     def transit_router_attachment_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTransitRouterRouteTableAssociation, "transit_router_attachment_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "transitRouterAttachmentId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="transitRouterRouteTableId")
     def transit_router_route_table_id(
         self,
     ) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: transitRouterRouteTableId: TransitRouterRouteTableId
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "transitRouterRouteTableId"))
 
     @transit_router_route_table_id.setter
     def transit_router_route_table_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTransitRouterRouteTableAssociation, "transit_router_route_table_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "transitRouterRouteTableId", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-cen.RosTransitRouterRouteTableAssociationProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -6457,14 +7586,18 @@
         transit_router_route_table_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
         '''Properties for defining a ``ALIYUN::CEN::TransitRouterRouteTableAssociation``.
 
         :param transit_router_attachment_id: 
         :param transit_router_route_table_id: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosTransitRouterRouteTableAssociationProps.__init__)
+            check_type(argname="argument transit_router_attachment_id", value=transit_router_attachment_id, expected_type=type_hints["transit_router_attachment_id"])
+            check_type(argname="argument transit_router_route_table_id", value=transit_router_route_table_id, expected_type=type_hints["transit_router_route_table_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "transit_router_attachment_id": transit_router_attachment_id,
             "transit_router_route_table_id": transit_router_route_table_id,
         }
 
     @builtins.property
     def transit_router_attachment_id(
@@ -6507,120 +7640,138 @@
 ):
     '''A ROS template type:  ``ALIYUN::CEN::TransitRouterRouteTablePropagation``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosTransitRouterRouteTablePropagationProps",
+        props: typing.Union["RosTransitRouterRouteTablePropagationProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::CEN::TransitRouterRouteTablePropagation``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosTransitRouterRouteTablePropagation.__init__)
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
+            type_hints = typing.get_type_hints(RosTransitRouterRouteTablePropagation._render_properties)
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
     @jsii.member(jsii_name="attrResourceId")
     def attr_resource_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ResourceId: ResourceId
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrResourceId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrResourceType")
     def attr_resource_type(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ResourceType: ResourceType
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrResourceType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTransitRouterAttachmentId")
     def attr_transit_router_attachment_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: TransitRouterAttachmentId: TransitRouterAttachmentId
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTransitRouterAttachmentId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTransitRouterRouteTableId")
     def attr_transit_router_route_table_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: TransitRouterRouteTableId: TransitRouterRouteTableId
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTransitRouterRouteTableId"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosTransitRouterRouteTablePropagation, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="transitRouterAttachmentId")
     def transit_router_attachment_id(
         self,
     ) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: transitRouterAttachmentId: TransitRouterAttachmentId
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "transitRouterAttachmentId"))
 
     @transit_router_attachment_id.setter
     def transit_router_attachment_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTransitRouterRouteTablePropagation, "transit_router_attachment_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "transitRouterAttachmentId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="transitRouterRouteTableId")
     def transit_router_route_table_id(
         self,
     ) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: transitRouterRouteTableId: TransitRouterRouteTableId
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "transitRouterRouteTableId"))
 
     @transit_router_route_table_id.setter
     def transit_router_route_table_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTransitRouterRouteTablePropagation, "transit_router_route_table_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "transitRouterRouteTableId", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-cen.RosTransitRouterRouteTablePropagationProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -6636,14 +7787,18 @@
         transit_router_route_table_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
         '''Properties for defining a ``ALIYUN::CEN::TransitRouterRouteTablePropagation``.
 
         :param transit_router_attachment_id: 
         :param transit_router_route_table_id: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosTransitRouterRouteTablePropagationProps.__init__)
+            check_type(argname="argument transit_router_attachment_id", value=transit_router_attachment_id, expected_type=type_hints["transit_router_attachment_id"])
+            check_type(argname="argument transit_router_route_table_id", value=transit_router_route_table_id, expected_type=type_hints["transit_router_route_table_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "transit_router_attachment_id": transit_router_attachment_id,
             "transit_router_route_table_id": transit_router_route_table_id,
         }
 
     @builtins.property
     def transit_router_attachment_id(
@@ -6698,14 +7853,19 @@
     ) -> None:
         '''Properties for defining a ``ALIYUN::CEN::TransitRouterRouteTable``.
 
         :param transit_router_id: 
         :param transit_router_route_table_description: 
         :param transit_router_route_table_name: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosTransitRouterRouteTableProps.__init__)
+            check_type(argname="argument transit_router_id", value=transit_router_id, expected_type=type_hints["transit_router_id"])
+            check_type(argname="argument transit_router_route_table_description", value=transit_router_route_table_description, expected_type=type_hints["transit_router_route_table_description"])
+            check_type(argname="argument transit_router_route_table_name", value=transit_router_route_table_name, expected_type=type_hints["transit_router_route_table_name"])
         self._values: typing.Dict[str, typing.Any] = {
             "transit_router_id": transit_router_id,
         }
         if transit_router_route_table_description is not None:
             self._values["transit_router_route_table_description"] = transit_router_route_table_description
         if transit_router_route_table_name is not None:
             self._values["transit_router_route_table_name"] = transit_router_route_table_name
@@ -6758,251 +7918,284 @@
 ):
     '''A ROS template type:  ``ALIYUN::CEN::TransitRouterVbrAttachment``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosTransitRouterVbrAttachmentProps",
+        props: typing.Union["RosTransitRouterVbrAttachmentProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::CEN::TransitRouterVbrAttachment``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosTransitRouterVbrAttachment.__init__)
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
+            type_hints = typing.get_type_hints(RosTransitRouterVbrAttachment._render_properties)
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
     @jsii.member(jsii_name="attrAutoPublishRouteEnabled")
     def attr_auto_publish_route_enabled(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: AutoPublishRouteEnabled: AutoPublishRouteEnabled
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAutoPublishRouteEnabled"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrCenId")
     def attr_cen_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: CenId: CenId
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrCenId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrClientToken")
     def attr_client_token(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ClientToken: ClientToken
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrClientToken"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrResourceType")
     def attr_resource_type(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ResourceType: ResourceType
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrResourceType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTransitRouterAttachmentDescription")
     def attr_transit_router_attachment_description(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: TransitRouterAttachmentDescription: TransitRouterAttachmentDescription
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTransitRouterAttachmentDescription"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTransitRouterAttachmentId")
     def attr_transit_router_attachment_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: TransitRouterAttachmentId: The first ID of the resource
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTransitRouterAttachmentId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTransitRouterAttachmentName")
     def attr_transit_router_attachment_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: TransitRouterAttachmentName: TransitRouterAttachmentName
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTransitRouterAttachmentName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTransitRouterId")
     def attr_transit_router_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: TransitRouterId: TransitRouterId
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTransitRouterId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVbrId")
     def attr_vbr_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: VbrId: VbrId
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVbrId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVbrOwnerId")
     def attr_vbr_owner_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: VbrOwnerId: VbrOwnerId
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVbrOwnerId"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosTransitRouterVbrAttachment, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vbrId")
     def vbr_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
         '''
         :Property: vbrId: VbrId
         '''
         return typing.cast(typing.Union[builtins.str, ros_cdk_core.IResolvable], jsii.get(self, "vbrId"))
 
     @vbr_id.setter
     def vbr_id(
         self,
         value: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTransitRouterVbrAttachment, "vbr_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "vbrId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="autoPublishRouteEnabled")
     def auto_publish_route_enabled(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property: autoPublishRouteEnabled: AutoPublishRouteEnabled
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "autoPublishRouteEnabled"))
 
     @auto_publish_route_enabled.setter
     def auto_publish_route_enabled(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTransitRouterVbrAttachment, "auto_publish_route_enabled").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "autoPublishRouteEnabled", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="cenId")
     def cen_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: cenId: CenId
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "cenId"))
 
     @cen_id.setter
     def cen_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTransitRouterVbrAttachment, "cen_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "cenId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="transitRouterAttachmentDescription")
     def transit_router_attachment_description(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: transitRouterAttachmentDescription: TransitRouterAttachmentDescription
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "transitRouterAttachmentDescription"))
 
     @transit_router_attachment_description.setter
     def transit_router_attachment_description(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTransitRouterVbrAttachment, "transit_router_attachment_description").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "transitRouterAttachmentDescription", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="transitRouterAttachmentName")
     def transit_router_attachment_name(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: transitRouterAttachmentName: TransitRouterAttachmentName
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "transitRouterAttachmentName"))
 
     @transit_router_attachment_name.setter
     def transit_router_attachment_name(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTransitRouterVbrAttachment, "transit_router_attachment_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "transitRouterAttachmentName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="transitRouterId")
     def transit_router_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: transitRouterId: TransitRouterId
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "transitRouterId"))
 
     @transit_router_id.setter
     def transit_router_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTransitRouterVbrAttachment, "transit_router_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "transitRouterId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vbrOwnerId")
     def vbr_owner_id(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: vbrOwnerId: VbrOwnerId
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "vbrOwnerId"))
 
     @vbr_owner_id.setter
     def vbr_owner_id(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTransitRouterVbrAttachment, "vbr_owner_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "vbrOwnerId", value)
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-cen.RosTransitRouterVbrAttachmentProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -7033,14 +8226,23 @@
         :param auto_publish_route_enabled: 
         :param cen_id: 
         :param transit_router_attachment_description: 
         :param transit_router_attachment_name: 
         :param transit_router_id: 
         :param vbr_owner_id: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosTransitRouterVbrAttachmentProps.__init__)
+            check_type(argname="argument vbr_id", value=vbr_id, expected_type=type_hints["vbr_id"])
+            check_type(argname="argument auto_publish_route_enabled", value=auto_publish_route_enabled, expected_type=type_hints["auto_publish_route_enabled"])
+            check_type(argname="argument cen_id", value=cen_id, expected_type=type_hints["cen_id"])
+            check_type(argname="argument transit_router_attachment_description", value=transit_router_attachment_description, expected_type=type_hints["transit_router_attachment_description"])
+            check_type(argname="argument transit_router_attachment_name", value=transit_router_attachment_name, expected_type=type_hints["transit_router_attachment_name"])
+            check_type(argname="argument transit_router_id", value=transit_router_id, expected_type=type_hints["transit_router_id"])
+            check_type(argname="argument vbr_owner_id", value=vbr_owner_id, expected_type=type_hints["vbr_owner_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "vbr_id": vbr_id,
         }
         if auto_publish_route_enabled is not None:
             self._values["auto_publish_route_enabled"] = auto_publish_route_enabled
         if cen_id is not None:
             self._values["cen_id"] = cen_id
@@ -7141,328 +8343,376 @@
 ):
     '''A ROS template type:  ``ALIYUN::CEN::TransitRouterVpcAttachment``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RosTransitRouterVpcAttachmentProps",
+        props: typing.Union["RosTransitRouterVpcAttachmentProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: builtins.bool,
     ) -> None:
         '''Create a new ``ALIYUN::CEN::TransitRouterVpcAttachment``.
 
         :param scope: - scope in which this resource is defined.
         :param id: - scoped id of the resource.
         :param props: - resource properties.
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosTransitRouterVpcAttachment.__init__)
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
+            type_hints = typing.get_type_hints(RosTransitRouterVpcAttachment._render_properties)
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
     @jsii.member(jsii_name="attrCenId")
     def attr_cen_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: CenId: CenId
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrCenId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrClientToken")
     def attr_client_token(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ClientToken: ClientToken
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrClientToken"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrResourceType")
     def attr_resource_type(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: ResourceType: ResourceType
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrResourceType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTransitRouterAttachmentDescription")
     def attr_transit_router_attachment_description(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: TransitRouterAttachmentDescription: TransitRouterAttachmentDescription
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTransitRouterAttachmentDescription"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTransitRouterAttachmentId")
     def attr_transit_router_attachment_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: TransitRouterAttachmentId: The first ID of the resource
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTransitRouterAttachmentId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTransitRouterAttachmentName")
     def attr_transit_router_attachment_name(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: TransitRouterAttachmentName: TransitRouterAttachmentName
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTransitRouterAttachmentName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTransitRouterId")
     def attr_transit_router_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: TransitRouterId: TransitRouterId
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTransitRouterId"))
 
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
     @jsii.member(jsii_name="attrVpcOwnerId")
     def attr_vpc_owner_id(self) -> ros_cdk_core.IResolvable:
         '''
         :Attribute: VpcOwnerId: VpcOwnerId
         '''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVpcOwnerId"))
 
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
+            type_hints = typing.get_type_hints(getattr(RosTransitRouterVpcAttachment, "enable_resource_property_constraint").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "enableResourcePropertyConstraint", value)
 
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
+            type_hints = typing.get_type_hints(getattr(RosTransitRouterVpcAttachment, "vpc_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "vpcId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="zoneMappings")
     def zone_mappings(
         self,
     ) -> typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosTransitRouterVpcAttachment.ZoneMappingsProperty"]]]:
         '''
         :Property: zoneMappings: ZoneMappingss
         '''
         return typing.cast(typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosTransitRouterVpcAttachment.ZoneMappingsProperty"]]], jsii.get(self, "zoneMappings"))
 
     @zone_mappings.setter
     def zone_mappings(
         self,
         value: typing.Union[ros_cdk_core.IResolvable, typing.List[typing.Union[ros_cdk_core.IResolvable, "RosTransitRouterVpcAttachment.ZoneMappingsProperty"]]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTransitRouterVpcAttachment, "zone_mappings").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "zoneMappings", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="autoCreateVpcRoute")
     def auto_create_vpc_route(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property: autoCreateVpcRoute: undefined
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "autoCreateVpcRoute"))
 
     @auto_create_vpc_route.setter
     def auto_create_vpc_route(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTransitRouterVpcAttachment, "auto_create_vpc_route").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "autoCreateVpcRoute", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="cenId")
     def cen_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: cenId: CenId
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "cenId"))
 
     @cen_id.setter
     def cen_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTransitRouterVpcAttachment, "cen_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "cenId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="chargeType")
     def charge_type(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: chargeType:
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "chargeType"))
 
     @charge_type.setter
     def charge_type(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTransitRouterVpcAttachment, "charge_type").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "chargeType", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="deletionForce")
     def deletion_force(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property: deletionForce: Whether force delete related resources, like vpc route entry, route table association, route propagation.
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "deletionForce"))
 
     @deletion_force.setter
     def deletion_force(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTransitRouterVpcAttachment, "deletion_force").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "deletionForce", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="routeTableAssociationEnabled")
     def route_table_association_enabled(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property: routeTableAssociationEnabled: undefined
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "routeTableAssociationEnabled"))
 
     @route_table_association_enabled.setter
     def route_table_association_enabled(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTransitRouterVpcAttachment, "route_table_association_enabled").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "routeTableAssociationEnabled", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="routeTablePropagationEnabled")
     def route_table_propagation_enabled(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]]:
         '''
         :Property: routeTablePropagationEnabled: undefined
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]], jsii.get(self, "routeTablePropagationEnabled"))
 
     @route_table_propagation_enabled.setter
     def route_table_propagation_enabled(
         self,
         value: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTransitRouterVpcAttachment, "route_table_propagation_enabled").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "routeTablePropagationEnabled", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="transitRouterAttachmentDescription")
     def transit_router_attachment_description(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: transitRouterAttachmentDescription: TransitRouterAttachmentDescription
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "transitRouterAttachmentDescription"))
 
     @transit_router_attachment_description.setter
     def transit_router_attachment_description(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTransitRouterVpcAttachment, "transit_router_attachment_description").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "transitRouterAttachmentDescription", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="transitRouterAttachmentName")
     def transit_router_attachment_name(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: transitRouterAttachmentName: TransitRouterAttachmentName
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "transitRouterAttachmentName"))
 
     @transit_router_attachment_name.setter
     def transit_router_attachment_name(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTransitRouterVpcAttachment, "transit_router_attachment_name").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "transitRouterAttachmentName", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="transitRouterId")
     def transit_router_id(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]]:
         '''
         :Property: transitRouterId: TransitRouterId
         '''
         return typing.cast(typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]], jsii.get(self, "transitRouterId"))
 
     @transit_router_id.setter
     def transit_router_id(
         self,
         value: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTransitRouterVpcAttachment, "transit_router_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "transitRouterId", value)
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="vpcOwnerId")
     def vpc_owner_id(
         self,
     ) -> typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]]:
         '''
         :Property: vpcOwnerId: VpcOwnerId
         '''
         return typing.cast(typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]], jsii.get(self, "vpcOwnerId"))
 
     @vpc_owner_id.setter
     def vpc_owner_id(
         self,
         value: typing.Optional[typing.Union[jsii.Number, ros_cdk_core.IResolvable]],
     ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(getattr(RosTransitRouterVpcAttachment, "vpc_owner_id").fset)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "vpcOwnerId", value)
 
     @jsii.data_type(
         jsii_type="@alicloud/ros-cdk-cen.RosTransitRouterVpcAttachment.ZoneMappingsProperty",
         jsii_struct_bases=[],
         name_mapping={"v_switch_id": "vSwitchId", "zone_id": "zoneId"},
     )
@@ -7473,14 +8723,18 @@
             v_switch_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
             zone_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
         ) -> None:
             '''
             :param v_switch_id: 
             :param zone_id: 
             '''
+            if __debug__:
+                type_hints = typing.get_type_hints(RosTransitRouterVpcAttachment.ZoneMappingsProperty.__init__)
+                check_type(argname="argument v_switch_id", value=v_switch_id, expected_type=type_hints["v_switch_id"])
+                check_type(argname="argument zone_id", value=zone_id, expected_type=type_hints["zone_id"])
             self._values: typing.Dict[str, typing.Any] = {
                 "v_switch_id": v_switch_id,
                 "zone_id": zone_id,
             }
 
         @builtins.property
         def v_switch_id(self) -> typing.Union[builtins.str, ros_cdk_core.IResolvable]:
@@ -7531,15 +8785,15 @@
     },
 )
 class RosTransitRouterVpcAttachmentProps:
     def __init__(
         self,
         *,
         vpc_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
-        zone_mappings: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosTransitRouterVpcAttachment.ZoneMappingsProperty]]],
+        zone_mappings: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosTransitRouterVpcAttachment.ZoneMappingsProperty, typing.Dict[str, typing.Any]]]]],
         auto_create_vpc_route: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         cen_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         charge_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         deletion_force: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         route_table_association_enabled: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         route_table_propagation_enabled: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         transit_router_attachment_description: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
@@ -7558,14 +8812,28 @@
         :param route_table_association_enabled: 
         :param route_table_propagation_enabled: 
         :param transit_router_attachment_description: 
         :param transit_router_attachment_name: 
         :param transit_router_id: 
         :param vpc_owner_id: 
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RosTransitRouterVpcAttachmentProps.__init__)
+            check_type(argname="argument vpc_id", value=vpc_id, expected_type=type_hints["vpc_id"])
+            check_type(argname="argument zone_mappings", value=zone_mappings, expected_type=type_hints["zone_mappings"])
+            check_type(argname="argument auto_create_vpc_route", value=auto_create_vpc_route, expected_type=type_hints["auto_create_vpc_route"])
+            check_type(argname="argument cen_id", value=cen_id, expected_type=type_hints["cen_id"])
+            check_type(argname="argument charge_type", value=charge_type, expected_type=type_hints["charge_type"])
+            check_type(argname="argument deletion_force", value=deletion_force, expected_type=type_hints["deletion_force"])
+            check_type(argname="argument route_table_association_enabled", value=route_table_association_enabled, expected_type=type_hints["route_table_association_enabled"])
+            check_type(argname="argument route_table_propagation_enabled", value=route_table_propagation_enabled, expected_type=type_hints["route_table_propagation_enabled"])
+            check_type(argname="argument transit_router_attachment_description", value=transit_router_attachment_description, expected_type=type_hints["transit_router_attachment_description"])
+            check_type(argname="argument transit_router_attachment_name", value=transit_router_attachment_name, expected_type=type_hints["transit_router_attachment_name"])
+            check_type(argname="argument transit_router_id", value=transit_router_id, expected_type=type_hints["transit_router_id"])
+            check_type(argname="argument vpc_owner_id", value=vpc_owner_id, expected_type=type_hints["vpc_owner_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "vpc_id": vpc_id,
             "zone_mappings": zone_mappings,
         }
         if auto_create_vpc_route is not None:
             self._values["auto_create_vpc_route"] = auto_create_vpc_route
         if cen_id is not None:
@@ -7726,28 +8994,34 @@
 ):
     '''A ROS resource type:  ``ALIYUN::CEN::RouteEntry``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "RouteEntryProps",
+        props: typing.Union["RouteEntryProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::CEN::RouteEntry``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RouteEntry.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
 
 @jsii.data_type(
     jsii_type="@alicloud/ros-cdk-cen.RouteEntryProps",
     jsii_struct_bases=[],
     name_mapping={
@@ -7775,14 +9049,22 @@
         :param cen_id: Property cenId: The ID of the CEN instance where the route entry is published.
         :param child_instance_id: Property childInstanceId: The ID of the attached network (VPC or VBR).
         :param child_instance_region_id: Property childInstanceRegionId: The ID of the region where the attached VBR or VPC is located.
         :param child_instance_route_table_id: Property childInstanceRouteTableId: The route table of the attached VBR or VPC.
         :param child_instance_type: Property childInstanceType: The type of the network, value: VPC VBR.
         :param destination_cidr_block: Property destinationCidrBlock: The destination CIDR block of the route entry to publish.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(RouteEntryProps.__init__)
+            check_type(argname="argument cen_id", value=cen_id, expected_type=type_hints["cen_id"])
+            check_type(argname="argument child_instance_id", value=child_instance_id, expected_type=type_hints["child_instance_id"])
+            check_type(argname="argument child_instance_region_id", value=child_instance_region_id, expected_type=type_hints["child_instance_region_id"])
+            check_type(argname="argument child_instance_route_table_id", value=child_instance_route_table_id, expected_type=type_hints["child_instance_route_table_id"])
+            check_type(argname="argument child_instance_type", value=child_instance_type, expected_type=type_hints["child_instance_type"])
+            check_type(argname="argument destination_cidr_block", value=destination_cidr_block, expected_type=type_hints["destination_cidr_block"])
         self._values: typing.Dict[str, typing.Any] = {
             "cen_id": cen_id,
             "child_instance_id": child_instance_id,
             "child_instance_region_id": child_instance_region_id,
             "child_instance_route_table_id": child_instance_route_table_id,
             "child_instance_type": child_instance_type,
             "destination_cidr_block": destination_cidr_block,
@@ -7857,67 +9139,73 @@
 ):
     '''A ROS resource type:  ``ALIYUN::CEN::TransitRouter``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "TransitRouterProps",
+        props: typing.Union["TransitRouterProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::CEN::TransitRouter``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(TransitRouter.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrAliUid")
     def attr_ali_uid(self) -> ros_cdk_core.IResolvable:
         '''Attribute AliUid: AliUid.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAliUid"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrCenId")
     def attr_cen_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute CenId: CenId.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrCenId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrSystemTransitRouterRouteTableId")
     def attr_system_transit_router_route_table_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute SystemTransitRouterRouteTableId: The system route table ID of transit router.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrSystemTransitRouterRouteTableId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTransitRouterDescription")
     def attr_transit_router_description(self) -> ros_cdk_core.IResolvable:
         '''Attribute TransitRouterDescription: TransitRouterDescription.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTransitRouterDescription"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTransitRouterId")
     def attr_transit_router_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute TransitRouterId: TransitRouterId.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTransitRouterId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTransitRouterName")
     def attr_transit_router_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute TransitRouterName: TransitRouterName.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTransitRouterName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrType")
     def attr_type(self) -> ros_cdk_core.IResolvable:
         '''Attribute Type: Type.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrType"))
 
 
 class TransitRouterPeerAttachment(
@@ -7927,109 +9215,115 @@
 ):
     '''A ROS resource type:  ``ALIYUN::CEN::TransitRouterPeerAttachment``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "TransitRouterPeerAttachmentProps",
+        props: typing.Union["TransitRouterPeerAttachmentProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::CEN::TransitRouterPeerAttachment``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(TransitRouterPeerAttachment.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrAutoPublishRouteEnabled")
     def attr_auto_publish_route_enabled(self) -> ros_cdk_core.IResolvable:
         '''Attribute AutoPublishRouteEnabled: AutoPublishRouteEnabled.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAutoPublishRouteEnabled"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrBandwidth")
     def attr_bandwidth(self) -> ros_cdk_core.IResolvable:
         '''Attribute Bandwidth: Bandwidth.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrBandwidth"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrCenBandwidthPackageId")
     def attr_cen_bandwidth_package_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute CenBandwidthPackageId: BandwidthPackageId.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrCenBandwidthPackageId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrCenId")
     def attr_cen_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute CenId: CenId.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrCenId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrClientToken")
     def attr_client_token(self) -> ros_cdk_core.IResolvable:
         '''Attribute ClientToken: ClientToken.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrClientToken"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrGeographicSpanId")
     def attr_geographic_span_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute GeographicSpanId: GeographicSpanId.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrGeographicSpanId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPeerTransitRouterId")
     def attr_peer_transit_router_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute PeerTransitRouterId: PeerTransitRouterId.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPeerTransitRouterId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPeerTransitRouterOwnerId")
     def attr_peer_transit_router_owner_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute PeerTransitRouterOwnerId: PeerTransitRouterOwnerId.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPeerTransitRouterOwnerId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrPeerTransitRouterRegionId")
     def attr_peer_transit_router_region_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute PeerTransitRouterRegionId: PeerTransitRouterRegionId.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrPeerTransitRouterRegionId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrResourceType")
     def attr_resource_type(self) -> ros_cdk_core.IResolvable:
         '''Attribute ResourceType: ResourceType.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrResourceType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTransitRouterAttachmentDescription")
     def attr_transit_router_attachment_description(self) -> ros_cdk_core.IResolvable:
         '''Attribute TransitRouterAttachmentDescription: TransitRouterAttachmentDescription.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTransitRouterAttachmentDescription"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTransitRouterAttachmentId")
     def attr_transit_router_attachment_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute TransitRouterAttachmentId: The first ID of the resource.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTransitRouterAttachmentId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTransitRouterAttachmentName")
     def attr_transit_router_attachment_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute TransitRouterAttachmentName: TransitRouterAttachmentName.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTransitRouterAttachmentName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTransitRouterId")
     def attr_transit_router_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute TransitRouterId: TransitRouterId.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTransitRouterId"))
 
 
 @jsii.data_type(
@@ -8069,14 +9363,25 @@
         :param cen_bandwidth_package_id: Property cenBandwidthPackageId: BandwidthPackageId.
         :param cen_id: Property cenId: CenId.
         :param peer_transit_router_region_id: Property peerTransitRouterRegionId: PeerTransitRouterRegionId.
         :param transit_router_attachment_description: Property transitRouterAttachmentDescription: TransitRouterAttachmentDescription.
         :param transit_router_attachment_name: Property transitRouterAttachmentName: TransitRouterAttachmentName.
         :param transit_router_id: Property transitRouterId: TransitRouterId.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(TransitRouterPeerAttachmentProps.__init__)
+            check_type(argname="argument peer_transit_router_id", value=peer_transit_router_id, expected_type=type_hints["peer_transit_router_id"])
+            check_type(argname="argument auto_publish_route_enabled", value=auto_publish_route_enabled, expected_type=type_hints["auto_publish_route_enabled"])
+            check_type(argname="argument bandwidth", value=bandwidth, expected_type=type_hints["bandwidth"])
+            check_type(argname="argument cen_bandwidth_package_id", value=cen_bandwidth_package_id, expected_type=type_hints["cen_bandwidth_package_id"])
+            check_type(argname="argument cen_id", value=cen_id, expected_type=type_hints["cen_id"])
+            check_type(argname="argument peer_transit_router_region_id", value=peer_transit_router_region_id, expected_type=type_hints["peer_transit_router_region_id"])
+            check_type(argname="argument transit_router_attachment_description", value=transit_router_attachment_description, expected_type=type_hints["transit_router_attachment_description"])
+            check_type(argname="argument transit_router_attachment_name", value=transit_router_attachment_name, expected_type=type_hints["transit_router_attachment_name"])
+            check_type(argname="argument transit_router_id", value=transit_router_id, expected_type=type_hints["transit_router_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "peer_transit_router_id": peer_transit_router_id,
         }
         if auto_publish_route_enabled is not None:
             self._values["auto_publish_route_enabled"] = auto_publish_route_enabled
         if bandwidth is not None:
             self._values["bandwidth"] = bandwidth
@@ -8197,14 +9502,19 @@
     ) -> None:
         '''Properties for defining a ``ALIYUN::CEN::TransitRouter``.
 
         :param cen_id: Property cenId: CenId.
         :param transit_router_description: Property transitRouterDescription: TransitRouterDescription.
         :param transit_router_name: Property transitRouterName: TransitRouterName.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(TransitRouterProps.__init__)
+            check_type(argname="argument cen_id", value=cen_id, expected_type=type_hints["cen_id"])
+            check_type(argname="argument transit_router_description", value=transit_router_description, expected_type=type_hints["transit_router_description"])
+            check_type(argname="argument transit_router_name", value=transit_router_name, expected_type=type_hints["transit_router_name"])
         self._values: typing.Dict[str, typing.Any] = {
             "cen_id": cen_id,
         }
         if transit_router_description is not None:
             self._values["transit_router_description"] = transit_router_description
         if transit_router_name is not None:
             self._values["transit_router_name"] = transit_router_name
@@ -8251,75 +9561,81 @@
 ):
     '''A ROS resource type:  ``ALIYUN::CEN::TransitRouterRouteEntry``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "TransitRouterRouteEntryProps",
+        props: typing.Union["TransitRouterRouteEntryProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::CEN::TransitRouterRouteEntry``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(TransitRouterRouteEntry.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTransitRouterRouteEntryDescription")
     def attr_transit_router_route_entry_description(self) -> ros_cdk_core.IResolvable:
         '''Attribute TransitRouterRouteEntryDescription: TransitRouterRouteEntryDescription.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTransitRouterRouteEntryDescription"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTransitRouterRouteEntryDestinationCidrBlock")
     def attr_transit_router_route_entry_destination_cidr_block(
         self,
     ) -> ros_cdk_core.IResolvable:
         '''Attribute TransitRouterRouteEntryDestinationCidrBlock: TransitRouterRouteEntryDestinationCidrBlock.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTransitRouterRouteEntryDestinationCidrBlock"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTransitRouterRouteEntryId")
     def attr_transit_router_route_entry_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute TransitRouterRouteEntryId: The first ID of the resource.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTransitRouterRouteEntryId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTransitRouterRouteEntryName")
     def attr_transit_router_route_entry_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute TransitRouterRouteEntryName: TransitRouterRouteEntryName.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTransitRouterRouteEntryName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTransitRouterRouteEntryNextHopId")
     def attr_transit_router_route_entry_next_hop_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute TransitRouterRouteEntryNextHopId: TransitRouterRouteEntryNextHopId.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTransitRouterRouteEntryNextHopId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTransitRouterRouteEntryNextHopType")
     def attr_transit_router_route_entry_next_hop_type(self) -> ros_cdk_core.IResolvable:
         '''Attribute TransitRouterRouteEntryNextHopType: TransitRouterRouteEntryNextHopType.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTransitRouterRouteEntryNextHopType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTransitRouterRouteEntryType")
     def attr_transit_router_route_entry_type(self) -> ros_cdk_core.IResolvable:
         '''Attribute TransitRouterRouteEntryType: TransitRouterRouteEntryType.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTransitRouterRouteEntryType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTransitRouterRouteTableId")
     def attr_transit_router_route_table_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute TransitRouterRouteTableId: TransitRouterRouteTableId.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTransitRouterRouteTableId"))
 
 
 @jsii.data_type(
@@ -8350,14 +9666,22 @@
         :param transit_router_route_entry_destination_cidr_block: Property transitRouterRouteEntryDestinationCidrBlock: TransitRouterRouteEntryDestinationCidrBlock.
         :param transit_router_route_entry_next_hop_type: Property transitRouterRouteEntryNextHopType: TransitRouterRouteEntryNextHopType.
         :param transit_router_route_table_id: Property transitRouterRouteTableId: TransitRouterRouteTableId.
         :param transit_router_route_entry_description: Property transitRouterRouteEntryDescription: TransitRouterRouteEntryDescription.
         :param transit_router_route_entry_name: Property transitRouterRouteEntryName: TransitRouterRouteEntryName.
         :param transit_router_route_entry_next_hop_id: Property transitRouterRouteEntryNextHopId: TransitRouterRouteEntryNextHopId.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(TransitRouterRouteEntryProps.__init__)
+            check_type(argname="argument transit_router_route_entry_destination_cidr_block", value=transit_router_route_entry_destination_cidr_block, expected_type=type_hints["transit_router_route_entry_destination_cidr_block"])
+            check_type(argname="argument transit_router_route_entry_next_hop_type", value=transit_router_route_entry_next_hop_type, expected_type=type_hints["transit_router_route_entry_next_hop_type"])
+            check_type(argname="argument transit_router_route_table_id", value=transit_router_route_table_id, expected_type=type_hints["transit_router_route_table_id"])
+            check_type(argname="argument transit_router_route_entry_description", value=transit_router_route_entry_description, expected_type=type_hints["transit_router_route_entry_description"])
+            check_type(argname="argument transit_router_route_entry_name", value=transit_router_route_entry_name, expected_type=type_hints["transit_router_route_entry_name"])
+            check_type(argname="argument transit_router_route_entry_next_hop_id", value=transit_router_route_entry_next_hop_id, expected_type=type_hints["transit_router_route_entry_next_hop_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "transit_router_route_entry_destination_cidr_block": transit_router_route_entry_destination_cidr_block,
             "transit_router_route_entry_next_hop_type": transit_router_route_entry_next_hop_type,
             "transit_router_route_table_id": transit_router_route_table_id,
         }
         if transit_router_route_entry_description is not None:
             self._values["transit_router_route_entry_description"] = transit_router_route_entry_description
@@ -8436,61 +9760,67 @@
 ):
     '''A ROS resource type:  ``ALIYUN::CEN::TransitRouterRouteTable``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "TransitRouterRouteTableProps",
+        props: typing.Union["TransitRouterRouteTableProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::CEN::TransitRouterRouteTable``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(TransitRouterRouteTable.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrClientToken")
     def attr_client_token(self) -> ros_cdk_core.IResolvable:
         '''Attribute ClientToken: ClientToken.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrClientToken"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTransitRouterId")
     def attr_transit_router_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute TransitRouterId: TransitRouterId.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTransitRouterId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTransitRouterRouteTableDescription")
     def attr_transit_router_route_table_description(self) -> ros_cdk_core.IResolvable:
         '''Attribute TransitRouterRouteTableDescription: TransitRouterRouteTableDescription.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTransitRouterRouteTableDescription"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTransitRouterRouteTableId")
     def attr_transit_router_route_table_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute TransitRouterRouteTableId: TransitRouterRouteTableId.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTransitRouterRouteTableId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTransitRouterRouteTableName")
     def attr_transit_router_route_table_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute TransitRouterRouteTableName: TransitRouterRouteTableName.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTransitRouterRouteTableName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTransitRouterRouteTableType")
     def attr_transit_router_route_table_type(self) -> ros_cdk_core.IResolvable:
         '''Attribute TransitRouterRouteTableType: TransitRouterRouteTableType.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTransitRouterRouteTableType"))
 
 
 class TransitRouterRouteTableAssociation(
@@ -8500,49 +9830,55 @@
 ):
     '''A ROS resource type:  ``ALIYUN::CEN::TransitRouterRouteTableAssociation``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "TransitRouterRouteTableAssociationProps",
+        props: typing.Union["TransitRouterRouteTableAssociationProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::CEN::TransitRouterRouteTableAssociation``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(TransitRouterRouteTableAssociation.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrResourceId")
     def attr_resource_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute ResourceId: ResourceId.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrResourceId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrResourceType")
     def attr_resource_type(self) -> ros_cdk_core.IResolvable:
         '''Attribute ResourceType: ResourceType.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrResourceType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTransitRouterAttachmentId")
     def attr_transit_router_attachment_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute TransitRouterAttachmentId: TransitRouterAttachmentId.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTransitRouterAttachmentId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTransitRouterRouteTableId")
     def attr_transit_router_route_table_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute TransitRouterRouteTableId: TransitRouterRouteTableId.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTransitRouterRouteTableId"))
 
 
 @jsii.data_type(
@@ -8561,14 +9897,18 @@
         transit_router_route_table_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
         '''Properties for defining a ``ALIYUN::CEN::TransitRouterRouteTableAssociation``.
 
         :param transit_router_attachment_id: Property transitRouterAttachmentId: TransitRouterAttachmentId.
         :param transit_router_route_table_id: Property transitRouterRouteTableId: TransitRouterRouteTableId.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(TransitRouterRouteTableAssociationProps.__init__)
+            check_type(argname="argument transit_router_attachment_id", value=transit_router_attachment_id, expected_type=type_hints["transit_router_attachment_id"])
+            check_type(argname="argument transit_router_route_table_id", value=transit_router_route_table_id, expected_type=type_hints["transit_router_route_table_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "transit_router_attachment_id": transit_router_attachment_id,
             "transit_router_route_table_id": transit_router_route_table_id,
         }
 
     @builtins.property
     def transit_router_attachment_id(
@@ -8607,49 +9947,55 @@
 ):
     '''A ROS resource type:  ``ALIYUN::CEN::TransitRouterRouteTablePropagation``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "TransitRouterRouteTablePropagationProps",
+        props: typing.Union["TransitRouterRouteTablePropagationProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::CEN::TransitRouterRouteTablePropagation``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(TransitRouterRouteTablePropagation.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrResourceId")
     def attr_resource_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute ResourceId: ResourceId.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrResourceId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrResourceType")
     def attr_resource_type(self) -> ros_cdk_core.IResolvable:
         '''Attribute ResourceType: ResourceType.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrResourceType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTransitRouterAttachmentId")
     def attr_transit_router_attachment_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute TransitRouterAttachmentId: TransitRouterAttachmentId.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTransitRouterAttachmentId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTransitRouterRouteTableId")
     def attr_transit_router_route_table_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute TransitRouterRouteTableId: TransitRouterRouteTableId.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTransitRouterRouteTableId"))
 
 
 @jsii.data_type(
@@ -8668,14 +10014,18 @@
         transit_router_route_table_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
     ) -> None:
         '''Properties for defining a ``ALIYUN::CEN::TransitRouterRouteTablePropagation``.
 
         :param transit_router_attachment_id: Property transitRouterAttachmentId: TransitRouterAttachmentId.
         :param transit_router_route_table_id: Property transitRouterRouteTableId: TransitRouterRouteTableId.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(TransitRouterRouteTablePropagationProps.__init__)
+            check_type(argname="argument transit_router_attachment_id", value=transit_router_attachment_id, expected_type=type_hints["transit_router_attachment_id"])
+            check_type(argname="argument transit_router_route_table_id", value=transit_router_route_table_id, expected_type=type_hints["transit_router_route_table_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "transit_router_attachment_id": transit_router_attachment_id,
             "transit_router_route_table_id": transit_router_route_table_id,
         }
 
     @builtins.property
     def transit_router_attachment_id(
@@ -8726,14 +10076,19 @@
     ) -> None:
         '''Properties for defining a ``ALIYUN::CEN::TransitRouterRouteTable``.
 
         :param transit_router_id: Property transitRouterId: TransitRouterId.
         :param transit_router_route_table_description: Property transitRouterRouteTableDescription: TransitRouterRouteTableDescription.
         :param transit_router_route_table_name: Property transitRouterRouteTableName: TransitRouterRouteTableName.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(TransitRouterRouteTableProps.__init__)
+            check_type(argname="argument transit_router_id", value=transit_router_id, expected_type=type_hints["transit_router_id"])
+            check_type(argname="argument transit_router_route_table_description", value=transit_router_route_table_description, expected_type=type_hints["transit_router_route_table_description"])
+            check_type(argname="argument transit_router_route_table_name", value=transit_router_route_table_name, expected_type=type_hints["transit_router_route_table_name"])
         self._values: typing.Dict[str, typing.Any] = {
             "transit_router_id": transit_router_id,
         }
         if transit_router_route_table_description is not None:
             self._values["transit_router_route_table_description"] = transit_router_route_table_description
         if transit_router_route_table_name is not None:
             self._values["transit_router_route_table_name"] = transit_router_route_table_name
@@ -8780,85 +10135,91 @@
 ):
     '''A ROS resource type:  ``ALIYUN::CEN::TransitRouterVbrAttachment``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "TransitRouterVbrAttachmentProps",
+        props: typing.Union["TransitRouterVbrAttachmentProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::CEN::TransitRouterVbrAttachment``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(TransitRouterVbrAttachment.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrAutoPublishRouteEnabled")
     def attr_auto_publish_route_enabled(self) -> ros_cdk_core.IResolvable:
         '''Attribute AutoPublishRouteEnabled: AutoPublishRouteEnabled.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrAutoPublishRouteEnabled"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrCenId")
     def attr_cen_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute CenId: CenId.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrCenId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrClientToken")
     def attr_client_token(self) -> ros_cdk_core.IResolvable:
         '''Attribute ClientToken: ClientToken.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrClientToken"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrResourceType")
     def attr_resource_type(self) -> ros_cdk_core.IResolvable:
         '''Attribute ResourceType: ResourceType.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrResourceType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTransitRouterAttachmentDescription")
     def attr_transit_router_attachment_description(self) -> ros_cdk_core.IResolvable:
         '''Attribute TransitRouterAttachmentDescription: TransitRouterAttachmentDescription.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTransitRouterAttachmentDescription"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTransitRouterAttachmentId")
     def attr_transit_router_attachment_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute TransitRouterAttachmentId: The first ID of the resource.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTransitRouterAttachmentId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTransitRouterAttachmentName")
     def attr_transit_router_attachment_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute TransitRouterAttachmentName: TransitRouterAttachmentName.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTransitRouterAttachmentName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTransitRouterId")
     def attr_transit_router_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute TransitRouterId: TransitRouterId.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTransitRouterId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVbrId")
     def attr_vbr_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute VbrId: VbrId.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVbrId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVbrOwnerId")
     def attr_vbr_owner_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute VbrOwnerId: VbrOwnerId.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVbrOwnerId"))
 
 
 @jsii.data_type(
@@ -8892,14 +10253,23 @@
         :param auto_publish_route_enabled: Property autoPublishRouteEnabled: AutoPublishRouteEnabled.
         :param cen_id: Property cenId: CenId.
         :param transit_router_attachment_description: Property transitRouterAttachmentDescription: TransitRouterAttachmentDescription.
         :param transit_router_attachment_name: Property transitRouterAttachmentName: TransitRouterAttachmentName.
         :param transit_router_id: Property transitRouterId: TransitRouterId.
         :param vbr_owner_id: Property vbrOwnerId: VbrOwnerId.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(TransitRouterVbrAttachmentProps.__init__)
+            check_type(argname="argument vbr_id", value=vbr_id, expected_type=type_hints["vbr_id"])
+            check_type(argname="argument auto_publish_route_enabled", value=auto_publish_route_enabled, expected_type=type_hints["auto_publish_route_enabled"])
+            check_type(argname="argument cen_id", value=cen_id, expected_type=type_hints["cen_id"])
+            check_type(argname="argument transit_router_attachment_description", value=transit_router_attachment_description, expected_type=type_hints["transit_router_attachment_description"])
+            check_type(argname="argument transit_router_attachment_name", value=transit_router_attachment_name, expected_type=type_hints["transit_router_attachment_name"])
+            check_type(argname="argument transit_router_id", value=transit_router_id, expected_type=type_hints["transit_router_id"])
+            check_type(argname="argument vbr_owner_id", value=vbr_owner_id, expected_type=type_hints["vbr_owner_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "vbr_id": vbr_id,
         }
         if auto_publish_route_enabled is not None:
             self._values["auto_publish_route_enabled"] = auto_publish_route_enabled
         if cen_id is not None:
             self._values["cen_id"] = cen_id
@@ -8986,79 +10356,85 @@
 ):
     '''A ROS resource type:  ``ALIYUN::CEN::TransitRouterVpcAttachment``.'''
 
     def __init__(
         self,
         scope: ros_cdk_core.Construct,
         id: builtins.str,
-        props: "TransitRouterVpcAttachmentProps",
+        props: typing.Union["TransitRouterVpcAttachmentProps", typing.Dict[str, typing.Any]],
         enable_resource_property_constraint: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''Create a new ``ALIYUN::CEN::TransitRouterVpcAttachment``.
 
         Param scope - scope in which this resource is defined
         Param id    - scoped id of the resource
         Param props - resource properties
 
         :param scope: -
         :param id: -
         :param props: -
         :param enable_resource_property_constraint: -
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(TransitRouterVpcAttachment.__init__)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument props", value=props, expected_type=type_hints["props"])
+            check_type(argname="argument enable_resource_property_constraint", value=enable_resource_property_constraint, expected_type=type_hints["enable_resource_property_constraint"])
         jsii.create(self.__class__, self, [scope, id, props, enable_resource_property_constraint])
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrCenId")
     def attr_cen_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute CenId: CenId.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrCenId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrClientToken")
     def attr_client_token(self) -> ros_cdk_core.IResolvable:
         '''Attribute ClientToken: ClientToken.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrClientToken"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrResourceType")
     def attr_resource_type(self) -> ros_cdk_core.IResolvable:
         '''Attribute ResourceType: ResourceType.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrResourceType"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTransitRouterAttachmentDescription")
     def attr_transit_router_attachment_description(self) -> ros_cdk_core.IResolvable:
         '''Attribute TransitRouterAttachmentDescription: TransitRouterAttachmentDescription.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTransitRouterAttachmentDescription"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTransitRouterAttachmentId")
     def attr_transit_router_attachment_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute TransitRouterAttachmentId: The first ID of the resource.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTransitRouterAttachmentId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTransitRouterAttachmentName")
     def attr_transit_router_attachment_name(self) -> ros_cdk_core.IResolvable:
         '''Attribute TransitRouterAttachmentName: TransitRouterAttachmentName.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTransitRouterAttachmentName"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrTransitRouterId")
     def attr_transit_router_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute TransitRouterId: TransitRouterId.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrTransitRouterId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVpcId")
     def attr_vpc_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute VpcId: VpcId.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVpcId"))
 
-    @builtins.property # type: ignore[misc]
+    @builtins.property
     @jsii.member(jsii_name="attrVpcOwnerId")
     def attr_vpc_owner_id(self) -> ros_cdk_core.IResolvable:
         '''Attribute VpcOwnerId: VpcOwnerId.'''
         return typing.cast(ros_cdk_core.IResolvable, jsii.get(self, "attrVpcOwnerId"))
 
 
 @jsii.data_type(
@@ -9080,15 +10456,15 @@
     },
 )
 class TransitRouterVpcAttachmentProps:
     def __init__(
         self,
         *,
         vpc_id: typing.Union[builtins.str, ros_cdk_core.IResolvable],
-        zone_mappings: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, RosTransitRouterVpcAttachment.ZoneMappingsProperty]]],
+        zone_mappings: typing.Union[ros_cdk_core.IResolvable, typing.Sequence[typing.Union[ros_cdk_core.IResolvable, typing.Union[RosTransitRouterVpcAttachment.ZoneMappingsProperty, typing.Dict[str, typing.Any]]]]],
         auto_create_vpc_route: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         cen_id: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         charge_type: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
         deletion_force: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         route_table_association_enabled: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         route_table_propagation_enabled: typing.Optional[typing.Union[builtins.bool, ros_cdk_core.IResolvable]] = None,
         transit_router_attachment_description: typing.Optional[typing.Union[builtins.str, ros_cdk_core.IResolvable]] = None,
@@ -9107,14 +10483,28 @@
         :param route_table_association_enabled: Property routeTableAssociationEnabled: undefined.
         :param route_table_propagation_enabled: Property routeTablePropagationEnabled: undefined.
         :param transit_router_attachment_description: Property transitRouterAttachmentDescription: TransitRouterAttachmentDescription.
         :param transit_router_attachment_name: Property transitRouterAttachmentName: TransitRouterAttachmentName.
         :param transit_router_id: Property transitRouterId: TransitRouterId.
         :param vpc_owner_id: Property vpcOwnerId: VpcOwnerId.
         '''
+        if __debug__:
+            type_hints = typing.get_type_hints(TransitRouterVpcAttachmentProps.__init__)
+            check_type(argname="argument vpc_id", value=vpc_id, expected_type=type_hints["vpc_id"])
+            check_type(argname="argument zone_mappings", value=zone_mappings, expected_type=type_hints["zone_mappings"])
+            check_type(argname="argument auto_create_vpc_route", value=auto_create_vpc_route, expected_type=type_hints["auto_create_vpc_route"])
+            check_type(argname="argument cen_id", value=cen_id, expected_type=type_hints["cen_id"])
+            check_type(argname="argument charge_type", value=charge_type, expected_type=type_hints["charge_type"])
+            check_type(argname="argument deletion_force", value=deletion_force, expected_type=type_hints["deletion_force"])
+            check_type(argname="argument route_table_association_enabled", value=route_table_association_enabled, expected_type=type_hints["route_table_association_enabled"])
+            check_type(argname="argument route_table_propagation_enabled", value=route_table_propagation_enabled, expected_type=type_hints["route_table_propagation_enabled"])
+            check_type(argname="argument transit_router_attachment_description", value=transit_router_attachment_description, expected_type=type_hints["transit_router_attachment_description"])
+            check_type(argname="argument transit_router_attachment_name", value=transit_router_attachment_name, expected_type=type_hints["transit_router_attachment_name"])
+            check_type(argname="argument transit_router_id", value=transit_router_id, expected_type=type_hints["transit_router_id"])
+            check_type(argname="argument vpc_owner_id", value=vpc_owner_id, expected_type=type_hints["vpc_owner_id"])
         self._values: typing.Dict[str, typing.Any] = {
             "vpc_id": vpc_id,
             "zone_mappings": zone_mappings,
         }
         if auto_create_vpc_route is not None:
             self._values["auto_create_vpc_route"] = auto_create_vpc_route
         if cen_id is not None:
@@ -9257,14 +10647,16 @@
     "CenInstanceProps",
     "CenRouteMap",
     "CenRouteMapProps",
     "CenRouteService",
     "CenRouteServiceProps",
     "CenVbrHealthCheck",
     "CenVbrHealthCheckProps",
+    "ChildInstanceRouteEntryToAttachment",
+    "ChildInstanceRouteEntryToAttachmentProps",
     "RosCenBandwidthLimit",
     "RosCenBandwidthLimitProps",
     "RosCenBandwidthPackage",
     "RosCenBandwidthPackageAssociation",
     "RosCenBandwidthPackageAssociationProps",
     "RosCenBandwidthPackageProps",
     "RosCenInstance",
@@ -9273,14 +10665,16 @@
     "RosCenInstanceProps",
     "RosCenRouteMap",
     "RosCenRouteMapProps",
     "RosCenRouteService",
     "RosCenRouteServiceProps",
     "RosCenVbrHealthCheck",
     "RosCenVbrHealthCheckProps",
+    "RosChildInstanceRouteEntryToAttachment",
+    "RosChildInstanceRouteEntryToAttachmentProps",
     "RosRouteEntry",
     "RosRouteEntryProps",
     "RosTransitRouter",
     "RosTransitRouterPeerAttachment",
     "RosTransitRouterPeerAttachmentProps",
     "RosTransitRouterProps",
     "RosTransitRouterRouteEntry",
```

### Comparing `ros-cdk-cen-1.0.8/src/ros_cdk_cen.egg-info/PKG-INFO` & `ros-cdk-cen-1.0.9/src/ros_cdk_cen.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ros-cdk-cen
-Version: 1.0.8
+Version: 1.0.9
 Summary: Aliyun SDK Copyright (C) Alibaba Cloud Computing All rights reserved. http://www.aliyun.com
 Home-page: https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Author: ROS Development Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/aliyun/Resource-Orchestration-Service-Cloud-Development-Kit.git
 Description: ## Aliyun ROS CEN Construct Library
```

